# Comparing `tmp/newrelic-8.8.0.tar.gz` & `tmp/newrelic-8.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic-8.8.0.tar", last modified: Thu Mar 30 21:18:06 2023, max compression
+gzip compressed data, was "newrelic-8.8.1.tar", last modified: Mon Jun 26 21:30:53 2023, max compression
```

## Comparing `newrelic-8.8.0.tar` & `newrelic-8.8.1.tar`

### file list

```diff
@@ -1,1191 +1,1217 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.358904 newrelic-8.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.198905 newrelic-8.8.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-30 21:17:49.000000 newrelic-8.8.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-30 21:17:49.000000 newrelic-8.8.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.198905 newrelic-8.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.198905 newrelic-8.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/ISSUE_TEMPLATE/troubleshooting.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.178905 newrelic-8.8.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.198905 newrelic-8.8.0/.github/actions/setup-python-matrix/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/actions/setup-python-matrix/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.198905 newrelic-8.8.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/scripts/retry.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.202905 newrelic-8.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/workflows/deploy-python.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/workflows/get-envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/workflows/mega-linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)    20783 2023-03-30 21:17:49.000000 newrelic-8.8.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-30 21:17:49.000000 newrelic-8.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-30 21:17:49.000000 newrelic-8.8.0/.mega-linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-03-30 21:17:49.000000 newrelic-8.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-30 21:17:49.000000 newrelic-8.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-30 21:17:49.000000 newrelic-8.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-03-30 21:18:06.358904 newrelic-8.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-03-30 21:17:49.000000 newrelic-8.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-30 21:17:49.000000 newrelic-8.8.0/ROADMAP.md
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-30 21:17:49.000000 newrelic-8.8.0/THIRD_PARTY_NOTICES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.202905 newrelic-8.8.0/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.206905 newrelic-8.8.0/newrelic/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/debug_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/generate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/license_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/network_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/record_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/run_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/run_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/server_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/admin/validate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.214905 newrelic-8.8.0/newrelic/api/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/asgi_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/background_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/cat_header_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/database_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/datastore_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/error_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/external_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/function_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/function_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/generator_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/graphql_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/html_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/in_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/memcache_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/message_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/message_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/object_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/out_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/post_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/pre_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/profile_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/solr_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/supportability.py
--rw-r--r--   0 runner    (1001) docker     (123)    26330 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/time_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    69566 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/transaction_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    35165 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/web_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    25411 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/api/wsgi_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.214905 newrelic-8.8.0/newrelic/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/bootstrap/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.218905 newrelic-8.8.0/newrelic/common/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/_monotonic.c
--rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/agent_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/async_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    64813 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/coroutine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18641 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/encoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/log_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/object_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/object_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/package_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/streaming_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/common/utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)   115246 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18465 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.226905 newrelic-8.8.0/newrelic/core/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/_thread_utilization.c
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/adaptive_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31544 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/agent_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/agent_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    70315 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    40694 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/custom_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/database_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/datastore_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/error_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/error_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/external_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/graphql_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/graphql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/infinite_tracing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/infinite_tracing_v3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/infinite_tracing_v4_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/internal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/log_event_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/loop_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/memcache_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/message_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/node_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16490 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/profile_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/root_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/rules_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/solr_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/stack_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    64178 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/stats_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/string_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/thread_utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/trace_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22650 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/core/transaction_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.226905 newrelic-8.8.0/newrelic/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.226905 newrelic-8.8.0/newrelic/extras/framework_django/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/extras/framework_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.226905 newrelic-8.8.0/newrelic/extras/framework_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/extras/framework_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.250904 newrelic-8.8.0/newrelic/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_asgiref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_cheroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_cherrypy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_daphne.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_flup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_gevent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_hypercorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_meinheld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_paste.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_uvicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_waitress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/adapter_wsgiref.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/application_celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/application_gearman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/component_cornice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/component_djangorestframework.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/component_flask_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/component_graphqlserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/component_piston.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/component_sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/component_tastypie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/coroutines_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/coroutines_gevent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_cx_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_ibm_db_dbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_oursql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_psycopg2cffi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_psycopg2ct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_pymssql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_pymysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_pyodbc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/database_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_aioredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_aredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_bmemcached.py
--rw-r--r--   0 runner    (1001) docker     (123)    21862 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_memcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_motor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_pyelasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_pylibmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_pymemcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_pysolr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_solrpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/datastore_umemcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_botocore.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_facepy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_feedparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_httplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_httplib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_pywapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_thrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_urllib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/external_xmlrpclib.py
--rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_ariadne.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_cherrypy.py
--rw-r--r--   0 runner    (1001) docker     (123)    42753 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_django.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_django_py3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_falcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_graphene.py
--rw-r--r--   0 runner    (1001) docker     (123)    17278 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_pylons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_sanic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_strawberry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_twisted.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_web2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/framework_webpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/logger_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/logger_loguru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/memcache_memcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/memcache_pylibmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/memcache_umemcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/messagebroker_confluentkafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/messagebroker_kafkapython.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/messagebroker_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/middleware_flask_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/middleware_weberror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/nosql_pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/nosql_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/solr_pysolr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/solr_solrpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/template_genshi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/template_jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/hooks/template_mako.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.250904 newrelic-8.8.0/newrelic/network/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/network/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/network/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/newrelic.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.250904 newrelic-8.8.0/newrelic/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/asgiref_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/six.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.254905 newrelic-8.8.0/newrelic/packages/urllib3/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20080 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    37587 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.254905 newrelic-8.8.0/newrelic/packages/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.254905 newrelic-8.8.0/newrelic/packages/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34417 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.254905 newrelic-8.8.0/newrelic/packages/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.254905 newrelic-8.8.0/newrelic/packages/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    34666 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/packages/six.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.254905 newrelic-8.8.0/newrelic/packages/urllib3/packages/ssl_match_hostname/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    28203 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.258905 newrelic-8.8.0/newrelic/packages/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    21391 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/urllib3/util/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.258905 newrelic-8.8.0/newrelic/packages/wrapt/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/wrapt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/wrapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95815 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/wrapt/_wrappers.c
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/wrapt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/wrapt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/wrapt/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35521 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/packages/wrapt/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.262905 newrelic-8.8.0/newrelic/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/samplers/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/samplers/data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/samplers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/samplers/gc_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-30 21:17:49.000000 newrelic-8.8.0/newrelic/samplers/memory_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-30 21:18:05.000000 newrelic-8.8.0/newrelic/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.202905 newrelic-8.8.0/newrelic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-03-30 21:18:06.000000 newrelic-8.8.0/newrelic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    53781 2023-03-30 21:18:06.000000 newrelic-8.8.0/newrelic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 21:18:06.000000 newrelic-8.8.0/newrelic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-30 21:18:06.000000 newrelic-8.8.0/newrelic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 21:18:06.000000 newrelic-8.8.0/newrelic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-30 21:18:06.000000 newrelic-8.8.0/newrelic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-30 21:18:06.000000 newrelic-8.8.0/newrelic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-30 21:17:49.000000 newrelic-8.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.262905 newrelic-8.8.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/scripts/newrelic-admin
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-30 21:18:06.358904 newrelic-8.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-03-30 21:17:49.000000 newrelic-8.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.194905 newrelic-8.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.262905 newrelic-8.8.0/tests/adapter_cheroot/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_cheroot/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_cheroot/test_wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.262905 newrelic-8.8.0/tests/adapter_daphne/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_daphne/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_daphne/test_daphne.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.262905 newrelic-8.8.0/tests/adapter_gevent/
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gevent/_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gevent/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gevent/test_patching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gevent/test_pywsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.266904 newrelic-8.8.0/tests/adapter_gunicorn/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gunicorn/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gunicorn/asgi_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gunicorn/async_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gunicorn/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gunicorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gunicorn/test_asgi_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gunicorn/test_gaiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_gunicorn/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.266904 newrelic-8.8.0/tests/adapter_hypercorn/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_hypercorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_hypercorn/test_hypercorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.266904 newrelic-8.8.0/tests/adapter_uvicorn/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_uvicorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/adapter_uvicorn/test_uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.274904 newrelic-8.8.0/tests/agent_features/
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/_test_async_coroutine_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/_test_async_coroutine_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/_test_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_apdex_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    32501 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_asgi_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_asgi_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_asgi_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_asgi_w3c_trace_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_async_context_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_async_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    35348 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_attributes_in_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_background_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    33137 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_browser_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_collector_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    20320 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_coroutine_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_coroutine_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_custom_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_dead_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_error_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_error_group_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_event_loop_wait_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    12523 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_exception_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_function_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_high_security_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_ignore_expected_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_log_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_logs_in_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_notice_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_priority_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_serverless_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    24684 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_span_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_stack_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_supportability_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_synthetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_time_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_transaction_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_transaction_trace_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_w3c_trace_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_web_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_features/test_wsgi_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.278904 newrelic-8.8.0/tests/agent_streaming/
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_streaming/_test_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_streaming/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_streaming/test_infinite_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_streaming/test_span_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_streaming/test_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_streaming/test_streaming_rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.282904 newrelic-8.8.0/tests/agent_unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/_test_import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_agent_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_agent_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_check_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_connect_response_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_distributed_tracing_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_full_uri_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_harvest_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    20941 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_infinite_trace_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_package_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_region_aware_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_sampler_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_serverless_mode_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_trace_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/agent_unittests/test_utilization_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.282904 newrelic-8.8.0/tests/application_celery/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/application_celery/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/application_celery/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/application_celery/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/application_celery/test_celery_max_tasks_per_child.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.282904 newrelic-8.8.0/tests/application_gearman/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/application_gearman/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/application_gearman/test_gearman.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.286904 newrelic-8.8.0/tests/component_djangorestframework/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_djangorestframework/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_djangorestframework/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_djangorestframework/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_djangorestframework/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_djangorestframework/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_djangorestframework/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.286904 newrelic-8.8.0/tests/component_flask_rest/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_flask_rest/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_flask_rest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_flask_rest/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.286904 newrelic-8.8.0/tests/component_graphqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_graphqlserver/_test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_graphqlserver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_graphqlserver/test_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.286904 newrelic-8.8.0/tests/component_tastypie/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_tastypie/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_tastypie/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_tastypie/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_tastypie/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_tastypie/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_tastypie/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/component_tastypie/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.286904 newrelic-8.8.0/tests/coroutines_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/coroutines_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/coroutines_asyncio/test_context_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.290904 newrelic-8.8.0/tests/cross_agent/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.294904 newrelic-8.8.0/tests/cross_agent/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/attribute_configuration.json
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/cat_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/collector_hostname.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.294904 newrelic-8.8.0/tests/cross_agent/fixtures/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/datastores/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/datastores/datastore_instances.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.294904 newrelic-8.8.0/tests/cross_agent/fixtures/distributed_tracing/
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/distributed_tracing/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    48250 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json
--rw-r--r--   0 runner    (1001) docker     (123)    58950 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.294904 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/cases.json
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-0.9.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/empty.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/heroku.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/invalid-length.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-lxc-container.txt
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-no-container.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.10-no-container.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/labels.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.298904 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_auth.json
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/batch_get.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/batch_submit.json
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudformation_create.json
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudwatch_logs.json
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cognito_sync.json
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_analytics.json
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_apache.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_invoke.json
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/lex_appointment.json
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/lex_book_car.json
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/scheduled_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/ses.json
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_discovery.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_turn_off.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/sns.json
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.306904 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.query.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.310904 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_1logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_2core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/malformed_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.310904 newrelic-8.8.0/tests/cross_agent/fixtures/proc_meminfo/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_meminfo/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_meminfo/malformed_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_client_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_cookie.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.310904 newrelic-8.8.0/tests/cross_agent/fixtures/rum_footer_insertion_location/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_footer_insertion_location/close-body-in-comment.html
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_footer_insertion_location/dynamic-iframe.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.314904 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/empty_head
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.318904 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.322904 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.322904 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/sql_parsing.json
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/transaction_segment_terms.json
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/url_clean.json
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/url_domain_extraction.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.322904 newrelic-8.8.0/tests/cross_agent/fixtures/utilization/
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/utilization/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/utilization/boot_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/utilization/utilization_json.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.322904 newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_agent_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_aws_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_azure_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_boot_id_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_cat_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_collector_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_datstore_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_gcp_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_labels_and_rollups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_lambda_event_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_pcf_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_rum_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_sql_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_transaction_segment_terms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_utilization_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/cross_agent/test_w3c_trace_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.322904 newrelic-8.8.0/tests/datastore_aioredis/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aioredis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.326904 newrelic-8.8.0/tests/datastore_aredis/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aredis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aredis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aredis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aredis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aredis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aredis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aredis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aredis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_aredis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.326904 newrelic-8.8.0/tests/datastore_asyncpg/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_asyncpg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_asyncpg/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_asyncpg/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.326904 newrelic-8.8.0/tests/datastore_bmemcached/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_bmemcached/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_bmemcached/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.326904 newrelic-8.8.0/tests/datastore_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_elasticsearch/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_elasticsearch/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_elasticsearch/test_database_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_elasticsearch/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_elasticsearch/test_instrumented_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_elasticsearch/test_mget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_elasticsearch/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_elasticsearch/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_elasticsearch/test_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.326904 newrelic-8.8.0/tests/datastore_memcache/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_memcache/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_memcache/test_all_methods_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_memcache/test_memcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_memcache/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_memcache/test_span_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.326904 newrelic-8.8.0/tests/datastore_mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_mysql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_mysql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.326904 newrelic-8.8.0/tests/datastore_postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_postgresql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_postgresql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_psycopg2/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_database_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_explain_plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_forward_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_rollback.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_slow_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_psycopg2cffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2cffi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2cffi/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_psycopg2cffi/test_explain_plans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_pyelasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pyelasticsearch/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pyelasticsearch/test_pyelasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_pylibmc/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pylibmc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pylibmc/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_pymemcache/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pymemcache/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pymemcache/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_pymongo/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pymongo/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pymongo/test_pymongo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_pymysql/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pymysql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pymysql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_pysolr/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pysolr/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_pysolr/test_solr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_redis/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/test_rb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_redis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_solrpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_solrpy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_solrpy/test_solr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_sqlite/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_sqlite/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_sqlite/test_obfuscation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.330904 newrelic-8.8.0/tests/datastore_umemcache/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_umemcache/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/datastore_umemcache/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/external_boto3/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_boto3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_boto3/test_boto3_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_boto3/test_boto3_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_boto3/test_boto3_sns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/external_botocore/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_botocore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_botocore/test_botocore_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_botocore/test_botocore_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_botocore/test_botocore_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_botocore/test_botocore_sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/external_feedparser/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_feedparser/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_feedparser/packages.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_feedparser/test_feedparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/external_http/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_http/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_http/test_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/external_httplib/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_httplib/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_httplib/test_httplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_httplib/test_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_httplib/test_urllib2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/external_httplib2/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_httplib2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_httplib2/test_httplib2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/external_httpx/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_httpx/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_httpx/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/external_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_requests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_requests/test_span_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/external_urllib3/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_urllib3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/external_urllib3/test_urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.334904 newrelic-8.8.0/tests/framework_aiohttp/
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/test_client_async_await.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/test_client_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/test_externals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/test_server_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_aiohttp/test_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.338904 newrelic-8.8.0/tests/framework_ariadne/
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_ariadne/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_ariadne/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_ariadne/schema.graphql
--rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_ariadne/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_ariadne/test_application_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_ariadne/test_asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_ariadne/test_wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.338904 newrelic-8.8.0/tests/framework_bottle/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_bottle/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_bottle/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_bottle/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.338904 newrelic-8.8.0/tests/framework_cherrypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_cherrypy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_cherrypy/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_cherrypy/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_cherrypy/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_cherrypy/test_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.338904 newrelic-8.8.0/tests/framework_django/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.338904 newrelic-8.8.0/tests/framework_django/dummy_app/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/dummy_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.338904 newrelic-8.8.0/tests/framework_django/dummy_app/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/dummy_app/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/dummy_app/templatetags/custom_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.338904 newrelic-8.8.0/tests/framework_django/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/templates/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/templates/render_exception.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/templates/results.html
--rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/test_asgi_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_django/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.338904 newrelic-8.8.0/tests/framework_falcon/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_falcon/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_falcon/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_falcon/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.338904 newrelic-8.8.0/tests/framework_fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_fastapi/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_fastapi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_fastapi/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.342904 newrelic-8.8.0/tests/framework_flask/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/_test_application_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/_test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/_test_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/_test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/_test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/_test_user_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/_test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/_test_views_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/test_user_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_flask/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.342904 newrelic-8.8.0/tests/framework_graphene/
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_graphene/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_graphene/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_graphene/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.342904 newrelic-8.8.0/tests/framework_graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_graphql/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_graphql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_graphql/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_graphql/test_application_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.342904 newrelic-8.8.0/tests/framework_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/_test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.342904 newrelic-8.8.0/tests/framework_grpc/sample_application/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/sample_application/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/sample_application/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/sample_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/sample_application/sample_application.proto
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_grpc/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.346904 newrelic-8.8.0/tests/framework_pyramid/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_pyramid/_test_append_slash_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_pyramid/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_pyramid/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_pyramid/test_append_slash_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_pyramid/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_pyramid/test_cornice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.346904 newrelic-8.8.0/tests/framework_sanic/
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_sanic/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_sanic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_sanic/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_sanic/test_cross_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.346904 newrelic-8.8.0/tests/framework_starlette/
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_starlette/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_starlette/_test_bg_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_starlette/_test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_starlette/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_starlette/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_starlette/test_bg_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_starlette/test_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.346904 newrelic-8.8.0/tests/framework_strawberry/
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_strawberry/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_strawberry/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_strawberry/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_strawberry/test_application_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_strawberry/test_asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.346904 newrelic-8.8.0/tests/framework_tornado/
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_tornado/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_tornado/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_tornado/test_custom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_tornado/test_externals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_tornado/test_inbound_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/framework_tornado/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.346904 newrelic-8.8.0/tests/logger_logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_logging/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_logging/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_logging/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_logging/test_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_logging/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_logging/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.346904 newrelic-8.8.0/tests/logger_loguru/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_loguru/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_loguru/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_loguru/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_loguru/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_loguru/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/logger_loguru/test_stack_inspection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.350904 newrelic-8.8.0/tests/messagebroker_confluentkafka/
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_confluentkafka/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_confluentkafka/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_confluentkafka/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_confluentkafka/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.350904 newrelic-8.8.0/tests/messagebroker_kafkapython/
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_kafkapython/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_kafkapython/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_kafkapython/test_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_kafkapython/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_kafkapython/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.350904 newrelic-8.8.0/tests/messagebroker_pika/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/minversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/test_memory_leak.py
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/test_pika_async_connection_consume.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/test_pika_produce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/messagebroker_pika/test_pika_supportability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.350904 newrelic-8.8.0/tests/template_mako/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/template_mako/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/template_mako/test_mako.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.350904 newrelic-8.8.0/tests/testing_support/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/asgi_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/db_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/external_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.350904 newrelic-8.8.0/tests/testing_support/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/fixture/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    61831 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/mock_external_grpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/mock_external_http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/mock_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/sample_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/sample_asgi_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:18:06.358904 newrelic-8.8.0/tests/testing_support/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_apdex_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_application_error_event_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_application_error_trace_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_application_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_cross_process_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_custom_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_database_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_database_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_database_trace_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_datastore_trace_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_distributed_trace_accepted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_distributed_tracing_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_error_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_error_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_error_trace_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_external_node_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_function_called.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_internal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_log_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_log_event_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_log_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_log_events_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_messagebroker_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_metric_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_non_transaction_error_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_outbound_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_serverless_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_serverless_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_serverless_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_slow_sql_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_span_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_sql_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_synthetics_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_transaction_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_transaction_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_transaction_event_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_transaction_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_transaction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_transaction_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-03-30 21:17:49.000000 newrelic-8.8.0/tests/testing_support/validators/validate_tt_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    25750 2023-03-30 21:17:49.000000 newrelic-8.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.301334 newrelic-8.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 21:30:38.000000 newrelic-8.8.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 21:30:38.000000 newrelic-8.8.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/ISSUE_TEMPLATE/troubleshooting.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.153334 newrelic-8.8.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/actions/setup-python-matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/actions/setup-python-matrix/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/containers/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/containers/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1704 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/containers/install-python.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/containers/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1263 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/scripts/retry.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/build-ci-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/deploy-python.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      964 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/get-envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22953 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-26 21:30:38.000000 newrelic-8.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-26 21:30:38.000000 newrelic-8.8.1/.mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-06-26 21:30:38.000000 newrelic-8.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-26 21:30:38.000000 newrelic-8.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-26 21:30:38.000000 newrelic-8.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-26 21:30:53.301334 newrelic-8.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-26 21:30:38.000000 newrelic-8.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-26 21:30:38.000000 newrelic-8.8.1/ROADMAP.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-26 21:30:38.000000 newrelic-8.8.1/THIRD_PARTY_NOTICES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-26 21:30:38.000000 newrelic-8.8.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.165334 newrelic-8.8.1/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.165334 newrelic-8.8.1/newrelic/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/debug_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/license_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/network_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/record_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/run_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/server_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/validate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.169334 newrelic-8.8.1/newrelic/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/asgi_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/background_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/cat_header_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/database_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/datastore_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/error_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/external_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/function_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/function_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/generator_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/graphql_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/html_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/in_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/memcache_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/message_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/message_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/object_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/out_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/post_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/pre_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/profile_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/solr_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/supportability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26330 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/time_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69566 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/transaction_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35165 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/web_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25411 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/wsgi_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.169334 newrelic-8.8.1/newrelic/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/bootstrap/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.173334 newrelic-8.8.1/newrelic/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/_monotonic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/agent_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/async_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64813 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18641 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/encoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/log_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/object_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/object_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/package_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/streaming_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114637 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18465 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.177334 newrelic-8.8.1/newrelic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/_thread_utilization.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/adaptive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31544 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/agent_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/agent_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70315 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40694 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/database_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/datastore_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/error_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/error_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/external_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/graphql_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/graphql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/infinite_tracing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/infinite_tracing_v3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/infinite_tracing_v4_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/internal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/log_event_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/loop_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/memcache_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/message_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/node_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16490 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/profile_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/root_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/rules_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/solr_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/stack_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64178 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/stats_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/string_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/thread_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/trace_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22650 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/transaction_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.181334 newrelic-8.8.1/newrelic/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.181334 newrelic-8.8.1/newrelic/extras/framework_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/extras/framework_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.181334 newrelic-8.8.1/newrelic/extras/framework_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/extras/framework_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/extras/framework_django/templatetags/newrelic_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_asgiref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_cheroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_cherrypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_daphne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_flup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_gevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_hypercorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_meinheld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_paste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_uvicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_waitress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_wsgiref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/application_celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/application_gearman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_cornice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_djangorestframework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_flask_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_graphqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_piston.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_tastypie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/coroutines_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/coroutines_gevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_cx_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_ibm_db_dbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_oursql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_psycopg2cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_psycopg2ct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_pymssql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_pymysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_pyodbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_aioredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_aredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_bmemcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21862 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pyelasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pylibmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pymemcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pysolr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_solrpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_umemcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_botocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_facepy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_feedparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_pywapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_thrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_urllib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_xmlrpclib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_cherrypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42753 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_django_py3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_graphene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17278 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_pylons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_sanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_web2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_webpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/logger_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/logger_loguru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/memcache_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/messagebroker_confluentkafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/messagebroker_kafkapython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/messagebroker_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/middleware_flask_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/middleware_weberror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/template_genshi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/template_jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/template_mako.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/network/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/network/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/newrelic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/asgiref_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/packages/isort/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/packages/isort/stdlibs/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py27.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py311.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py36.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py37.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py38.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py39.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34549 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/six.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95815 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/_wrappers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35521 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/gc_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/memory_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.165334 newrelic-8.8.1/newrelic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54801 2023-06-26 21:30:53.000000 newrelic-8.8.1/newrelic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 21:30:38.000000 newrelic-8.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/scripts/newrelic-admin
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 21:30:53.301334 newrelic-8.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-06-26 21:30:38.000000 newrelic-8.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_cheroot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_cheroot/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_cheroot/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_daphne/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_daphne/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_daphne/test_daphne.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_gevent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gevent/_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gevent/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gevent/test_patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gevent/test_pywsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/asgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/async_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/test_aiohttp_app_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/test_asgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/test_gaiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_hypercorn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_hypercorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_hypercorn/test_hypercorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_uvicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_uvicorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_uvicorn/test_uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.205334 newrelic-8.8.1/tests/adapter_waitress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_waitress/_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_waitress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_waitress/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.209334 newrelic-8.8.1/tests/agent_features/
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/_test_async_coroutine_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/_test_async_coroutine_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/_test_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_apdex_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32524 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_asgi_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_asgi_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_asgi_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_asgi_w3c_trace_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_async_context_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_async_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35695 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_attributes_in_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_background_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33137 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_browser_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_collector_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20320 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_coroutine_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_coroutine_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_custom_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_dead_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_error_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_error_group_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_event_loop_wait_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12523 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_exception_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_function_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24665 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_high_security_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_ignore_expected_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_log_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_logs_in_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_notice_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_priority_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_serverless_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24778 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_stack_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_supportability_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_synthetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_time_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_transaction_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_transaction_trace_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_w3c_trace_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_web_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_wsgi_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.209334 newrelic-8.8.1/tests/agent_streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/_test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/test_infinite_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/test_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/test_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/test_streaming_rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/agent_unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/_test_import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_agent_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_agent_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_check_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_connect_response_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_distributed_tracing_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_full_uri_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_harvest_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20941 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_infinite_trace_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_package_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_region_aware_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_sampler_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_serverless_mode_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_trace_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_utilization_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/application_celery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_celery/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_celery/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_celery/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_celery/test_celery_max_tasks_per_child.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/application_gearman/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_gearman/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_gearman/test_gearman.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/component_djangorestframework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/component_flask_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_flask_rest/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_flask_rest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_flask_rest/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/component_graphqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_graphqlserver/_test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_graphqlserver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_graphqlserver/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/component_tastypie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/coroutines_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/coroutines_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/coroutines_asyncio/test_context_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.217334 newrelic-8.8.1/tests/cross_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.217334 newrelic-8.8.1/tests/cross_agent/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/attribute_configuration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/cat_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/collector_hostname.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.217334 newrelic-8.8.1/tests/cross_agent/fixtures/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/datastores/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/datastores/datastore_instances.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.221334 newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    48250 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58950 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/trace_context.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.221334 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/cases.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-0.9.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/heroku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/invalid-length.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-lxc-container.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-no-container.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.10-no-container.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/labels.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.225334 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/api_gateway_auth.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/batch_get.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/batch_submit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudformation_create.json
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudwatch_logs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/codecommit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cognito_sync.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_analytics.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_apache.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_invoke.json
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/lex_appointment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/lex_book_car.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/s3_put.json
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/scheduled_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/ses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/smarthome_discovery.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/smarthome_turn_off.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/sns.json
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/sqs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.233334 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.query.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.237334 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_1logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_2core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/malformed_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.237334 newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/malformed_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_client_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_cookie.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.237334 newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/close-body-in-comment.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/dynamic-iframe.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.241334 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/empty_head
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.245334 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.245334 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.245334 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_parsing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/transaction_segment_terms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/url_clean.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/url_domain_extraction.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.245334 newrelic-8.8.1/tests/cross_agent/fixtures/utilization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization/boot_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization/utilization_json.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_agent_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_aws_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_azure_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_boot_id_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_cat_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_collector_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_datstore_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_gcp_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_labels_and_rollups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_lambda_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_pcf_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_rum_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_sql_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_transaction_segment_terms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_utilization_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_w3c_trace_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_aioredis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_aredis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_asyncpg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_asyncpg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_asyncpg/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_asyncpg/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_bmemcached/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_bmemcached/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_bmemcached/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_database_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_instrumented_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_mget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_memcache/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/test_all_methods_wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/test_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/test_span_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_mysql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_mysql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_postgresql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_postgresql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_psycopg2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_database_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_explain_plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_forward_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_rollback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_slow_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_psycopg2cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2cffi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2cffi/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2cffi/test_explain_plans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pylibmc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pylibmc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pylibmc/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pymemcache/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymemcache/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymemcache/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pymongo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymongo/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymongo/test_pymongo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pymysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymysql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymysql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pyodbc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pyodbc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pyodbc/test_pyodbc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pysolr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pysolr/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pysolr/test_solr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.261334 newrelic-8.8.1/tests/datastore_redis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_rb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.261334 newrelic-8.8.1/tests/datastore_solrpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_solrpy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_solrpy/test_solr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.261334 newrelic-8.8.1/tests/datastore_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_sqlite/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_sqlite/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_sqlite/test_obfuscation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.261334 newrelic-8.8.1/tests/external_boto3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_boto3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_boto3/test_boto3_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_boto3/test_boto3_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_boto3/test_boto3_sns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_botocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/test_botocore_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/test_botocore_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/test_botocore_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/test_botocore_sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_feedparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_feedparser/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_feedparser/packages.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_feedparser/test_feedparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_http/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_http/test_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_httplib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib/test_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib/test_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib/test_urllib2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_httplib2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib2/test_httplib2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_httpx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httpx/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httpx/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_requests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_requests/test_span_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_urllib3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_urllib3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_urllib3/test_urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_client_async_await.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_client_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_externals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_server_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_ariadne/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/schema.graphql
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/test_application_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/test_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_bottle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_bottle/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_bottle/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_bottle/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_cherrypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_django/dummy_app/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/dummy_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/custom_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_django/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/templates/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/templates/render_exception.html
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/templates/results.html
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/test_asgi_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_falcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_falcon/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_falcon/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_falcon/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_fastapi/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_fastapi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_fastapi/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.277334 newrelic-8.8.1/tests/framework_flask/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_application_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_user_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_views_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_user_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.277334 newrelic-8.8.1/tests/framework_graphene/
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphene/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphene/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphene/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.277334 newrelic-8.8.1/tests/framework_graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphql/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphql/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphql/test_application_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.277334 newrelic-8.8.1/tests/framework_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/_test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.281334 newrelic-8.8.1/tests/framework_grpc/sample_application/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/sample_application/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/sample_application/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/sample_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/sample_application/sample_application.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.281334 newrelic-8.8.1/tests/framework_pyramid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/_test_append_slash_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/test_append_slash_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/test_cornice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.285334 newrelic-8.8.1/tests/framework_sanic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_sanic/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_sanic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_sanic/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_sanic/test_cross_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/framework_starlette/
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/_test_bg_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/_test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/test_bg_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/framework_strawberry/
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/test_application_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/test_asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/framework_tornado/
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/test_custom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/test_externals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/test_inbound_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/logger_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/logger_loguru/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_stack_inspection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/messagebroker_confluentkafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_confluentkafka/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_confluentkafka/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_confluentkafka/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_confluentkafka/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/messagebroker_kafkapython/
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/test_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/messagebroker_pika/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/minversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_memory_leak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_async_connection_consume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_blocking_connection_consume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_produce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_supportability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/template_genshi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/template_genshi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/template_genshi/test_genshi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/template_mako/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/template_mako/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/template_mako/test_mako.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/testing_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/asgi_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/db_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/external_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/testing_support/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/fixture/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50495 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/mock_external_grpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/mock_external_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/mock_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/sample_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/sample_asgi_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.301334 newrelic-8.8.1/tests/testing_support/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_apdex_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_application_error_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_application_error_trace_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_application_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_browser_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_cross_process_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_custom_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_database_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_database_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_database_trace_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_datastore_trace_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_distributed_trace_accepted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_distributed_tracing_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_event_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_external_node_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_function_called.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_internal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_event_count_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_events_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_messagebroker_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_metric_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_non_transaction_error_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_outbound_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_serverless_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_serverless_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_serverless_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_slow_sql_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_sql_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_synthetics_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_synthetics_transaction_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_time_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_error_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_event_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_slow_sql_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_tt_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_tt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_tt_segment_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26114 2023-06-26 21:30:38.000000 newrelic-8.8.1/tox.ini
```

### Comparing `newrelic-8.8.0/.devcontainer/devcontainer.json` & `newrelic-8.8.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `newrelic-8.8.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.github/ISSUE_TEMPLATE/config.yml` & `newrelic-8.8.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `newrelic-8.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.github/actions/setup-python-matrix/action.yml` & `newrelic-8.8.1/.github/actions/setup-python-matrix/action.yml`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,18 @@
   using: "composite"
   steps:
     - uses: actions/setup-python@v4
       with:
         python-version: "pypy-3.7"
         architecture: x64
 
-    - uses: actions/setup-python@v4
-      with:
-        python-version: "pypy-2.7"
-        architecture: x64
+    # - uses: actions/setup-python@v4
+    #   with:
+    #     python-version: "pypy-2.7"
+    #     architecture: x64
 
     - uses: actions/setup-python@v4
       with:
         python-version: "3.7"
         architecture: x64
 
     - uses: actions/setup-python@v4
@@ -34,17 +34,17 @@
         architecture: x64
 
     - uses: actions/setup-python@v4
       with:
         python-version: "3.11"
         architecture: x64
 
-    - uses: actions/setup-python@v4
-      with:
-        python-version: "2.7"
-        architecture: x64
+    # - uses: actions/setup-python@v4
+    #   with:
+    #     python-version: "2.7"
+    #     architecture: x64
 
     - name: Install Dependencies
       shell: bash
       run: |
         python3.10 -m pip install -U pip
-        python3.10 -m pip install -U wheel setuptools 'tox<4' virtualenv!=20.0.24
+        python3.10 -m pip install -U wheel setuptools tox 'virtualenv<20.22.0'
```

### Comparing `newrelic-8.8.0/.github/mergify.yml` & `newrelic-8.8.1/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.github/pull_request_template.md` & `newrelic-8.8.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.github/stale.yml` & `newrelic-8.8.1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.github/workflows/deploy-python.yml` & `newrelic-8.8.1/.github/workflows/deploy-python.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.github/workflows/mega-linter.yml` & `newrelic-8.8.1/.github/workflows/mega-linter.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.github/workflows/tests.yml` & `newrelic-8.8.1/.github/workflows/tests.yml`

 * *Files 26% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     runs-on: ubuntu-20.04
     needs:
       - python
       - elasticsearchserver07
       - elasticsearchserver08
       - gearman
       - grpc
-      - kafka
-      - libcurl
+      #- kafka
       - memcached
       - mongodb
       - mysql
       - postgres
       - rabbitmq
       - redis
       - solr
@@ -57,14 +56,15 @@
     if: success() || failure() # Does not run on cancelled workflows
     runs-on: ubuntu-20.04
     needs:
       - tests
 
     steps:
       - uses: actions/checkout@v3
+
       - uses: actions/setup-python@v4
         with:
           python-version: "3.10"
           architecture: x64
 
       - name: Download Coverage Artifacts
         uses: actions/download-artifact@v3
@@ -113,110 +113,83 @@
             17,
             18,
             19,
             20,
           ]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
-
-      - name: Get Environments
-        id: get-envs
-        run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
-        env:
-          GROUP_NUMBER: ${{ matrix.group-number }}
 
-      - name: Test
+      - name: Fetch git tags
         run: |
-          tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
-        env:
-          TOX_PARALLEL_NO_SPINNER: 1
-          PY_COLORS: 0
-
-      - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v3
-        with:
-          name: coverage-${{ github.job }}-${{ strategy.job-index }}
-          path: ./**/.coverage.*
-          retention-days: 1
-
-  grpc:
-    env:
-      TOTAL_GROUPS: 1
-
-    strategy:
-      fail-fast: false
-      matrix:
-        group-number: [1]
-
-    runs-on: ubuntu-20.04
-    timeout-minutes: 30
-
-    steps:
-      - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
-          tox -vv -e ${{ steps.get-envs.outputs.envs }}
+          tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
         uses: actions/upload-artifact@v3
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
-  libcurl:
+  grpc:
     env:
       TOTAL_GROUPS: 1
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
 
-      # Special case packages
-      - name: Install libcurl-dev
+      - name: Fetch git tags
         run: |
-          sudo apt-get update
-          sudo apt-get install libcurl4-openssl-dev
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
-          tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
+          tox -vv -e ${{ steps.get-envs.outputs.envs }}
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
         uses: actions/upload-artifact@v3
         with:
@@ -230,14 +203,18 @@
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1, 2]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       postgres:
         image: postgres:9
         env:
           POSTGRES_PASSWORD: postgres
@@ -249,20 +226,24 @@
           --health-cmd pg_isready
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
@@ -282,14 +263,18 @@
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1, 2]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       mysql:
         image: mysql:5.6
         env:
           MYSQL_RANDOM_ROOT_PASSWORD: "true"
@@ -304,20 +289,24 @@
           --health-cmd "mysqladmin ping -h localhost"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
@@ -337,14 +326,18 @@
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1, 2]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       redis:
         image: redis
         ports:
           - 8080:6379
@@ -354,20 +347,24 @@
           --health-cmd "redis-cli ping"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
@@ -387,14 +384,18 @@
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       solr:
         image: bitnami/solr:8.8.2
         env:
           SOLR_CORE: collection
@@ -406,20 +407,24 @@
           --health-cmd "curl localhost:8983/solr/collection/admin/ping | grep OK"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
@@ -439,14 +444,18 @@
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1, 2]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       memcached:
         image: memcached
         ports:
           - 8080:11211
@@ -456,20 +465,24 @@
           --health-cmd "timeout 5 bash -c 'cat < /dev/null > /dev/udp/127.0.0.1/11211'"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
@@ -489,14 +502,18 @@
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       rabbitmq:
         image: rabbitmq
         env:
           RABBITMQ_PASSWORD: rabbitmq
@@ -507,20 +524,24 @@
           --health-cmd "rabbitmq-diagnostics status"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
@@ -530,96 +551,108 @@
       - name: Upload Coverage Artifacts
         uses: actions/upload-artifact@v3
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
-  kafka:
-    env:
-      TOTAL_GROUPS: 4
+  # kafka:
+  #   env:
+  #     TOTAL_GROUPS: 4
 
-    strategy:
-      fail-fast: false
-      matrix:
-        group-number: [1, 2, 3, 4]
+  #   strategy:
+  #     fail-fast: false
+  #     matrix:
+  #       group-number: [1, 2, 3, 4]
 
-    runs-on: ubuntu-20.04
-    timeout-minutes: 30
+  #   runs-on: ubuntu-20.04
+  #   container:
+  #     image: ghcr.io/${{ github.repository }}-ci:latest
+  #     options: >-
+  #       --add-host=host.docker.internal:host-gateway
+  #   timeout-minutes: 30
 
-    services:
-      zookeeper:
-        image: bitnami/zookeeper:3.7
-        env:
-          ALLOW_ANONYMOUS_LOGIN: yes
+  #   services:
+  #     zookeeper:
+  #       image: bitnami/zookeeper:3.7
+  #       env:
+  #         ALLOW_ANONYMOUS_LOGIN: yes
 
-        ports:
-          - 2181:2181
+  #       ports:
+  #         - 2181:2181
 
-      kafka:
-        image: bitnami/kafka:3.2
-        ports:
-          - 8080:8080
-          - 8081:8081
-        env:
-          ALLOW_PLAINTEXT_LISTENER: yes
-          KAFKA_ZOOKEEPER_CONNECT: zookeeper:2181
-          KAFKA_CFG_AUTO_CREATE_TOPICS_ENABLE: true
-          KAFKA_CFG_LISTENERS: L1://:8080,L2://:8081
-          KAFKA_CFG_ADVERTISED_LISTENERS: L1://127.0.0.1:8080,L2://kafka:8081,
-          KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP: L1:PLAINTEXT,L2:PLAINTEXT
-          KAFKA_CFG_INTER_BROKER_LISTENER_NAME: L2
+  #     kafka:
+  #       image: bitnami/kafka:3.2
+  #       ports:
+  #         - 8080:8080
+  #         - 8081:8081
+  #       env:
+  #         ALLOW_PLAINTEXT_LISTENER: yes
+  #         KAFKA_ZOOKEEPER_CONNECT: zookeeper:2181
+  #         KAFKA_CFG_AUTO_CREATE_TOPICS_ENABLE: true
+  #         KAFKA_CFG_LISTENERS: L1://:8080,L2://:8081
+  #         KAFKA_CFG_ADVERTISED_LISTENERS: L1://127.0.0.1:8080,L2://kafka:8081,
+  #         KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP: L1:PLAINTEXT,L2:PLAINTEXT
+  #         KAFKA_CFG_INTER_BROKER_LISTENER_NAME: L2
 
-    steps:
-      - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+  #   steps:
+  #     - uses: actions/checkout@v3
 
-      # Special case packages
-      - name: Install librdkafka-dev
-        run: |
-          # Use lsb-release to find the codename of Ubuntu to use to install the correct library name
-          sudo apt-get update
-          sudo ln -fs /usr/share/zoneinfo/America/Los_Angeles /etc/localtime
-          sudo apt-get install -y wget gnupg2 software-properties-common
-          sudo wget -qO - https://packages.confluent.io/deb/7.2/archive.key | sudo apt-key add -
-          sudo add-apt-repository "deb https://packages.confluent.io/clients/deb $(lsb_release -cs) main"
-          sudo apt-get update
-          sudo apt-get install -y librdkafka-dev/$(lsb_release -c | cut -f 2)
+  #     - name: Fetch git tags
+  #       run: |
+  #         git config --global --add safe.directory "$GITHUB_WORKSPACE"
+  #         git fetch --tags origin
 
-      - name: Get Environments
-        id: get-envs
-        run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
-        env:
-          GROUP_NUMBER: ${{ matrix.group-number }}
+  #     # Special case packages
+  #     - name: Install librdkafka-dev
+  #       run: |
+  #         # Use lsb-release to find the codename of Ubuntu to use to install the correct library name
+  #         sudo apt-get update
+  #         sudo ln -fs /usr/share/zoneinfo/America/Los_Angeles /etc/localtime
+  #         sudo apt-get install -y wget gnupg2 software-properties-common
+  #         sudo wget -qO - https://packages.confluent.io/deb/7.2/archive.key | sudo apt-key add -
+  #         sudo add-apt-repository "deb https://packages.confluent.io/clients/deb $(lsb_release -cs) main"
+  #         sudo apt-get update
+  #         sudo apt-get install -y librdkafka-dev/$(lsb_release -c | cut -f 2)
 
-      - name: Test
-        run: |
-          tox -vv -e ${{ steps.get-envs.outputs.envs }}
-        env:
-          TOX_PARALLEL_NO_SPINNER: 1
-          PY_COLORS: 0
+  #     - name: Get Environments
+  #       id: get-envs
+  #       run: |
+  #         echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
+  #       env:
+  #         GROUP_NUMBER: ${{ matrix.group-number }}
 
-      - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v3
-        with:
-          name: coverage-${{ github.job }}-${{ strategy.job-index }}
-          path: ./**/.coverage.*
-          retention-days: 1
+  #     - name: Test
+  #       run: |
+  #         tox -vv -e ${{ steps.get-envs.outputs.envs }}
+  #       env:
+  #         TOX_PARALLEL_NO_SPINNER: 1
+  #         PY_COLORS: 0
+
+  #     - name: Upload Coverage Artifacts
+  #       uses: actions/upload-artifact@v3
+  #       with:
+  #         name: coverage-${{ github.job }}-${{ strategy.job-index }}
+  #         path: ./**/.coverage.*
+  #         retention-days: 1
 
   mongodb:
     env:
       TOTAL_GROUPS: 1
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       mongodb:
         image: mongo:3.6.4
         ports:
           - 8080:27017
@@ -629,20 +662,24 @@
           --health-cmd "echo 'db.runCommand(\"ping\").ok' | mongo localhost:27017/test --quiet || exit 1"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
@@ -662,18 +699,22 @@
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
-      es07:
+      elasticsearch:
         image: elasticsearch:7.17.8
         env:
           "discovery.type": "single-node"
         ports:
           - 8080:9200
           - 8081:9200
         # Set health checks to wait until elasticsearch has started
@@ -681,20 +722,24 @@
           --health-cmd "curl --silent --fail localhost:9200/_cluster/health || exit 1"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
@@ -714,18 +759,22 @@
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
-      es08:
+      elasticsearch:
         image: elasticsearch:8.6.0
         env:
           "xpack.security.enabled": "false"
           "discovery.type": "single-node"
         ports:
           - 8080:9200
           - 8081:9200
@@ -734,20 +783,24 @@
           --health-cmd "curl --silent --fail localhost:9200/_cluster/health || exit 1"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
@@ -767,36 +820,44 @@
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/${{ github.repository }}-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       gearman:
         image: artefactual/gearmand
         ports:
-          - 4730:4730
+          - 8080:4730
         # Set health checks to wait until gearman has started
         options: >-
           --health-cmd "(echo status ; sleep 0.1) | nc 127.0.0.1 4730 -w 1"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
       - uses: actions/checkout@v3
-      - uses: ./.github/actions/setup-python-matrix
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
 
       - name: Get Environments
         id: get-envs
         run: |
-          echo "::set-output name=envs::$(tox -l | grep "^${{ github.job }}\-" | ./.github/workflows/get-envs.py)"
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
         env:
           GROUP_NUMBER: ${{ matrix.group-number }}
 
       - name: Test
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
```

### Comparing `newrelic-8.8.0/.gitignore` & `newrelic-8.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/.mega-linter.yml` & `newrelic-8.8.1/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/CONTRIBUTING.rst` & `newrelic-8.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/LICENSE` & `newrelic-8.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/PKG-INFO` & `newrelic-8.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic
-Version: 8.8.0
+Version: 8.8.1
 Summary: New Relic Python Agent
 Home-page: https://docs.newrelic.com/docs/apm/agents/python-agent/
 Author: New Relic
 Author-email: support@newrelic.com
 Maintainer: New Relic
 Maintainer-email: support@newrelic.com
 License: Apache-2.0
```

### Comparing `newrelic-8.8.0/README.rst` & `newrelic-8.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/ROADMAP.md` & `newrelic-8.8.1/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/THIRD_PARTY_NOTICES.md` & `newrelic-8.8.1/THIRD_PARTY_NOTICES.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,46 +10,55 @@
 
 ## [asgiref](https://pypi.org/project/asgiref/)
 
 Copyright (c) Django Software Foundation and individual contributors.
 
 Distributed under the following license(s):
 
-  * [The BSD 3-Clause License](https://opensource.org/licenses/BSD-3-Clause)
+* [The BSD 3-Clause License](https://opensource.org/licenses/BSD-3-Clause)
+
+
+## [isort](https://pypi.org/project/isort)
+
+Copyright (c) 2013 Timothy Edmund Crosley
+
+Distributed under the following license(s):
+
+* [The MIT License](http://opensource.org/licenses/MIT)
 
 
 ## [six](https://pypi.org/project/six)
 
 Copyright (c) 2010-2013 Benjamin Peterson
 
 Distributed under the following license(s):
 
-  * [The MIT License](http://opensource.org/licenses/MIT)
+* [The MIT License](http://opensource.org/licenses/MIT)
 
 
 ## [time.monotonic](newrelic/common/_monotonic.c)
 
 Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013 Python Software Foundation; All Rights Reserved
 
 Distributed under the following license(s):
 
-  * [Python Software Foundation](https://docs.python.org/3/license.html)
+* [Python Software Foundation](https://docs.python.org/3/license.html)
 
 
 ## [urllib3](https://pypi.org/project/urllib3)
 
 Copyright (c) 2008-2019 Andrey Petrov and contributors (see CONTRIBUTORS.txt)
 
 Distributed under the following license(s):
 
-  * [The MIT License](http://opensource.org/licenses/MIT)
+* [The MIT License](http://opensource.org/licenses/MIT)
 
 
 ## [wrapt](https://pypi.org/project/wrapt)
 
 Copyright (c) 2013-2019, Graham Dumpleton
 All rights reserved.
 
 Distributed under the following license(s):
 
-  * [The BSD 2-Clause License](http://opensource.org/licenses/BSD-2-Clause)
+* [The BSD 2-Clause License](http://opensource.org/licenses/BSD-2-Clause)
```

### Comparing `newrelic-8.8.0/newrelic/__init__.py` & `newrelic-8.8.1/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/__init__.py` & `newrelic-8.8.1/newrelic/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/__main__.py` & `newrelic-8.8.1/newrelic/admin/__main__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/debug_console.py` & `newrelic-8.8.1/newrelic/admin/debug_console.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/generate_config.py` & `newrelic-8.8.1/newrelic/admin/generate_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/license_key.py` & `newrelic-8.8.1/newrelic/admin/license_key.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/local_config.py` & `newrelic-8.8.1/newrelic/admin/local_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/network_config.py` & `newrelic-8.8.1/newrelic/admin/network_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/record_deploy.py` & `newrelic-8.8.1/newrelic/admin/record_deploy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/run_program.py` & `newrelic-8.8.1/newrelic/admin/run_program.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/run_python.py` & `newrelic-8.8.1/newrelic/admin/run_python.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/server_config.py` & `newrelic-8.8.1/newrelic/admin/server_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/admin/validate_config.py` & `newrelic-8.8.1/newrelic/admin/validate_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/agent.py` & `newrelic-8.8.1/newrelic/agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/__init__.py` & `newrelic-8.8.1/newrelic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/application.py` & `newrelic-8.8.1/newrelic/api/application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/asgi_application.py` & `newrelic-8.8.1/newrelic/api/asgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/background_task.py` & `newrelic-8.8.1/newrelic/api/background_task.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/cat_header_mixin.py` & `newrelic-8.8.1/newrelic/api/cat_header_mixin.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/database_trace.py` & `newrelic-8.8.1/newrelic/api/database_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/datastore_trace.py` & `newrelic-8.8.1/newrelic/api/datastore_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/error_trace.py` & `newrelic-8.8.1/newrelic/api/error_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/exceptions.py` & `newrelic-8.8.1/newrelic/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/external_trace.py` & `newrelic-8.8.1/newrelic/api/external_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/function_profile.py` & `newrelic-8.8.1/newrelic/api/function_profile.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/function_trace.py` & `newrelic-8.8.1/newrelic/api/function_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/generator_trace.py` & `newrelic-8.8.1/newrelic/api/generator_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/graphql_trace.py` & `newrelic-8.8.1/newrelic/api/graphql_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/html_insertion.py` & `newrelic-8.8.1/newrelic/api/html_insertion.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/import_hook.py` & `newrelic-8.8.1/newrelic/api/import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/in_function.py` & `newrelic-8.8.1/newrelic/api/in_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/lambda_handler.py` & `newrelic-8.8.1/newrelic/api/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/log.py` & `newrelic-8.8.1/newrelic/api/log.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/memcache_trace.py` & `newrelic-8.8.1/newrelic/api/memcache_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/message_trace.py` & `newrelic-8.8.1/newrelic/api/message_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/message_transaction.py` & `newrelic-8.8.1/newrelic/api/message_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/object_wrapper.py` & `newrelic-8.8.1/newrelic/api/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/out_function.py` & `newrelic-8.8.1/newrelic/api/out_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/post_function.py` & `newrelic-8.8.1/newrelic/api/post_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/pre_function.py` & `newrelic-8.8.1/newrelic/api/pre_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/profile_trace.py` & `newrelic-8.8.1/newrelic/api/profile_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/settings.py` & `newrelic-8.8.1/newrelic/api/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/solr_trace.py` & `newrelic-8.8.1/newrelic/api/solr_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/supportability.py` & `newrelic-8.8.1/newrelic/api/supportability.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/time_trace.py` & `newrelic-8.8.1/newrelic/api/time_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/transaction.py` & `newrelic-8.8.1/newrelic/api/transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/transaction_name.py` & `newrelic-8.8.1/newrelic/api/transaction_name.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/web_transaction.py` & `newrelic-8.8.1/newrelic/api/web_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/api/wsgi_application.py` & `newrelic-8.8.1/newrelic/api/wsgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/bootstrap/__init__.py` & `newrelic-8.8.1/newrelic/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/bootstrap/sitecustomize.py` & `newrelic-8.8.1/newrelic/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/__init__.py` & `newrelic-8.8.1/newrelic/common/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/_monotonic.c` & `newrelic-8.8.1/newrelic/common/_monotonic.c`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/agent_http.py` & `newrelic-8.8.1/newrelic/common/agent_http.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/async_proxy.py` & `newrelic-8.8.1/newrelic/common/async_proxy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/async_wrapper.py` & `newrelic-8.8.1/newrelic/common/async_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/cacert.pem` & `newrelic-8.8.1/newrelic/common/cacert.pem`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/certs.py` & `newrelic-8.8.1/newrelic/common/certs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/coroutine.py` & `newrelic-8.8.1/newrelic/common/coroutine.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/encoding_utils.py` & `newrelic-8.8.1/newrelic/common/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/log_file.py` & `newrelic-8.8.1/newrelic/common/log_file.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/object_names.py` & `newrelic-8.8.1/newrelic/common/object_names.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/object_wrapper.py` & `newrelic-8.8.1/newrelic/common/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/package_version_utils.py` & `newrelic-8.8.1/newrelic/common/package_version_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,18 @@
 
 def _get_package_version(name):
     module = sys.modules.get(name, None)
     version = None
     for attr in VERSION_ATTRS:
         try:
             version = getattr(module, attr, None)
+            # In certain cases like importlib_metadata.version, version is a callable
+            # function.
+            if callable(version):
+                continue
             # Cast any version specified as a list into a tuple.
             version = tuple(version) if isinstance(version, list) else version
             if version not in NULL_VERSIONS:
                 return version
         except Exception:
             pass
 
@@ -91,8 +95,8 @@
 
     if "pkg_resources" in sys.modules:
         try:
             version = sys.modules["pkg_resources"].get_distribution(name).version
             if version not in NULL_VERSIONS:
                 return version
         except Exception:
-            pass
+            pass
```

### Comparing `newrelic-8.8.0/newrelic/common/stopwatch.py` & `newrelic-8.8.1/newrelic/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/streaming_utils.py` & `newrelic-8.8.1/newrelic/common/streaming_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/system_info.py` & `newrelic-8.8.1/newrelic/common/system_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/common/utilization.py` & `newrelic-8.8.1/newrelic/common/utilization.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/config.py` & `newrelic-8.8.1/newrelic/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3010,27 +3010,14 @@
 
     _process_module_definition(
         "cornice.service",
         "newrelic.hooks.component_cornice",
         "instrument_cornice_service",
     )
 
-    # _process_module_definition('twisted.web.server',
-    #        'newrelic.hooks.framework_twisted',
-    #        'instrument_twisted_web_server')
-    # _process_module_definition('twisted.web.http',
-    #        'newrelic.hooks.framework_twisted',
-    #        'instrument_twisted_web_http')
-    # _process_module_definition('twisted.web.resource',
-    #        'newrelic.hooks.framework_twisted',
-    #        'instrument_twisted_web_resource')
-    # _process_module_definition('twisted.internet.defer',
-    #        'newrelic.hooks.framework_twisted',
-    #        'instrument_twisted_internet_defer')
-
     _process_module_definition("gevent.monkey", "newrelic.hooks.coroutines_gevent", "instrument_gevent_monkey")
 
     _process_module_definition(
         "weberror.errormiddleware",
         "newrelic.hooks.middleware_weberror",
         "instrument_weberror_errormiddleware",
     )
```

### Comparing `newrelic-8.8.0/newrelic/console.py` & `newrelic-8.8.1/newrelic/console.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/__init__.py` & `newrelic-8.8.1/newrelic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/_thread_utilization.c` & `newrelic-8.8.1/newrelic/core/_thread_utilization.c`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/adaptive_sampler.py` & `newrelic-8.8.1/newrelic/core/adaptive_sampler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/agent.py` & `newrelic-8.8.1/newrelic/core/agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/agent_protocol.py` & `newrelic-8.8.1/newrelic/core/agent_protocol.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/agent_streaming.py` & `newrelic-8.8.1/newrelic/core/agent_streaming.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/application.py` & `newrelic-8.8.1/newrelic/core/application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/attribute.py` & `newrelic-8.8.1/newrelic/core/attribute.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/attribute_filter.py` & `newrelic-8.8.1/newrelic/core/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/code_level_metrics.py` & `newrelic-8.8.1/newrelic/core/code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/config.py` & `newrelic-8.8.1/newrelic/core/config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/context.py` & `newrelic-8.8.1/newrelic/core/context.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/custom_event.py` & `newrelic-8.8.1/newrelic/core/custom_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/data_collector.py` & `newrelic-8.8.1/newrelic/core/data_collector.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/database_node.py` & `newrelic-8.8.1/newrelic/core/database_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/database_utils.py` & `newrelic-8.8.1/newrelic/core/database_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/datastore_node.py` & `newrelic-8.8.1/newrelic/core/datastore_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/environment.py` & `newrelic-8.8.1/newrelic/core/environment.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,32 +13,35 @@
 # limitations under the License.
 
 """This module provides functions to collect information about the operating
 system, Python and hosting environment.
 
 """
 
+import logging
 import os
 import platform
 import sys
-import sysconfig
 
 import newrelic
 from newrelic.common.package_version_utils import get_package_version
 from newrelic.common.system_info import (
     logical_processor_count,
     physical_processor_count,
     total_physical_memory,
 )
+from newrelic.packages.isort import stdlibs as isort_stdlibs
 
 try:
     import newrelic.core._thread_utilization
 except ImportError:
     pass
 
+_logger = logging.getLogger(__name__)
+
 
 def environment_settings():
     """Returns an array of arrays of environment settings"""
     env = []
 
     # Agent information.
 
@@ -191,46 +194,66 @@
         tornado = sys.modules["tornado"]
         if hasattr(tornado, "version_info"):
             dispatcher.append(("Dispatcher Version", str(tornado.version_info)))
 
     env.extend(dispatcher)
 
     # Module information.
-    purelib = sysconfig.get_path("purelib")
-    platlib = sysconfig.get_path("platlib")
+    stdlib_builtin_module_names = _get_stdlib_builtin_module_names()
 
     plugins = []
 
     # Using any iterable to create a snapshot of sys.modules can occassionally
     # fail in a rare case when modules are imported in parallel by different
     # threads.
     #
     # TL;DR: Do NOT use an iterable on the original sys.modules to generate the
     # list
     for name, module in sys.modules.copy().items():
         # Exclude lib.sub_paths as independent modules except for newrelic.hooks.
-        if "." in name and not name.startswith("newrelic.hooks."):
+        nr_hook = name.startswith("newrelic.hooks.")
+        if "." in name and not nr_hook or name.startswith("_"):
             continue
+
         # If the module isn't actually loaded (such as failed relative imports
         # in Python 2.7), the module will be None and should not be reported.
         if not module:
             continue
+
         # Exclude standard library/built-in modules.
-        # Third-party modules can be installed in either purelib or platlib directories.
-        # See https://docs.python.org/3/library/sysconfig.html#installation-paths.
-        if (
-            not hasattr(module, "__file__")
-            or not module.__file__
-            or not module.__file__.startswith(purelib)
-            or not module.__file__.startswith(platlib)
-        ):
+        if name in stdlib_builtin_module_names:
             continue
 
         try:
             version = get_package_version(name)
-            plugins.append("%s (%s)" % (name, version))
         except Exception:
-            plugins.append(name)
+            version = None
+
+        # If it has no version it's likely not a real package so don't report it unless
+        # it's a new relic hook.
+        if version or nr_hook:
+            plugins.append("%s (%s)" % (name, version))
 
     env.append(("Plugin List", plugins))
 
     return env
+
+
+def _get_stdlib_builtin_module_names():
+    builtins = set(sys.builtin_module_names)
+    # Since sys.stdlib_module_names is not available in versions of python below 3.10,
+    # use isort's hardcoded stdlibs instead.
+    python_version = sys.version_info[0:2]
+    if python_version < (3,):
+        stdlibs = isort_stdlibs.py27.stdlib
+    elif (3, 7) <= python_version < (3, 8):
+        stdlibs = isort_stdlibs.py37.stdlib
+    elif python_version < (3, 9):
+        stdlibs = isort_stdlibs.py38.stdlib
+    elif python_version < (3, 10):
+        stdlibs = isort_stdlibs.py39.stdlib
+    elif python_version >= (3, 10):
+        stdlibs = sys.stdlib_module_names
+    else:
+        _logger.warn("Unsupported Python version. Unable to determine stdlibs.")
+        return builtins
+    return builtins | stdlibs
```

### Comparing `newrelic-8.8.0/newrelic/core/error_collector.py` & `newrelic-8.8.1/newrelic/core/error_collector.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/error_node.py` & `newrelic-8.8.1/newrelic/core/error_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/external_node.py` & `newrelic-8.8.1/newrelic/core/external_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/function_node.py` & `newrelic-8.8.1/newrelic/core/function_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/graphql_node.py` & `newrelic-8.8.1/newrelic/core/graphql_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/graphql_utils.py` & `newrelic-8.8.1/newrelic/core/graphql_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/infinite_tracing_pb2.py` & `newrelic-8.8.1/newrelic/core/infinite_tracing_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/infinite_tracing_v3_pb2.py` & `newrelic-8.8.1/newrelic/core/infinite_tracing_v3_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/infinite_tracing_v4_pb2.py` & `newrelic-8.8.1/newrelic/core/infinite_tracing_v4_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/internal_metrics.py` & `newrelic-8.8.1/newrelic/core/internal_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/log_event_node.py` & `newrelic-8.8.1/newrelic/core/log_event_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/loop_node.py` & `newrelic-8.8.1/newrelic/core/loop_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/memcache_node.py` & `newrelic-8.8.1/newrelic/core/memcache_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/message_node.py` & `newrelic-8.8.1/newrelic/core/message_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/metric.py` & `newrelic-8.8.1/newrelic/core/metric.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/node_mixin.py` & `newrelic-8.8.1/newrelic/core/node_mixin.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/profile_sessions.py` & `newrelic-8.8.1/newrelic/core/profile_sessions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/root_node.py` & `newrelic-8.8.1/newrelic/core/root_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/rules_engine.py` & `newrelic-8.8.1/newrelic/core/rules_engine.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/solr_node.py` & `newrelic-8.8.1/newrelic/core/solr_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/stack_trace.py` & `newrelic-8.8.1/newrelic/core/stack_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/stats_engine.py` & `newrelic-8.8.1/newrelic/core/stats_engine.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/string_table.py` & `newrelic-8.8.1/newrelic/core/string_table.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/thread_utilization.py` & `newrelic-8.8.1/newrelic/core/thread_utilization.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/trace_cache.py` & `newrelic-8.8.1/newrelic/core/trace_cache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/trace_node.py` & `newrelic-8.8.1/newrelic/core/trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/core/transaction_node.py` & `newrelic-8.8.1/newrelic/core/transaction_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/extras/__init__.py` & `newrelic-8.8.1/newrelic/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/extras/framework_django/__init__.py` & `newrelic-8.8.1/newrelic/extras/framework_django/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/extras/framework_django/templatetags/__init__.py` & `newrelic-8.8.1/newrelic/extras/framework_django/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py` & `newrelic-8.8.1/newrelic/extras/framework_django/templatetags/newrelic_tags.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/__init__.py` & `newrelic-8.8.1/newrelic/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_asgiref.py` & `newrelic-8.8.1/newrelic/hooks/adapter_asgiref.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_cheroot.py` & `newrelic-8.8.1/newrelic/hooks/adapter_cheroot.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_cherrypy.py` & `newrelic-8.8.1/newrelic/hooks/adapter_cherrypy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_daphne.py` & `newrelic-8.8.1/newrelic/hooks/adapter_daphne.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_flup.py` & `newrelic-8.8.1/newrelic/hooks/adapter_flup.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_gevent.py` & `newrelic-8.8.1/newrelic/hooks/adapter_gevent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_gunicorn.py` & `newrelic-8.8.1/newrelic/hooks/adapter_gunicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_hypercorn.py` & `newrelic-8.8.1/newrelic/hooks/adapter_hypercorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_meinheld.py` & `newrelic-8.8.1/newrelic/hooks/adapter_meinheld.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_paste.py` & `newrelic-8.8.1/newrelic/hooks/adapter_paste.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_uvicorn.py` & `newrelic-8.8.1/newrelic/hooks/adapter_uvicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/adapter_waitress.py` & `newrelic-8.8.1/newrelic/hooks/adapter_wsgiref.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import newrelic.api.wsgi_application
 import newrelic.api.in_function
 
-def instrument_waitress_server(module):
+def instrument_wsgiref_simple_server(module):
 
     def wrap_wsgi_application_entry_point(server, application,
                                           *args, **kwargs):
         application = newrelic.api.wsgi_application.WSGIApplicationWrapper(
                 application)
         args = [server, application] + list(args)
         return (args, kwargs)
 
     newrelic.api.in_function.wrap_in_function(module,
-            'WSGIServer.__init__', wrap_wsgi_application_entry_point)
+            'WSGIServer.set_app', wrap_wsgi_application_entry_point)
```

### Comparing `newrelic-8.8.0/newrelic/hooks/application_celery.py` & `newrelic-8.8.1/newrelic/hooks/application_celery.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/application_gearman.py` & `newrelic-8.8.1/newrelic/hooks/application_gearman.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/component_cornice.py` & `newrelic-8.8.1/newrelic/hooks/component_cornice.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/component_djangorestframework.py` & `newrelic-8.8.1/newrelic/hooks/component_djangorestframework.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/component_flask_rest.py` & `newrelic-8.8.1/newrelic/hooks/component_flask_rest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/component_graphqlserver.py` & `newrelic-8.8.1/newrelic/hooks/component_graphqlserver.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/component_piston.py` & `newrelic-8.8.1/newrelic/hooks/component_piston.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/component_sentry.py` & `newrelic-8.8.1/newrelic/hooks/component_sentry.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/component_tastypie.py` & `newrelic-8.8.1/newrelic/hooks/component_tastypie.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/coroutines_asyncio.py` & `newrelic-8.8.1/newrelic/hooks/coroutines_asyncio.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/coroutines_gevent.py` & `newrelic-8.8.1/newrelic/hooks/coroutines_gevent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_asyncpg.py` & `newrelic-8.8.1/newrelic/hooks/database_asyncpg.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_cx_oracle.py` & `newrelic-8.8.1/newrelic/hooks/database_cx_oracle.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_dbapi2.py` & `newrelic-8.8.1/newrelic/hooks/database_dbapi2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_ibm_db_dbi.py` & `newrelic-8.8.1/newrelic/hooks/database_ibm_db_dbi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_mysql.py` & `newrelic-8.8.1/newrelic/hooks/database_mysql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_mysqldb.py` & `newrelic-8.8.1/newrelic/hooks/database_mysqldb.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_oursql.py` & `newrelic-8.8.1/newrelic/hooks/database_oursql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_postgresql.py` & `newrelic-8.8.1/newrelic/hooks/database_postgresql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_psycopg2.py` & `newrelic-8.8.1/newrelic/hooks/database_psycopg2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_psycopg2cffi.py` & `newrelic-8.8.1/newrelic/hooks/database_psycopg2cffi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_psycopg2ct.py` & `newrelic-8.8.1/newrelic/hooks/database_psycopg2ct.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_pymssql.py` & `newrelic-8.8.1/newrelic/hooks/database_pymssql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_pymysql.py` & `newrelic-8.8.1/newrelic/hooks/database_pymysql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_pyodbc.py` & `newrelic-8.8.1/newrelic/hooks/database_pyodbc.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/database_sqlite.py` & `newrelic-8.8.1/newrelic/hooks/database_sqlite.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_aioredis.py` & `newrelic-8.8.1/newrelic/hooks/datastore_aioredis.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from newrelic.api.datastore_trace import DatastoreTrace
 from newrelic.api.time_trace import current_trace
 from newrelic.api.transaction import current_transaction
-from newrelic.common.object_wrapper import wrap_function_wrapper, function_wrapper
+from newrelic.common.object_wrapper import function_wrapper, wrap_function_wrapper
+from newrelic.common.package_version_utils import get_package_version_tuple
 from newrelic.hooks.datastore_redis import (
     _redis_client_methods,
     _redis_multipart_commands,
     _redis_operation_re,
 )
-from newrelic.common.package_version_utils import get_package_version_tuple
 
 
 def _conn_attrs_to_dict(connection):
     host = getattr(connection, "host", None)
     port = getattr(connection, "port", None)
     if not host and not port and hasattr(connection, "_address"):
         host, port = connection._address
@@ -35,39 +35,39 @@
         "path": getattr(connection, "path", None),
         "db": getattr(connection, "db", getattr(connection, "_db", None)),
     }
 
 
 def _instance_info(kwargs):
     host = kwargs.get("host") or "localhost"
-    port_path_or_id = str(kwargs.get("port") or kwargs.get("path", 6379))
+    port_path_or_id = str(kwargs.get("path") or kwargs.get("port", 6379))
     db = str(kwargs.get("db") or 0)
 
     return (host, port_path_or_id, db)
 
 
 def _wrap_AioRedis_method_wrapper(module, instance_class_name, operation):
-
     @function_wrapper
     async def _nr_wrapper_AioRedis_async_method_(wrapped, instance, args, kwargs):
         transaction = current_transaction()
         if transaction is None:
             return await wrapped(*args, **kwargs)
 
         with DatastoreTrace(product="Redis", target=None, operation=operation):
             return await wrapped(*args, **kwargs)
-    
+
     def _nr_wrapper_AioRedis_method_(wrapped, instance, args, kwargs):
         # Check for transaction and return early if found.
         # Method will return synchronously without executing,
         # it will be added to the command stack and run later.
         aioredis_version = get_package_version_tuple("aioredis")
         if aioredis_version and aioredis_version < (2,):
             # AioRedis v1 uses a RedisBuffer instead of a real connection for queueing up pipeline commands
             from aioredis.commands.transaction import _RedisBuffer
+
             if isinstance(instance._pool_or_conn, _RedisBuffer):
                 # Method will return synchronously without executing,
                 # it will be added to the command stack and run later.
                 return wrapped(*args, **kwargs)
         else:
             # AioRedis v2 uses a Pipeline object for a client and internally queues up pipeline commands
             if aioredis_version:
@@ -76,15 +76,14 @@
                 from redis.asyncio.client import Pipeline
             if isinstance(instance, Pipeline):
                 return wrapped(*args, **kwargs)
 
         # Method should be run when awaited, therefore we wrap in an async wrapper.
         return _nr_wrapper_AioRedis_async_method_(wrapped)(*args, **kwargs)
 
-
     name = "%s.%s" % (instance_class_name, operation)
     wrap_function_wrapper(module, name, _nr_wrapper_AioRedis_method_)
 
 
 async def wrap_Connection_send_command(wrapped, instance, args, kwargs):
     transaction = current_transaction()
     if not transaction:
@@ -105,15 +104,17 @@
     # detect those and grab the next argument from the set of arguments.
 
     operation = args[0].strip().lower()
 
     # If it's not a multi part command, there's no need to trace it, so
     # we can return early.
 
-    if operation.split()[0] not in _redis_multipart_commands:        # Set the datastore info on the DatastoreTrace containing this function call.
+    if (
+        operation.split()[0] not in _redis_multipart_commands
+    ):  # Set the datastore info on the DatastoreTrace containing this function call.
         trace = current_trace()
 
         # Find DatastoreTrace no matter how many other traces are inbetween
         while trace is not None and not isinstance(trace, DatastoreTrace):
             trace = getattr(trace, "parent", None)
 
         if trace is not None:
@@ -157,15 +158,17 @@
     # detect those and grab the next argument from the set of arguments.
 
     operation = args[0].strip().lower()
 
     # If it's not a multi part command, there's no need to trace it, so
     # we can return early.
 
-    if operation.split()[0] not in _redis_multipart_commands:        # Set the datastore info on the DatastoreTrace containing this function call.
+    if (
+        operation.split()[0] not in _redis_multipart_commands
+    ):  # Set the datastore info on the DatastoreTrace containing this function call.
         trace = current_trace()
 
         # Find DatastoreTrace no matter how many other traces are inbetween
         while trace is not None and not isinstance(trace, DatastoreTrace):
             trace = getattr(trace, "parent", None)
 
         if trace is not None:
```

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_aredis.py` & `newrelic-8.8.1/newrelic/hooks/datastore_aredis.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_bmemcached.py` & `newrelic-8.8.1/newrelic/hooks/datastore_bmemcached.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_elasticsearch.py` & `newrelic-8.8.1/newrelic/hooks/datastore_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_memcache.py` & `newrelic-8.8.1/newrelic/hooks/datastore_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_motor.py` & `newrelic-8.8.1/newrelic/hooks/datastore_motor.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_pyelasticsearch.py` & `newrelic-8.8.1/newrelic/hooks/datastore_pyelasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_pylibmc.py` & `newrelic-8.8.1/newrelic/hooks/datastore_pylibmc.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_pymemcache.py` & `newrelic-8.8.1/newrelic/hooks/datastore_pymemcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_pymongo.py` & `newrelic-8.8.1/newrelic/hooks/datastore_pymongo.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_pysolr.py` & `newrelic-8.8.1/newrelic/hooks/datastore_pysolr.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_redis.py` & `newrelic-8.8.1/newrelic/hooks/datastore_redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,14 +390,15 @@
     "trimmed_mean",
     "ttl",
     "type",
     "unlink",
     "unsubscribe",
     "unwatch",
     "wait",
+    "waitaof",
     "watch",
     "xack",
     "xadd",
     "xautoclaim",
     "xclaim",
     "xdel",
     "xgroup_create",
```

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_solrpy.py` & `newrelic-8.8.1/newrelic/hooks/datastore_solrpy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/datastore_umemcache.py` & `newrelic-8.8.1/newrelic/hooks/datastore_umemcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_botocore.py` & `newrelic-8.8.1/newrelic/hooks/external_botocore.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_dropbox.py` & `newrelic-8.8.1/newrelic/hooks/external_dropbox.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_facepy.py` & `newrelic-8.8.1/newrelic/hooks/external_facepy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_feedparser.py` & `newrelic-8.8.1/newrelic/hooks/external_feedparser.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_httplib.py` & `newrelic-8.8.1/newrelic/hooks/external_httplib.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_httplib2.py` & `newrelic-8.8.1/newrelic/hooks/external_httplib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_httpx.py` & `newrelic-8.8.1/newrelic/hooks/external_httpx.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_pywapi.py` & `newrelic-8.8.1/newrelic/hooks/external_pywapi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_requests.py` & `newrelic-8.8.1/newrelic/hooks/external_requests.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_thrift.py` & `newrelic-8.8.1/newrelic/hooks/external_thrift.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_urllib.py` & `newrelic-8.8.1/newrelic/hooks/external_urllib.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_urllib2.py` & `newrelic-8.8.1/newrelic/hooks/external_urllib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_urllib3.py` & `newrelic-8.8.1/newrelic/hooks/external_urllib3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/external_xmlrpclib.py` & `newrelic-8.8.1/newrelic/hooks/external_xmlrpclib.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_aiohttp.py` & `newrelic-8.8.1/newrelic/hooks/framework_aiohttp.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_ariadne.py` & `newrelic-8.8.1/newrelic/hooks/framework_ariadne.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_bottle.py` & `newrelic-8.8.1/newrelic/hooks/framework_bottle.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_cherrypy.py` & `newrelic-8.8.1/newrelic/hooks/framework_cherrypy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_django.py` & `newrelic-8.8.1/newrelic/hooks/framework_django.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_django_py3.py` & `newrelic-8.8.1/newrelic/hooks/framework_django_py3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_falcon.py` & `newrelic-8.8.1/newrelic/hooks/framework_falcon.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_fastapi.py` & `newrelic-8.8.1/newrelic/hooks/framework_fastapi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_flask.py` & `newrelic-8.8.1/newrelic/hooks/framework_flask.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_graphene.py` & `newrelic-8.8.1/newrelic/hooks/framework_graphene.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_graphql.py` & `newrelic-8.8.1/newrelic/hooks/framework_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_grpc.py` & `newrelic-8.8.1/newrelic/hooks/framework_grpc.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_pylons.py` & `newrelic-8.8.1/newrelic/hooks/framework_pylons.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_pyramid.py` & `newrelic-8.8.1/newrelic/hooks/framework_pyramid.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_sanic.py` & `newrelic-8.8.1/newrelic/hooks/framework_sanic.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_starlette.py` & `newrelic-8.8.1/newrelic/hooks/framework_starlette.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_strawberry.py` & `newrelic-8.8.1/newrelic/hooks/framework_strawberry.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_tornado.py` & `newrelic-8.8.1/newrelic/hooks/framework_tornado.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_web2py.py` & `newrelic-8.8.1/newrelic/hooks/framework_web2py.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/framework_webpy.py` & `newrelic-8.8.1/newrelic/hooks/framework_webpy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/logger_logging.py` & `newrelic-8.8.1/newrelic/hooks/logger_logging.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/logger_loguru.py` & `newrelic-8.8.1/newrelic/hooks/logger_loguru.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,26 @@
 
 import logging
 import sys
 
 from newrelic.api.application import application_instance
 from newrelic.api.transaction import current_transaction, record_log_event
 from newrelic.common.object_wrapper import wrap_function_wrapper
+from newrelic.common.signature import bind_args
 from newrelic.core.config import global_settings
 from newrelic.hooks.logger_logging import add_nr_linking_metadata
 from newrelic.packages import six
 
-_logger = logging.getLogger(__name__) 
+_logger = logging.getLogger(__name__)
 is_pypy = hasattr(sys, "pypy_version_info")
 
+
 def loguru_version():
     from loguru import __version__
+
     return tuple(int(x) for x in __version__.split("."))
 
 
 def _nr_log_forwarder(message_instance):
     transaction = current_transaction()
     record = message_instance.record
     message = record.get("_nr_original_message", record["message"])
@@ -50,32 +53,31 @@
                 transaction.record_custom_metric("Logging/lines", {"count": 1})
                 transaction.record_custom_metric("Logging/lines/%s" % level_name, {"count": 1})
             else:
                 application = application_instance(activate=False)
                 if application and application.enabled:
                     application.record_custom_metric("Logging/lines", {"count": 1})
                     application.record_custom_metric("Logging/lines/%s" % level_name, {"count": 1})
-            
+
         if settings.application_logging.forwarding and settings.application_logging.forwarding.enabled:
             try:
                 record_log_event(message, level_name, int(record["time"].timestamp()))
             except Exception:
                 pass
 
 
 ALLOWED_LOGURU_OPTIONS_LENGTHS = frozenset((8, 9))
 
-def bind_log(level_id, static_level_no, from_decorator, options, message, args, kwargs):
-    assert len(options) in ALLOWED_LOGURU_OPTIONS_LENGTHS  # Assert the options signature we expect
-    return level_id, static_level_no, from_decorator, list(options), message, args, kwargs
-
 
 def wrap_log(wrapped, instance, args, kwargs):
     try:
-        level_id, static_level_no, from_decorator, options, message, subargs, subkwargs = bind_log(*args, **kwargs)
+        bound_args = bind_args(wrapped, args, kwargs)
+        options = bound_args["options"] = list(bound_args["options"])
+        assert len(options) in ALLOWED_LOGURU_OPTIONS_LENGTHS  # Assert the options signature we expect
+
         options[-2] = nr_log_patcher(options[-2])
         # Loguru looks into the stack trace to find the caller's module and function names.
         # options[1] tells loguru how far up to look in the stack trace to find the caller.
         # Because wrap_log is an extra call in the stack trace, loguru needs to look 1 level higher.
         if not is_pypy:
             options[1] += 1
         else:
@@ -83,22 +85,22 @@
             # add another frame on PyPy but not on CPython.
             options[1] += 2
 
     except Exception as e:
         _logger.debug("Exception in loguru handling: %s" % str(e))
         return wrapped(*args, **kwargs)
     else:
-        return wrapped(level_id, static_level_no, from_decorator, options, message, subargs, subkwargs)
+        return wrapped(**bound_args)
 
 
 def nr_log_patcher(original_patcher=None):
     def _nr_log_patcher(record):
         if original_patcher:
             record = original_patcher(record)
-        
+
         transaction = current_transaction()
 
         if transaction:
             settings = transaction.settings
         else:
             settings = global_settings()
```

### Comparing `newrelic-8.8.0/newrelic/hooks/memcache_memcache.py` & `newrelic-8.8.1/newrelic/hooks/memcache_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/messagebroker_confluentkafka.py` & `newrelic-8.8.1/newrelic/hooks/messagebroker_confluentkafka.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/messagebroker_kafkapython.py` & `newrelic-8.8.1/newrelic/hooks/messagebroker_kafkapython.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/messagebroker_pika.py` & `newrelic-8.8.1/newrelic/hooks/messagebroker_pika.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/middleware_flask_compress.py` & `newrelic-8.8.1/newrelic/hooks/middleware_flask_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/middleware_weberror.py` & `newrelic-8.8.1/newrelic/hooks/middleware_weberror.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/nosql_pymongo.py` & `newrelic-8.8.1/tests/adapter_gevent/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,37 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import newrelic.api.function_trace
+import pytest
+import webtest
 
-_methods = ['save', 'insert', 'update', 'drop', 'remove', 'find_one',
-            'find', 'count', 'create_index', 'ensure_index', 'drop_indexes',
-            'drop_index', 'reindex', 'index_information', 'options',
-            'group', 'rename', 'distinct', 'map_reduce', 'inline_map_reduce',
-            'find_and_modify']
+from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
 
-def instrument_pymongo_connection(module):
-
-    # Must name function explicitly as pymongo overrides the
-    # __getattr__() method in a way that breaks introspection.
-
-    newrelic.api.function_trace.wrap_function_trace(
-        module, 'Connection.__init__',
-        name='%s:Connection.__init__' % module.__name__)
-
-def instrument_pymongo_collection(module):
-
-    # Must name function explicitly as pymongo overrides the
-    # __getattr__() method in a way that breaks introspection.
-
-    for method in _methods:
-        if hasattr(module.Collection, method):
-            #newrelic.api.function_trace.wrap_function_trace(
-            #        module, 'Collection.%s' % method,
-            #        name=method, group='Custom/MongoDB')
-            newrelic.api.function_trace.wrap_function_trace(
-                    module, 'Collection.%s' % method,
-                    name='%s:Collection.%s' % (module.__name__, method))
+_default_settings = {
+    'transaction_tracer.explain_threshold': 0.0,
+    'transaction_tracer.transaction_threshold': 0.0,
+    'transaction_tracer.stack_trace_threshold': 0.0,
+    'debug.log_data_collector_payloads': True,
+    'debug.record_transaction_failure': True,
+    'debug.disable_harvest_until_shutdown': False,
+}
+
+collector_agent_registration = collector_agent_registration_fixture(
+        app_name='Python Agent Test (adapter_gevent)',
+        default_settings=_default_settings)
+
+@pytest.fixture(autouse=True, scope='session')
+def target_application():
+    import _application
+    port = _application.setup_application()
+    return webtest.TestApp('http://localhost:%d' % port)
```

### Comparing `newrelic-8.8.0/newrelic/hooks/template_genshi.py` & `newrelic-8.8.1/newrelic/hooks/template_genshi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/template_jinja2.py` & `newrelic-8.8.1/newrelic/hooks/template_jinja2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/hooks/template_mako.py` & `newrelic-8.8.1/newrelic/hooks/template_mako.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/network/__init__.py` & `newrelic-8.8.1/newrelic/network/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/network/addresses.py` & `newrelic-8.8.1/newrelic/network/addresses.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/network/exceptions.py` & `newrelic-8.8.1/newrelic/network/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/newrelic.ini` & `newrelic-8.8.1/newrelic/newrelic.ini`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/asgiref_compatibility.py` & `newrelic-8.8.1/newrelic/packages/asgiref_compatibility.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/LICENSE.txt` & `newrelic-8.8.1/newrelic/packages/urllib3/LICENSE.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2008-2019 Andrey Petrov and contributors (see CONTRIBUTORS.txt)
+Copyright (c) 2008-2020 Andrey Petrov and contributors (see CONTRIBUTORS.txt)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/__init__.py` & `newrelic-8.8.1/newrelic/packages/urllib3/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .poolmanager import PoolManager, ProxyManager, proxy_from_url
 from .response import HTTPResponse
 from .util.request import make_headers
 from .util.retry import Retry
 from .util.timeout import Timeout
 from .util.url import get_host
 
+
 __author__ = "Andrey Petrov (andrey.petrov@shazow.net)"
 __license__ = "MIT"
 __version__ = __version__
 
 __all__ = (
     "HTTPConnectionPool",
     "HTTPSConnectionPool",
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/_collections.py` & `newrelic-8.8.1/newrelic/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/connection.py` & `newrelic-8.8.1/newrelic/packages/urllib3/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,32 +47,32 @@
 from ._version import __version__
 from .exceptions import (
     ConnectTimeoutError,
     NewConnectionError,
     SubjectAltNameWarning,
     SystemTimeWarning,
 )
-from .packages.ssl_match_hostname import CertificateError, match_hostname
 from .util import SKIP_HEADER, SKIPPABLE_HEADERS, connection
 from .util.ssl_ import (
     assert_fingerprint,
     create_urllib3_context,
     is_ipaddress,
     resolve_cert_reqs,
     resolve_ssl_version,
     ssl_wrap_socket,
 )
+from .util.ssl_match_hostname import CertificateError, match_hostname
 
 log = logging.getLogger(__name__)
 
 port_by_scheme = {"http": 80, "https": 443}
 
 # When it comes time to update this value as a part of regular maintenance
 # (ie test_recent_date is failing) update it to ~6 months before the current date.
-RECENT_DATE = datetime.date(2020, 7, 1)
+RECENT_DATE = datetime.date(2022, 1, 1)
 
 _CONTAINS_CONTROL_CHAR_RE = re.compile(r"[^-!#$%&'*+.^_`|~0-9a-zA-Z]")
 
 
 class HTTPConnection(_HTTPConnection, object):
     """
     Based on :class:`http.client.HTTPConnection` but provides an extra constructor
@@ -225,14 +225,19 @@
         elif six.ensure_str(header.lower()) not in SKIPPABLE_HEADERS:
             raise ValueError(
                 "urllib3.util.SKIP_HEADER only supports '%s'"
                 % ("', '".join(map(str.title, sorted(SKIPPABLE_HEADERS))),)
             )
 
     def request(self, method, url, body=None, headers=None):
+        # Update the inner socket's timeout value to send the request.
+        # This only triggers if the connection is re-used.
+        if getattr(self, "sock", None) is not None:
+            self.sock.settimeout(self.timeout)
+
         if headers is None:
             headers = {}
         else:
             # Avoid modifying the headers passed into .request()
             headers = headers.copy()
         if "user-agent" not in (six.ensure_str(k.lower()) for k in headers):
             headers["User-Agent"] = _get_default_user_agent()
@@ -351,25 +356,23 @@
         self.assert_fingerprint = assert_fingerprint
         self.ca_certs = ca_certs and os.path.expanduser(ca_certs)
         self.ca_cert_dir = ca_cert_dir and os.path.expanduser(ca_cert_dir)
         self.ca_cert_data = ca_cert_data
 
     def connect(self):
         # Add certificate verification
-        conn = self._new_conn()
+        self.sock = conn = self._new_conn()
         hostname = self.host
         tls_in_tls = False
 
         if self._is_using_tunnel():
             if self.tls_in_tls_required:
-                conn = self._connect_tls_proxy(hostname, conn)
+                self.sock = conn = self._connect_tls_proxy(hostname, conn)
                 tls_in_tls = True
 
-            self.sock = conn
-
             # Calls self._set_hostport(), so self.host is
             # self._tunnel_host below.
             self._tunnel()
             # Mark this connection as not reusable
             self.auto_open = 0
 
             # Override the host with the one we're requesting data from.
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/connectionpool.py` & `newrelic-8.8.1/newrelic/packages/urllib3/connectionpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import absolute_import
 
 import errno
 import logging
+import re
 import socket
 import sys
 import warnings
 from socket import error as SocketError
 from socket import timeout as SocketTimeout
 
 from .connection import (
@@ -31,23 +32,23 @@
     ProxyError,
     ReadTimeoutError,
     SSLError,
     TimeoutError,
 )
 from .packages import six
 from .packages.six.moves import queue
-from .packages.ssl_match_hostname import CertificateError
 from .request import RequestMethods
 from .response import HTTPResponse
 from .util.connection import is_connection_dropped
 from .util.proxy import connection_requires_http_tunnel
 from .util.queue import LifoQueue
 from .util.request import set_file_position
 from .util.response import assert_header_parsing
 from .util.retry import Retry
+from .util.ssl_match_hostname import CertificateError
 from .util.timeout import Timeout
 from .util.url import Url, _encode_target
 from .util.url import _normalize_host as normalize_host
 from .util.url import get_host, parse_url
 
 xrange = six.moves.xrange
 
@@ -297,16 +298,19 @@
             self.pool.put(conn, block=False)
             return  # Everything is dandy, done.
         except AttributeError:
             # self.pool is None.
             pass
         except queue.Full:
             # This should never happen if self.block == True
-            log.warning("Connection pool is full, discarding connection: %s", self.host)
-
+            log.warning(
+                "Connection pool is full, discarding connection: %s. Connection pool size: %s",
+                self.host,
+                self.pool.qsize(),
+            )
         # Connection never got put back into the pool, close it.
         if conn:
             conn.close()
 
     def _validate_conn(self, conn):
         """
         Called right before a request is made, after the socket is created.
@@ -371,15 +375,15 @@
             :class:`urllib3.util.Timeout`, which gives you more fine-grained
             control over your timeouts.
         """
         self.num_requests += 1
 
         timeout_obj = self._get_timeout(timeout)
         timeout_obj.start_connect()
-        conn.timeout = timeout_obj.connect_timeout
+        conn.timeout = Timeout.resolve_default_timeout(timeout_obj.connect_timeout)
 
         # Trigger any extra validation we need to do.
         try:
             self._validate_conn(conn)
         except (SocketTimeout, BaseSSLError) as e:
             # Py2 raises this as a BaseSSLError, Py3 raises it as socket timeout.
             self._raise_timeout(err=e, url=url, timeout_value=conn.timeout)
@@ -741,15 +745,43 @@
             BaseSSLError,
             SSLError,
             CertificateError,
         ) as e:
             # Discard the connection for these exceptions. It will be
             # replaced during the next _get_conn() call.
             clean_exit = False
-            if isinstance(e, (BaseSSLError, CertificateError)):
+
+            def _is_ssl_error_message_from_http_proxy(ssl_error):
+                # We're trying to detect the message 'WRONG_VERSION_NUMBER' but
+                # SSLErrors are kinda all over the place when it comes to the message,
+                # so we try to cover our bases here!
+                message = " ".join(re.split("[^a-z]", str(ssl_error).lower()))
+                return (
+                    "wrong version number" in message or "unknown protocol" in message
+                )
+
+            # Try to detect a common user error with proxies which is to
+            # set an HTTP proxy to be HTTPS when it should be 'http://'
+            # (ie {'http': 'http://proxy', 'https': 'https://proxy'})
+            # Instead we add a nice error message and point to a URL.
+            if (
+                isinstance(e, BaseSSLError)
+                and self.proxy
+                and _is_ssl_error_message_from_http_proxy(e)
+                and conn.proxy
+                and conn.proxy.scheme == "https"
+            ):
+                e = ProxyError(
+                    "Your proxy appears to only use HTTP and not HTTPS, "
+                    "try changing your proxy URL to be HTTP. See: "
+                    "https://urllib3.readthedocs.io/en/1.26.x/advanced-usage.html"
+                    "#https-proxy-error-http-proxy",
+                    SSLError(e),
+                )
+            elif isinstance(e, (BaseSSLError, CertificateError)):
                 e = SSLError(e)
             elif isinstance(e, (SocketError, NewConnectionError)) and self.proxy:
                 e = ProxyError("Cannot connect to proxy.", e)
             elif isinstance(e, (SocketError, HTTPException)):
                 e = ProtocolError("Connection aborted.", e)
 
             retries = retries.increment(
@@ -826,15 +858,15 @@
                 release_conn=release_conn,
                 chunked=chunked,
                 body_pos=body_pos,
                 **response_kw
             )
 
         # Check if we should retry the HTTP response.
-        has_retry_after = bool(response.getheader("Retry-After"))
+        has_retry_after = bool(response.headers.get("Retry-After"))
         if retries.is_retry(method, response.status, has_retry_after):
             try:
                 retries = retries.increment(method, url, response=response, _pool=self)
             except MaxRetryError:
                 if retries.raise_on_status:
                     response.drain_conn()
                     raise
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/contrib/_appengine_environ.py` & `newrelic-8.8.1/newrelic/packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py` & `newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py` & `newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/contrib/appengine.py` & `newrelic-8.8.1/newrelic/packages/urllib3/contrib/appengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
                     retries=retries,
                     redirect=redirect,
                     timeout=timeout,
                     **response_kw
                 )
 
         # Check if we should retry the HTTP response.
-        has_retry_after = bool(http_response.getheader("Retry-After"))
+        has_retry_after = bool(http_response.headers.get("Retry-After"))
         if retries.is_retry(method, http_response.status, has_retry_after):
             retries = retries.increment(method, url, response=http_response, _pool=self)
             log.debug("Retry: %s", url)
             retries.sleep(http_response)
             return self.urlopen(
                 method,
                 url,
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/contrib/ntlmpool.py` & `newrelic-8.8.1/newrelic/packages/urllib3/contrib/ntlmpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         # Send negotiation message
         headers[req_header] = "NTLM %s" % ntlm.create_NTLM_NEGOTIATE_MESSAGE(
             self.rawuser
         )
         log.debug("Request headers: %s", headers)
         conn.request("GET", self.authurl, None, headers)
         res = conn.getresponse()
-        reshdr = dict(res.getheaders())
+        reshdr = dict(res.headers)
         log.debug("Response status: %s %s", res.status, res.reason)
         log.debug("Response headers: %s", reshdr)
         log.debug("Response data: %s [...]", res.read(100))
 
         # Remove the reference to the socket, so that it can not be closed by
         # the response object (we want to keep the socket open)
         res.fp = None
@@ -97,15 +97,15 @@
             ServerChallenge, self.user, self.domain, self.pw, NegotiateFlags
         )
         headers[req_header] = "NTLM %s" % auth_msg
         log.debug("Request headers: %s", headers)
         conn.request("GET", self.authurl, None, headers)
         res = conn.getresponse()
         log.debug("Response status: %s %s", res.status, res.reason)
-        log.debug("Response headers: %s", dict(res.getheaders()))
+        log.debug("Response headers: %s", dict(res.headers))
         log.debug("Response data: %s [...]", res.read()[:100])
         if res.status != 200:
             if res.status == 401:
                 raise Exception("Server rejected request: wrong username or password")
             raise Exception("Wrong server response: %s %s" % (res.status, res.reason))
 
         res.fp = None
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/contrib/pyopenssl.py` & `newrelic-8.8.1/newrelic/packages/urllib3/contrib/pyopenssl.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 .. _crime attack: https://en.wikipedia.org/wiki/CRIME_(security_exploit)
 .. _pyopenssl: https://www.pyopenssl.org
 .. _cryptography: https://cryptography.io
 .. _idna: https://github.com/kjd/idna
 """
 from __future__ import absolute_import
 
+import OpenSSL.crypto
 import OpenSSL.SSL
 from cryptography import x509
 from cryptography.hazmat.backends.openssl import backend as openssl_backend
-from cryptography.hazmat.backends.openssl.x509 import _Certificate
 
 try:
     from cryptography.x509 import UnsupportedExtension
 except ImportError:
     # UnsupportedExtension is gone in cryptography >= 2.1.0
     class UnsupportedExtension(Exception):
         pass
@@ -69,19 +69,28 @@
 except ImportError:  # Platform-specific: Python 3
     _fileobject = None
     from ..packages.backports.makefile import backport_makefile
 
 import logging
 import ssl
 import sys
+import warnings
 
 from .. import util
 from ..packages import six
 from ..util.ssl_ import PROTOCOL_TLS_CLIENT
 
+warnings.warn(
+    "'urllib3.contrib.pyopenssl' module is deprecated and will be removed "
+    "in a future release of urllib3 2.x. Read more in this issue: "
+    "https://github.com/urllib3/urllib3/issues/2680",
+    category=DeprecationWarning,
+    stacklevel=2,
+)
+
 __all__ = ["inject_into_urllib3", "extract_from_urllib3"]
 
 # SNI always works.
 HAS_SNI = True
 
 # Map from urllib3 to PyOpenSSL compatible parameter-values.
 _openssl_versions = {
@@ -215,17 +224,16 @@
     """
     Given an PyOpenSSL certificate, provides all the subject alternative names.
     """
     # Pass the cert to cryptography, which has much better APIs for this.
     if hasattr(peer_cert, "to_cryptography"):
         cert = peer_cert.to_cryptography()
     else:
-        # This is technically using private APIs, but should work across all
-        # relevant versions before PyOpenSSL got a proper API for this.
-        cert = _Certificate(openssl_backend, peer_cert._x509)
+        der = OpenSSL.crypto.dump_certificate(OpenSSL.crypto.FILETYPE_ASN1, peer_cert)
+        cert = x509.load_der_x509_certificate(der, openssl_backend)
 
     # We want to find the SAN extension. Ask Cryptography to locate it (it's
     # faster than looping in Python)
     try:
         ext = cert.extensions.get_extension_for_class(x509.SubjectAlternativeName).value
     except x509.ExtensionNotFound:
         # No such extension, return the empty list.
@@ -402,15 +410,14 @@
 
 if _fileobject:  # Platform-specific: Python 2
 
     def makefile(self, mode, bufsize=-1):
         self._makefile_refs += 1
         return _fileobject(self, mode, bufsize, close=True)
 
-
 else:  # Platform-specific: Python 3
     makefile = backport_makefile
 
 WrappedSocket.makefile = makefile
 
 
 class PyOpenSSLContext(object):
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/contrib/securetransport.py` & `newrelic-8.8.1/newrelic/packages/urllib3/contrib/securetransport.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,14 @@
 
 if _fileobject:  # Platform-specific: Python 2
 
     def makefile(self, mode, bufsize=-1):
         self._makefile_refs += 1
         return _fileobject(self, mode, bufsize, close=True)
 
-
 else:  # Platform-specific: Python 3
 
     def makefile(self, mode="r", buffering=None, *args, **kwargs):
         # We disable buffering with SecureTransport because it conflicts with
         # the buffering that ST does internally (see issue #1153 for more).
         buffering = 0
         return backport_makefile(self, mode, buffering, *args, **kwargs)
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/contrib/socks.py` & `newrelic-8.8.1/newrelic/packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/exceptions.py` & `newrelic-8.8.1/newrelic/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/fields.py` & `newrelic-8.8.1/newrelic/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/filepost.py` & `newrelic-8.8.1/newrelic/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/packages/backports/makefile.py` & `newrelic-8.8.1/newrelic/packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/packages/six.py` & `newrelic-8.8.1/newrelic/packages/urllib3/packages/six.py`

 * *Files 0% similar despite different names*

```diff
@@ -768,15 +768,14 @@
             if value.__traceback__ is not tb:
                 raise value.with_traceback(tb)
             raise value
         finally:
             value = None
             tb = None
 
-
 else:
 
     def exec_(_code_, _globs_=None, _locs_=None):
         """Execute code in a namespace."""
         if _globs_ is None:
             frame = sys._getframe(1)
             _globs_ = frame.f_globals
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/packages/ssl_match_hostname/_implementation.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/ssl_match_hostname.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 import sys
 
 # ipaddress has been backported to 2.6+ in pypi.  If it is installed on the
 # system, use it to handle IPAddress ServerAltnames (this was added in
 # python-3.5) otherwise only do DNS matching.  This allows
-# backports.ssl_match_hostname to continue to be used in Python 2.7.
+# util.ssl_match_hostname to continue to be used in Python 2.7.
 try:
     import ipaddress
 except ImportError:
     ipaddress = None
 
 __version__ = "3.5.0.1"
 
@@ -74,15 +74,16 @@
 
     pat = re.compile(r"\A" + r"\.".join(pats) + r"\Z", re.IGNORECASE)
     return pat.match(hostname)
 
 
 def _to_unicode(obj):
     if isinstance(obj, str) and sys.version_info < (3,):
-        obj = unicode(obj, encoding="ascii", errors="strict")
+        # ignored flake8 # F821 to support python 2.7 function
+        obj = unicode(obj, encoding="ascii", errors="strict")  # noqa: F821
     return obj
 
 
 def _ipaddress_match(ipname, host_ip):
     """Exact matching of IP addresses.
 
     RFC 6125 explicitly doesn't define an algorithm for this
@@ -107,27 +108,25 @@
             "empty or no certificate, match_hostname needs a "
             "SSL socket or SSL context with either "
             "CERT_OPTIONAL or CERT_REQUIRED"
         )
     try:
         # Divergence from upstream: ipaddress can't handle byte str
         host_ip = ipaddress.ip_address(_to_unicode(hostname))
-    except ValueError:
-        # Not an IP address (common case)
-        host_ip = None
-    except UnicodeError:
-        # Divergence from upstream: Have to deal with ipaddress not taking
+    except (UnicodeError, ValueError):
+        # ValueError: Not an IP address (common case)
+        # UnicodeError: Divergence from upstream: Have to deal with ipaddress not taking
         # byte strings.  addresses should be all ascii, so we consider it not
         # an ipaddress in this case
         host_ip = None
     except AttributeError:
         # Divergence from upstream: Make ipaddress library optional
         if ipaddress is None:
             host_ip = None
-        else:
+        else:  # Defensive
             raise
     dnsnames = []
     san = cert.get("subjectAltName", ())
     for key, value in san:
         if key == "DNS":
             if host_ip is None and _dnsname_match(value, hostname):
                 return
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/poolmanager.py` & `newrelic-8.8.1/newrelic/packages/urllib3/poolmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "cert_file",
     "cert_reqs",
     "ca_certs",
     "ssl_version",
     "ca_cert_dir",
     "ssl_context",
     "key_password",
+    "server_hostname",
 )
 
 # All known keyword arguments that could be provided to the pool manager, its
 # pools, or the underlying connections. This is used to construct a pool key.
 _key_fields = (
     "key_scheme",  # str
     "key_host",  # str
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/request.py` & `newrelic-8.8.1/newrelic/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/response.py` & `newrelic-8.8.1/newrelic/packages/urllib3/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from __future__ import absolute_import
 
 import io
 import logging
+import sys
+import warnings
 import zlib
 from contextlib import contextmanager
 from socket import error as SocketError
 from socket import timeout as SocketTimeout
 
 try:
-    import brotli
+    try:
+        import brotlicffi as brotli
+    except ImportError:
+        import brotli
 except ImportError:
     brotli = None
 
+from . import util
 from ._collections import HTTPHeaderDict
 from .connection import BaseSSLError, HTTPException
 from .exceptions import (
     BodyNotHttplibCompatible,
     DecodeError,
     HTTPError,
     IncompleteRead,
@@ -474,14 +480,62 @@
                     self._connection.close()
 
             # If we hold the original response but it's closed now, we should
             # return the connection back to the pool.
             if self._original_response and self._original_response.isclosed():
                 self.release_conn()
 
+    def _fp_read(self, amt):
+        """
+        Read a response with the thought that reading the number of bytes
+        larger than can fit in a 32-bit int at a time via SSL in some
+        known cases leads to an overflow error that has to be prevented
+        if `amt` or `self.length_remaining` indicate that a problem may
+        happen.
+
+        The known cases:
+          * 3.8 <= CPython < 3.9.7 because of a bug
+            https://github.com/urllib3/urllib3/issues/2513#issuecomment-1152559900.
+          * urllib3 injected with pyOpenSSL-backed SSL-support.
+          * CPython < 3.10 only when `amt` does not fit 32-bit int.
+        """
+        assert self._fp
+        c_int_max = 2 ** 31 - 1
+        if (
+            (
+                (amt and amt > c_int_max)
+                or (self.length_remaining and self.length_remaining > c_int_max)
+            )
+            and not util.IS_SECURETRANSPORT
+            and (util.IS_PYOPENSSL or sys.version_info < (3, 10))
+        ):
+            buffer = io.BytesIO()
+            # Besides `max_chunk_amt` being a maximum chunk size, it
+            # affects memory overhead of reading a response by this
+            # method in CPython.
+            # `c_int_max` equal to 2 GiB - 1 byte is the actual maximum
+            # chunk size that does not lead to an overflow error, but
+            # 256 MiB is a compromise.
+            max_chunk_amt = 2 ** 28
+            while amt is None or amt != 0:
+                if amt is not None:
+                    chunk_amt = min(amt, max_chunk_amt)
+                    amt -= chunk_amt
+                else:
+                    chunk_amt = max_chunk_amt
+                data = self._fp.read(chunk_amt)
+                if not data:
+                    break
+                buffer.write(data)
+                del data  # to reduce peak memory usage by `max_chunk_amt`.
+            return buffer.getvalue()
+        else:
+            # StringIO doesn't like amt=None
+            return self._fp.read(amt) if amt is not None else self._fp.read()
+
     def read(self, amt=None, decode_content=None, cache_content=False):
         """
         Similar to :meth:`http.client.HTTPResponse.read`, but with two additional
         parameters: ``decode_content`` and ``cache_content``.
 
         :param amt:
             How much of the content to read. If specified, caching is skipped
@@ -506,21 +560,19 @@
         if self._fp is None:
             return
 
         flush_decoder = False
         fp_closed = getattr(self._fp, "closed", False)
 
         with self._error_catcher():
+            data = self._fp_read(amt) if not fp_closed else b""
             if amt is None:
-                # cStringIO doesn't like amt=None
-                data = self._fp.read() if not fp_closed else b""
                 flush_decoder = True
             else:
                 cache_content = False
-                data = self._fp.read(amt) if not fp_closed else b""
                 if (
                     amt != 0 and not data
                 ):  # Platform-specific: Buggy versions of Python.
                     # Close the connection when no data is returned
                     #
                     # This is redundant to what httplib/http.client _should_
                     # already do.  However, versions of python released before
@@ -608,17 +660,29 @@
             original_response=r,
             **response_kw
         )
         return resp
 
     # Backwards-compatibility methods for http.client.HTTPResponse
     def getheaders(self):
+        warnings.warn(
+            "HTTPResponse.getheaders() is deprecated and will be removed "
+            "in urllib3 v2.1.0. Instead access HTTPResponse.headers directly.",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
         return self.headers
 
     def getheader(self, name, default=None):
+        warnings.warn(
+            "HTTPResponse.getheader() is deprecated and will be removed "
+            "in urllib3 v2.1.0. Instead use HTTPResponse.headers.get(name, default).",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
         return self.headers.get(name, default)
 
     # Backwards compatibility for http.cookiejar
     def info(self):
         return self.headers
 
     # Overrides from io.IOBase
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/__init__.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/connection.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import absolute_import
 
 import socket
 
-from ..exceptions import LocationParseError
-
 from ..contrib import _appengine_environ
+from ..exceptions import LocationParseError
 from ..packages import six
 from .wait import NoWayToWaitForSocketError, wait_for_read
 
 
 def is_connection_dropped(conn):  # Platform-specific
     """
     Returns True if the connection is dropped and should be closed.
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/proxy.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/request.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 # The only headers that are supported are ``Accept-Encoding``,
 # ``Host``, and ``User-Agent``.
 SKIP_HEADER = "@@@SKIP_HEADER@@@"
 SKIPPABLE_HEADERS = frozenset(["accept-encoding", "host", "user-agent"])
 
 ACCEPT_ENCODING = "gzip,deflate"
 try:
-    import brotli as _unused_module_brotli  # noqa: F401
+    try:
+        import brotlicffi as _unused_module_brotli  # noqa: F401
+    except ImportError:
+        import brotli as _unused_module_brotli  # noqa: F401
 except ImportError:
     pass
 else:
     ACCEPT_ENCODING += ",br"
 
 _FAILEDTELL = object()
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/response.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/retry.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/retry.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,14 +65,32 @@
         warnings.warn(
             "Using 'Retry.DEFAULT_REDIRECT_HEADERS_BLACKLIST' is deprecated and "
             "will be removed in v2.0. Use 'Retry.DEFAULT_REMOVE_HEADERS_ON_REDIRECT' instead",
             DeprecationWarning,
         )
         cls.DEFAULT_REMOVE_HEADERS_ON_REDIRECT = value
 
+    @property
+    def BACKOFF_MAX(cls):
+        warnings.warn(
+            "Using 'Retry.BACKOFF_MAX' is deprecated and "
+            "will be removed in v2.0. Use 'Retry.DEFAULT_BACKOFF_MAX' instead",
+            DeprecationWarning,
+        )
+        return cls.DEFAULT_BACKOFF_MAX
+
+    @BACKOFF_MAX.setter
+    def BACKOFF_MAX(cls, value):
+        warnings.warn(
+            "Using 'Retry.BACKOFF_MAX' is deprecated and "
+            "will be removed in v2.0. Use 'Retry.DEFAULT_BACKOFF_MAX' instead",
+            DeprecationWarning,
+        )
+        cls.DEFAULT_BACKOFF_MAX = value
+
 
 @six.add_metaclass(_RetryMeta)
 class Retry(object):
     """Retry configuration.
 
     Each retry attempt will create a new Retry object with updated values, so
     they can be safely reused.
@@ -158,15 +176,15 @@
         idempotent (multiple requests with the same parameters end with the
         same state). See :attr:`Retry.DEFAULT_ALLOWED_METHODS`.
 
         Set to a ``False`` value to retry on any verb.
 
         .. warning::
 
-            Previously this parameter was named ``method_allowlist``, that
+            Previously this parameter was named ``method_whitelist``, that
             usage is deprecated in v1.26.0 and will be removed in v2.0.
 
     :param iterable status_forcelist:
         A set of integer HTTP status codes that we should force a retry on.
         A retry is initiated if the request method is in ``allowed_methods``
         and the response status code is in ``status_forcelist``.
 
@@ -177,15 +195,15 @@
         (most errors are resolved immediately by a second try without a
         delay). urllib3 will sleep for::
 
             {backoff factor} * (2 ** ({number of total retries} - 1))
 
         seconds. If the backoff_factor is 0.1, then :func:`.sleep` will sleep
         for [0.0s, 0.2s, 0.4s, ...] between retries. It will never be longer
-        than :attr:`Retry.BACKOFF_MAX`.
+        than :attr:`Retry.DEFAULT_BACKOFF_MAX`.
 
         By default, backoff is disabled (set to 0).
 
     :param bool raise_on_redirect: Whether, if the number of redirects is
         exhausted, to raise a MaxRetryError, or to return a response with a
         response code in the 3xx range.
 
@@ -216,15 +234,15 @@
     #: Default status codes to be used for ``status_forcelist``
     RETRY_AFTER_STATUS_CODES = frozenset([413, 429, 503])
 
     #: Default headers to be used for ``remove_headers_on_redirect``
     DEFAULT_REMOVE_HEADERS_ON_REDIRECT = frozenset(["Authorization"])
 
     #: Maximum backoff time.
-    BACKOFF_MAX = 120
+    DEFAULT_BACKOFF_MAX = 120
 
     def __init__(
         self,
         total=10,
         connect=None,
         read=None,
         redirect=None,
@@ -235,31 +253,31 @@
         backoff_factor=0,
         raise_on_redirect=True,
         raise_on_status=True,
         history=None,
         respect_retry_after_header=True,
         remove_headers_on_redirect=_Default,
         # TODO: Deprecated, remove in v2.0
-        method_allowlist=_Default,
+        method_whitelist=_Default,
     ):
 
-        if method_allowlist is not _Default:
+        if method_whitelist is not _Default:
             if allowed_methods is not _Default:
                 raise ValueError(
                     "Using both 'allowed_methods' and "
-                    "'method_allowlist' together is not allowed. "
+                    "'method_whitelist' together is not allowed. "
                     "Instead only use 'allowed_methods'"
                 )
             warnings.warn(
-                "Using 'method_allowlist' with Retry is deprecated and "
+                "Using 'method_whitelist' with Retry is deprecated and "
                 "will be removed in v2.0. Use 'allowed_methods' instead",
                 DeprecationWarning,
                 stacklevel=2,
             )
-            allowed_methods = method_allowlist
+            allowed_methods = method_whitelist
         if allowed_methods is _Default:
             allowed_methods = self.DEFAULT_ALLOWED_METHODS
         if remove_headers_on_redirect is _Default:
             remove_headers_on_redirect = self.DEFAULT_REMOVE_HEADERS_ON_REDIRECT
 
         self.total = total
         self.connect = connect
@@ -298,25 +316,25 @@
             history=self.history,
             remove_headers_on_redirect=self.remove_headers_on_redirect,
             respect_retry_after_header=self.respect_retry_after_header,
         )
 
         # TODO: If already given in **kw we use what's given to us
         # If not given we need to figure out what to pass. We decide
-        # based on whether our class has the 'method_allowlist' property
-        # and if so we pass the deprecated 'method_allowlist' otherwise
+        # based on whether our class has the 'method_whitelist' property
+        # and if so we pass the deprecated 'method_whitelist' otherwise
         # we use 'allowed_methods'. Remove in v2.0
-        if "method_allowlist" not in kw and "allowed_methods" not in kw:
-            if "method_allowlist" in self.__dict__:
+        if "method_whitelist" not in kw and "allowed_methods" not in kw:
+            if "method_whitelist" in self.__dict__:
                 warnings.warn(
-                    "Using 'method_allowlist' with Retry is deprecated and "
+                    "Using 'method_whitelist' with Retry is deprecated and "
                     "will be removed in v2.0. Use 'allowed_methods' instead",
                     DeprecationWarning,
                 )
-                params["method_allowlist"] = self.allowed_methods
+                params["method_whitelist"] = self.allowed_methods
             else:
                 params["allowed_methods"] = self.allowed_methods
 
         params.update(kw)
         return type(self)(**params)
 
     @classmethod
@@ -344,15 +362,15 @@
                 takewhile(lambda x: x.redirect_location is None, reversed(self.history))
             )
         )
         if consecutive_errors_len <= 1:
             return 0
 
         backoff_value = self.backoff_factor * (2 ** (consecutive_errors_len - 1))
-        return min(self.BACKOFF_MAX, backoff_value)
+        return min(self.DEFAULT_BACKOFF_MAX, backoff_value)
 
     def parse_retry_after(self, retry_after):
         # Whitespace: https://tools.ietf.org/html/rfc7230#section-3.2.4
         if re.match(r"^\s*[0-9]+\s*$", retry_after):
             seconds = int(retry_after)
         else:
             retry_date_tuple = email.utils.parsedate_tz(retry_after)
@@ -372,15 +390,15 @@
             seconds = 0
 
         return seconds
 
     def get_retry_after(self, response):
         """Get the value of Retry-After in seconds."""
 
-        retry_after = response.getheader("Retry-After")
+        retry_after = response.headers.get("Retry-After")
 
         if retry_after is None:
             return None
 
         return self.parse_retry_after(retry_after)
 
     def sleep_for_retry(self, response=None):
@@ -427,23 +445,23 @@
         """
         return isinstance(err, (ReadTimeoutError, ProtocolError))
 
     def _is_method_retryable(self, method):
         """Checks if a given HTTP method should be retried upon, depending if
         it is included in the allowed_methods
         """
-        # TODO: For now favor if the Retry implementation sets its own method_allowlist
+        # TODO: For now favor if the Retry implementation sets its own method_whitelist
         # property outside of our constructor to avoid breaking custom implementations.
-        if "method_allowlist" in self.__dict__:
+        if "method_whitelist" in self.__dict__:
             warnings.warn(
-                "Using 'method_allowlist' with Retry is deprecated and "
+                "Using 'method_whitelist' with Retry is deprecated and "
                 "will be removed in v2.0. Use 'allowed_methods' instead",
                 DeprecationWarning,
             )
-            allowed_methods = self.method_allowlist
+            allowed_methods = self.method_whitelist
         else:
             allowed_methods = self.allowed_methods
 
         if allowed_methods and method.upper() not in allowed_methods:
             return False
         return True
 
@@ -580,18 +598,18 @@
     def __repr__(self):
         return (
             "{cls.__name__}(total={self.total}, connect={self.connect}, "
             "read={self.read}, redirect={self.redirect}, status={self.status})"
         ).format(cls=type(self), self=self)
 
     def __getattr__(self, item):
-        if item == "method_allowlist":
+        if item == "method_whitelist":
             # TODO: Remove this deprecated alias in v2.0
             warnings.warn(
-                "Using 'method_allowlist' with Retry is deprecated and "
+                "Using 'method_whitelist' with Retry is deprecated and "
                 "will be removed in v2.0. Use 'allowed_methods' instead",
                 DeprecationWarning,
             )
             return self.allowed_methods
         try:
             return getattr(super(Retry, self), item)
         except AttributeError:
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/ssl_.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/ssltransport.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/timeout.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/timeout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import absolute_import
 
 import time
 
-# The default socket timeout, used by httplib to indicate that no timeout was
-# specified by the user
-from socket import _GLOBAL_DEFAULT_TIMEOUT
+# The default socket timeout, used by httplib to indicate that no timeout was; specified by the user
+from socket import _GLOBAL_DEFAULT_TIMEOUT, getdefaulttimeout
 
 from ..exceptions import TimeoutStateError
 
 # A sentinel value to indicate that no timeout was specified by the user in
 # urllib3
 _Default = object()
 
@@ -113,14 +112,18 @@
             self.total,
         )
 
     # __str__ provided for backwards compatibility
     __str__ = __repr__
 
     @classmethod
+    def resolve_default_timeout(cls, timeout):
+        return getdefaulttimeout() if timeout is cls.DEFAULT_TIMEOUT else timeout
+
+    @classmethod
     def _validate_timeout(cls, value, name):
         """Check that a timeout attribute is valid.
 
         :param value: The timeout value to validate
         :param name: The name of the timeout attribute to validate. This is
             used to specify in error messages.
         :return: The validated and casted version of the given value.
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/url.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,28 +46,28 @@
     "(?:(?:%(hex)s:){0,4}%(hex)s)?::%(ls32)s",
     # [ *5( h16 ":" ) h16 ] "::"              h16
     "(?:(?:%(hex)s:){0,5}%(hex)s)?::%(hex)s",
     # [ *6( h16 ":" ) h16 ] "::"
     "(?:(?:%(hex)s:){0,6}%(hex)s)?::",
 ]
 
-UNRESERVED_PAT = r"ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789._!\-~"
+UNRESERVED_PAT = r"ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789._\-~"
 IPV6_PAT = "(?:" + "|".join([x % _subs for x in _variations]) + ")"
 ZONE_ID_PAT = "(?:%25|%)(?:[" + UNRESERVED_PAT + "]|%[a-fA-F0-9]{2})+"
 IPV6_ADDRZ_PAT = r"\[" + IPV6_PAT + r"(?:" + ZONE_ID_PAT + r")?\]"
 REG_NAME_PAT = r"(?:[^\[\]%:/?#]|%[a-fA-F0-9]{2})*"
 TARGET_RE = re.compile(r"^(/[^?#]*)(?:\?([^#]*))?(?:#.*)?$")
 
 IPV4_RE = re.compile("^" + IPV4_PAT + "$")
 IPV6_RE = re.compile("^" + IPV6_PAT + "$")
 IPV6_ADDRZ_RE = re.compile("^" + IPV6_ADDRZ_PAT + "$")
 BRACELESS_IPV6_ADDRZ_RE = re.compile("^" + IPV6_ADDRZ_PAT[2:-2] + "$")
 ZONE_ID_RE = re.compile("(" + ZONE_ID_PAT + r")\]$")
 
-_HOST_PORT_PAT = ("^(%s|%s|%s)(?::([0-9]{0,5}))?$") % (
+_HOST_PORT_PAT = ("^(%s|%s|%s)(?::0*?(|0|[1-9][0-9]{0,4}))?$") % (
     REG_NAME_PAT,
     IPV4_PAT,
     IPV6_ADDRZ_PAT,
 )
 _HOST_PORT_RE = re.compile(_HOST_PORT_PAT, re.UNICODE | re.DOTALL)
 
 UNRESERVED_CHARS = set(
@@ -275,14 +275,17 @@
     if host:
         if isinstance(host, six.binary_type):
             host = six.ensure_str(host)
 
         if scheme in NORMALIZABLE_SCHEMES:
             is_ipv6 = IPV6_ADDRZ_RE.match(host)
             if is_ipv6:
+                # IPv6 hosts of the form 'a::b%zone' are encoded in a URL as
+                # such per RFC 6874: 'a::b%25zone'. Unquote the ZoneID
+                # separator as necessary to return a valid RFC 4007 scoped IP.
                 match = ZONE_ID_RE.search(host)
                 if match:
                     start, end = match.span(1)
                     zone_id = host[start:end]
 
                     if zone_id.startswith("%25") and zone_id != "%25":
                         zone_id = zone_id[3:]
@@ -296,15 +299,15 @@
                 return six.ensure_str(
                     b".".join([_idna_encode(label) for label in host.split(".")])
                 )
     return host
 
 
 def _idna_encode(name):
-    if name and any([ord(x) > 128 for x in name]):
+    if name and any(ord(x) >= 128 for x in name):
         try:
             import idna
         except ImportError:
             six.raise_from(
                 LocationParseError("Unable to parse URL without the 'idna' module"),
                 None,
             )
@@ -327,15 +330,15 @@
     return target
 
 
 def parse_url(url):
     """
     Given a url, return a parsed :class:`.Url` namedtuple. Best-effort is
     performed to parse incomplete urls. Fields not provided will be None.
-    This parser is RFC 3986 compliant.
+    This parser is RFC 3986 and RFC 6874 compliant.
 
     The parser logic and helper functions are based heavily on
     work done in the ``rfc3986`` module.
 
     :param str url: URL to parse into a :class:`.Url` namedtuple.
 
     Partly backwards-compatible with :mod:`urlparse`.
```

### Comparing `newrelic-8.8.0/newrelic/packages/urllib3/util/wait.py` & `newrelic-8.8.1/newrelic/packages/urllib3/util/wait.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 # fall back to select() in case poll() is somehow broken or missing.
 
 if sys.version_info >= (3, 5):
     # Modern Python, that retries syscalls by default
     def _retry_on_intr(fn, timeout):
         return fn(timeout)
 
-
 else:
     # Old and broken Pythons.
     def _retry_on_intr(fn, timeout):
         if timeout is None:
             deadline = float("inf")
         else:
             deadline = monotonic() + timeout
```

### Comparing `newrelic-8.8.0/newrelic/packages/wrapt/LICENSE` & `newrelic-8.8.1/newrelic/packages/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/wrapt/__init__.py` & `newrelic-8.8.1/newrelic/packages/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/wrapt/_wrappers.c` & `newrelic-8.8.1/newrelic/packages/wrapt/_wrappers.c`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/wrapt/arguments.py` & `newrelic-8.8.1/newrelic/packages/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/wrapt/decorators.py` & `newrelic-8.8.1/newrelic/packages/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/wrapt/importer.py` & `newrelic-8.8.1/newrelic/packages/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/packages/wrapt/wrappers.py` & `newrelic-8.8.1/newrelic/packages/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/samplers/__init__.py` & `newrelic-8.8.1/newrelic/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/samplers/cpu_usage.py` & `newrelic-8.8.1/newrelic/samplers/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/samplers/data_sampler.py` & `newrelic-8.8.1/newrelic/samplers/data_sampler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/samplers/decorators.py` & `newrelic-8.8.1/newrelic/samplers/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/samplers/gc_data.py` & `newrelic-8.8.1/newrelic/samplers/gc_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic/samplers/memory_usage.py` & `newrelic-8.8.1/newrelic/samplers/memory_usage.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/newrelic.egg-info/PKG-INFO` & `newrelic-8.8.1/newrelic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic
-Version: 8.8.0
+Version: 8.8.1
 Summary: New Relic Python Agent
 Home-page: https://docs.newrelic.com/docs/apm/agents/python-agent/
 Author: New Relic
 Author-email: support@newrelic.com
 Maintainer: New Relic
 Maintainer-email: support@newrelic.com
 License: Apache-2.0
```

### Comparing `newrelic-8.8.0/newrelic.egg-info/SOURCES.txt` & `newrelic-8.8.1/newrelic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .mega-linter.yml
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 ROADMAP.md
 THIRD_PARTY_NOTICES.md
+codecov.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/CODEOWNERS
@@ -17,15 +18,20 @@
 .github/pull_request_template.md
 .github/stale.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/troubleshooting.md
 .github/actions/setup-python-matrix/action.yml
+.github/containers/Dockerfile
+.github/containers/Makefile
+.github/containers/install-python.sh
+.github/containers/requirements.txt
 .github/scripts/retry.sh
+.github/workflows/build-ci-image.yml
 .github/workflows/deploy-python.yml
 .github/workflows/get-envs.py
 .github/workflows/mega-linter.yml
 .github/workflows/tests.yml
 newrelic/__init__.py
 newrelic/agent.py
 newrelic/config.py
@@ -97,14 +103,15 @@
 newrelic/common/certs.py
 newrelic/common/coroutine.py
 newrelic/common/encoding_utils.py
 newrelic/common/log_file.py
 newrelic/common/object_names.py
 newrelic/common/object_wrapper.py
 newrelic/common/package_version_utils.py
+newrelic/common/signature.py
 newrelic/common/stopwatch.py
 newrelic/common/streaming_utils.py
 newrelic/common/system_info.py
 newrelic/common/utilization.py
 newrelic/core/__init__.py
 newrelic/core/_thread_utilization.c
 newrelic/core/adaptive_sampler.py
@@ -236,40 +243,46 @@
 newrelic/hooks/framework_grpc.py
 newrelic/hooks/framework_pylons.py
 newrelic/hooks/framework_pyramid.py
 newrelic/hooks/framework_sanic.py
 newrelic/hooks/framework_starlette.py
 newrelic/hooks/framework_strawberry.py
 newrelic/hooks/framework_tornado.py
-newrelic/hooks/framework_twisted.py
 newrelic/hooks/framework_web2py.py
 newrelic/hooks/framework_webpy.py
 newrelic/hooks/logger_logging.py
 newrelic/hooks/logger_loguru.py
 newrelic/hooks/memcache_memcache.py
-newrelic/hooks/memcache_pylibmc.py
-newrelic/hooks/memcache_umemcache.py
 newrelic/hooks/messagebroker_confluentkafka.py
 newrelic/hooks/messagebroker_kafkapython.py
 newrelic/hooks/messagebroker_pika.py
 newrelic/hooks/middleware_flask_compress.py
 newrelic/hooks/middleware_weberror.py
-newrelic/hooks/nosql_pymongo.py
-newrelic/hooks/nosql_redis.py
-newrelic/hooks/solr_pysolr.py
-newrelic/hooks/solr_solrpy.py
 newrelic/hooks/template_genshi.py
 newrelic/hooks/template_jinja2.py
 newrelic/hooks/template_mako.py
 newrelic/network/__init__.py
 newrelic/network/addresses.py
 newrelic/network/exceptions.py
 newrelic/packages/__init__.py
 newrelic/packages/asgiref_compatibility.py
 newrelic/packages/six.py
+newrelic/packages/isort/LICENSE
+newrelic/packages/isort/__init__.py
+newrelic/packages/isort/stdlibs/__init__.py
+newrelic/packages/isort/stdlibs/all.py
+newrelic/packages/isort/stdlibs/py2.py
+newrelic/packages/isort/stdlibs/py27.py
+newrelic/packages/isort/stdlibs/py3.py
+newrelic/packages/isort/stdlibs/py310.py
+newrelic/packages/isort/stdlibs/py311.py
+newrelic/packages/isort/stdlibs/py36.py
+newrelic/packages/isort/stdlibs/py37.py
+newrelic/packages/isort/stdlibs/py38.py
+newrelic/packages/isort/stdlibs/py39.py
 newrelic/packages/urllib3/LICENSE.txt
 newrelic/packages/urllib3/__init__.py
 newrelic/packages/urllib3/_collections.py
 newrelic/packages/urllib3/_version.py
 newrelic/packages/urllib3/connection.py
 newrelic/packages/urllib3/connectionpool.py
 newrelic/packages/urllib3/exceptions.py
@@ -288,24 +301,23 @@
 newrelic/packages/urllib3/contrib/_securetransport/__init__.py
 newrelic/packages/urllib3/contrib/_securetransport/bindings.py
 newrelic/packages/urllib3/contrib/_securetransport/low_level.py
 newrelic/packages/urllib3/packages/__init__.py
 newrelic/packages/urllib3/packages/six.py
 newrelic/packages/urllib3/packages/backports/__init__.py
 newrelic/packages/urllib3/packages/backports/makefile.py
-newrelic/packages/urllib3/packages/ssl_match_hostname/__init__.py
-newrelic/packages/urllib3/packages/ssl_match_hostname/_implementation.py
 newrelic/packages/urllib3/util/__init__.py
 newrelic/packages/urllib3/util/connection.py
 newrelic/packages/urllib3/util/proxy.py
 newrelic/packages/urllib3/util/queue.py
 newrelic/packages/urllib3/util/request.py
 newrelic/packages/urllib3/util/response.py
 newrelic/packages/urllib3/util/retry.py
 newrelic/packages/urllib3/util/ssl_.py
+newrelic/packages/urllib3/util/ssl_match_hostname.py
 newrelic/packages/urllib3/util/ssltransport.py
 newrelic/packages/urllib3/util/timeout.py
 newrelic/packages/urllib3/util/url.py
 newrelic/packages/urllib3/util/wait.py
 newrelic/packages/wrapt/LICENSE
 newrelic/packages/wrapt/__init__.py
 newrelic/packages/wrapt/_wrappers.c
@@ -337,14 +349,17 @@
 tests/adapter_gunicorn/test_asgi_app.py
 tests/adapter_gunicorn/test_gaiohttp.py
 tests/adapter_gunicorn/worker.py
 tests/adapter_hypercorn/conftest.py
 tests/adapter_hypercorn/test_hypercorn.py
 tests/adapter_uvicorn/conftest.py
 tests/adapter_uvicorn/test_uvicorn.py
+tests/adapter_waitress/_application.py
+tests/adapter_waitress/conftest.py
+tests/adapter_waitress/test_wsgi.py
 tests/agent_features/_test_async_coroutine_trace.py
 tests/agent_features/_test_async_coroutine_transaction.py
 tests/agent_features/_test_code_level_metrics.py
 tests/agent_features/conftest.py
 tests/agent_features/test_apdex_metrics.py
 tests/agent_features/test_asgi_browser.py
 tests/agent_features/test_asgi_distributed_tracing.py
@@ -412,14 +427,15 @@
 tests/agent_unittests/test_http_client.py
 tests/agent_unittests/test_import_hook.py
 tests/agent_unittests/test_infinite_trace_settings.py
 tests/agent_unittests/test_package_version_utils.py
 tests/agent_unittests/test_region_aware_settings.py
 tests/agent_unittests/test_sampler_metrics.py
 tests/agent_unittests/test_serverless_mode_settings.py
+tests/agent_unittests/test_signature.py
 tests/agent_unittests/test_trace_cache.py
 tests/agent_unittests/test_utilization_settings.py
 tests/application_celery/conftest.py
 tests/application_celery/tasks.py
 tests/application_celery/test_celery.py
 tests/application_celery/test_celery_max_tasks_per_child.py
 tests/application_gearman/conftest.py
@@ -803,24 +819,24 @@
 tests/datastore_psycopg2/test_slow_sql.py
 tests/datastore_psycopg2/test_span_event.py
 tests/datastore_psycopg2/test_trace_node.py
 tests/datastore_psycopg2/utils.py
 tests/datastore_psycopg2cffi/conftest.py
 tests/datastore_psycopg2cffi/test_database.py
 tests/datastore_psycopg2cffi/test_explain_plans.py
-tests/datastore_pyelasticsearch/conftest.py
-tests/datastore_pyelasticsearch/test_pyelasticsearch.py
 tests/datastore_pylibmc/conftest.py
 tests/datastore_pylibmc/test_memcache.py
 tests/datastore_pymemcache/conftest.py
 tests/datastore_pymemcache/test_memcache.py
 tests/datastore_pymongo/conftest.py
 tests/datastore_pymongo/test_pymongo.py
 tests/datastore_pymysql/conftest.py
 tests/datastore_pymysql/test_database.py
+tests/datastore_pyodbc/conftest.py
+tests/datastore_pyodbc/test_pyodbc.py
 tests/datastore_pysolr/conftest.py
 tests/datastore_pysolr/test_solr.py
 tests/datastore_redis/conftest.py
 tests/datastore_redis/test_custom_conn_pool.py
 tests/datastore_redis/test_execute_command.py
 tests/datastore_redis/test_get_and_set.py
 tests/datastore_redis/test_instance_info.py
@@ -830,16 +846,14 @@
 tests/datastore_redis/test_trace_node.py
 tests/datastore_redis/test_uninstrumented_methods.py
 tests/datastore_solrpy/conftest.py
 tests/datastore_solrpy/test_solr.py
 tests/datastore_sqlite/conftest.py
 tests/datastore_sqlite/test_database.py
 tests/datastore_sqlite/test_obfuscation.py
-tests/datastore_umemcache/conftest.py
-tests/datastore_umemcache/test_memcache.py
 tests/external_boto3/conftest.py
 tests/external_boto3/test_boto3_iam.py
 tests/external_boto3/test_boto3_s3.py
 tests/external_boto3/test_boto3_sns.py
 tests/external_botocore/conftest.py
 tests/external_botocore/test_botocore_dynamodb.py
 tests/external_botocore/test_botocore_ec2.py
@@ -999,14 +1013,16 @@
 tests/messagebroker_pika/test_distributed_tracing.py
 tests/messagebroker_pika/test_memory_leak.py
 tests/messagebroker_pika/test_pika_async_connection_consume.py
 tests/messagebroker_pika/test_pika_blocking_connection_consume.py
 tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
 tests/messagebroker_pika/test_pika_produce.py
 tests/messagebroker_pika/test_pika_supportability.py
+tests/template_genshi/conftest.py
+tests/template_genshi/test_genshi.py
 tests/template_mako/conftest.py
 tests/template_mako/test_mako.py
 tests/testing_support/__init__.py
 tests/testing_support/asgi_testing.py
 tests/testing_support/db_settings.py
 tests/testing_support/external_fixtures.py
 tests/testing_support/fixtures.py
@@ -1019,26 +1035,31 @@
 tests/testing_support/fixture/__init__.py
 tests/testing_support/fixture/event_loop.py
 tests/testing_support/validators/__init__.py
 tests/testing_support/validators/validate_apdex_metrics.py
 tests/testing_support/validators/validate_application_error_event_count.py
 tests/testing_support/validators/validate_application_error_trace_count.py
 tests/testing_support/validators/validate_application_errors.py
+tests/testing_support/validators/validate_browser_attributes.py
 tests/testing_support/validators/validate_code_level_metrics.py
 tests/testing_support/validators/validate_cross_process_headers.py
+tests/testing_support/validators/validate_custom_event_collector_json.py
 tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
 tests/testing_support/validators/validate_custom_parameters.py
 tests/testing_support/validators/validate_database_duration.py
 tests/testing_support/validators/validate_database_node.py
 tests/testing_support/validators/validate_database_trace_inputs.py
 tests/testing_support/validators/validate_datastore_trace_inputs.py
 tests/testing_support/validators/validate_distributed_trace_accepted.py
 tests/testing_support/validators/validate_distributed_tracing_header.py
+tests/testing_support/validators/validate_error_event_attributes.py
+tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py
 tests/testing_support/validators/validate_error_event_collector_json.py
 tests/testing_support/validators/validate_error_trace_attributes.py
+tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py
 tests/testing_support/validators/validate_error_trace_collector_json.py
 tests/testing_support/validators/validate_external_node_params.py
 tests/testing_support/validators/validate_function_called.py
 tests/testing_support/validators/validate_internal_metrics.py
 tests/testing_support/validators/validate_log_event_collector_json.py
 tests/testing_support/validators/validate_log_event_count.py
 tests/testing_support/validators/validate_log_event_count_outside_transaction.py
@@ -1061,8 +1082,10 @@
 tests/testing_support/validators/validate_transaction_error_trace_attributes.py
 tests/testing_support/validators/validate_transaction_errors.py
 tests/testing_support/validators/validate_transaction_event_attributes.py
 tests/testing_support/validators/validate_transaction_event_collector_json.py
 tests/testing_support/validators/validate_transaction_metrics.py
 tests/testing_support/validators/validate_transaction_slow_sql_count.py
 tests/testing_support/validators/validate_transaction_trace_attributes.py
-tests/testing_support/validators/validate_tt_collector_json.py
+tests/testing_support/validators/validate_tt_collector_json.py
+tests/testing_support/validators/validate_tt_parameters.py
+tests/testing_support/validators/validate_tt_segment_params.py
```

### Comparing `newrelic-8.8.0/setup.py` & `newrelic-8.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,21 +98,22 @@
     "newrelic.core",
     "newrelic.extras",
     "newrelic.extras.framework_django",
     "newrelic.extras.framework_django.templatetags",
     "newrelic.hooks",
     "newrelic.network",
     "newrelic/packages",
+    "newrelic/packages/isort",
+    "newrelic/packages/isort/stdlibs",
     "newrelic/packages/urllib3",
     "newrelic/packages/urllib3/util",
     "newrelic/packages/urllib3/contrib",
     "newrelic/packages/urllib3/contrib/_securetransport",
     "newrelic/packages/urllib3/packages",
     "newrelic/packages/urllib3/packages/backports",
-    "newrelic/packages/urllib3/packages/ssl_match_hostname",
     "newrelic/packages/wrapt",
     "newrelic.samplers",
 ]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
@@ -171,15 +172,14 @@
             return ctypes.util.find_library("rt")
     except Exception:
         pass
 
 
 def run_setup(with_extensions):
     def _run_setup():
-
         # Create a local copy of kwargs, if there is no c compiler run_setup
         # will need to be re-run, and these arguments can not be present.
 
         kwargs_tmp = dict(kwargs)
 
         if with_extensions:
             monotonic_libraries = []
@@ -240,15 +240,14 @@
     run_setup(with_extensions=with_extensions)
 
 else:
     try:
         run_setup(with_extensions=True)
 
     except BuildExtFailed:
-
         print(75 * "*")
 
         print(WARNING)
         print("INFO: Trying to build without extensions.")
 
         print()
         print(75 * "*")
```

### Comparing `newrelic-8.8.0/tests/adapter_cheroot/conftest.py` & `newrelic-8.8.1/tests/adapter_cheroot/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_cheroot/test_wsgi.py` & `newrelic-8.8.1/tests/adapter_cheroot/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_daphne/conftest.py` & `newrelic-8.8.1/tests/adapter_daphne/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_daphne/test_daphne.py` & `newrelic-8.8.1/tests/adapter_daphne/test_daphne.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gevent/_application.py` & `newrelic-8.8.1/tests/adapter_gevent/_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gevent/conftest.py` & `newrelic-8.8.1/tests/datastore_pylibmc/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,29 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-import webtest
 
 from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
 
+
 _default_settings = {
     'transaction_tracer.explain_threshold': 0.0,
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
-    'debug.record_transaction_failure': True,
-    'debug.disable_harvest_until_shutdown': False,
+    'debug.record_transaction_failure': True
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (adapter_gevent)',
-        default_settings=_default_settings)
-
-@pytest.fixture(autouse=True, scope='session')
-def target_application():
-    import _application
-    port = _application.setup_application()
-    return webtest.TestApp('http://localhost:%d' % port)
+        app_name='Python Agent Test (datastore_pylibmc)',
+        default_settings=_default_settings,
+        linked_applications=['Python Agent Test (datastore)'])
```

### Comparing `newrelic-8.8.0/tests/adapter_gevent/test_patching.py` & `newrelic-8.8.1/tests/adapter_gevent/test_patching.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gevent/test_pywsgi.py` & `newrelic-8.8.1/tests/adapter_gevent/test_pywsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gunicorn/app.py` & `newrelic-8.8.1/tests/adapter_gunicorn/app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gunicorn/asgi_app.py` & `newrelic-8.8.1/tests/adapter_gunicorn/asgi_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gunicorn/async_app.py` & `newrelic-8.8.1/tests/adapter_gunicorn/async_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gunicorn/conftest.py` & `newrelic-8.8.1/tests/adapter_gunicorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py` & `newrelic-8.8.1/tests/adapter_gunicorn/test_aiohttp_app_factory.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gunicorn/test_asgi_app.py` & `newrelic-8.8.1/tests/adapter_gunicorn/test_asgi_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gunicorn/test_gaiohttp.py` & `newrelic-8.8.1/tests/adapter_gunicorn/test_gaiohttp.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_gunicorn/worker.py` & `newrelic-8.8.1/tests/adapter_gunicorn/worker.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_hypercorn/conftest.py` & `newrelic-8.8.1/tests/adapter_hypercorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_hypercorn/test_hypercorn.py` & `newrelic-8.8.1/tests/adapter_hypercorn/test_hypercorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_uvicorn/conftest.py` & `newrelic-8.8.1/tests/adapter_uvicorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/adapter_uvicorn/test_uvicorn.py` & `newrelic-8.8.1/tests/adapter_uvicorn/test_uvicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/_test_async_coroutine_trace.py` & `newrelic-8.8.1/tests/agent_features/_test_async_coroutine_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/_test_async_coroutine_transaction.py` & `newrelic-8.8.1/tests/agent_features/_test_async_coroutine_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/_test_code_level_metrics.py` & `newrelic-8.8.1/tests/agent_features/_test_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/conftest.py` & `newrelic-8.8.1/tests/agent_features/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_apdex_metrics.py` & `newrelic-8.8.1/tests/agent_features/test_apdex_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_asgi_browser.py` & `newrelic-8.8.1/tests/agent_features/test_asgi_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     assert data["errorBeacon"] == settings.error_beacon
 
     assert data["applicationTime"] >= 0
     assert data["queueTime"] >= 0
 
     obfuscation_key = settings.license_key[:13]
 
-    type_transaction_data = unicode if six.PY2 else str  # noqa: F821
+    type_transaction_data = unicode if six.PY2 else str  # noqa: F821, pylint: disable=E0602
     assert isinstance(data["transactionName"], type_transaction_data)
 
     txn_name = deobfuscate(data["transactionName"], obfuscation_key)
 
     assert txn_name == "WebTransaction/Uri/"
 
     assert "atts" not in data
```

### Comparing `newrelic-8.8.0/tests/agent_features/test_asgi_distributed_tracing.py` & `newrelic-8.8.1/tests/agent_features/test_asgi_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_asgi_transaction.py` & `newrelic-8.8.1/tests/agent_features/test_asgi_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_asgi_w3c_trace_context.py` & `newrelic-8.8.1/tests/agent_features/test_asgi_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_async_context_propagation.py` & `newrelic-8.8.1/tests/agent_features/test_async_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_async_timing.py` & `newrelic-8.8.1/tests/agent_features/test_async_timing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_attribute.py` & `newrelic-8.8.1/tests/agent_features/test_attribute.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_attributes_in_action.py` & `newrelic-8.8.1/tests/agent_features/test_attributes_in_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,30 @@
 import webtest
 from testing_support.fixtures import (
     cat_enabled,
     dt_enabled,
     override_application_settings,
     reset_core_stats_engine,
     validate_attributes,
+)
+from testing_support.validators.validate_browser_attributes import (
     validate_browser_attributes,
+)
+from testing_support.validators.validate_error_event_attributes import (
     validate_error_event_attributes,
+)
+from testing_support.validators.validate_error_event_attributes_outside_transaction import (
     validate_error_event_attributes_outside_transaction,
-    validate_error_trace_attributes_outside_transaction,
 )
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
+from testing_support.validators.validate_error_trace_attributes_outside_transaction import (
+    validate_error_trace_attributes_outside_transaction,
+)
 from testing_support.validators.validate_span_events import validate_span_events
 from testing_support.validators.validate_transaction_error_trace_attributes import (
     validate_transaction_error_trace_attributes,
 )
 from testing_support.validators.validate_transaction_event_attributes import (
     validate_transaction_event_attributes,
 )
@@ -39,15 +47,15 @@
     validate_transaction_trace_attributes,
 )
 
 from newrelic.api.application import application_instance as application
 from newrelic.api.background_task import background_task
 from newrelic.api.message_transaction import message_transaction
 from newrelic.api.time_trace import notice_error
-from newrelic.api.transaction import add_custom_attribute, current_transaction, set_user_id
+from newrelic.api.transaction import add_custom_attribute, set_user_id
 from newrelic.api.wsgi_application import wsgi_application
 from newrelic.common.object_names import callable_name
 
 try:
     from testing_support.asgi_testing import AsgiTest
     from testing_support.sample_asgi_applications import normal_asgi_application
 except SyntaxError:
@@ -926,43 +934,50 @@
     pass
 
 
 _required_agent_attributes = ["enduser.id"]
 _forgone_agent_attributes = []
 
 
-@pytest.mark.parametrize('input_user_id, reported_user_id, high_security',(
+@pytest.mark.parametrize(
+    "input_user_id, reported_user_id, high_security",
+    (
         ("1234", "1234", True),
-        ("a" * 260,  "a" * 255, False),
-))
+        ("a" * 260, "a" * 255, False),
+    ),
+)
 def test_enduser_id_attribute_api_valid_types(input_user_id, reported_user_id, high_security):
     @reset_core_stats_engine()
     @validate_error_trace_attributes(
         callable_name(ValueError), exact_attrs={"user": {}, "intrinsic": {}, "agent": {"enduser.id": reported_user_id}}
     )
-    @validate_error_event_attributes(exact_attrs={"user": {}, "intrinsic": {}, "agent": {"enduser.id": reported_user_id}})
+    @validate_error_event_attributes(
+        exact_attrs={"user": {}, "intrinsic": {}, "agent": {"enduser.id": reported_user_id}}
+    )
     @validate_attributes("agent", _required_agent_attributes, _forgone_agent_attributes)
     @background_task()
     @override_application_settings({"high_security": high_security})
     def _test():
         set_user_id(input_user_id)
 
         try:
             raise ValueError()
         except Exception:
             notice_error()
+
     _test()
 
 
-@pytest.mark.parametrize('input_user_id',(None, '', 123))
+@pytest.mark.parametrize("input_user_id", (None, "", 123))
 def test_enduser_id_attribute_api_invalid_types(input_user_id):
     @reset_core_stats_engine()
     @validate_attributes("agent", [], ["enduser.id"])
     @background_task()
     def _test():
         set_user_id(input_user_id)
 
         try:
             raise ValueError()
         except Exception:
             notice_error()
+
     _test()
```

### Comparing `newrelic-8.8.0/tests/agent_features/test_background_task.py` & `newrelic-8.8.1/tests/agent_features/test_background_task.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_browser.py` & `newrelic-8.8.1/tests/agent_features/test_browser.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_browser_middleware.py` & `newrelic-8.8.1/tests/agent_features/test_browser_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_cat.py` & `newrelic-8.8.1/tests/agent_features/test_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_code_level_metrics.py` & `newrelic-8.8.1/tests/agent_features/test_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_collector_payloads.py` & `newrelic-8.8.1/tests/agent_features/test_collector_payloads.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 import webtest
-from testing_support.fixtures import (
-    override_application_settings,
-    validate_custom_event_collector_json,
-)
+from testing_support.fixtures import override_application_settings
 from testing_support.sample_applications import (
     simple_app,
     simple_custom_event_app,
     simple_exceptional_app,
 )
+from testing_support.validators.validate_custom_event_collector_json import (
+    validate_custom_event_collector_json,
+)
 from testing_support.validators.validate_error_event_collector_json import (
     validate_error_event_collector_json,
 )
 from testing_support.validators.validate_error_trace_collector_json import (
     validate_error_trace_collector_json,
 )
 from testing_support.validators.validate_log_event_collector_json import (
```

### Comparing `newrelic-8.8.0/tests/agent_features/test_configuration.py` & `newrelic-8.8.1/tests/agent_features/test_configuration.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_coroutine_trace.py` & `newrelic-8.8.1/tests/agent_features/test_coroutine_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_coroutine_transaction.py` & `newrelic-8.8.1/tests/agent_features/test_coroutine_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_custom_events.py` & `newrelic-8.8.1/tests/agent_features/test_custom_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_dead_transactions.py` & `newrelic-8.8.1/tests/agent_features/test_dead_transactions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_distributed_tracing.py` & `newrelic-8.8.1/tests/agent_features/test_distributed_tracing.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,361 +8,354 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import copy
 import json
+
 import pytest
 import webtest
-import copy
+from testing_support.fixtures import override_application_settings, validate_attributes
+from testing_support.validators.validate_error_event_attributes import (
+    validate_error_event_attributes,
+)
+from testing_support.validators.validate_transaction_event_attributes import (
+    validate_transaction_event_attributes,
+)
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
 
 from newrelic.api.application import application_instance
-from newrelic.api.background_task import background_task, BackgroundTask
-from newrelic.api.transaction import (current_transaction, current_trace_id,
-        current_span_id)
+from newrelic.api.background_task import BackgroundTask, background_task
 from newrelic.api.time_trace import current_trace
+from newrelic.api.transaction import (
+    current_span_id,
+    current_trace_id,
+    current_transaction,
+)
 from newrelic.api.web_transaction import WSGIWebTransaction
 from newrelic.api.wsgi_application import wsgi_application
 
-from testing_support.fixtures import (override_application_settings,
-        validate_attributes, 
-        validate_error_event_attributes)
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-from testing_support.validators.validate_transaction_event_attributes import validate_transaction_event_attributes
-
-distributed_trace_intrinsics = ['guid', 'traceId', 'priority', 'sampled']
-inbound_payload_intrinsics = ['parent.type', 'parent.app', 'parent.account',
-        'parent.transportType', 'parent.transportDuration']
+distributed_trace_intrinsics = ["guid", "traceId", "priority", "sampled"]
+inbound_payload_intrinsics = [
+    "parent.type",
+    "parent.app",
+    "parent.account",
+    "parent.transportType",
+    "parent.transportDuration",
+]
 
 payload = {
-    'v': [0, 1],
-    'd': {
-        'ac': '1',
-        'ap': '2827902',
-        'id': '7d3efb1b173fecfa',
-        'pa': '5e5733a911cfbc73',
-        'pr': 10.001,
-        'sa': True,
-        'ti': 1518469636035,
-        'tr': 'd6b4ba0c3a712ca',
-        'ty': 'App',
-    }
+    "v": [0, 1],
+    "d": {
+        "ac": "1",
+        "ap": "2827902",
+        "id": "7d3efb1b173fecfa",
+        "pa": "5e5733a911cfbc73",
+        "pr": 10.001,
+        "sa": True,
+        "ti": 1518469636035,
+        "tr": "d6b4ba0c3a712ca",
+        "ty": "App",
+    },
 }
-parent_order = ['parent_type', 'parent_account',
-                'parent_app', 'parent_transport_type']
+parent_order = ["parent_type", "parent_account", "parent_app", "parent_transport_type"]
 parent_info = {
-    'parent_type': payload['d']['ty'],
-    'parent_account': payload['d']['ac'],
-    'parent_app': payload['d']['ap'],
-    'parent_transport_type': 'HTTP'
+    "parent_type": payload["d"]["ty"],
+    "parent_account": payload["d"]["ac"],
+    "parent_app": payload["d"]["ap"],
+    "parent_transport_type": "HTTP",
 }
 
 
 @wsgi_application()
 def target_wsgi_application(environ, start_response):
-    status = '200 OK'
-    output = b'hello world'
-    response_headers = [('Content-type', 'text/html; charset=utf-8'),
-                        ('Content-Length', str(len(output)))]
+    status = "200 OK"
+    output = b"hello world"
+    response_headers = [("Content-type", "text/html; charset=utf-8"), ("Content-Length", str(len(output)))]
 
     txn = current_transaction()
 
     # Make assertions on the WSGIWebTransaction object
     assert txn._distributed_trace_state
-    assert txn.parent_type == 'App'
-    assert txn.parent_app == '2827902'
-    assert txn.parent_account == '1'
-    assert txn.parent_span == '7d3efb1b173fecfa'
-    assert txn.parent_transport_type == 'HTTP'
+    assert txn.parent_type == "App"
+    assert txn.parent_app == "2827902"
+    assert txn.parent_account == "1"
+    assert txn.parent_span == "7d3efb1b173fecfa"
+    assert txn.parent_transport_type == "HTTP"
     assert isinstance(txn.parent_transport_duration, float)
-    assert txn._trace_id == 'd6b4ba0c3a712ca'
+    assert txn._trace_id == "d6b4ba0c3a712ca"
     assert txn.priority == 10.001
     assert txn.sampled
 
     start_response(status, response_headers)
     return [output]
 
 
 test_application = webtest.TestApp(target_wsgi_application)
 
 _override_settings = {
-    'trusted_account_key': '1',
-    'distributed_tracing.enabled': True,
+    "trusted_account_key": "1",
+    "distributed_tracing.enabled": True,
 }
 
 
 _metrics = [
-        ('Supportability/DistributedTrace/AcceptPayload/Success', 1),
-        ('Supportability/TraceContext/Accept/Success', None)
+    ("Supportability/DistributedTrace/AcceptPayload/Success", 1),
+    ("Supportability/TraceContext/Accept/Success", None),
 ]
 
 
 @override_application_settings(_override_settings)
-@validate_transaction_metrics(
-    '',
-    group='Uri',
-    rollup_metrics=_metrics)
+@validate_transaction_metrics("", group="Uri", rollup_metrics=_metrics)
 def test_distributed_tracing_web_transaction():
-    headers = {'newrelic': json.dumps(payload)}
-    response = test_application.get('/', headers=headers)
-    assert 'X-NewRelic-App-Data' not in response.headers
+    headers = {"newrelic": json.dumps(payload)}
+    response = test_application.get("/", headers=headers)
+    assert "X-NewRelic-App-Data" not in response.headers
 
 
-@pytest.mark.parametrize('span_events', (True, False))
-@pytest.mark.parametrize('accept_payload', (True, False))
+@pytest.mark.parametrize("span_events", (True, False))
+@pytest.mark.parametrize("accept_payload", (True, False))
 def test_distributed_trace_attributes(span_events, accept_payload):
     if accept_payload:
-        _required_intrinsics = (
-                distributed_trace_intrinsics + inbound_payload_intrinsics)
+        _required_intrinsics = distributed_trace_intrinsics + inbound_payload_intrinsics
         _forgone_txn_intrinsics = []
         _forgone_error_intrinsics = []
         _exact_intrinsics = {
-            'parent.type': 'Mobile',
-            'parent.app': '2827902',
-            'parent.account': '1',
-            'parent.transportType': 'HTTP',
-            'traceId': 'd6b4ba0c3a712ca',
+            "parent.type": "Mobile",
+            "parent.app": "2827902",
+            "parent.account": "1",
+            "parent.transportType": "HTTP",
+            "traceId": "d6b4ba0c3a712ca",
         }
-        _exact_txn_attributes = {'agent': {}, 'user': {},
-                'intrinsic': _exact_intrinsics.copy()}
-        _exact_error_attributes = {'agent': {}, 'user': {},
-                'intrinsic': _exact_intrinsics.copy()}
-        _exact_txn_attributes['intrinsic']['parentId'] = '7d3efb1b173fecfa'
-        _exact_txn_attributes['intrinsic']['parentSpanId'] = 'c86df80de2e6f51c'
-
-        _forgone_error_intrinsics.append('parentId')
-        _forgone_error_intrinsics.append('parentSpanId')
-        _forgone_txn_intrinsics.append('grandparentId')
-        _forgone_error_intrinsics.append('grandparentId')
-
-        _required_attributes = {
-                'intrinsic': _required_intrinsics, 'agent': [], 'user': []}
-        _forgone_txn_attributes = {'intrinsic': _forgone_txn_intrinsics,
-                'agent': [], 'user': []}
-        _forgone_error_attributes = {'intrinsic': _forgone_error_intrinsics,
-                'agent': [], 'user': []}
+        _exact_txn_attributes = {"agent": {}, "user": {}, "intrinsic": _exact_intrinsics.copy()}
+        _exact_error_attributes = {"agent": {}, "user": {}, "intrinsic": _exact_intrinsics.copy()}
+        _exact_txn_attributes["intrinsic"]["parentId"] = "7d3efb1b173fecfa"
+        _exact_txn_attributes["intrinsic"]["parentSpanId"] = "c86df80de2e6f51c"
+
+        _forgone_error_intrinsics.append("parentId")
+        _forgone_error_intrinsics.append("parentSpanId")
+        _forgone_txn_intrinsics.append("grandparentId")
+        _forgone_error_intrinsics.append("grandparentId")
+
+        _required_attributes = {"intrinsic": _required_intrinsics, "agent": [], "user": []}
+        _forgone_txn_attributes = {"intrinsic": _forgone_txn_intrinsics, "agent": [], "user": []}
+        _forgone_error_attributes = {"intrinsic": _forgone_error_intrinsics, "agent": [], "user": []}
     else:
         _required_intrinsics = distributed_trace_intrinsics
-        _forgone_txn_intrinsics = _forgone_error_intrinsics = \
-                inbound_payload_intrinsics + ['grandparentId', 'parentId',
-                'parentSpanId']
-
-        _required_attributes = {
-                'intrinsic': _required_intrinsics, 'agent': [], 'user': []}
-        _forgone_txn_attributes = {'intrinsic': _forgone_txn_intrinsics,
-                'agent': [], 'user': []}
-        _forgone_error_attributes = {'intrinsic': _forgone_error_intrinsics,
-                'agent': [], 'user': []}
+        _forgone_txn_intrinsics = _forgone_error_intrinsics = inbound_payload_intrinsics + [
+            "grandparentId",
+            "parentId",
+            "parentSpanId",
+        ]
+
+        _required_attributes = {"intrinsic": _required_intrinsics, "agent": [], "user": []}
+        _forgone_txn_attributes = {"intrinsic": _forgone_txn_intrinsics, "agent": [], "user": []}
+        _forgone_error_attributes = {"intrinsic": _forgone_error_intrinsics, "agent": [], "user": []}
         _exact_txn_attributes = _exact_error_attributes = None
 
     _forgone_trace_intrinsics = _forgone_error_intrinsics
 
     test_settings = _override_settings.copy()
-    test_settings['span_events.enabled'] = span_events
+    test_settings["span_events.enabled"] = span_events
 
     @override_application_settings(test_settings)
-    @validate_transaction_event_attributes(
-            _required_attributes, _forgone_txn_attributes,
-            _exact_txn_attributes)
-    @validate_error_event_attributes(
-            _required_attributes, _forgone_error_attributes,
-            _exact_error_attributes)
-    @validate_attributes('intrinsic',
-            _required_intrinsics, _forgone_trace_intrinsics)
-    @background_task(name='test_distributed_trace_attributes')
+    @validate_transaction_event_attributes(_required_attributes, _forgone_txn_attributes, _exact_txn_attributes)
+    @validate_error_event_attributes(_required_attributes, _forgone_error_attributes, _exact_error_attributes)
+    @validate_attributes("intrinsic", _required_intrinsics, _forgone_trace_intrinsics)
+    @background_task(name="test_distributed_trace_attributes")
     def _test():
         txn = current_transaction()
 
         payload = {
             "v": [0, 1],
             "d": {
                 "ty": "Mobile",
                 "ac": "1",
                 "ap": "2827902",
                 "id": "c86df80de2e6f51c",
                 "tr": "d6b4ba0c3a712ca",
                 "ti": 1518469636035,
-                "tx": "7d3efb1b173fecfa"
-            }
+                "tx": "7d3efb1b173fecfa",
+            },
         }
-        payload['d']['pa'] = "5e5733a911cfbc73"
+        payload["d"]["pa"] = "5e5733a911cfbc73"
 
         if accept_payload:
             result = txn.accept_distributed_trace_payload(payload)
             assert result
         else:
             txn._create_distributed_trace_payload()
 
         try:
-            raise ValueError('cookies')
+            raise ValueError("cookies")
         except ValueError:
             txn.notice_error()
 
     _test()
 
 
 _forgone_attributes = {
-    'agent': [],
-    'user': [],
-    'intrinsic': (inbound_payload_intrinsics + ['grandparentId']),
+    "agent": [],
+    "user": [],
+    "intrinsic": (inbound_payload_intrinsics + ["grandparentId"]),
 }
 
 
 @override_application_settings(_override_settings)
-@validate_transaction_event_attributes(
-        {}, _forgone_attributes)
-@validate_error_event_attributes(
-        {}, _forgone_attributes)
-@validate_attributes('intrinsic',
-        {}, _forgone_attributes['intrinsic'])
-@background_task(name='test_distributed_trace_attrs_omitted')
+@validate_transaction_event_attributes({}, _forgone_attributes)
+@validate_error_event_attributes({}, _forgone_attributes)
+@validate_attributes("intrinsic", {}, _forgone_attributes["intrinsic"])
+@background_task(name="test_distributed_trace_attrs_omitted")
 def test_distributed_trace_attrs_omitted():
     txn = current_transaction()
     try:
-        raise ValueError('cookies')
+        raise ValueError("cookies")
     except ValueError:
         txn.notice_error()
 
 
 # test our distributed_trace metrics by creating a transaction and then forcing
 # it to process a distributed trace payload
-@pytest.mark.parametrize('web_transaction', (True, False))
-@pytest.mark.parametrize('gen_error', (True, False))
-@pytest.mark.parametrize('has_parent', (True, False))
+@pytest.mark.parametrize("web_transaction", (True, False))
+@pytest.mark.parametrize("gen_error", (True, False))
+@pytest.mark.parametrize("has_parent", (True, False))
 def test_distributed_tracing_metrics(web_transaction, gen_error, has_parent):
     def _make_dt_tag(pi):
         return "%s/%s/%s/%s/all" % tuple(pi[x] for x in parent_order)
 
     # figure out which metrics we'll see based on the test params
     # note: we'll always see DurationByCaller if the distributed
     # tracing flag is turned on
-    metrics = ['DurationByCaller']
+    metrics = ["DurationByCaller"]
     if gen_error:
-        metrics.append('ErrorsByCaller')
+        metrics.append("ErrorsByCaller")
     if has_parent:
-        metrics.append('TransportDuration')
+        metrics.append("TransportDuration")
 
     tag = None
     dt_payload = copy.deepcopy(payload)
 
     # if has_parent is True, our metric name will be info about the parent,
     # otherwise it is Unknown/Unknown/Unknown/Unknown
     if has_parent:
         tag = _make_dt_tag(parent_info)
     else:
-        tag = _make_dt_tag(dict((x, 'Unknown') for x in parent_info.keys()))
-        del dt_payload['d']['tr']
+        # tag = _make_dt_tag(dict((x, "Unknown") for x in parent_order))
+        tag = _make_dt_tag(dict((x, "Unknown") for x in parent_info.keys()))
+        del dt_payload["d"]["tr"]
 
     # now run the test
-    transaction_name = "test_dt_metrics_%s" % '_'.join(metrics)
+    transaction_name = "test_dt_metrics_%s" % "_".join(metrics)
     _rollup_metrics = [
-        ("%s/%s%s" % (x, tag, bt), 1)
-        for x in metrics
-        for bt in ['', 'Web' if web_transaction else 'Other']
+        ("%s/%s%s" % (x, tag, bt), 1) for x in metrics for bt in ["", "Web" if web_transaction else "Other"]
     ]
 
     def _make_test_transaction():
         application = application_instance()
 
         if not web_transaction:
             return BackgroundTask(application, transaction_name)
 
-        environ = {'REQUEST_URI': '/trace_ends_after_txn'}
+        environ = {"REQUEST_URI": "/trace_ends_after_txn"}
         tn = WSGIWebTransaction(application, environ)
         tn.set_transaction_name(transaction_name)
         return tn
 
     @override_application_settings(_override_settings)
     @validate_transaction_metrics(
-        transaction_name,
-        background_task=not(web_transaction),
-        rollup_metrics=_rollup_metrics)
+        transaction_name, background_task=not (web_transaction), rollup_metrics=_rollup_metrics
+    )
     def _test():
         with _make_test_transaction() as transaction:
             transaction.accept_distributed_trace_payload(dt_payload)
 
             if gen_error:
                 try:
                     1 / 0
                 except ZeroDivisionError:
                     transaction.notice_error()
 
     _test()
 
 
-NEW_RELIC_ACCEPTED = \
-        [('Supportability/DistributedTrace/AcceptPayload/Success', 1),
-         ('Supportability/TraceContext/Accept/Success', None),
-         ('Supportability/TraceContext/TraceParent/Accept/Success', None),
-         ('Supportability/TraceContext/Accept/Success', None)]
-TRACE_CONTEXT_ACCEPTED = \
-        [('Supportability/TraceContext/Accept/Success', 1),
-         ('Supportability/TraceContext/TraceParent/Accept/Success', 1),
-         ('Supportability/TraceContext/Accept/Success', 1),
-         ('Supportability/DistributedTrace/AcceptPayload/Success', None)]
-NO_HEADERS_ACCEPTED = \
-        [('Supportability/DistributedTrace/AcceptPayload/Success', None),
-        ('Supportability/TraceContext/Accept/Success', None),
-        ('Supportability/TraceContext/TraceParent/Accept/Success', None),
-        ('Supportability/TraceContext/Accept/Success', None)]
-TRACEPARENT = '00-0af7651916cd43dd8448eb211c80319c-00f067aa0ba902b7-01'
-TRACESTATE = 'rojo=f06a0ba902b7,congo=t61rcWkgMzE'
-
-
-@pytest.mark.parametrize('traceparent,tracestate,newrelic,metrics',
-                         [(False, False, False, NO_HEADERS_ACCEPTED),
-                          (False, False, True, NEW_RELIC_ACCEPTED),
-                          (False, True, True, NEW_RELIC_ACCEPTED),
-                          (False, True, False, NO_HEADERS_ACCEPTED),
-                          (True, True, True, TRACE_CONTEXT_ACCEPTED),
-                          (True, False, False, TRACE_CONTEXT_ACCEPTED),
-                          (True, False, True, TRACE_CONTEXT_ACCEPTED),
-                          (True, True, False, TRACE_CONTEXT_ACCEPTED)]
-                         )
+NEW_RELIC_ACCEPTED = [
+    ("Supportability/DistributedTrace/AcceptPayload/Success", 1),
+    ("Supportability/TraceContext/Accept/Success", None),
+    ("Supportability/TraceContext/TraceParent/Accept/Success", None),
+    ("Supportability/TraceContext/Accept/Success", None),
+]
+TRACE_CONTEXT_ACCEPTED = [
+    ("Supportability/TraceContext/Accept/Success", 1),
+    ("Supportability/TraceContext/TraceParent/Accept/Success", 1),
+    ("Supportability/TraceContext/Accept/Success", 1),
+    ("Supportability/DistributedTrace/AcceptPayload/Success", None),
+]
+NO_HEADERS_ACCEPTED = [
+    ("Supportability/DistributedTrace/AcceptPayload/Success", None),
+    ("Supportability/TraceContext/Accept/Success", None),
+    ("Supportability/TraceContext/TraceParent/Accept/Success", None),
+    ("Supportability/TraceContext/Accept/Success", None),
+]
+TRACEPARENT = "00-0af7651916cd43dd8448eb211c80319c-00f067aa0ba902b7-01"
+TRACESTATE = "rojo=f06a0ba902b7,congo=t61rcWkgMzE"
+
+
+@pytest.mark.parametrize(
+    "traceparent,tracestate,newrelic,metrics",
+    [
+        (False, False, False, NO_HEADERS_ACCEPTED),
+        (False, False, True, NEW_RELIC_ACCEPTED),
+        (False, True, True, NEW_RELIC_ACCEPTED),
+        (False, True, False, NO_HEADERS_ACCEPTED),
+        (True, True, True, TRACE_CONTEXT_ACCEPTED),
+        (True, False, False, TRACE_CONTEXT_ACCEPTED),
+        (True, False, True, TRACE_CONTEXT_ACCEPTED),
+        (True, True, False, TRACE_CONTEXT_ACCEPTED),
+    ],
+)
 @override_application_settings(_override_settings)
-def test_distributed_tracing_backwards_compatibility(traceparent,
-                                                     tracestate,
-                                                     newrelic,
-                                                     metrics):
+def test_distributed_tracing_backwards_compatibility(traceparent, tracestate, newrelic, metrics):
 
     headers = []
     if traceparent:
-        headers.append(('traceparent', TRACEPARENT))
+        headers.append(("traceparent", TRACEPARENT))
     if tracestate:
-        headers.append(('tracestate', TRACESTATE))
+        headers.append(("tracestate", TRACESTATE))
     if newrelic:
-        headers.append(('newrelic', json.dumps(payload)))
+        headers.append(("newrelic", json.dumps(payload)))
 
     @validate_transaction_metrics(
-        "test_distributed_tracing_backwards_compatibility",
-        background_task=True,
-        rollup_metrics=metrics)
-    @background_task(name='test_distributed_tracing_backwards_compatibility')
+        "test_distributed_tracing_backwards_compatibility", background_task=True, rollup_metrics=metrics
+    )
+    @background_task(name="test_distributed_tracing_backwards_compatibility")
     def _test():
         transaction = current_transaction()
         transaction.accept_distributed_trace_headers(headers)
 
     _test()
 
 
-@background_task(name='test_current_trace_id_api_inside_transaction')
+@background_task(name="test_current_trace_id_api_inside_transaction")
 def test_current_trace_id_api_inside_transaction():
     trace_id = current_trace_id()
     assert len(trace_id) == 32
     assert trace_id == current_transaction().trace_id
 
 
 def test_current_trace_id_api_outside_transaction():
     trace_id = current_trace_id()
     assert trace_id is None
 
 
-@background_task(name='test_current_span_id_api_inside_transaction')
+@background_task(name="test_current_span_id_api_inside_transaction")
 def test_current_span_id_inside_transaction():
     span_id = current_span_id()
     assert span_id == current_trace().guid
 
 
 def test_current_span_id_outside_transaction():
     span_id = current_span_id()
```

### Comparing `newrelic-8.8.0/tests/agent_features/test_error_events.py` & `newrelic-8.8.1/tests/agent_features/test_error_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_error_group_callback.py` & `newrelic-8.8.1/tests/agent_features/test_error_group_callback.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,43 +8,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
 import threading
 import traceback
-import sys
 
 import pytest
-
 from testing_support.fixtures import (
     override_application_settings,
     reset_core_stats_engine,
+)
+from testing_support.validators.validate_error_event_attributes import (
     validate_error_event_attributes,
+)
+from testing_support.validators.validate_error_event_attributes_outside_transaction import (
     validate_error_event_attributes_outside_transaction,
-    validate_error_trace_attributes_outside_transaction,
 )
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
+from testing_support.validators.validate_error_trace_attributes_outside_transaction import (
+    validate_error_trace_attributes_outside_transaction,
+)
 
 from newrelic.api.application import application_instance as application
 from newrelic.api.background_task import background_task
+from newrelic.api.settings import set_error_group_callback
 from newrelic.api.time_trace import notice_error
 from newrelic.api.transaction import current_transaction
-from newrelic.api.settings import set_error_group_callback
 from newrelic.api.web_transaction import web_transaction
 from newrelic.common.object_names import callable_name
 
-
 _callback_called = threading.Event()
 _truncated_value = "A" * 300
 
+
 def error_group_callback(exc, data):
     _callback_called.set()
 
     if isinstance(exc, ValueError):
         return "value"
     elif isinstance(exc, ZeroDivisionError):
         return _truncated_value
@@ -60,55 +65,54 @@
     settings = application().settings
     set_error_group_callback(lambda x, y: None)
     assert settings.error_collector.error_group_callback is not None, "Failed to set callback."
     set_error_group_callback(None)
     assert settings.error_collector.error_group_callback is None, "Failed to clear callback."
 
 
-@pytest.mark.parametrize("callback,accepted", [
-    (error_group_callback, True),
-    (lambda x, y: None, True),
-    (None, False),
-    ("string", False)
-])
+@pytest.mark.parametrize(
+    "callback,accepted", [(error_group_callback, True), (lambda x, y: None, True), (None, False), ("string", False)]
+)
 def test_set_error_group_callback(callback, accepted):
     try:
         set_error_group_callback(callback)
         settings = application().settings
         if accepted:
             assert settings.error_collector.error_group_callback is not None, "Failed to set callback."
         else:
             assert settings.error_collector.error_group_callback is None, "Accepted bad callback."
     finally:
         set_error_group_callback(None)
 
 
-@pytest.mark.parametrize("exc_class,group_name,high_security", [
-    (ValueError, "value", False),
-    (ValueError, "value", True),
-    (TypeError, None, False),
-    (RuntimeError, None, False),
-    (IndexError, None, False),
-    (LookupError, None, False),
-    (ZeroDivisionError, _truncated_value[:255], False),
-], ids=("standard", "high-security", "empty-string", "None-value", "list-type", "int-type", "truncated-value"))
+@pytest.mark.parametrize(
+    "exc_class,group_name,high_security",
+    [
+        (ValueError, "value", False),
+        (ValueError, "value", True),
+        (TypeError, None, False),
+        (RuntimeError, None, False),
+        (IndexError, None, False),
+        (LookupError, None, False),
+        (ZeroDivisionError, _truncated_value[:255], False),
+    ],
+    ids=("standard", "high-security", "empty-string", "None-value", "list-type", "int-type", "truncated-value"),
+)
 @reset_core_stats_engine()
 def test_error_group_name_callback(exc_class, group_name, high_security):
     _callback_called.clear()
 
     if group_name is not None:
         exact = {"user": {}, "intrinsic": {}, "agent": {"error.group.name": group_name}}
         forgone = None
     else:
         exact = None
         forgone = {"user": [], "intrinsic": [], "agent": ["error.group.name"]}
 
-    @validate_error_trace_attributes(
-        callable_name(exc_class), forgone_params=forgone, exact_attrs=exact
-    )
+    @validate_error_trace_attributes(callable_name(exc_class), forgone_params=forgone, exact_attrs=exact)
     @validate_error_event_attributes(forgone_params=forgone, exact_attrs=exact)
     @override_application_settings({"high_security": high_security})
     @background_task()
     def _test():
 
         try:
             raise exc_class()
@@ -120,23 +124,27 @@
     try:
         set_error_group_callback(error_group_callback)
         _test()
     finally:
         set_error_group_callback(None)
 
 
-@pytest.mark.parametrize("exc_class,group_name,high_security", [
-    (ValueError, "value", False),
-    (ValueError, "value", True),
-    (TypeError, None, False),
-    (RuntimeError, None, False),
-    (IndexError, None, False),
-    (LookupError, None, False),
-    (ZeroDivisionError, _truncated_value[:255], False),
-], ids=("standard", "high-security", "empty-string", "None-value", "list-type", "int-type", "truncated-value"))
+@pytest.mark.parametrize(
+    "exc_class,group_name,high_security",
+    [
+        (ValueError, "value", False),
+        (ValueError, "value", True),
+        (TypeError, None, False),
+        (RuntimeError, None, False),
+        (IndexError, None, False),
+        (LookupError, None, False),
+        (ZeroDivisionError, _truncated_value[:255], False),
+    ],
+    ids=("standard", "high-security", "empty-string", "None-value", "list-type", "int-type", "truncated-value"),
+)
 @reset_core_stats_engine()
 def test_error_group_name_callback_outside_transaction(exc_class, group_name, high_security):
     _callback_called.clear()
 
     if group_name is not None:
         exact = {"user": {}, "intrinsic": {}, "agent": {"error.group.name": group_name}}
         forgone = None
@@ -151,67 +159,79 @@
     @override_application_settings({"high_security": high_security})
     def _test():
         try:
             raise exc_class()
         except Exception:
             app = application()
             notice_error(application=app)
-        
+
         assert _callback_called.is_set()
 
     try:
         set_error_group_callback(error_group_callback)
         _test()
     finally:
         set_error_group_callback(None)
 
 
-@pytest.mark.parametrize("transaction_decorator", [
-    background_task(name="TestBackgroundTask"),
-    web_transaction(name="TestWebTransaction", host="localhost", port=1234, request_method="GET", request_path="/", headers=[],),
-    None,
-], ids=("background_task", "web_transation", "outside_transaction"))
+@pytest.mark.parametrize(
+    "transaction_decorator",
+    [
+        background_task(name="TestBackgroundTask"),
+        web_transaction(
+            name="TestWebTransaction",
+            host="localhost",
+            port=1234,
+            request_method="GET",
+            request_path="/",
+            headers=[],
+        ),
+        None,
+    ],
+    ids=("background_task", "web_transation", "outside_transaction"),
+)
 @reset_core_stats_engine()
 def test_error_group_name_callback_attributes(transaction_decorator):
     callback_errors = []
     _data = []
 
     def callback(error, data):
         def _callback():
             import types
+
             _data.append(data)
             txn = current_transaction()
 
             # Standard attributes
             assert isinstance(error, Exception)
             assert isinstance(data["traceback"], types.TracebackType)
             assert data["error.class"] is type(error)
             assert data["error.message"] == "text"
             assert data["error.expected"] is False
 
             # All attributes should always be included, but set to None when not relevant.
             if txn is None:  # Outside transaction
                 assert data["transactionName"] is None
-                assert data["custom_params"] == {'notice_error_attribute': 1}
+                assert data["custom_params"] == {"notice_error_attribute": 1}
                 assert data["response.status"] is None
                 assert data["request.method"] is None
                 assert data["request.uri"] is None
             elif txn.background_task:  # Background task
                 assert data["transactionName"] == "TestBackgroundTask"
-                assert data["custom_params"] == {'notice_error_attribute': 1, 'txn_attribute': 2}
+                assert data["custom_params"] == {"notice_error_attribute": 1, "txn_attribute": 2}
                 assert data["response.status"] is None
                 assert data["request.method"] is None
                 assert data["request.uri"] is None
             else:  # Web transaction
                 assert data["transactionName"] == "TestWebTransaction"
-                assert data["custom_params"] == {'notice_error_attribute': 1, 'txn_attribute': 2}
+                assert data["custom_params"] == {"notice_error_attribute": 1, "txn_attribute": 2}
                 assert data["response.status"] == 200
                 assert data["request.method"] == "GET"
                 assert data["request.uri"] == "/"
-        
+
         try:
             _callback()
         except Exception:
             callback_errors.append(sys.exc_info())
             raise
 
     def _test():
@@ -221,16 +241,19 @@
                 txn.add_custom_attribute("txn_attribute", 2)
                 if not txn.background_task:
                     txn.process_response(200, [])
             raise Exception("text")
         except Exception:
             app = application() if transaction_decorator is None else None  # Only set outside transaction
             notice_error(application=app, attributes={"notice_error_attribute": 1})
-        
-        assert not callback_errors, "Callback inputs failed to validate.\nerror: %s\ndata: %s" % (traceback.format_exception(*callback_errors[0]), str(_data[0]))
+
+        assert not callback_errors, "Callback inputs failed to validate.\nerror: %s\ndata: %s" % (
+            traceback.format_exception(*callback_errors[0]),
+            str(_data[0]),
+        )
 
     if transaction_decorator is not None:
         _test = transaction_decorator(_test)  # Manually decorate test function
 
     try:
         set_error_group_callback(callback)
         _test()
```

### Comparing `newrelic-8.8.0/tests/agent_features/test_event_loop_wait_time.py` & `newrelic-8.8.1/tests/agent_features/test_event_loop_wait_time.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_exception_messages.py` & `newrelic-8.8.1/tests/agent_features/test_exception_messages.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_function_trace.py` & `newrelic-8.8.1/tests/agent_features/test_function_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_high_security_mode.py` & `newrelic-8.8.1/tests/agent_features/test_high_security_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,25 +21,27 @@
     override_application_settings,
     override_generic_settings,
     reset_core_stats_engine,
     validate_attributes_complete,
     validate_custom_event_count,
     validate_custom_event_in_application_stats_engine,
     validate_request_params_omitted,
-    validate_tt_segment_params,
 )
 from testing_support.validators.validate_custom_parameters import (
     validate_custom_parameters,
 )
 from testing_support.validators.validate_non_transaction_error_event import (
     validate_non_transaction_error_event,
 )
 from testing_support.validators.validate_transaction_errors import (
     validate_transaction_errors,
 )
+from testing_support.validators.validate_tt_segment_params import (
+    validate_tt_segment_params,
+)
 
 from newrelic.api.application import application_instance as application
 from newrelic.api.background_task import background_task
 from newrelic.api.function_trace import FunctionTrace
 from newrelic.api.message_trace import MessageTrace
 from newrelic.api.settings import STRIP_EXCEPTION_MESSAGE
 from newrelic.api.time_trace import notice_error
```

### Comparing `newrelic-8.8.0/tests/agent_features/test_ignore_expected_errors.py` & `newrelic-8.8.1/tests/agent_features/test_ignore_expected_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 from testing_support.fixtures import (
     override_application_settings,
     reset_core_stats_engine,
-    validate_error_event_attributes_outside_transaction,
     validate_error_event_sample_data,
+)
+from testing_support.validators.validate_error_event_attributes_outside_transaction import (
+    validate_error_event_attributes_outside_transaction,
+)
+from testing_support.validators.validate_error_trace_attributes_outside_transaction import (
     validate_error_trace_attributes_outside_transaction,
 )
 from testing_support.validators.validate_time_metrics_outside_transaction import (
     validate_time_metrics_outside_transaction,
 )
 from testing_support.validators.validate_transaction_error_trace_attributes import (
     validate_transaction_error_trace_attributes,
```

### Comparing `newrelic-8.8.0/tests/agent_features/test_lambda_handler.py` & `newrelic-8.8.1/tests/agent_features/test_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_log_events.py` & `newrelic-8.8.1/tests/agent_features/test_log_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_logs_in_context.py` & `newrelic-8.8.1/tests/agent_features/test_logs_in_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_notice_error.py` & `newrelic-8.8.1/tests/agent_features/test_notice_error.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_priority_sampling.py` & `newrelic-8.8.1/tests/agent_features/test_priority_sampling.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_serverless_mode.py` & `newrelic-8.8.1/tests/agent_features/test_serverless_mode.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_span_events.py` & `newrelic-8.8.1/tests/agent_features/test_span_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 import sys
 
 import pytest
 from testing_support.fixtures import (
     dt_enabled,
     function_not_called,
     override_application_settings,
-    validate_tt_segment_params,
 )
 from testing_support.validators.validate_span_events import validate_span_events
 from testing_support.validators.validate_transaction_event_attributes import (
     validate_transaction_event_attributes,
 )
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
+from testing_support.validators.validate_tt_segment_params import (
+    validate_tt_segment_params,
+)
 
 from newrelic.api.background_task import background_task
 from newrelic.api.database_trace import DatabaseTrace
 from newrelic.api.datastore_trace import DatastoreTrace
 from newrelic.api.external_trace import ExternalTrace
 from newrelic.api.function_trace import FunctionTrace, function_trace
 from newrelic.api.memcache_trace import MemcacheTrace
@@ -721,15 +723,15 @@
 def test_span_event_notice_error_overrides_observed(trace_type, args):
     try:
         with trace_type(*args):
             try:
                 raise ERROR
             except Exception:
                 notice_error()
-                raise ValueError  # pylint: disable
+                raise ValueError  # pylint: disable (Py2/Py3 compatibility)
     except ValueError:
         pass
 
 
 @pytest.mark.parametrize(
     "trace_type,args",
     (
```

### Comparing `newrelic-8.8.0/tests/agent_features/test_stack_trace.py` & `newrelic-8.8.1/tests/agent_features/test_stack_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_supportability_metrics.py` & `newrelic-8.8.1/tests/agent_features/test_supportability_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_synthetics.py` & `newrelic-8.8.1/tests/agent_features/test_synthetics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_time_trace.py` & `newrelic-8.8.1/tests/agent_features/test_time_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py` & `newrelic-8.8.1/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_transaction_name.py` & `newrelic-8.8.1/tests/agent_features/test_transaction_name.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_transaction_trace_segments.py` & `newrelic-8.8.1/tests/agent_features/test_transaction_trace_segments.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-from testing_support.fixtures import (
-    override_application_settings,
+from testing_support.fixtures import override_application_settings
+from testing_support.validators.validate_tt_segment_params import (
     validate_tt_segment_params,
 )
 
 from newrelic.api.background_task import background_task
 from newrelic.api.database_trace import DatabaseTrace
 from newrelic.api.datastore_trace import DatastoreTrace
 from newrelic.api.external_trace import ExternalTrace, external_trace
```

### Comparing `newrelic-8.8.0/tests/agent_features/test_w3c_trace_context.py` & `newrelic-8.8.1/tests/agent_features/test_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_web_transaction.py` & `newrelic-8.8.1/tests/agent_features/test_web_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_features/test_wsgi_attributes.py` & `newrelic-8.8.1/tests/agent_features/test_wsgi_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import webtest
-from testing_support.fixtures import (
-    dt_enabled,
-    override_application_settings,
+from testing_support.fixtures import dt_enabled, override_application_settings
+from testing_support.sample_applications import fully_featured_app
+from testing_support.validators.validate_error_event_attributes import (
     validate_error_event_attributes,
 )
-from testing_support.sample_applications import fully_featured_app
 from testing_support.validators.validate_transaction_error_trace_attributes import (
     validate_transaction_error_trace_attributes,
 )
 from testing_support.validators.validate_transaction_event_attributes import (
     validate_transaction_event_attributes,
 )
```

### Comparing `newrelic-8.8.0/tests/agent_streaming/_test_handler.py` & `newrelic-8.8.1/tests/agent_streaming/_test_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_streaming/conftest.py` & `newrelic-8.8.1/tests/agent_streaming/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_streaming/test_infinite_tracing.py` & `newrelic-8.8.1/tests/agent_streaming/test_infinite_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_streaming/test_span_events.py` & `newrelic-8.8.1/tests/agent_streaming/test_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_streaming/test_stream_buffer.py` & `newrelic-8.8.1/tests/agent_streaming/test_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_streaming/test_streaming_rpc.py` & `newrelic-8.8.1/tests/agent_streaming/test_streaming_rpc.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/_test_import_hook.py` & `newrelic-8.8.1/tests/agent_unittests/_test_import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/cert.pem` & `newrelic-8.8.1/tests/agent_unittests/cert.pem`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/conftest.py` & `newrelic-8.8.1/tests/agent_unittests/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_agent.py` & `newrelic-8.8.1/tests/agent_unittests/test_agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_agent_connect.py` & `newrelic-8.8.1/tests/agent_unittests/test_agent_connect.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_agent_protocol.py` & `newrelic-8.8.1/tests/agent_unittests/test_agent_protocol.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_check_environment.py` & `newrelic-8.8.1/tests/agent_unittests/test_check_environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_connect_response_fields.py` & `newrelic-8.8.1/tests/agent_unittests/test_connect_response_fields.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_distributed_tracing_settings.py` & `newrelic-8.8.1/tests/agent_unittests/test_distributed_tracing_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_environment.py` & `newrelic-8.8.1/tests/agent_unittests/test_environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_full_uri_payloads.py` & `newrelic-8.8.1/tests/agent_unittests/test_full_uri_payloads.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_harvest_loop.py` & `newrelic-8.8.1/tests/agent_unittests/test_harvest_loop.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_http_client.py` & `newrelic-8.8.1/tests/agent_unittests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_import_hook.py` & `newrelic-8.8.1/tests/agent_unittests/test_import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_infinite_trace_settings.py` & `newrelic-8.8.1/tests/agent_unittests/test_infinite_trace_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_package_version_utils.py` & `newrelic-8.8.1/tests/agent_unittests/test_package_version_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,28 @@
     # pytest instead for our purposes
     setattr(pytest, attr, value)
     version = get_package_version("pytest")
     assert version == expected_value
     delattr(pytest, attr)
 
 
+def test_skips_version_callables():
+    # There is no file/module here, so we monkeypatch
+    # pytest instead for our purposes
+    setattr(pytest, "version", lambda x: "1.2.3.4")
+    setattr(pytest, "version_tuple", [3, 1, "0b2"])
+
+    version = get_package_version("pytest")
+
+    assert version == "3.1.0b2"
+
+    delattr(pytest, "version")
+    delattr(pytest, "version_tuple")
+
+
 @pytest.mark.parametrize(
     "attr,value,expected_value",
     (
         ("version", "1.2.3.4", (1, 2, 3, 4)),
         ("__version__", "1.3.5rc2", (1, 3, "5rc2")),
         ("__version_tuple__", (3, 5, 8), (3, 5, 8)),
         ("version_tuple", [3, 1, "0b2"], (3, 1, "0b2")),
```

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_region_aware_settings.py` & `newrelic-8.8.1/tests/agent_unittests/test_region_aware_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_sampler_metrics.py` & `newrelic-8.8.1/tests/agent_unittests/test_sampler_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_serverless_mode_settings.py` & `newrelic-8.8.1/tests/agent_unittests/test_serverless_mode_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_trace_cache.py` & `newrelic-8.8.1/tests/agent_unittests/test_trace_cache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/agent_unittests/test_utilization_settings.py` & `newrelic-8.8.1/tests/agent_unittests/test_utilization_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/application_celery/conftest.py` & `newrelic-8.8.1/tests/application_celery/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/application_celery/tasks.py` & `newrelic-8.8.1/tests/application_celery/tasks.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/application_celery/test_celery.py` & `newrelic-8.8.1/tests/application_celery/test_celery.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/application_celery/test_celery_max_tasks_per_child.py` & `newrelic-8.8.1/tests/application_celery/test_celery_max_tasks_per_child.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/application_gearman/conftest.py` & `newrelic-8.8.1/tests/application_gearman/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/application_gearman/test_gearman.py` & `newrelic-8.8.1/tests/application_gearman/test_gearman.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 
 import os
 import threading
 
 import gearman
 
 from newrelic.api.background_task import background_task
+from testing_support.db_settings import gearman_settings
 
 worker_thread = None
 worker_event = threading.Event()
 
 gm_client = None
 
-GEARMAND_HOST = os.environ.get("GEARMAND_PORT_4730_TCP_ADDR", "localhost")
-GEARMAND_PORT = os.environ.get("GEARMAND_PORT_4730_TCP_PORT", "4730")
+GEARMAND_SETTINGS = gearman_settings()[0]
+GEARMAND_HOST = GEARMAND_SETTINGS["host"]
+GEARMAND_PORT = GEARMAND_SETTINGS["port"]
 
 GEARMAND_ADDR = "%s:%s" % (GEARMAND_HOST, GEARMAND_PORT)
 
 
 class GearmanWorker(gearman.GearmanWorker):
     def after_poll(self, any_activity):
         try:
```

### Comparing `newrelic-8.8.0/tests/component_djangorestframework/conftest.py` & `newrelic-8.8.1/tests/component_djangorestframework/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_djangorestframework/settings.py` & `newrelic-8.8.1/tests/component_djangorestframework/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_djangorestframework/test_application.py` & `newrelic-8.8.1/tests/component_djangorestframework/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_djangorestframework/urls.py` & `newrelic-8.8.1/tests/component_djangorestframework/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_djangorestframework/views.py` & `newrelic-8.8.1/tests/component_djangorestframework/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_djangorestframework/wsgi.py` & `newrelic-8.8.1/tests/component_djangorestframework/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_flask_rest/_test_application.py` & `newrelic-8.8.1/tests/component_flask_rest/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_flask_rest/conftest.py` & `newrelic-8.8.1/tests/component_flask_rest/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_flask_rest/test_application.py` & `newrelic-8.8.1/tests/component_flask_rest/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_graphqlserver/_test_graphql.py` & `newrelic-8.8.1/tests/component_graphqlserver/_test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_graphqlserver/conftest.py` & `newrelic-8.8.1/tests/component_graphqlserver/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_graphqlserver/test_graphql.py` & `newrelic-8.8.1/tests/component_graphqlserver/test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_tastypie/api.py` & `newrelic-8.8.1/tests/component_tastypie/api.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_tastypie/conftest.py` & `newrelic-8.8.1/tests/component_tastypie/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_tastypie/settings.py` & `newrelic-8.8.1/tests/component_tastypie/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_tastypie/test_application.py` & `newrelic-8.8.1/tests/component_tastypie/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_tastypie/urls.py` & `newrelic-8.8.1/tests/component_tastypie/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_tastypie/views.py` & `newrelic-8.8.1/tests/component_tastypie/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/component_tastypie/wsgi.py` & `newrelic-8.8.1/tests/component_tastypie/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/coroutines_asyncio/conftest.py` & `newrelic-8.8.1/tests/coroutines_asyncio/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/coroutines_asyncio/test_context_propagation.py` & `newrelic-8.8.1/tests/coroutines_asyncio/test_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/conftest.py` & `newrelic-8.8.1/tests/cross_agent/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/README.md` & `newrelic-8.8.1/tests/cross_agent/fixtures/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/attribute_configuration.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/attribute_configuration.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/cat_map.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/cat_map.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/collector_hostname.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/collector_hostname.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/datastores/README.md` & `newrelic-8.8.1/tests/cross_agent/fixtures/datastores/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/datastores/datastore_instances.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/datastores/datastore_instances.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/distributed_tracing/README.md` & `newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/trace_context.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/cases.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/cases.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/labels.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/labels.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/codecommit.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/s3_put.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/ses.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/ses.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/sns.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/sns.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/sqs.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/lambda_event_source.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md` & `newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt` & `newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rules.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/rules.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_client_config.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_client_config.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_cookie.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_cookie.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_footer_insertion_location/close-body-in-comment.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/close-body-in-comment.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_footer_insertion_location/dynamic-iframe.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/dynamic-iframe.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html` & `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/README.md` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/sql_parsing.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/sql_parsing.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/transaction_segment_terms.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/transaction_segment_terms.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/url_clean.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/url_clean.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/url_domain_extraction.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/url_domain_extraction.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/utilization/README.md` & `newrelic-8.8.1/tests/cross_agent/fixtures/utilization/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/utilization/boot_id.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/utilization/boot_id.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/utilization/utilization_json.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/utilization/utilization_json.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md` & `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json` & `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_agent_attributes.py` & `newrelic-8.8.1/tests/cross_agent/test_agent_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_aws_utilization_data.py` & `newrelic-8.8.1/tests/cross_agent/test_aws_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_azure_utilization_data.py` & `newrelic-8.8.1/tests/cross_agent/test_azure_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_boot_id_utilization_data.py` & `newrelic-8.8.1/tests/cross_agent/test_boot_id_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_cat_map.py` & `newrelic-8.8.1/tests/cross_agent/test_cat_map.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,191 +14,217 @@
 
 """
 This is an implementation of the cross agent tests for cat map using a wsgi
 application. Another implementation of these tests using a tornado application
 can be found in test/framework_tornado_r3/test_cat_map.py
 """
 
-import webtest
-import pytest
 import json
 import os
 
+import pytest
+import webtest
+
 try:
     from urllib2 import urlopen  # Py2.X
 except ImportError:
-    from urllib.request import urlopen   # Py3.X
+    from urllib.request import urlopen  # Py3.X
 
-from newrelic.packages import six
+from testing_support.fixtures import (
+    make_cross_agent_headers,
+    override_application_name,
+    override_application_settings,
+    validate_analytics_catmap_data,
+)
+from testing_support.mock_external_http_server import (
+    MockExternalHTTPHResponseHeadersServer,
+)
+from testing_support.validators.validate_tt_parameters import validate_tt_parameters
 
 from newrelic.api.external_trace import ExternalTrace
-from newrelic.api.transaction import (get_browser_timing_header,
-        set_transaction_name, get_browser_timing_footer, set_background_task,
-        current_transaction)
+from newrelic.api.transaction import (
+    current_transaction,
+    get_browser_timing_footer,
+    get_browser_timing_header,
+    set_background_task,
+    set_transaction_name,
+)
 from newrelic.api.wsgi_application import wsgi_application
-from newrelic.common.encoding_utils import obfuscate, json_encode
-
-from testing_support.fixtures import (override_application_settings,
-        override_application_name, validate_tt_parameters,
-        make_cross_agent_headers, validate_analytics_catmap_data)
-from testing_support.mock_external_http_server import (
-        MockExternalHTTPHResponseHeadersServer)
+from newrelic.common.encoding_utils import json_encode, obfuscate
+from newrelic.packages import six
 
-ENCODING_KEY = '1234567890123456789012345678901234567890'
+ENCODING_KEY = "1234567890123456789012345678901234567890"
 CURRENT_DIR = os.path.dirname(os.path.realpath(__file__))
-JSON_DIR = os.path.normpath(os.path.join(CURRENT_DIR, 'fixtures'))
+JSON_DIR = os.path.normpath(os.path.join(CURRENT_DIR, "fixtures"))
 OUTBOUD_REQUESTS = {}
 
-_parameters_list = ["name", "appName", "transactionName", "transactionGuid",
-        "inboundPayload", "outboundRequests", "expectedIntrinsicFields",
-        "nonExpectedIntrinsicFields"]
+_parameters_list = [
+    "name",
+    "appName",
+    "transactionName",
+    "transactionGuid",
+    "inboundPayload",
+    "outboundRequests",
+    "expectedIntrinsicFields",
+    "nonExpectedIntrinsicFields",
+]
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def server():
     with MockExternalHTTPHResponseHeadersServer() as _server:
         yield _server
 
 
 def load_tests():
     result = []
-    path = os.path.join(JSON_DIR, 'cat_map.json')
-    with open(path, 'r') as fh:
+    path = os.path.join(JSON_DIR, "cat_map.json")
+    with open(path, "r") as fh:
         tests = json.load(fh)
 
     for test in tests:
         values = tuple([test.get(param, None) for param in _parameters_list])
         result.append(values)
 
     return result
 
 
 _parameters = ",".join(_parameters_list)
 
 
 @wsgi_application()
 def target_wsgi_application(environ, start_response):
-    status = '200 OK'
+    status = "200 OK"
 
-    txn_name = environ.get('txn')
+    txn_name = environ.get("txn")
     if six.PY2:
-        txn_name = txn_name.decode('UTF-8')
-    txn_name = txn_name.split('/', 3)
+        txn_name = txn_name.decode("UTF-8")
+    txn_name = txn_name.split("/", 3)
 
-    guid = environ.get('guid')
-    old_cat = environ.get('old_cat') == 'True'
+    guid = environ.get("guid")
+    old_cat = environ.get("old_cat") == "True"
     txn = current_transaction()
 
     txn.guid = guid
     for req in OUTBOUD_REQUESTS:
         # Change the transaction name before making an outbound call.
-        outgoing_name = req['outboundTxnName'].split('/', 3)
-        if outgoing_name[0] != 'WebTransaction':
+        outgoing_name = req["outboundTxnName"].split("/", 3)
+        if outgoing_name[0] != "WebTransaction":
             set_background_task(True)
 
         set_transaction_name(outgoing_name[2], group=outgoing_name[1])
 
-        expected_outbound_header = obfuscate(
-                json_encode(req['expectedOutboundPayload']), ENCODING_KEY)
-        generated_outbound_header = dict(
-                ExternalTrace.generate_request_headers(txn))
+        expected_outbound_header = obfuscate(json_encode(req["expectedOutboundPayload"]), ENCODING_KEY)
+        generated_outbound_header = dict(ExternalTrace.generate_request_headers(txn))
 
         # A 500 error is returned because 'assert' statements in the wsgi app
         # are ignored.
 
         if old_cat:
-            if (expected_outbound_header !=
-                    generated_outbound_header['X-NewRelic-Transaction']):
-                status = '500 Outbound Headers Check Failed.'
+            if expected_outbound_header != generated_outbound_header["X-NewRelic-Transaction"]:
+                status = "500 Outbound Headers Check Failed."
         else:
-            if 'X-NewRelic-Transaction' in generated_outbound_header:
-                status = '500 Outbound Headers Check Failed.'
-        r = urlopen(environ['server_url'])
+            if "X-NewRelic-Transaction" in generated_outbound_header:
+                status = "500 Outbound Headers Check Failed."
+        r = urlopen(environ["server_url"])  # nosec B310
         r.read(10)
 
     # Set the final transaction name.
 
-    if txn_name[0] != 'WebTransaction':
+    if txn_name[0] != "WebTransaction":
         set_background_task(True)
     set_transaction_name(txn_name[2], group=txn_name[1])
 
-    text = '<html><head>%s</head><body><p>RESPONSE</p>%s</body></html>'
+    text = "<html><head>%s</head><body><p>RESPONSE</p>%s</body></html>"
 
-    output = (text % (get_browser_timing_header(),
-            get_browser_timing_footer())).encode('UTF-8')
+    output = (text % (get_browser_timing_header(), get_browser_timing_footer())).encode("UTF-8")
 
-    response_headers = [('Content-type', 'text/html; charset=utf-8'),
-                        ('Content-Length', str(len(output)))]
+    response_headers = [("Content-type", "text/html; charset=utf-8"), ("Content-Length", str(len(output)))]
     start_response(status, response_headers)
 
     return [output]
 
 
 target_application = webtest.TestApp(target_wsgi_application)
 
 
 @pytest.mark.parametrize(_parameters, load_tests())
-@pytest.mark.parametrize('old_cat', (True, False))
-def test_cat_map(name, appName, transactionName, transactionGuid,
-        inboundPayload, outboundRequests, expectedIntrinsicFields,
-        nonExpectedIntrinsicFields, old_cat, server):
+@pytest.mark.parametrize("old_cat", (True, False))
+def test_cat_map(
+    name,
+    appName,
+    transactionName,
+    transactionGuid,
+    inboundPayload,
+    outboundRequests,
+    expectedIntrinsicFields,
+    nonExpectedIntrinsicFields,
+    old_cat,
+    server,
+):
     global OUTBOUD_REQUESTS
     OUTBOUD_REQUESTS = outboundRequests or {}
 
     _custom_settings = {
-            'cross_process_id': '1#1',
-            'encoding_key': ENCODING_KEY,
-            'trusted_account_ids': [1],
-            'cross_application_tracer.enabled': True,
-            'distributed_tracing.enabled': not old_cat,
-            'transaction_tracer.transaction_threshold': 0.0,
+        "cross_process_id": "1#1",
+        "encoding_key": ENCODING_KEY,
+        "trusted_account_ids": [1],
+        "cross_application_tracer.enabled": True,
+        "distributed_tracing.enabled": not old_cat,
+        "transaction_tracer.transaction_threshold": 0.0,
     }
 
     if expectedIntrinsicFields and old_cat:
         _external_node_params = {
-                'path_hash': expectedIntrinsicFields['nr.pathHash'],
-                'trip_id': expectedIntrinsicFields['nr.tripId'],
+            "path_hash": expectedIntrinsicFields["nr.pathHash"],
+            "trip_id": expectedIntrinsicFields["nr.tripId"],
         }
     else:
         _external_node_params = []
 
     if not old_cat:
         # since no better cat headers will be generated, no intrinsics should
         # be added
         expectedIntrinsicFields = {}
 
     @validate_tt_parameters(required_params=_external_node_params)
-    @validate_analytics_catmap_data(transactionName,
-            expected_attributes=expectedIntrinsicFields,
-            non_expected_attributes=nonExpectedIntrinsicFields)
+    @validate_analytics_catmap_data(
+        transactionName, expected_attributes=expectedIntrinsicFields, non_expected_attributes=nonExpectedIntrinsicFields
+    )
     @override_application_settings(_custom_settings)
     @override_application_name(appName)
     def run_cat_test():
 
         if six.PY2:
-            txn_name = transactionName.encode('UTF-8')
-            guid = transactionGuid.encode('UTF-8')
+            txn_name = transactionName.encode("UTF-8")
+            guid = transactionGuid.encode("UTF-8")
         else:
             txn_name = transactionName
             guid = transactionGuid
 
         # Only generate old cat style headers. This will test to make sure we
         # are properly ignoring these headers when the agent is using better
         # cat.
 
-        headers = make_cross_agent_headers(inboundPayload, ENCODING_KEY, '1#1')
-        response = target_application.get('/', headers=headers,
-                extra_environ={'txn': txn_name, 'guid': guid,
-                    'old_cat': str(old_cat),
-                    'server_url': 'http://localhost:%d' % server.port})
+        headers = make_cross_agent_headers(inboundPayload, ENCODING_KEY, "1#1")
+        response = target_application.get(
+            "/",
+            headers=headers,
+            extra_environ={
+                "txn": txn_name,
+                "guid": guid,
+                "old_cat": str(old_cat),
+                "server_url": "http://localhost:%d" % server.port,
+            },
+        )
 
         # Validation of analytic data happens in the decorator.
 
-        assert response.status == '200 OK'
+        assert response.status == "200 OK"
 
         content = response.html.html.body.p.string
 
         # Validate actual body content as sanity check.
 
-        assert content == 'RESPONSE'
+        assert content == "RESPONSE"
 
     run_cat_test()
```

### Comparing `newrelic-8.8.0/tests/cross_agent/test_collector_hostname.py` & `newrelic-8.8.1/tests/cross_agent/test_collector_hostname.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_datstore_instance.py` & `newrelic-8.8.1/tests/cross_agent/test_datstore_instance.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_distributed_tracing.py` & `newrelic-8.8.1/tests/cross_agent/test_distributed_tracing.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,221 +10,235 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
+
 import pytest
 import webtest
+from testing_support.fixtures import override_application_settings, validate_attributes
+from testing_support.validators.validate_error_event_attributes import (
+    validate_error_event_attributes,
+)
+from testing_support.validators.validate_span_events import validate_span_events
+from testing_support.validators.validate_transaction_event_attributes import (
+    validate_transaction_event_attributes,
+)
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
 
 from newrelic.api.transaction import current_transaction
 from newrelic.api.wsgi_application import wsgi_application
 from newrelic.common.encoding_utils import DistributedTracePayload
 from newrelic.common.object_wrapper import transient_function_wrapper
 
-from testing_support.fixtures import (override_application_settings,
-        validate_error_event_attributes, validate_attributes)
-from testing_support.validators.validate_span_events import (
-        validate_span_events)
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-from testing_support.validators.validate_transaction_event_attributes import validate_transaction_event_attributes
-
 CURRENT_DIR = os.path.dirname(os.path.realpath(__file__))
-JSON_DIR = os.path.normpath(os.path.join(CURRENT_DIR, 'fixtures',
-    'distributed_tracing'))
+JSON_DIR = os.path.normpath(os.path.join(CURRENT_DIR, "fixtures", "distributed_tracing"))
 
-_parameters_list = ['account_id', 'comment', 'expected_metrics',
-        'force_sampled_true', 'inbound_payloads', 'intrinsics',
-        'major_version', 'minor_version', 'outbound_payloads',
-        'raises_exception', 'span_events_enabled', 'test_name',
-        'transport_type', 'trusted_account_key', 'web_transaction']
-_parameters = ','.join(_parameters_list)
+_parameters_list = [
+    "account_id",
+    "comment",
+    "expected_metrics",
+    "force_sampled_true",
+    "inbound_payloads",
+    "intrinsics",
+    "major_version",
+    "minor_version",
+    "outbound_payloads",
+    "raises_exception",
+    "span_events_enabled",
+    "test_name",
+    "transport_type",
+    "trusted_account_key",
+    "web_transaction",
+]
+_parameters = ",".join(_parameters_list)
 
 
 def load_tests():
     result = []
-    path = os.path.join(JSON_DIR, 'distributed_tracing.json')
-    with open(path, 'r') as fh:
+    path = os.path.join(JSON_DIR, "distributed_tracing.json")
+    with open(path, "r") as fh:
         tests = json.load(fh)
 
     for test in tests:
         values = (test.get(param, None) for param in _parameters_list)
-        param = pytest.param(*values, id=test.get('test_name'))
+        param = pytest.param(*values, id=test.get("test_name"))
         result.append(param)
 
     return result
 
 
 def override_compute_sampled(override):
-    @transient_function_wrapper('newrelic.core.adaptive_sampler',
-            'AdaptiveSampler.compute_sampled')
+    @transient_function_wrapper("newrelic.core.adaptive_sampler", "AdaptiveSampler.compute_sampled")
     def _override_compute_sampled(wrapped, instance, args, kwargs):
         if override:
             return True
         return wrapped(*args, **kwargs)
+
     return _override_compute_sampled
 
 
 def assert_payload(payload, payload_assertions, major_version, minor_version):
     assert payload
 
     # flatten payload so it matches the test:
     #   payload['d']['ac'] -> payload['d.ac']
-    d = payload.pop('d')
+    d = payload.pop("d")
     for key, value in d.items():
-        payload['d.%s' % key] = value
+        payload["d.%s" % key] = value
 
-    for expected in payload_assertions.get('expected', []):
+    for expected in payload_assertions.get("expected", []):
         assert expected in payload
 
-    for unexpected in payload_assertions.get('unexpected', []):
+    for unexpected in payload_assertions.get("unexpected", []):
         assert unexpected not in payload
 
-    for key, value in payload_assertions.get('exact', {}).items():
+    for key, value in payload_assertions.get("exact", {}).items():
         assert key in payload
         if isinstance(value, list):
             value = tuple(value)
         assert payload[key] == value
 
-    assert payload['v'][0] == major_version
-    assert payload['v'][1] == minor_version
+    assert payload["v"][0] == major_version
+    assert payload["v"][1] == minor_version
 
 
 @wsgi_application()
 def target_wsgi_application(environ, start_response):
-    status = '200 OK'
-    output = b'hello world'
-    response_headers = [('Content-type', 'text/html; charset=utf-8'),
-                        ('Content-Length', str(len(output)))]
+    status = "200 OK"
+    output = b"hello world"
+    response_headers = [("Content-type", "text/html; charset=utf-8"), ("Content-Length", str(len(output)))]
 
     txn = current_transaction()
-    txn.set_transaction_name(test_settings['test_name'])
+    txn.set_transaction_name(test_settings["test_name"])
 
-    if not test_settings['web_transaction']:
+    if not test_settings["web_transaction"]:
         txn.background_task = True
 
-    if test_settings['raises_exception']:
+    if test_settings["raises_exception"]:
         try:
             1 / 0
         except ZeroDivisionError:
             txn.notice_error()
 
-    extra_inbound_payloads = test_settings['extra_inbound_payloads']
+    extra_inbound_payloads = test_settings["extra_inbound_payloads"]
     for payload, expected_result in extra_inbound_payloads:
-        result = txn.accept_distributed_trace_payload(payload,
-                test_settings['transport_type'])
+        result = txn.accept_distributed_trace_payload(payload, test_settings["transport_type"])
         assert result is expected_result
 
-    outbound_payloads = test_settings['outbound_payloads']
+    outbound_payloads = test_settings["outbound_payloads"]
     if outbound_payloads:
         for payload_assertions in outbound_payloads:
             payload = txn._create_distributed_trace_payload()
-            assert_payload(payload, payload_assertions,
-                    test_settings['major_version'],
-                    test_settings['minor_version'])
+            assert_payload(payload, payload_assertions, test_settings["major_version"], test_settings["minor_version"])
 
     start_response(status, response_headers)
     return [output]
 
 
 test_application = webtest.TestApp(target_wsgi_application)
 
 
 @pytest.mark.parametrize(_parameters, load_tests())
-def test_distributed_tracing(account_id, comment, expected_metrics,
-        force_sampled_true, inbound_payloads, intrinsics, major_version,
-        minor_version, outbound_payloads, raises_exception,
-        span_events_enabled, test_name, transport_type, trusted_account_key,
-        web_transaction):
+def test_distributed_tracing(
+    account_id,
+    comment,
+    expected_metrics,
+    force_sampled_true,
+    inbound_payloads,
+    intrinsics,
+    major_version,
+    minor_version,
+    outbound_payloads,
+    raises_exception,
+    span_events_enabled,
+    test_name,
+    transport_type,
+    trusted_account_key,
+    web_transaction,
+):
 
     extra_inbound_payloads = []
-    if transport_type != 'HTTP':
+    if transport_type != "HTTP":
         # Since wsgi_application calls accept_distributed_trace_payload
         # automatically with transport_type='HTTP', we must defer this call
         # until we can specify the transport type.
         extra_inbound_payloads.append((inbound_payloads.pop(), True))
     elif not inbound_payloads:
         # In order to assert that accept_distributed_trace_payload returns
         # False in this instance, we defer.
         extra_inbound_payloads.append((inbound_payloads, False))
     elif len(inbound_payloads) > 1:
         for payload in inbound_payloads[1:]:
             extra_inbound_payloads.append((payload, False))
 
     global test_settings
     test_settings = {
-        'test_name': test_name,
-        'web_transaction': web_transaction,
-        'raises_exception': raises_exception,
-        'extra_inbound_payloads': extra_inbound_payloads,
-        'outbound_payloads': outbound_payloads,
-        'transport_type': transport_type,
-        'major_version': major_version,
-        'minor_version': minor_version,
+        "test_name": test_name,
+        "web_transaction": web_transaction,
+        "raises_exception": raises_exception,
+        "extra_inbound_payloads": extra_inbound_payloads,
+        "outbound_payloads": outbound_payloads,
+        "transport_type": transport_type,
+        "major_version": major_version,
+        "minor_version": minor_version,
     }
 
     override_settings = {
-        'distributed_tracing.enabled': True,
-        'span_events.enabled': span_events_enabled,
-        'account_id': account_id,
-        'trusted_account_key': trusted_account_key,
+        "distributed_tracing.enabled": True,
+        "span_events.enabled": span_events_enabled,
+        "account_id": account_id,
+        "trusted_account_key": trusted_account_key,
     }
 
-    common_required = intrinsics['common']['expected']
-    common_forgone = intrinsics['common']['unexpected']
-    common_exact = intrinsics['common'].get('exact', {})
-
-    txn_intrinsics = intrinsics.get('Transaction', {})
-    txn_event_required = {'agent': [], 'user': [],
-            'intrinsic': txn_intrinsics.get('expected', [])}
-    txn_event_required['intrinsic'].extend(common_required)
-    txn_event_forgone = {'agent': [], 'user': [],
-            'intrinsic': txn_intrinsics.get('unexpected', [])}
-    txn_event_forgone['intrinsic'].extend(common_forgone)
-    txn_event_exact = {'agent': {}, 'user': {},
-            'intrinsic': txn_intrinsics.get('exact', {})}
-    txn_event_exact['intrinsic'].update(common_exact)
+    common_required = intrinsics["common"]["expected"]
+    common_forgone = intrinsics["common"]["unexpected"]
+    common_exact = intrinsics["common"].get("exact", {})
+
+    txn_intrinsics = intrinsics.get("Transaction", {})
+    txn_event_required = {"agent": [], "user": [], "intrinsic": txn_intrinsics.get("expected", [])}
+    txn_event_required["intrinsic"].extend(common_required)
+    txn_event_forgone = {"agent": [], "user": [], "intrinsic": txn_intrinsics.get("unexpected", [])}
+    txn_event_forgone["intrinsic"].extend(common_forgone)
+    txn_event_exact = {"agent": {}, "user": {}, "intrinsic": txn_intrinsics.get("exact", {})}
+    txn_event_exact["intrinsic"].update(common_exact)
 
     headers = {}
     if inbound_payloads:
         payload = DistributedTracePayload(inbound_payloads[0])
-        headers['newrelic'] = payload.http_safe()
+        headers["newrelic"] = payload.http_safe()
 
-    @validate_transaction_metrics(test_name,
-            rollup_metrics=expected_metrics,
-            background_task=not web_transaction)
-    @validate_transaction_event_attributes(
-            txn_event_required, txn_event_forgone, txn_event_exact)
-    @validate_attributes('intrinsic', common_required, common_forgone)
+    @validate_transaction_metrics(test_name, rollup_metrics=expected_metrics, background_task=not web_transaction)
+    @validate_transaction_event_attributes(txn_event_required, txn_event_forgone, txn_event_exact)
+    @validate_attributes("intrinsic", common_required, common_forgone)
     @override_compute_sampled(force_sampled_true)
     @override_application_settings(override_settings)
     def _test():
-        response = test_application.get('/', headers=headers)
-        assert 'X-NewRelic-App-Data' not in response.headers
+        response = test_application.get("/", headers=headers)
+        assert "X-NewRelic-App-Data" not in response.headers
 
-    if 'Span' in intrinsics:
-        span_intrinsics = intrinsics.get('Span')
-        span_expected = span_intrinsics.get('expected', [])
+    if "Span" in intrinsics:
+        span_intrinsics = intrinsics.get("Span")
+        span_expected = span_intrinsics.get("expected", [])
         span_expected.extend(common_required)
-        span_unexpected = span_intrinsics.get('unexpected', [])
+        span_unexpected = span_intrinsics.get("unexpected", [])
         span_unexpected.extend(common_forgone)
-        span_exact = span_intrinsics.get('exact', {})
+        span_exact = span_intrinsics.get("exact", {})
         span_exact.update(common_exact)
 
-        _test = validate_span_events(exact_intrinsics=span_exact,
-            expected_intrinsics=span_expected,
-            unexpected_intrinsics=span_unexpected)(_test)
+        _test = validate_span_events(
+            exact_intrinsics=span_exact, expected_intrinsics=span_expected, unexpected_intrinsics=span_unexpected
+        )(_test)
     elif not span_events_enabled:
         _test = validate_span_events(count=0)(_test)
 
     if raises_exception:
-        error_event_required = {'agent': [], 'user': [],
-                'intrinsic': common_required}
-        error_event_forgone = {'agent': [], 'user': [],
-                'intrinsic': common_forgone}
-        error_event_exact = {'agent': {}, 'user': {},
-                'intrinsic': common_exact}
-        _test = validate_error_event_attributes(error_event_required,
-                error_event_forgone, error_event_exact)(_test)
+        error_event_required = {"agent": [], "user": [], "intrinsic": common_required}
+        error_event_forgone = {"agent": [], "user": [], "intrinsic": common_forgone}
+        error_event_exact = {"agent": {}, "user": {}, "intrinsic": common_exact}
+        _test = validate_error_event_attributes(error_event_required, error_event_forgone, error_event_exact)(_test)
 
     _test()
```

### Comparing `newrelic-8.8.0/tests/cross_agent/test_docker.py` & `newrelic-8.8.1/tests/cross_agent/test_docker.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_gcp_utilization_data.py` & `newrelic-8.8.1/tests/cross_agent/test_gcp_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_labels_and_rollups.py` & `newrelic-8.8.1/tests/cross_agent/test_labels_and_rollups.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_lambda_event_source.py` & `newrelic-8.8.1/tests/cross_agent/test_lambda_event_source.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_pcf_utilization_data.py` & `newrelic-8.8.1/tests/cross_agent/test_pcf_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_rules.py` & `newrelic-8.8.1/tests/cross_agent/test_rules.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_rum_client_config.py` & `newrelic-8.8.1/tests/cross_agent/test_rum_client_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_sql_obfuscation.py` & `newrelic-8.8.1/tests/cross_agent/test_sql_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_system_info.py` & `newrelic-8.8.1/tests/cross_agent/test_system_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_transaction_segment_terms.py` & `newrelic-8.8.1/tests/cross_agent/test_transaction_segment_terms.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_utilization_configs.py` & `newrelic-8.8.1/tests/cross_agent/test_utilization_configs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/cross_agent/test_w3c_trace_context.py` & `newrelic-8.8.1/tests/cross_agent/test_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/conftest.py` & `newrelic-8.8.1/tests/datastore_aioredis/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
 import pytest
 
 from newrelic.common.package_version_utils import get_package_version_tuple
 from testing_support.db_settings import redis_settings
 
 from testing_support.fixture.event_loop import event_loop as loop
 from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
@@ -63,7 +64,11 @@
     else:
         if request.param == "Redis":
             return loop.run_until_complete(aioredis.create_redis("redis://%s:%d" % (DB_SETTINGS["host"], DB_SETTINGS["port"]), db=0))
         elif request.param == "StrictRedis":
             pytest.skip("StrictRedis not implemented.")
         else:
             raise NotImplementedError()
+
+@pytest.fixture(scope="session")
+def key():
+    return "AIOREDIS-TEST-" + str(os.getpid())
```

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/test_custom_conn_pool.py` & `newrelic-8.8.1/tests/datastore_aioredis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/test_execute_command.py` & `newrelic-8.8.1/tests/datastore_aioredis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/test_get_and_set.py` & `newrelic-8.8.1/tests/datastore_aioredis/test_get_and_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,34 +60,34 @@
 _instance_metric_name = "Datastore/instance/Redis/%s/%s" % (_host, _port)
 
 _enable_rollup_metrics.append((_instance_metric_name, 2))
 
 _disable_rollup_metrics.append((_instance_metric_name, None))
 
 
-async def exercise_redis(client):
-    await client.set("key", "value")
-    await client.get("key")
+async def exercise_redis(client, key):
+    await client.set(key, "value")
+    await client.get(key)
 
 
 @override_application_settings(_enable_instance_settings)
 @validate_transaction_metrics(
     "test_get_and_set:test_redis_client_operation_enable_instance",
     scoped_metrics=_enable_scoped_metrics,
     rollup_metrics=_enable_rollup_metrics,
     background_task=True,
 )
 @background_task()
-def test_redis_client_operation_enable_instance(client, loop):
-    loop.run_until_complete(exercise_redis(client))
+def test_redis_client_operation_enable_instance(client, loop, key):
+    loop.run_until_complete(exercise_redis(client, key))
 
 
 @override_application_settings(_disable_instance_settings)
 @validate_transaction_metrics(
     "test_get_and_set:test_redis_client_operation_disable_instance",
     scoped_metrics=_disable_scoped_metrics,
     rollup_metrics=_disable_rollup_metrics,
     background_task=True,
 )
 @background_task()
-def test_redis_client_operation_disable_instance(client, loop):
-    loop.run_until_complete(exercise_redis(client))
+def test_redis_client_operation_disable_instance(client, loop, key):
+    loop.run_until_complete(exercise_redis(client, key))
```

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/test_instance_info.py` & `newrelic-8.8.1/tests/datastore_aioredis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/test_multiple_dbs.py` & `newrelic-8.8.1/tests/datastore_aioredis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/test_span_event.py` & `newrelic-8.8.1/tests/datastore_aioredis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/test_trace_node.py` & `newrelic-8.8.1/tests/datastore_aioredis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/test_transactions.py` & `newrelic-8.8.1/tests/datastore_aioredis/test_transactions.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,61 +19,63 @@
 )
 
 from newrelic.api.background_task import background_task
 
 
 @background_task()
 @pytest.mark.parametrize("in_transaction", (True, False))
-def test_pipelines_no_harm(client, in_transaction, loop):
+def test_pipelines_no_harm(client, in_transaction, loop, key):
     async def exercise():
         if AIOREDIS_VERSION >= (2,):
             pipe = client.pipeline(transaction=in_transaction)
         else:
             pipe = client.pipeline()  # Transaction kwarg unsupported
 
-        pipe.set("TXN", 1)
+        pipe.set(key, 1)
         return await pipe.execute()
 
     status = loop.run_until_complete(exercise())
     assert status == [True]
 
 
-def exercise_transaction_sync(pipe):
-    pipe.set("TXN", 1)
+def exercise_transaction_sync(key):
+    def _run(pipe):
+        pipe.set(key, 1)
+    return _run
 
 
-async def exercise_transaction_async(pipe):
-    await pipe.set("TXN", 1)
+def exercise_transaction_async(key):
+    async def _run(pipe):
+        await pipe.set(key, 1)
+    return _run
 
 
 @SKIPIF_AIOREDIS_V1
 @pytest.mark.parametrize("exercise", (exercise_transaction_sync, exercise_transaction_async))
 @background_task()
-def test_transactions_no_harm(client, loop, exercise):
-    status = loop.run_until_complete(client.transaction(exercise))
+def test_transactions_no_harm(client, loop, key, exercise):
+    status = loop.run_until_complete(client.transaction(exercise(key)))
     assert status == [True]
 
 
 @SKIPIF_AIOREDIS_V2
 @background_task()
-def test_multi_exec_no_harm(client, loop):
+def test_multi_exec_no_harm(client, loop, key):
     async def exercise():
         pipe = client.multi_exec()
-        pipe.set("key", "value")
+        pipe.set(key, "value")
         status = await pipe.execute()
         assert status == [True]
 
     loop.run_until_complete(exercise())
 
 
 @SKIPIF_AIOREDIS_V1
 @background_task()
-def test_pipeline_immediate_execution_no_harm(client, loop):
-    key = "TXN_WATCH"
-
+def test_pipeline_immediate_execution_no_harm(client, loop, key):
     async def exercise():
         await client.set(key, 1)
 
         if AIOREDIS_VERSION >= (2,):
             pipe = client.pipeline(transaction=True)
         else:
             pipe = client.pipeline()  # Transaction kwarg unsupported
@@ -90,17 +92,15 @@
         assert int(await client.get(key)) == 2
 
     loop.run_until_complete(exercise())
 
 
 @SKIPIF_AIOREDIS_V1
 @background_task()
-def test_transaction_immediate_execution_no_harm(client, loop):
-    key = "TXN_WATCH"
-
+def test_transaction_immediate_execution_no_harm(client, loop, key):
     async def exercise():
         async def exercise_transaction(pipe):
             value = int(await pipe.get(key))
             assert value == 1
             value += 1
             pipe.multi()
             pipe.set(key, value)
@@ -115,17 +115,15 @@
     status = loop.run_until_complete(exercise())
     assert status == []
 
 
 @SKIPIF_AIOREDIS_V1
 @validate_transaction_errors([])
 @background_task()
-def test_transaction_watch_error_no_harm(client, loop):
-    key = "TXN_WATCH"
-
+def test_transaction_watch_error_no_harm(client, loop, key):
     async def exercise():
         async def exercise_transaction(pipe):
             value = int(await pipe.get(key))
             if value == 1:
                 # Only run set the first pass, as this runs repeatedly until no watch error is raised.
                 await pipe.set(key, 2)
```

### Comparing `newrelic-8.8.0/tests/datastore_aioredis/test_uninstrumented_methods.py` & `newrelic-8.8.1/tests/datastore_aioredis/test_uninstrumented_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 IGNORED_METHODS = {
     "address",
     "auto_close_connection_pool",
     "channels",
     "client_tracking_off",
     "client_tracking_on",
+    "client_no_touch",
     "close",
     "closed",
     "connection_pool",
     "connection",
     "db",
     "encoding",
     "execute_command",
```

### Comparing `newrelic-8.8.0/tests/datastore_aredis/conftest.py` & `newrelic-8.8.1/tests/datastore_aredis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aredis/test_custom_conn_pool.py` & `newrelic-8.8.1/tests/datastore_aredis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aredis/test_execute_command.py` & `newrelic-8.8.1/tests/datastore_aredis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aredis/test_get_and_set.py` & `newrelic-8.8.1/tests/datastore_aredis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aredis/test_instance_info.py` & `newrelic-8.8.1/tests/datastore_aredis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aredis/test_multiple_dbs.py` & `newrelic-8.8.1/tests/datastore_aredis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aredis/test_span_event.py` & `newrelic-8.8.1/tests/datastore_aredis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aredis/test_trace_node.py` & `newrelic-8.8.1/tests/datastore_aredis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_aredis/test_uninstrumented_methods.py` & `newrelic-8.8.1/tests/datastore_aredis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_asyncpg/conftest.py` & `newrelic-8.8.1/tests/datastore_asyncpg/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_asyncpg/test_multiple_dbs.py` & `newrelic-8.8.1/tests/datastore_asyncpg/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_asyncpg/test_query.py` & `newrelic-8.8.1/tests/datastore_asyncpg/test_query.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_bmemcached/conftest.py` & `newrelic-8.8.1/tests/datastore_bmemcached/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_bmemcached/test_memcache.py` & `newrelic-8.8.1/tests/datastore_bmemcached/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_elasticsearch/conftest.py` & `newrelic-8.8.1/tests/datastore_elasticsearch/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_elasticsearch/test_connection.py` & `newrelic-8.8.1/tests/datastore_elasticsearch/test_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def test_connection_default():
     if IS_V8:
         conn = Connection(NodeConfig(**HOST))
     else:
         conn = Connection(**HOST)
 
-    assert conn._nr_host_port == ("localhost", ES_SETTINGS["port"])
+    assert conn._nr_host_port == (ES_SETTINGS["host"], ES_SETTINGS["port"])
 
 
 @SKIP_IF_V7
 def test_connection_config():
     conn = Connection(NodeConfig(scheme="http", host="foo", port=8888))
     assert conn._nr_host_port == ("foo", "8888")
```

### Comparing `newrelic-8.8.0/tests/datastore_elasticsearch/test_database_duration.py` & `newrelic-8.8.1/tests/datastore_elasticsearch/test_database_duration.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_elasticsearch/test_elasticsearch.py` & `newrelic-8.8.1/tests/datastore_elasticsearch/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_elasticsearch/test_instrumented_methods.py` & `newrelic-8.8.1/tests/datastore_elasticsearch/test_instrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_elasticsearch/test_mget.py` & `newrelic-8.8.1/tests/datastore_elasticsearch/test_mget.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_elasticsearch/test_multiple_dbs.py` & `newrelic-8.8.1/tests/datastore_elasticsearch/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_elasticsearch/test_trace_node.py` & `newrelic-8.8.1/tests/datastore_elasticsearch/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_elasticsearch/test_transport.py` & `newrelic-8.8.1/tests/datastore_elasticsearch/test_transport.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_memcache/conftest.py` & `newrelic-8.8.1/tests/datastore_memcache/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_memcache/test_all_methods_wrapped.py` & `newrelic-8.8.1/tests/datastore_memcache/test_all_methods_wrapped.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_memcache/test_memcache.py` & `newrelic-8.8.1/tests/datastore_memcache/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_memcache/test_multiple_dbs.py` & `newrelic-8.8.1/tests/datastore_memcache/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_memcache/test_span_event.py` & `newrelic-8.8.1/tests/datastore_memcache/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_mysql/conftest.py` & `newrelic-8.8.1/tests/datastore_mysql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_mysql/test_database.py` & `newrelic-8.8.1/tests/datastore_mysql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_postgresql/conftest.py` & `newrelic-8.8.1/tests/datastore_postgresql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_postgresql/test_database.py` & `newrelic-8.8.1/tests/datastore_postgresql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/conftest.py` & `newrelic-8.8.1/tests/datastore_psycopg2/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_as_string.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_as_string.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_async.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_cursor.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_cursor.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_database_instance_info.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_database_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_explain_plans.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_explain_plans.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_forward_compat.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_forward_compat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_multiple_dbs.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_obfuscation.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_register.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_register.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_rollback.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_rollback.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_slow_sql.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_slow_sql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_span_event.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/test_trace_node.py` & `newrelic-8.8.1/tests/datastore_psycopg2/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2/utils.py` & `newrelic-8.8.1/tests/datastore_psycopg2/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2cffi/conftest.py` & `newrelic-8.8.1/tests/datastore_psycopg2cffi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2cffi/test_database.py` & `newrelic-8.8.1/tests/datastore_psycopg2cffi/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_psycopg2cffi/test_explain_plans.py` & `newrelic-8.8.1/tests/datastore_psycopg2cffi/test_explain_plans.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_pyelasticsearch/conftest.py` & `newrelic-8.8.1/tests/datastore_pymemcache/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
     'debug.record_transaction_failure': True
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (datastore_pyelasticsearch)',
+        app_name='Python Agent Test (datastore_pymemcache)',
         default_settings=_default_settings,
         linked_applications=['Python Agent Test (datastore)'])
```

### Comparing `newrelic-8.8.0/tests/datastore_pylibmc/conftest.py` & `newrelic-8.8.1/tests/framework_falcon/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 
 
 _default_settings = {
     'transaction_tracer.explain_threshold': 0.0,
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
-    'debug.record_transaction_failure': True
+    'debug.record_transaction_failure': True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (datastore_pylibmc)',
-        default_settings=_default_settings,
-        linked_applications=['Python Agent Test (datastore)'])
+        app_name='Python Agent Test (framework_falcon)',
+        default_settings=_default_settings)
+
+
+@pytest.fixture()
+def app():
+    from _target_application import _target_application
+    return _target_application
```

### Comparing `newrelic-8.8.0/tests/datastore_pylibmc/test_memcache.py` & `newrelic-8.8.1/tests/datastore_pylibmc/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_pymemcache/conftest.py` & `newrelic-8.8.1/tests/datastore_sqlite/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 _default_settings = {
     'transaction_tracer.explain_threshold': 0.0,
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
-    'debug.record_transaction_failure': True
+    'debug.record_transaction_failure': True,
+    'debug.log_explain_plan_queries': True
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (datastore_pymemcache)',
+        app_name='Python Agent Test (datastore_sqlite)',
         default_settings=_default_settings,
         linked_applications=['Python Agent Test (datastore)'])
```

### Comparing `newrelic-8.8.0/tests/datastore_pymemcache/test_memcache.py` & `newrelic-8.8.1/tests/datastore_pymemcache/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_pymongo/conftest.py` & `newrelic-8.8.1/tests/datastore_pymongo/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_pymongo/test_pymongo.py` & `newrelic-8.8.1/tests/datastore_pymongo/test_pymongo.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_pymysql/conftest.py` & `newrelic-8.8.1/tests/datastore_pymysql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_pymysql/test_database.py` & `newrelic-8.8.1/tests/datastore_pymysql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_pysolr/conftest.py` & `newrelic-8.8.1/tests/datastore_pysolr/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_pysolr/test_solr.py` & `newrelic-8.8.1/tests/datastore_pysolr/test_solr.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/conftest.py` & `newrelic-8.8.1/tests/datastore_redis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/test_custom_conn_pool.py` & `newrelic-8.8.1/tests/datastore_redis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/test_execute_command.py` & `newrelic-8.8.1/tests/datastore_redis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/test_get_and_set.py` & `newrelic-8.8.1/tests/datastore_redis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/test_instance_info.py` & `newrelic-8.8.1/tests/datastore_redis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/test_multiple_dbs.py` & `newrelic-8.8.1/tests/datastore_redis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/test_rb.py` & `newrelic-8.8.1/tests/datastore_redis/test_rb.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/test_span_event.py` & `newrelic-8.8.1/tests/datastore_redis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/test_trace_node.py` & `newrelic-8.8.1/tests/datastore_redis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_redis/test_uninstrumented_methods.py` & `newrelic-8.8.1/tests/datastore_redis/test_uninstrumented_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 import redis
-
 from testing_support.db_settings import redis_settings
 
 DB_SETTINGS = redis_settings()[0]
 
-redis_client = redis.Redis(host=DB_SETTINGS['host'], port=DB_SETTINGS['port'], db=0)
-strict_redis_client = redis.StrictRedis(host=DB_SETTINGS['host'], port=DB_SETTINGS['port'], db=0)
+redis_client = redis.Redis(host=DB_SETTINGS["host"], port=DB_SETTINGS["port"], db=0)
+strict_redis_client = redis.StrictRedis(host=DB_SETTINGS["host"], port=DB_SETTINGS["port"], db=0)
 
 
 IGNORED_METHODS = {
-    'MODULE_CALLBACKS',
-    'MODULE_VERSION',
-    'NAME',
+    "MODULE_CALLBACKS",
+    "MODULE_VERSION",
+    "NAME",
     "add_edge",
     "add_node",
     "append_bucket_size",
     "append_capacity",
     "append_error",
     "append_expansion",
     "append_items_and_increments",
@@ -40,14 +39,15 @@
     "append_no_scale",
     "append_values_and_weights",
     "append_weights",
     "batch_indexer",
     "BatchIndexer",
     "bulk",
     "call_procedure",
+    "client_no_touch",
     "client_tracking_off",
     "client_tracking_on",
     "client",
     "close",
     "commandmixin",
     "connection_pool",
     "connection",
```

### Comparing `newrelic-8.8.0/tests/datastore_solrpy/conftest.py` & `newrelic-8.8.1/tests/datastore_solrpy/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_solrpy/test_solr.py` & `newrelic-8.8.1/tests/datastore_solrpy/test_solr.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_sqlite/conftest.py` & `newrelic-8.8.1/tests/framework_django/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
 _default_settings = {
     'transaction_tracer.explain_threshold': 0.0,
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
     'debug.record_transaction_failure': True,
-    'debug.log_explain_plan_queries': True
+    'debug.log_autorum_middleware': True,
+    'feature_flag': set(['django.instrumentation.inclusion-tags.r1']),
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (datastore_sqlite)',
-        default_settings=_default_settings,
-        linked_applications=['Python Agent Test (datastore)'])
+        app_name='Python Agent Test (framework_django)',
+        default_settings=_default_settings)
```

### Comparing `newrelic-8.8.0/tests/datastore_sqlite/test_database.py` & `newrelic-8.8.1/tests/datastore_sqlite/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_sqlite/test_obfuscation.py` & `newrelic-8.8.1/tests/datastore_sqlite/test_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/datastore_umemcache/conftest.py` & `newrelic-8.8.1/tests/external_botocore/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,13 @@
 
 
 _default_settings = {
     'transaction_tracer.explain_threshold': 0.0,
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
-    'debug.record_transaction_failure': True
+    'debug.record_transaction_failure': True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (datastore_umemcache)',
-        default_settings=_default_settings,
-        linked_applications=['Python Agent Test (datastore)'])
+        app_name='Python Agent Test (external_botocore)',
+        default_settings=_default_settings)
```

### Comparing `newrelic-8.8.0/tests/external_boto3/conftest.py` & `newrelic-8.8.1/tests/external_boto3/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_boto3/test_boto3_iam.py` & `newrelic-8.8.1/tests/external_boto3/test_boto3_iam.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,73 +13,77 @@
 # limitations under the License.
 
 import sys
 import uuid
 
 import boto3
 import moto
+from testing_support.fixtures import override_application_settings
+from testing_support.validators.validate_span_events import validate_span_events
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
+from testing_support.validators.validate_tt_segment_params import (
+    validate_tt_segment_params,
+)
 
 from newrelic.api.background_task import background_task
-from testing_support.fixtures import (
-        validate_tt_segment_params, override_application_settings)
-from testing_support.validators.validate_span_events import (
-        validate_span_events)
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
 
-MOTO_VERSION = tuple(int(v) for v in moto.__version__.split('.')[:3])
+MOTO_VERSION = tuple(int(v) for v in moto.__version__.split(".")[:3])
 
 # patch earlier versions of moto to support py37
 if sys.version_info >= (3, 7) and MOTO_VERSION <= (1, 3, 1):
     import re
+
     moto.packages.responses.responses.re._pattern_type = re.Pattern
 
-AWS_ACCESS_KEY_ID = 'AAAAAAAAAAAACCESSKEY'
-AWS_SECRET_ACCESS_KEY = 'AAAAAASECRETKEY'
+AWS_ACCESS_KEY_ID = "AAAAAAAAAAAACCESSKEY"
+AWS_SECRET_ACCESS_KEY = "AAAAAASECRETKEY"  # nosec (This is fine for testing purposes)
 
-TEST_USER = 'python-agent-test-%s' % uuid.uuid4()
+TEST_USER = "python-agent-test-%s" % uuid.uuid4()
 
 _iam_scoped_metrics = [
-    ('External/iam.amazonaws.com/botocore/POST', 3),
+    ("External/iam.amazonaws.com/botocore/POST", 3),
 ]
 
 _iam_rollup_metrics = [
-    ('External/all', 3),
-    ('External/allOther', 3),
-    ('External/iam.amazonaws.com/all', 3),
-    ('External/iam.amazonaws.com/botocore/POST', 3),
+    ("External/all", 3),
+    ("External/allOther", 3),
+    ("External/iam.amazonaws.com/all", 3),
+    ("External/iam.amazonaws.com/botocore/POST", 3),
 ]
 
 
-@override_application_settings({'distributed_tracing.enabled': True})
-@validate_span_events(
-        exact_agents={'http.url': 'https://iam.amazonaws.com/'}, count=3)
-@validate_span_events(expected_agents=('aws.requestId',), count=3)
-@validate_span_events(exact_agents={'aws.operation': 'CreateUser'}, count=1)
-@validate_span_events(exact_agents={'aws.operation': 'GetUser'}, count=1)
-@validate_span_events(exact_agents={'aws.operation': 'DeleteUser'}, count=1)
-@validate_tt_segment_params(present_params=('aws.requestId',))
+@override_application_settings({"distributed_tracing.enabled": True})
+@validate_span_events(exact_agents={"http.url": "https://iam.amazonaws.com/"}, count=3)
+@validate_span_events(expected_agents=("aws.requestId",), count=3)
+@validate_span_events(exact_agents={"aws.operation": "CreateUser"}, count=1)
+@validate_span_events(exact_agents={"aws.operation": "GetUser"}, count=1)
+@validate_span_events(exact_agents={"aws.operation": "DeleteUser"}, count=1)
+@validate_tt_segment_params(present_params=("aws.requestId",))
 @validate_transaction_metrics(
-        'test_boto3_iam:test_iam',
-        scoped_metrics=_iam_scoped_metrics,
-        rollup_metrics=_iam_rollup_metrics,
-        background_task=True)
+    "test_boto3_iam:test_iam",
+    scoped_metrics=_iam_scoped_metrics,
+    rollup_metrics=_iam_rollup_metrics,
+    background_task=True,
+)
 @background_task()
 @moto.mock_iam
 def test_iam():
     iam = boto3.client(
-            'iam',
-            aws_access_key_id=AWS_ACCESS_KEY_ID,
-            aws_secret_access_key=AWS_SECRET_ACCESS_KEY,
+        "iam",
+        aws_access_key_id=AWS_ACCESS_KEY_ID,
+        aws_secret_access_key=AWS_SECRET_ACCESS_KEY,
     )
 
     # Create user
     resp = iam.create_user(UserName=TEST_USER)
-    assert resp['ResponseMetadata']['HTTPStatusCode'] == 200
+    assert resp["ResponseMetadata"]["HTTPStatusCode"] == 200
 
     # Get the user
     resp = iam.get_user(UserName=TEST_USER)
-    assert resp['ResponseMetadata']['HTTPStatusCode'] == 200
-    assert resp['User']['UserName'] == TEST_USER
+    assert resp["ResponseMetadata"]["HTTPStatusCode"] == 200
+    assert resp["User"]["UserName"] == TEST_USER
 
     # Delete the user
     resp = iam.delete_user(UserName=TEST_USER)
-    assert resp['ResponseMetadata']['HTTPStatusCode'] == 200
+    assert resp["ResponseMetadata"]["HTTPStatusCode"] == 200
```

### Comparing `newrelic-8.8.0/tests/external_boto3/test_boto3_s3.py` & `newrelic-8.8.1/tests/external_boto3/test_boto3_s3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_boto3/test_boto3_sns.py` & `newrelic-8.8.1/tests/external_boto3/test_boto3_sns.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,84 +9,95 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
+
 import boto3
 import moto
 import pytest
+from testing_support.fixtures import override_application_settings
+from testing_support.validators.validate_span_events import validate_span_events
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
+from testing_support.validators.validate_tt_segment_params import (
+    validate_tt_segment_params,
+)
 
 from newrelic.api.background_task import background_task
-from testing_support.fixtures import (
-        validate_tt_segment_params, override_application_settings)
-from testing_support.validators.validate_span_events import validate_span_events
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
 
-MOTO_VERSION = tuple(int(v) for v in moto.__version__.split('.')[:3])
+MOTO_VERSION = tuple(int(v) for v in moto.__version__.split(".")[:3])
 
 # patch earlier versions of moto to support py37
 if sys.version_info >= (3, 7) and MOTO_VERSION <= (1, 3, 1):
     import re
+
     moto.packages.responses.responses.re._pattern_type = re.Pattern
 
-AWS_ACCESS_KEY_ID = 'AAAAAAAAAAAACCESSKEY'
-AWS_SECRET_ACCESS_KEY = 'AAAAAASECRETKEY'
-AWS_REGION_NAME = 'us-east-1'
-SNS_URL = 'sns-us-east-1.amazonaws.com'
-TOPIC = 'arn:aws:sns:us-east-1:123456789012:some-topic'
-sns_metrics = [
-        ('MessageBroker/SNS/Topic'
-        '/Produce/Named/%s' % TOPIC, 1)]
-sns_metrics_phone = [
-        ('MessageBroker/SNS/Topic'
-        '/Produce/Named/PhoneNumber', 1)]
-
-
-@override_application_settings({'distributed_tracing.enabled': True})
-@validate_span_events(expected_agents=('aws.requestId',), count=2)
-@validate_span_events(exact_agents={'aws.operation': 'CreateTopic'}, count=1)
-@validate_span_events(exact_agents={'aws.operation': 'Publish'}, count=1)
-@validate_tt_segment_params(present_params=('aws.requestId',))
-@pytest.mark.parametrize('topic_argument', ('TopicArn', 'TargetArn'))
-@validate_transaction_metrics('test_boto3_sns:test_publish_to_sns_topic',
-        scoped_metrics=sns_metrics, rollup_metrics=sns_metrics,
-        background_task=True)
+AWS_ACCESS_KEY_ID = "AAAAAAAAAAAACCESSKEY"
+AWS_SECRET_ACCESS_KEY = "AAAAAASECRETKEY"  # nosec (This is fine for testing purposes)
+AWS_REGION_NAME = "us-east-1"
+SNS_URL = "sns-us-east-1.amazonaws.com"
+TOPIC = "arn:aws:sns:us-east-1:123456789012:some-topic"
+sns_metrics = [("MessageBroker/SNS/Topic" "/Produce/Named/%s" % TOPIC, 1)]
+sns_metrics_phone = [("MessageBroker/SNS/Topic" "/Produce/Named/PhoneNumber", 1)]
+
+
+@override_application_settings({"distributed_tracing.enabled": True})
+@validate_span_events(expected_agents=("aws.requestId",), count=2)
+@validate_span_events(exact_agents={"aws.operation": "CreateTopic"}, count=1)
+@validate_span_events(exact_agents={"aws.operation": "Publish"}, count=1)
+@validate_tt_segment_params(present_params=("aws.requestId",))
+@pytest.mark.parametrize("topic_argument", ("TopicArn", "TargetArn"))
+@validate_transaction_metrics(
+    "test_boto3_sns:test_publish_to_sns_topic",
+    scoped_metrics=sns_metrics,
+    rollup_metrics=sns_metrics,
+    background_task=True,
+)
 @background_task()
 @moto.mock_sns
 def test_publish_to_sns_topic(topic_argument):
-    conn = boto3.client('sns',
-            aws_access_key_id=AWS_ACCESS_KEY_ID,
-            aws_secret_access_key=AWS_SECRET_ACCESS_KEY,
-            region_name=AWS_REGION_NAME)
+    conn = boto3.client(
+        "sns",
+        aws_access_key_id=AWS_ACCESS_KEY_ID,
+        aws_secret_access_key=AWS_SECRET_ACCESS_KEY,
+        region_name=AWS_REGION_NAME,
+    )
 
-    topic_arn = conn.create_topic(Name='some-topic')['TopicArn']
+    topic_arn = conn.create_topic(Name="some-topic")["TopicArn"]
 
     kwargs = {topic_argument: topic_arn}
-    published_message = conn.publish(Message='my msg', **kwargs)
-    assert 'MessageId' in published_message
+    published_message = conn.publish(Message="my msg", **kwargs)
+    assert "MessageId" in published_message
 
 
-@override_application_settings({'distributed_tracing.enabled': True})
-@validate_span_events(expected_agents=('aws.requestId',), count=3)
-@validate_span_events(exact_agents={'aws.operation': 'CreateTopic'}, count=1)
-@validate_span_events(exact_agents={'aws.operation': 'Subscribe'}, count=1)
-@validate_span_events(exact_agents={'aws.operation': 'Publish'}, count=1)
-@validate_tt_segment_params(present_params=('aws.requestId',))
-@validate_transaction_metrics('test_boto3_sns:test_publish_to_sns_phone',
-        scoped_metrics=sns_metrics_phone, rollup_metrics=sns_metrics_phone,
-        background_task=True)
+@override_application_settings({"distributed_tracing.enabled": True})
+@validate_span_events(expected_agents=("aws.requestId",), count=3)
+@validate_span_events(exact_agents={"aws.operation": "CreateTopic"}, count=1)
+@validate_span_events(exact_agents={"aws.operation": "Subscribe"}, count=1)
+@validate_span_events(exact_agents={"aws.operation": "Publish"}, count=1)
+@validate_tt_segment_params(present_params=("aws.requestId",))
+@validate_transaction_metrics(
+    "test_boto3_sns:test_publish_to_sns_phone",
+    scoped_metrics=sns_metrics_phone,
+    rollup_metrics=sns_metrics_phone,
+    background_task=True,
+)
 @background_task()
 @moto.mock_sns
 def test_publish_to_sns_phone():
-    conn = boto3.client('sns',
-            aws_access_key_id=AWS_ACCESS_KEY_ID,
-            aws_secret_access_key=AWS_SECRET_ACCESS_KEY,
-            region_name=AWS_REGION_NAME)
-
-    topic_arn = conn.create_topic(Name='some-topic')['TopicArn']
-    conn.subscribe(TopicArn=topic_arn, Protocol='sms', Endpoint='5555555555')
-
-    published_message = conn.publish(
-            PhoneNumber='5555555555', Message='my msg')
-    assert 'MessageId' in published_message
+    conn = boto3.client(
+        "sns",
+        aws_access_key_id=AWS_ACCESS_KEY_ID,
+        aws_secret_access_key=AWS_SECRET_ACCESS_KEY,
+        region_name=AWS_REGION_NAME,
+    )
+
+    topic_arn = conn.create_topic(Name="some-topic")["TopicArn"]
+    conn.subscribe(TopicArn=topic_arn, Protocol="sms", Endpoint="5555555555")
+
+    published_message = conn.publish(PhoneNumber="5555555555", Message="my msg")
+    assert "MessageId" in published_message
```

### Comparing `newrelic-8.8.0/tests/external_botocore/conftest.py` & `newrelic-8.8.1/tests/framework_cherrypy/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,9 +22,9 @@
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
     'debug.record_transaction_failure': True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (external_botocore)',
+        app_name='Python Agent Test (framework_cherrypy)',
         default_settings=_default_settings)
```

### Comparing `newrelic-8.8.0/tests/external_botocore/test_botocore_s3.py` & `newrelic-8.8.1/tests/external_botocore/test_botocore_s3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_botocore/test_botocore_sqs.py` & `newrelic-8.8.1/tests/external_botocore/test_botocore_sqs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_feedparser/conftest.py` & `newrelic-8.8.1/tests/external_feedparser/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_feedparser/packages.xml` & `newrelic-8.8.1/tests/external_feedparser/packages.xml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_feedparser/test_feedparser.py` & `newrelic-8.8.1/tests/external_feedparser/test_feedparser.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_http/conftest.py` & `newrelic-8.8.1/tests/external_http/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_http/test_http.py` & `newrelic-8.8.1/tests/external_http/test_http.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_httplib/conftest.py` & `newrelic-8.8.1/tests/external_httplib/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_httplib/test_httplib.py` & `newrelic-8.8.1/tests/external_httplib/test_httplib.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,28 @@
 except ImportError:
     import httplib
 
 from testing_support.external_fixtures import (
     cache_outgoing_headers,
     insert_incoming_headers,
 )
-from testing_support.fixtures import (
-    cat_enabled,
-    override_application_settings,
-    validate_tt_segment_params,
-)
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
+from testing_support.fixtures import cat_enabled, override_application_settings
 from testing_support.validators.validate_cross_process_headers import (
     validate_cross_process_headers,
 )
 from testing_support.validators.validate_external_node_params import (
     validate_external_node_params,
 )
 from testing_support.validators.validate_span_events import validate_span_events
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
+from testing_support.validators.validate_tt_segment_params import (
+    validate_tt_segment_params,
+)
 
 from newrelic.api.background_task import background_task
 from newrelic.common.encoding_utils import DistributedTracePayload
 from newrelic.packages import six
 
 
 def select_python_version(py2, py3):
@@ -100,15 +101,16 @@
         "test_httplib:test_httplib_https_request",
         scoped_metrics=_test_httplib_https_request_scoped_metrics,
         rollup_metrics=_test_httplib_https_request_rollup_metrics,
         background_task=True,
     )
     @background_task(name="test_httplib:test_httplib_https_request")
     def _test():
-        connection = httplib.HTTPSConnection("localhost", server.port)
+        # fix HTTPSConnection: https://wiki.openstack.org/wiki/OSSN/OSSN-0033
+        connection = httplib.HTTPSConnection("localhost", server.port)  # nosec
         # It doesn't matter that a SSL exception is raised here because the
         # agent still records this as an external request
         try:
             connection.request("GET", "/")
         except Exception:
             pass
         connection.close()
```

### Comparing `newrelic-8.8.0/tests/external_httplib/test_urllib.py` & `newrelic-8.8.1/tests/external_httplib/test_urllib.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_httplib/test_urllib2.py` & `newrelic-8.8.1/tests/external_httplib/test_urllib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_httplib2/conftest.py` & `newrelic-8.8.1/tests/external_httplib2/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_httplib2/test_httplib2.py` & `newrelic-8.8.1/tests/external_httplib2/test_httplib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_httpx/conftest.py` & `newrelic-8.8.1/tests/external_httpx/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_httpx/test_client.py` & `newrelic-8.8.1/tests/external_httpx/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,31 @@
 import asyncio
 
 import pytest
 from testing_support.fixtures import (
     dt_enabled,
     override_application_settings,
     override_generic_settings,
-    validate_tt_segment_params,
 )
 from testing_support.mock_external_http_server import (
     MockExternalHTTPHResponseHeadersServer,
 )
 from testing_support.validators.validate_cross_process_headers import (
     validate_cross_process_headers,
 )
 from testing_support.validators.validate_span_events import validate_span_events
-from testing_support.validators.validate_transaction_errors import validate_transaction_errors
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
+from testing_support.validators.validate_transaction_errors import (
+    validate_transaction_errors,
+)
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
+from testing_support.validators.validate_tt_segment_params import (
+    validate_tt_segment_params,
+)
 
 from newrelic.api.background_task import background_task
 from newrelic.api.time_trace import current_trace
 from newrelic.api.transaction import current_transaction
 from newrelic.core.config import global_settings
 
 ENCODING_KEY = "1234567890123456789012345678901234567890"
```

### Comparing `newrelic-8.8.0/tests/external_requests/conftest.py` & `newrelic-8.8.1/tests/external_requests/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_requests/test_requests.py` & `newrelic-8.8.1/tests/external_requests/test_requests.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_requests/test_span_event.py` & `newrelic-8.8.1/tests/external_requests/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_urllib3/conftest.py` & `newrelic-8.8.1/tests/external_urllib3/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/external_urllib3/test_urllib3.py` & `newrelic-8.8.1/tests/external_urllib3/test_urllib3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/_target_application.py` & `newrelic-8.8.1/tests/framework_aiohttp/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/conftest.py` & `newrelic-8.8.1/tests/framework_aiohttp/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/test_client.py` & `newrelic-8.8.1/tests/framework_aiohttp/test_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/test_client_async_await.py` & `newrelic-8.8.1/tests/framework_aiohttp/test_client_async_await.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/test_client_cat.py` & `newrelic-8.8.1/tests/framework_aiohttp/test_client_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/test_externals.py` & `newrelic-8.8.1/tests/framework_aiohttp/test_externals.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/test_middleware.py` & `newrelic-8.8.1/tests/framework_aiohttp/test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/test_server.py` & `newrelic-8.8.1/tests/framework_aiohttp/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/test_server_cat.py` & `newrelic-8.8.1/tests/framework_aiohttp/test_server_cat.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ("/coro?hello=world", "_target_application:index"),
     ("/class?hello=world", "_target_application:HelloWorldView._respond"),
 ]
 
 
 def record_aiohttp1_raw_headers(raw_headers):
     try:
-        import aiohttp.protocol  # noqa: F401
+        import aiohttp.protocol  # noqa: F401, pylint: disable=W0611
     except ImportError:
 
         def pass_through(function):
             return function
 
         return pass_through
```

### Comparing `newrelic-8.8.0/tests/framework_aiohttp/test_ws.py` & `newrelic-8.8.1/tests/framework_aiohttp/test_ws.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_ariadne/_target_application.py` & `newrelic-8.8.1/tests/framework_ariadne/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_ariadne/conftest.py` & `newrelic-8.8.1/tests/framework_ariadne/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_ariadne/schema.graphql` & `newrelic-8.8.1/tests/framework_ariadne/schema.graphql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_ariadne/test_application.py` & `newrelic-8.8.1/tests/framework_ariadne/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_ariadne/test_application_async.py` & `newrelic-8.8.1/tests/framework_ariadne/test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_ariadne/test_asgi.py` & `newrelic-8.8.1/tests/framework_ariadne/test_asgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_ariadne/test_wsgi.py` & `newrelic-8.8.1/tests/framework_ariadne/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_bottle/_target_application.py` & `newrelic-8.8.1/tests/framework_bottle/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_bottle/conftest.py` & `newrelic-8.8.1/tests/framework_bottle/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_bottle/test_application.py` & `newrelic-8.8.1/tests/framework_bottle/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_cherrypy/conftest.py` & `newrelic-8.8.1/tests/framework_pyramid/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,9 +22,9 @@
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
     'debug.record_transaction_failure': True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (framework_cherrypy)',
+        app_name='Python Agent Test (framework_pyramid)',
         default_settings=_default_settings)
```

### Comparing `newrelic-8.8.0/tests/framework_cherrypy/test_application.py` & `newrelic-8.8.1/tests/framework_cherrypy/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_cherrypy/test_dispatch.py` & `newrelic-8.8.1/tests/framework_cherrypy/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_cherrypy/test_resource.py` & `newrelic-8.8.1/tests/framework_cherrypy/test_resource.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_cherrypy/test_routes.py` & `newrelic-8.8.1/tests/framework_cherrypy/test_routes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/_target_application.py` & `newrelic-8.8.1/tests/framework_django/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/conftest.py` & `newrelic-8.8.1/tests/template_mako/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
-
 from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
 
-
 _default_settings = {
     'transaction_tracer.explain_threshold': 0.0,
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
     'debug.record_transaction_failure': True,
-    'debug.log_autorum_middleware': True,
-    'feature_flag': set(['django.instrumentation.inclusion-tags.r1']),
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (framework_django)',
+        app_name='Python Agent Test (template_mako)',
         default_settings=_default_settings)
+
```

### Comparing `newrelic-8.8.0/tests/framework_django/dummy_app/__init__.py` & `newrelic-8.8.1/tests/framework_django/dummy_app/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/dummy_app/templatetags/__init__.py` & `newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/dummy_app/templatetags/custom_tags.py` & `newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/custom_tags.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/middleware.py` & `newrelic-8.8.1/tests/framework_django/middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/settings.py` & `newrelic-8.8.1/tests/framework_django/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/templates/main.html` & `newrelic-8.8.1/tests/framework_django/templates/main.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/templates/render_exception.html` & `newrelic-8.8.1/tests/framework_django/templates/render_exception.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/templates/results.html` & `newrelic-8.8.1/tests/framework_django/templates/results.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/test_application.py` & `newrelic-8.8.1/tests/framework_django/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/test_asgi_application.py` & `newrelic-8.8.1/tests/framework_django/test_asgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/urls.py` & `newrelic-8.8.1/tests/framework_django/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/views.py` & `newrelic-8.8.1/tests/framework_django/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_django/wsgi.py` & `newrelic-8.8.1/tests/framework_django/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_falcon/_target_application.py` & `newrelic-8.8.1/tests/framework_falcon/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_falcon/conftest.py` & `newrelic-8.8.1/tests/framework_graphql/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
+import six
 
 from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
 
 
 _default_settings = {
-    'transaction_tracer.explain_threshold': 0.0,
-    'transaction_tracer.transaction_threshold': 0.0,
-    'transaction_tracer.stack_trace_threshold': 0.0,
-    'debug.log_data_collector_payloads': True,
-    'debug.record_transaction_failure': True,
+    "transaction_tracer.explain_threshold": 0.0,
+    "transaction_tracer.transaction_threshold": 0.0,
+    "transaction_tracer.stack_trace_threshold": 0.0,
+    "debug.log_data_collector_payloads": True,
+    "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (framework_falcon)',
-        default_settings=_default_settings)
+    app_name="Python Agent Test (framework_graphql)",
+    default_settings=_default_settings,
+)
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def app():
     from _target_application import _target_application
+
     return _target_application
+
+
+if six.PY2:
+    collect_ignore = ["test_application_async.py"]
```

### Comparing `newrelic-8.8.0/tests/framework_falcon/test_application.py` & `newrelic-8.8.1/tests/framework_falcon/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_fastapi/_target_application.py` & `newrelic-8.8.1/tests/framework_fastapi/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_fastapi/conftest.py` & `newrelic-8.8.1/tests/framework_fastapi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_fastapi/test_application.py` & `newrelic-8.8.1/tests/framework_fastapi/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/_test_application.py` & `newrelic-8.8.1/tests/framework_flask/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/_test_application_async.py` & `newrelic-8.8.1/tests/framework_flask/_test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/_test_blueprints.py` & `newrelic-8.8.1/tests/framework_flask/_test_blueprints.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/_test_compress.py` & `newrelic-8.8.1/tests/framework_flask/_test_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/_test_middleware.py` & `newrelic-8.8.1/tests/framework_flask/_test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/_test_not_found.py` & `newrelic-8.8.1/tests/framework_flask/_test_not_found.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/_test_user_exceptions.py` & `newrelic-8.8.1/tests/framework_flask/_test_user_exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/_test_views.py` & `newrelic-8.8.1/tests/framework_flask/_test_views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/_test_views_async.py` & `newrelic-8.8.1/tests/framework_flask/_test_views_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/conftest.py` & `newrelic-8.8.1/tests/framework_flask/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/test_application.py` & `newrelic-8.8.1/tests/framework_flask/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/test_blueprints.py` & `newrelic-8.8.1/tests/framework_flask/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/test_compress.py` & `newrelic-8.8.1/tests/framework_flask/test_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/test_middleware.py` & `newrelic-8.8.1/tests/framework_flask/test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/test_not_found.py` & `newrelic-8.8.1/tests/framework_flask/test_not_found.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/test_user_exceptions.py` & `newrelic-8.8.1/tests/framework_flask/test_user_exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_flask/test_views.py` & `newrelic-8.8.1/tests/framework_flask/test_views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_graphene/_target_application.py` & `newrelic-8.8.1/tests/framework_graphene/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_graphene/conftest.py` & `newrelic-8.8.1/tests/framework_graphene/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_graphene/test_application.py` & `newrelic-8.8.1/tests/framework_graphene/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_graphql/_target_application.py` & `newrelic-8.8.1/tests/framework_graphql/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_graphql/conftest.py` & `newrelic-8.8.1/tests/framework_strawberry/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "transaction_tracer.transaction_threshold": 0.0,
     "transaction_tracer.stack_trace_threshold": 0.0,
     "debug.log_data_collector_payloads": True,
     "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-    app_name="Python Agent Test (framework_graphql)",
+    app_name="Python Agent Test (framework_strawberry)",
     default_settings=_default_settings,
 )
 
 
 @pytest.fixture(scope="session")
 def app():
     from _target_application import _target_application
```

### Comparing `newrelic-8.8.0/tests/framework_graphql/test_application.py` & `newrelic-8.8.1/tests/framework_graphql/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_graphql/test_application_async.py` & `newrelic-8.8.1/tests/framework_graphql/test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_grpc/_test_common.py` & `newrelic-8.8.1/tests/framework_grpc/_test_common.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_grpc/conftest.py` & `newrelic-8.8.1/tests/framework_grpc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_grpc/sample_application/__init__.py` & `newrelic-8.8.1/tests/framework_grpc/sample_application/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_grpc/sample_application/sample_application.proto` & `newrelic-8.8.1/tests/framework_grpc/sample_application/sample_application.proto`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_grpc/test_clients.py` & `newrelic-8.8.1/tests/framework_grpc/test_clients.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_grpc/test_distributed_tracing.py` & `newrelic-8.8.1/tests/framework_grpc/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_grpc/test_get_url.py` & `newrelic-8.8.1/tests/framework_grpc/test_get_url.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_grpc/test_server.py` & `newrelic-8.8.1/tests/framework_grpc/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_pyramid/_test_append_slash_app.py` & `newrelic-8.8.1/tests/framework_pyramid/_test_append_slash_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_pyramid/_test_application.py` & `newrelic-8.8.1/tests/framework_pyramid/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_pyramid/conftest.py` & `newrelic-8.8.1/tests/framework_starlette/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
-
 from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
 
 
 _default_settings = {
-    'transaction_tracer.explain_threshold': 0.0,
-    'transaction_tracer.transaction_threshold': 0.0,
-    'transaction_tracer.stack_trace_threshold': 0.0,
-    'debug.log_data_collector_payloads': True,
-    'debug.record_transaction_failure': True,
+    "transaction_tracer.explain_threshold": 0.0,
+    "transaction_tracer.transaction_threshold": 0.0,
+    "transaction_tracer.stack_trace_threshold": 0.0,
+    "debug.log_data_collector_payloads": True,
+    "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (framework_pyramid)',
-        default_settings=_default_settings)
+    app_name="Python Agent Test (framework_starlette)",
+    default_settings=_default_settings,
+)
```

### Comparing `newrelic-8.8.0/tests/framework_pyramid/test_append_slash_app.py` & `newrelic-8.8.1/tests/framework_pyramid/test_append_slash_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_pyramid/test_application.py` & `newrelic-8.8.1/tests/framework_pyramid/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_pyramid/test_cornice.py` & `newrelic-8.8.1/tests/framework_pyramid/test_cornice.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_sanic/_target_application.py` & `newrelic-8.8.1/tests/framework_sanic/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_sanic/conftest.py` & `newrelic-8.8.1/tests/framework_sanic/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_sanic/test_application.py` & `newrelic-8.8.1/tests/framework_sanic/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_sanic/test_cross_application.py` & `newrelic-8.8.1/tests/framework_sanic/test_cross_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_starlette/_test_application.py` & `newrelic-8.8.1/tests/framework_starlette/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_starlette/_test_bg_tasks.py` & `newrelic-8.8.1/tests/framework_starlette/_test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_starlette/_test_graphql.py` & `newrelic-8.8.1/tests/framework_starlette/_test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_starlette/conftest.py` & `newrelic-8.8.1/tests/template_genshi/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
-
+from testing_support.fixtures import (  # noqa: F401; pylint: disable=W0611
+    collector_agent_registration_fixture,
+    collector_available_fixture,
+)
 
 _default_settings = {
     "transaction_tracer.explain_threshold": 0.0,
     "transaction_tracer.transaction_threshold": 0.0,
     "transaction_tracer.stack_trace_threshold": 0.0,
     "debug.log_data_collector_payloads": True,
     "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-    app_name="Python Agent Test (framework_starlette)",
-    default_settings=_default_settings,
+    app_name="Python Agent Test (template_genshi)", default_settings=_default_settings
 )
```

### Comparing `newrelic-8.8.0/tests/framework_starlette/test_application.py` & `newrelic-8.8.1/tests/framework_starlette/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_starlette/test_bg_tasks.py` & `newrelic-8.8.1/tests/framework_starlette/test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_starlette/test_graphql.py` & `newrelic-8.8.1/tests/framework_starlette/test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_strawberry/_target_application.py` & `newrelic-8.8.1/tests/framework_strawberry/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_strawberry/conftest.py` & `newrelic-8.8.1/tests/adapter_waitress/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,35 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-import six
-
-from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
-
+import webtest
+from testing_support.fixtures import (  # noqa: F401; pylint: disable=W0611
+    collector_agent_registration_fixture,
+    collector_available_fixture,
+)
 
 _default_settings = {
     "transaction_tracer.explain_threshold": 0.0,
     "transaction_tracer.transaction_threshold": 0.0,
     "transaction_tracer.stack_trace_threshold": 0.0,
     "debug.log_data_collector_payloads": True,
     "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-    app_name="Python Agent Test (framework_strawberry)",
-    default_settings=_default_settings,
+    app_name="Python Agent Test (Waitress)", default_settings=_default_settings
 )
 
 
-@pytest.fixture(scope="session")
-def app():
-    from _target_application import _target_application
-
-    return _target_application
-
+@pytest.fixture(autouse=True, scope="session")
+def target_application():
+    import _application
 
-if six.PY2:
-    collect_ignore = ["test_application_async.py"]
+    port = _application.setup_application()
+    return webtest.TestApp("http://localhost:%d" % port)
```

### Comparing `newrelic-8.8.0/tests/framework_strawberry/test_application.py` & `newrelic-8.8.1/tests/framework_strawberry/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_strawberry/test_application_async.py` & `newrelic-8.8.1/tests/framework_strawberry/test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_strawberry/test_asgi.py` & `newrelic-8.8.1/tests/framework_strawberry/test_asgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_tornado/_target_application.py` & `newrelic-8.8.1/tests/framework_tornado/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_tornado/conftest.py` & `newrelic-8.8.1/tests/framework_tornado/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_tornado/test_custom_handler.py` & `newrelic-8.8.1/tests/framework_tornado/test_custom_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_tornado/test_externals.py` & `newrelic-8.8.1/tests/framework_tornado/test_externals.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_tornado/test_inbound_cat.py` & `newrelic-8.8.1/tests/framework_tornado/test_inbound_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/framework_tornado/test_server.py` & `newrelic-8.8.1/tests/framework_tornado/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_logging/conftest.py` & `newrelic-8.8.1/tests/logger_logging/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_logging/test_local_decorating.py` & `newrelic-8.8.1/tests/logger_logging/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_logging/test_log_forwarding.py` & `newrelic-8.8.1/tests/logger_logging/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_logging/test_logging_handler.py` & `newrelic-8.8.1/tests/logger_logging/test_logging_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_logging/test_metrics.py` & `newrelic-8.8.1/tests/logger_logging/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_logging/test_settings.py` & `newrelic-8.8.1/tests/logger_logging/test_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_loguru/conftest.py` & `newrelic-8.8.1/tests/logger_loguru/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_loguru/test_local_decorating.py` & `newrelic-8.8.1/tests/logger_loguru/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_loguru/test_log_forwarding.py` & `newrelic-8.8.1/tests/logger_loguru/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_loguru/test_metrics.py` & `newrelic-8.8.1/tests/logger_loguru/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_loguru/test_settings.py` & `newrelic-8.8.1/tests/logger_loguru/test_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/logger_loguru/test_stack_inspection.py` & `newrelic-8.8.1/tests/logger_loguru/test_stack_inspection.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_confluentkafka/conftest.py` & `newrelic-8.8.1/tests/messagebroker_confluentkafka/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_confluentkafka/test_consumer.py` & `newrelic-8.8.1/tests/messagebroker_confluentkafka/test_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 from conftest import cache_kafka_consumer_headers
-from testing_support.fixtures import (
-    reset_core_stats_engine,
-    validate_attributes,
-    validate_error_event_attributes_outside_transaction,
-)
+from testing_support.fixtures import reset_core_stats_engine, validate_attributes
 from testing_support.validators.validate_distributed_trace_accepted import (
     validate_distributed_trace_accepted,
 )
+from testing_support.validators.validate_error_event_attributes_outside_transaction import (
+    validate_error_event_attributes_outside_transaction,
+)
 from testing_support.validators.validate_transaction_count import (
     validate_transaction_count,
 )
 from testing_support.validators.validate_transaction_errors import (
     validate_transaction_errors,
 )
 from testing_support.validators.validate_transaction_metrics import (
```

### Comparing `newrelic-8.8.0/tests/messagebroker_confluentkafka/test_producer.py` & `newrelic-8.8.1/tests/messagebroker_confluentkafka/test_producer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_confluentkafka/test_serialization.py` & `newrelic-8.8.1/tests/messagebroker_confluentkafka/test_serialization.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_kafkapython/conftest.py` & `newrelic-8.8.1/tests/messagebroker_kafkapython/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_kafkapython/test_consumer.py` & `newrelic-8.8.1/tests/messagebroker_kafkapython/test_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 from conftest import cache_kafka_consumer_headers
-from testing_support.fixtures import (
-    reset_core_stats_engine,
-    validate_attributes,
-    validate_error_event_attributes_outside_transaction,
-)
+from testing_support.fixtures import reset_core_stats_engine, validate_attributes
 from testing_support.validators.validate_distributed_trace_accepted import (
     validate_distributed_trace_accepted,
 )
+from testing_support.validators.validate_error_event_attributes_outside_transaction import (
+    validate_error_event_attributes_outside_transaction,
+)
 from testing_support.validators.validate_transaction_count import (
     validate_transaction_count,
 )
 from testing_support.validators.validate_transaction_errors import (
     validate_transaction_errors,
 )
 from testing_support.validators.validate_transaction_metrics import (
```

### Comparing `newrelic-8.8.0/tests/messagebroker_kafkapython/test_heartbeat.py` & `newrelic-8.8.1/tests/messagebroker_kafkapython/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_kafkapython/test_producer.py` & `newrelic-8.8.1/tests/messagebroker_kafkapython/test_producer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_kafkapython/test_serialization.py` & `newrelic-8.8.1/tests/messagebroker_kafkapython/test_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 
 import pytest
-from testing_support.fixtures import (
-    reset_core_stats_engine,
+from testing_support.fixtures import reset_core_stats_engine
+from testing_support.validators.validate_error_event_attributes_outside_transaction import (
     validate_error_event_attributes_outside_transaction,
 )
 from testing_support.validators.validate_transaction_errors import (
     validate_transaction_errors,
 )
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
```

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/compat.py` & `newrelic-8.8.1/tests/messagebroker_pika/compat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/conftest.py` & `newrelic-8.8.1/tests/messagebroker_pika/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/minversion.py` & `newrelic-8.8.1/tests/messagebroker_pika/minversion.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/test_cat.py` & `newrelic-8.8.1/tests/messagebroker_pika/test_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/test_distributed_tracing.py` & `newrelic-8.8.1/tests/messagebroker_pika/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/test_memory_leak.py` & `newrelic-8.8.1/tests/messagebroker_pika/test_memory_leak.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/test_pika_async_connection_consume.py` & `newrelic-8.8.1/tests/messagebroker_pika/test_pika_async_connection_consume.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py` & `newrelic-8.8.1/tests/messagebroker_pika/test_pika_blocking_connection_consume.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py` & `newrelic-8.8.1/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/test_pika_produce.py` & `newrelic-8.8.1/tests/messagebroker_pika/test_pika_produce.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/messagebroker_pika/test_pika_supportability.py` & `newrelic-8.8.1/tests/messagebroker_pika/test_pika_supportability.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/template_mako/conftest.py` & `newrelic-8.8.1/tests/datastore_pyodbc/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,21 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
+from testing_support.fixtures import (  # noqa: F401; pylint: disable=W0611
+    collector_agent_registration_fixture,
+    collector_available_fixture,
+)
 
 _default_settings = {
-    'transaction_tracer.explain_threshold': 0.0,
-    'transaction_tracer.transaction_threshold': 0.0,
-    'transaction_tracer.stack_trace_threshold': 0.0,
-    'debug.log_data_collector_payloads': True,
-    'debug.record_transaction_failure': True,
+    "transaction_tracer.explain_threshold": 0.0,
+    "transaction_tracer.transaction_threshold": 0.0,
+    "transaction_tracer.stack_trace_threshold": 0.0,
+    "debug.log_data_collector_payloads": True,
+    "debug.record_transaction_failure": True,
+    "debug.log_explain_plan_queries": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (template_mako)',
-        default_settings=_default_settings)
-
+    app_name="Python Agent Test (datastore_pyodbc)",
+    default_settings=_default_settings,
+    linked_applications=["Python Agent Test (datastore)"],
+)
```

### Comparing `newrelic-8.8.0/tests/template_mako/test_mako.py` & `newrelic-8.8.1/tests/template_mako/test_mako.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from mako.template import Template
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
+
 from newrelic.api.background_task import background_task
 
 
 @validate_transaction_metrics(
-    'test_render',
+    "test_render",
     background_task=True,
-    scoped_metrics=(('Template/Render/<template>', 1),),
+    scoped_metrics=(("Template/Render/<template>", 1),),
 )
-@background_task(name='test_render')
+@background_task(name="test_render")
 def test_render():
     template = Template("hello, ${name}!")
     result = template.render(name="NR")
     assert result == "hello, NR!"
+
+
+def test_render_outside_txn():
+    template = Template("hello, ${name}!")
+    result = template.render(name="NR")
+    assert result == "hello, NR!"
```

### Comparing `newrelic-8.8.0/tests/testing_support/__init__.py` & `newrelic-8.8.1/tests/testing_support/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/asgi_testing.py` & `newrelic-8.8.1/tests/testing_support/asgi_testing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/db_settings.py` & `newrelic-8.8.1/tests/testing_support/db_settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,33 +25,23 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
-    if "GITHUB_ACTIONS" in os.environ:
-        instances = 2
-
-        user = password = db = "postgres"
-        base_port = 8080
-    else:
-        instances = 1
-
-        user = db = USER
-        password = ""
-        base_port = 5432
-
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "localhost"
+    instances = 2
     settings = [
         {
-            "user": user,
-            "password": password,
-            "name": db,
-            "host": "localhost",
-            "port": base_port + instance_num,
+            "user": "postgres",
+            "password": "postgres",
+            "name": "postgres",
+            "host": host,
+            "port": 8080 + instance_num,
             "table_name": "postgres_table_" + str(os.getpid()),
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
@@ -62,33 +52,23 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
-    if "GITHUB_ACTIONS" in os.environ:
-        instances = 2
-
-        user = password = db = "python_agent"
-        base_port = 8080
-    else:
-        instances = 1
-
-        user = db = USER
-        password = ""
-        base_port = 3306
-
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "127.0.0.1"
+    instances = 1
     settings = [
         {
-            "user": user,
-            "password": password,
-            "name": db,
-            "host": "127.0.0.1",
-            "port": base_port + instance_num,
+            "user": "python_agent",
+            "password": "python_agent",
+            "name": "python_agent",
+            "host": host,
+            "port": 8080 + instance_num,
             "namespace": str(os.getpid()),
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
@@ -99,25 +79,20 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
-    if "GITHUB_ACTIONS" in os.environ:
-        instances = 2
-        base_port = 8080
-    else:
-        instances = 1
-        base_port = 6379
-
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "localhost"
+    instances = 2
     settings = [
         {
-            "host": "localhost",
-            "port": base_port + instance_num,
+            "host": host,
+            "port": 8080 + instance_num,
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
 def memcached_settings():
@@ -127,25 +102,20 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
-    if "GITHUB_ACTIONS" in os.environ:
-        instances = 2
-        base_port = 8080
-    else:
-        instances = 1
-        base_port = 11211
-
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "127.0.0.1"
+    instances = 2
     settings = [
         {
-            "host": "127.0.0.1",
-            "port": base_port + instance_num,
+            "host": host,
+            "port": 8080 + instance_num,
             "namespace": str(os.getpid()),
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
@@ -156,23 +126,18 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
-    if "GITHUB_ACTIONS" in os.environ:
-        instances = 2
-        base_port = 8080
-    else:
-        instances = 1
-        base_port = 27017
-
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "127.0.0.1"
+    instances = 2
     settings = [
-        {"host": "127.0.0.1", "port": base_port + instance_num, "collection": "mongodb_collection_" + str(os.getpid())}
+        {"host": host, "port": 8080 + instance_num, "collection": "mongodb_collection_" + str(os.getpid())}
         for instance_num in range(instances)
     ]
     return settings
 
 
 def elasticsearch_settings():
     """Return a list of dict of settings for connecting to elasticsearch.
@@ -181,25 +146,20 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
-    if "GITHUB_ACTIONS" in os.environ:
-        instances = 2
-        base_port = 8080
-    else:
-        instances = 1
-        base_port = 9200
-
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "localhost"
+    instances = 2
     settings = [
         {
-            "host": "localhost",
-            "port": str(base_port + instance_num),
+            "host": host,
+            "port": str(8080 + instance_num),
             "namespace": str(os.getpid()),
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
@@ -210,25 +170,20 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
-    if "GITHUB_ACTIONS" in os.environ:
-        instances = 2
-        base_port = 8080
-    else:
-        instances = 1
-        base_port = 8983
-
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "127.0.0.1"
+    instances = 2
     settings = [
         {
-            "host": "127.0.0.1",
-            "port": base_port + instance_num,
+            "host": host,
+            "port": 8080 + instance_num,
             "namespace": str(os.getpid()),
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
@@ -239,21 +194,20 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "localhost"
     instances = 1
-    base_port = 5672
-
     settings = [
         {
-            "host": "localhost",
-            "port": base_port + instance_num,
+            "host": host,
+            "port": 5672 + instance_num,
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
 def kafka_settings():
@@ -263,22 +217,40 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
-    if "GITHUB_ACTIONS" in os.environ:
-        instances = 2
-        base_port = 8080
-    else:
-        instances = 1
-        base_port = 9092
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "localhost"
+    instances = 2
+    settings = [
+        {
+            "host": host,
+            "port": 8080 + instance_num,
+        }
+        for instance_num in range(instances)
+    ]
+    return settings
+
+
+def gearman_settings():
+    """Return a list of dict of settings for connecting to kafka.
+
+    Will return the correct settings, depending on which of the environments it
+    is running in. It attempts to set variables in the following order, where
+    later environments override earlier ones.
 
+        1. Local
+        2. Github Actions
+    """
+
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "localhost"
+    instances = 1
     settings = [
         {
-            "host": "localhost",
-            "port": base_port + instance_num,
+            "host": host,
+            "port": 8080 + instance_num,
         }
         for instance_num in range(instances)
     ]
     return settings
```

### Comparing `newrelic-8.8.0/tests/testing_support/external_fixtures.py` & `newrelic-8.8.1/tests/testing_support/external_fixtures.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/fixture/__init__.py` & `newrelic-8.8.1/tests/testing_support/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/fixture/event_loop.py` & `newrelic-8.8.1/tests/testing_support/fixture/event_loop.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/fixtures.py` & `newrelic-8.8.1/tests/testing_support/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,21 +36,15 @@
 from newrelic.admin.record_deploy import record_deploy
 from newrelic.api.application import (
     application_instance,
     application_settings,
     register_application,
 )
 from newrelic.common.agent_http import DeveloperModeClient
-from newrelic.common.encoding_utils import (
-    deobfuscate,
-    json_decode,
-    json_encode,
-    obfuscate,
-    unpack_field,
-)
+from newrelic.common.encoding_utils import json_encode, obfuscate
 from newrelic.common.object_names import callable_name
 from newrelic.common.object_wrapper import (
     ObjectProxy,
     function_wrapper,
     transient_function_wrapper,
     wrap_function_wrapper,
 )
@@ -59,18 +53,14 @@
 from newrelic.core.attribute import create_attributes
 from newrelic.core.attribute_filter import (
     DST_ERROR_COLLECTOR,
     DST_TRANSACTION_TRACER,
     AttributeFilter,
 )
 from newrelic.core.config import apply_config_setting, flatten_settings, global_settings
-from newrelic.core.database_utils import SQLConnections
-
-# from newrelic.core.internal_metrics import InternalTraceContext
-# from newrelic.core.stats_engine import CustomMetrics
 from newrelic.network.exceptions import RetryDataForRequest
 from newrelic.packages import six
 
 _logger = logging.getLogger("newrelic.tests")
 
 
 def _environ_as_bool(name, default=False):
@@ -430,391 +420,14 @@
             assert agent_attributes[param] == value, ((param, value), agent_attributes)
         for param, value in exact_attrs["user"].items():
             assert user_attributes[param] == value, ((param, value), user_attributes)
         for param, value in exact_attrs["intrinsic"].items():
             assert intrinsics[param] == value, ((param, value), intrinsics)
 
 
-def check_error_attributes(
-    parameters, required_params=None, forgone_params=None, exact_attrs=None, is_transaction=True
-):
-    required_params = required_params or {}
-    forgone_params = forgone_params or {}
-    exact_attrs = exact_attrs or {}
-
-    parameter_fields = ["userAttributes"]
-    if is_transaction:
-        parameter_fields.extend(["stack_trace", "agentAttributes", "intrinsics"])
-
-    for field in parameter_fields:
-        assert field in parameters
-
-    # we can remove this after agent attributes transition is all over
-    assert "parameter_groups" not in parameters
-    assert "custom_params" not in parameters
-    assert "request_params" not in parameters
-    assert "request_uri" not in parameters
-
-    check_attributes(parameters, required_params, forgone_params, exact_attrs)
-
-
-def check_attributes(parameters, required_params=None, forgone_params=None, exact_attrs=None):
-    required_params = required_params or {}
-    forgone_params = forgone_params or {}
-    exact_attrs = exact_attrs or {}
-
-    intrinsics = parameters.get("intrinsics", {})
-    user_attributes = parameters.get("userAttributes", {})
-    agent_attributes = parameters.get("agentAttributes", {})
-
-    if required_params:
-        for param in required_params["agent"]:
-            assert param in agent_attributes, (param, agent_attributes)
-        for param in required_params["user"]:
-            assert param in user_attributes, (param, user_attributes)
-        for param in required_params["intrinsic"]:
-            assert param in intrinsics, (param, intrinsics)
-
-    if forgone_params:
-        for param in forgone_params["agent"]:
-            assert param not in agent_attributes, (param, agent_attributes)
-        for param in forgone_params["user"]:
-            assert param not in user_attributes, (param, user_attributes)
-        for param in forgone_params["intrinsic"]:
-            assert param not in intrinsics, (param, intrinsics)
-
-    if exact_attrs:
-        for param, value in exact_attrs["agent"].items():
-            assert agent_attributes[param] == value, ((param, value), agent_attributes)
-        for param, value in exact_attrs["user"].items():
-            assert user_attributes[param] == value, ((param, value), user_attributes)
-        for param, value in exact_attrs["intrinsic"].items():
-            assert intrinsics[param] == value, ((param, value), intrinsics)
-
-
-def validate_custom_event_collector_json(num_events=1):
-    """Validate the format, types and number of custom events."""
-
-    @transient_function_wrapper("newrelic.core.application", "Application.record_transaction")
-    def _validate_custom_event_collector_json(wrapped, instance, args, kwargs):
-        try:
-            result = wrapped(*args, **kwargs)
-        except:
-            raise
-        else:
-            stats = instance._stats_engine
-            settings = stats.settings
-
-            agent_run_id = 666
-            sampling_info = stats.custom_events.sampling_info
-            samples = list(stats.custom_events)
-
-            # Emulate the payload used in data_collector.py
-
-            payload = (agent_run_id, sampling_info, samples)
-            collector_json = json_encode(payload)
-
-            decoded_json = json.loads(collector_json)
-
-            decoded_agent_run_id = decoded_json[0]
-            decoded_sampling_info = decoded_json[1]
-            decoded_events = decoded_json[2]
-
-            assert decoded_agent_run_id == agent_run_id
-            assert decoded_sampling_info == sampling_info
-
-            max_setting = settings.event_harvest_config.harvest_limits.custom_event_data
-            assert decoded_sampling_info["reservoir_size"] == max_setting
-
-            assert decoded_sampling_info["events_seen"] == num_events
-            assert len(decoded_events) == num_events
-
-            for intrinsics, attributes in decoded_events:
-                assert isinstance(intrinsics, dict)
-                assert isinstance(attributes, dict)
-
-        return result
-
-    return _validate_custom_event_collector_json
-
-
-def validate_tt_parameters(required_params=None, forgone_params=None):
-    required_params = required_params or {}
-    forgone_params = forgone_params or {}
-
-    @transient_function_wrapper("newrelic.core.stats_engine", "StatsEngine.record_transaction")
-    def _validate_tt_parameters(wrapped, instance, args, kwargs):
-        try:
-            result = wrapped(*args, **kwargs)
-        except:
-            raise
-        else:
-            # Now that transaction has been recorded, generate
-            # a transaction trace
-
-            connections = SQLConnections()
-            trace_data = instance.transaction_trace_data(connections)
-            pack_data = unpack_field(trace_data[0][4])
-            tt_intrinsics = pack_data[0][4]["intrinsics"]
-
-            for name in required_params:
-                assert name in tt_intrinsics, "name=%r, intrinsics=%r" % (name, tt_intrinsics)
-                assert tt_intrinsics[name] == required_params[name], "name=%r, value=%r, intrinsics=%r" % (
-                    name,
-                    required_params[name],
-                    tt_intrinsics,
-                )
-
-            for name in forgone_params:
-                assert name not in tt_intrinsics, "name=%r, intrinsics=%r" % (name, tt_intrinsics)
-
-        return result
-
-    return _validate_tt_parameters
-
-
-def validate_tt_segment_params(forgone_params=(), present_params=(), exact_params=None):
-    exact_params = exact_params or {}
-    recorded_traces = []
-
-    @transient_function_wrapper("newrelic.core.stats_engine", "StatsEngine.record_transaction")
-    def _extract_trace(wrapped, instance, args, kwargs):
-        result = wrapped(*args, **kwargs)
-
-        # Now that transaction has been recorded, generate
-        # a transaction trace
-
-        connections = SQLConnections()
-        trace_data = instance.transaction_trace_data(connections)
-        # Save the recorded traces
-        recorded_traces.extend(trace_data)
-
-        return result
-
-    @function_wrapper
-    def validator(wrapped, instance, args, kwargs):
-        new_wrapper = _extract_trace(wrapped)
-        result = new_wrapper(*args, **kwargs)
-
-        # Verify that traces have been recorded
-        assert recorded_traces
-
-        # Extract the first transaction trace
-        transaction_trace = recorded_traces[0]
-        pack_data = unpack_field(transaction_trace[4])
-
-        # Extract the root segment from the root node
-        root_segment = pack_data[0][3]
-
-        recorded_params = {}
-
-        def _validate_segment_params(segment):
-            segment_params = segment[3]
-
-            # Translate from the string cache
-            for key, value in segment_params.items():
-                if hasattr(value, "startswith") and value.startswith("`"):
-                    try:
-                        index = int(value[1:])
-                        value = pack_data[1][index]
-                    except ValueError:
-                        pass
-                segment_params[key] = value
-
-            recorded_params.update(segment_params)
-
-            for child_segment in segment[4]:
-                _validate_segment_params(child_segment)
-
-        _validate_segment_params(root_segment)
-
-        recorded_params_set = set(recorded_params.keys())
-
-        # Verify that the params in present params have been recorded
-        present_params_set = set(present_params)
-        assert recorded_params_set.issuperset(present_params_set)
-
-        # Verify that all forgone params are omitted
-        recorded_forgone_params = recorded_params_set & set(forgone_params)
-        assert not recorded_forgone_params
-
-        # Verify that all exact params are correct
-        for key, value in exact_params.items():
-            assert recorded_params[key] == value
-
-        return result
-
-    return validator
-
-
-def validate_browser_attributes(required_params=None, forgone_params=None):
-    required_params = required_params or {}
-    forgone_params = forgone_params or {}
-
-    @transient_function_wrapper("newrelic.api.web_transaction", "WSGIWebTransaction.browser_timing_footer")
-    def _validate_browser_attributes(wrapped, instance, args, kwargs):
-        try:
-            result = wrapped(*args, **kwargs)
-        except:
-            raise
-
-        # pick out attributes from footer string_types
-
-        footer_data = result.split("NREUM.info=")[1]
-        footer_data = footer_data.split("</script>")[0]
-        footer_data = json.loads(footer_data)
-
-        if "intrinsic" in required_params:
-            for attr in required_params["intrinsic"]:
-                assert attr in footer_data
-
-        if "atts" in footer_data:
-            obfuscation_key = instance._settings.license_key[:13]
-            attributes = json_decode(deobfuscate(footer_data["atts"], obfuscation_key))
-        else:
-            # if there are no user or agent attributes, there will be no dict
-            # for them in the browser data
-
-            attributes = None
-
-        if "user" in required_params:
-            for attr in required_params["user"]:
-                assert attr in attributes["u"]
-
-        if "agent" in required_params:
-            for attr in required_params["agent"]:
-                assert attr in attributes["a"]
-
-        if "user" in forgone_params:
-            if attributes:
-                if "u" in attributes:
-                    for attr in forgone_params["user"]:
-                        assert attr not in attributes["u"]
-
-        if "agent" in forgone_params:
-            if attributes:
-                if "a" in attributes:
-                    for attr in forgone_params["agent"]:
-                        assert attr not in attributes["a"]
-
-        return result
-
-    return _validate_browser_attributes
-
-
-def validate_error_event_attributes(required_params=None, forgone_params=None, exact_attrs=None):
-    """Check the error event for attributes, expect only one error to be
-    present in the transaction.
-    """
-    required_params = required_params or {}
-    forgone_params = forgone_params or {}
-    exact_attrs = exact_attrs or {}
-    error_data_samples = []
-
-    @function_wrapper
-    def _validate_wrapper(wrapped, instance, args, kwargs):
-        @transient_function_wrapper("newrelic.core.stats_engine", "StatsEngine.record_transaction")
-        def _validate_error_event_attributes(wrapped, instance, args, kwargs):
-            try:
-                result = wrapped(*args, **kwargs)
-            except:
-                raise
-            else:
-                event_data = instance.error_events
-                for sample in event_data:
-                    error_data_samples.append(sample)
-
-                check_event_attributes(event_data, required_params, forgone_params, exact_attrs)
-
-            return result
-
-        _new_wrapper = _validate_error_event_attributes(wrapped)
-        val = _new_wrapper(*args, **kwargs)
-        assert error_data_samples
-        return val
-
-    return _validate_wrapper
-
-
-def validate_error_trace_attributes_outside_transaction(
-    err_name, required_params=None, forgone_params=None, exact_attrs=None
-):
-    required_params = required_params or {}
-    forgone_params = forgone_params or {}
-    exact_attrs = exact_attrs or {}
-
-    target_error = []
-
-    @transient_function_wrapper("newrelic.core.stats_engine", "StatsEngine.notice_error")
-    def _validate_error_trace_attributes_outside_transaction(wrapped, instance, args, kwargs):
-        try:
-            result = wrapped(*args, **kwargs)
-        except:
-            raise
-        else:
-            target_error.append(core_application_stats_engine_error(err_name))
-
-        return result
-
-
-    @function_wrapper
-    def _validator_wrapper(wrapped, instance, args, kwargs):
-        result = _validate_error_trace_attributes_outside_transaction(wrapped)(*args, **kwargs)
-
-        assert target_error and target_error[0] is not None, "No error found with name %s" % err_name
-        check_error_attributes(target_error[0].parameters, required_params, forgone_params, exact_attrs)
-
-        return result
-
-
-    return _validator_wrapper
-
-
-def validate_error_event_attributes_outside_transaction(
-    required_params=None, forgone_params=None, exact_attrs=None, num_errors=None
-):
-    required_params = required_params or {}
-    forgone_params = forgone_params or {}
-
-    event_data = []
-
-    @transient_function_wrapper("newrelic.core.stats_engine", "StatsEngine.notice_error")
-    def _validate_error_event_attributes_outside_transaction(wrapped, instance, args, kwargs):
-        try:
-            result = wrapped(*args, **kwargs)
-        except:
-            raise
-        else:
-            for event in instance.error_events:
-                event_data.append(event)
-
-        return result
-
-    @function_wrapper
-    def wrapper(wrapped, instance, args, kwargs):
-        try:
-            result = _validate_error_event_attributes_outside_transaction(wrapped)(*args, **kwargs)
-        except:
-            raise
-        else:
-            if num_errors is not None:
-                exc_message = (
-                    "Expected: %d, Got: %d. Verify StatsEngine is being reset before using this validator."
-                    % (num_errors, len(event_data))
-                )
-                assert num_errors == len(event_data), exc_message
-
-            for event in event_data:
-                check_event_attributes([event], required_params, forgone_params, exact_attrs=exact_attrs)
-
-        return result
-
-    return wrapper
-
-
 def validate_request_params_omitted():
     @transient_function_wrapper("newrelic.core.stats_engine", "StatsEngine.record_transaction")
     def _validate_request_params(wrapped, instance, args, kwargs):
         def _bind_params(transaction, *args, **kwargs):
             return transaction
 
         transaction = _bind_params(*args, **kwargs)
@@ -1709,14 +1322,71 @@
                 raise raises()
 
         return wrapped(*args, **kwargs)
 
     return send_request_wrapper
 
 
+def check_attributes(parameters, required_params=None, forgone_params=None, exact_attrs=None):
+    required_params = required_params or {}
+    forgone_params = forgone_params or {}
+    exact_attrs = exact_attrs or {}
+
+    intrinsics = parameters.get("intrinsics", {})
+    user_attributes = parameters.get("userAttributes", {})
+    agent_attributes = parameters.get("agentAttributes", {})
+
+    if required_params:
+        for param in required_params["agent"]:
+            assert param in agent_attributes, (param, agent_attributes)
+        for param in required_params["user"]:
+            assert param in user_attributes, (param, user_attributes)
+        for param in required_params["intrinsic"]:
+            assert param in intrinsics, (param, intrinsics)
+
+    if forgone_params:
+        for param in forgone_params["agent"]:
+            assert param not in agent_attributes, (param, agent_attributes)
+        for param in forgone_params["user"]:
+            assert param not in user_attributes, (param, user_attributes)
+        for param in forgone_params["intrinsic"]:
+            assert param not in intrinsics, (param, intrinsics)
+
+    if exact_attrs:
+        for param, value in exact_attrs["agent"].items():
+            assert agent_attributes[param] == value, ((param, value), agent_attributes)
+        for param, value in exact_attrs["user"].items():
+            assert user_attributes[param] == value, ((param, value), user_attributes)
+        for param, value in exact_attrs["intrinsic"].items():
+            assert intrinsics[param] == value, ((param, value), intrinsics)
+
+
+def check_error_attributes(
+    parameters, required_params=None, forgone_params=None, exact_attrs=None, is_transaction=True
+):
+    required_params = required_params or {}
+    forgone_params = forgone_params or {}
+    exact_attrs = exact_attrs or {}
+
+    parameter_fields = ["userAttributes"]
+    if is_transaction:
+        parameter_fields.extend(["stack_trace", "agentAttributes", "intrinsics"])
+
+    for field in parameter_fields:
+        assert field in parameters
+
+    # we can remove this after agent attributes transition is all over
+    assert "parameter_groups" not in parameters
+    assert "custom_params" not in parameters
+    assert "request_params" not in parameters
+    assert "request_uri" not in parameters
+
+    check_attributes(parameters, required_params, forgone_params, exact_attrs)
+
+
 class Environ(object):
     """Context manager for setting environment variables temporarily."""
 
     def __init__(self, **kwargs):
         self._original_environ = os.environ
         self._environ_dict = kwargs
```

### Comparing `newrelic-8.8.0/tests/testing_support/mock_external_grpc_server.py` & `newrelic-8.8.1/tests/testing_support/mock_external_grpc_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/mock_external_http_server.py` & `newrelic-8.8.1/tests/testing_support/mock_external_http_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/mock_http_client.py` & `newrelic-8.8.1/tests/testing_support/mock_http_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/sample_applications.py` & `newrelic-8.8.1/tests/testing_support/sample_applications.py`

 * *Files 20% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     use_user_attrs = environ.get("record_attributes", "TRUE") == "TRUE"
 
     environ["wsgi.input"].read()
     environ["wsgi.input"].readline()
     environ["wsgi.input"].readlines()
 
     if use_user_attrs:
-
         for attr, val in _custom_parameters.items():
             add_custom_attribute(attr, val)
 
     if "db" in environ and int(environ["db"]) > 0:
         connection = db.connect(":memory:")
         for i in range(int(environ["db"]) - 1):
             connection.execute("create table test_db%d (a, b, c)" % i)
@@ -93,15 +92,14 @@
             r = urlopen("http://www.python.org")  # nosec
             r.read(10)
 
     if "err_message" in environ:
         n_errors = int(environ.get("n_errors", 1))
         for i in range(n_errors):
             try:
-
                 # append number to stats engine to get unique errors, so they
                 # don't immediately get filtered out.
 
                 raise ValueError(environ["err_message"] + str(i))
             except ValueError:
                 if use_user_attrs:
                     notice_error(attributes=_err_param)
@@ -118,15 +116,14 @@
     write(b"")
 
     return [output]
 
 
 @wsgi_application()
 def simple_exceptional_app(environ, start_response):
-
     start_response("500 :(", [])
 
     raise ValueError("Transaction had bad value")
 
 
 def simple_app_raw(environ, start_response):
     status = "200 OK"
@@ -136,15 +133,53 @@
 
     return []
 
 
 simple_app = wsgi_application()(simple_app_raw)
 
 
+def raise_exception_application(environ, start_response):
+    raise RuntimeError("raise_exception_application")
+
+    status = "200 OK"
+    output = b"WSGI RESPONSE"
+
+    response_headers = [("Content-type", "text/plain"), ("Content-Length", str(len(output)))]
+    start_response(status, response_headers)
+
+    return [output]
+
+
+def raise_exception_response(environ, start_response):
+    status = "200 OK"
+
+    response_headers = [("Content-type", "text/plain")]
+    start_response(status, response_headers)
+
+    yield b"WSGI"
+
+    raise RuntimeError("raise_exception_response")
+
+    yield b" "
+    yield b"RESPONSE"
+
+
+def raise_exception_finalize(environ, start_response):
+    status = "200 OK"
+
+    response_headers = [("Content-type", "text/plain")]
+    start_response(status, response_headers)
+
+    try:
+        yield b"WSGI RESPONSE"
+
+    finally:
+        raise RuntimeError("raise_exception_finalize")
+
+
 @wsgi_application()
 def simple_custom_event_app(environ, start_response):
-
     params = {"snowman": "\u2603", "foo": "bar"}
     record_custom_event("SimpleAppEvent", params)
 
     start_response(status="200 OK", response_headers=[])
     return []
```

### Comparing `newrelic-8.8.0/tests/testing_support/sample_asgi_applications.py` & `newrelic-8.8.1/tests/testing_support/sample_asgi_applications.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/util.py` & `newrelic-8.8.1/tests/testing_support/util.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/__init__.py` & `newrelic-8.8.1/tests/testing_support/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_apdex_metrics.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_apdex_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_application_error_event_count.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_application_error_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_application_error_trace_count.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_application_error_trace_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_application_errors.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_application_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_code_level_metrics.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_cross_process_headers.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_cross_process_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_custom_parameters.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_custom_parameters.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_database_duration.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_database_duration.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_database_node.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_database_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_database_trace_inputs.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_database_trace_inputs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_datastore_trace_inputs.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_datastore_trace_inputs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_distributed_trace_accepted.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_distributed_trace_accepted.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_distributed_tracing_header.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_distributed_tracing_header.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_error_event_collector_json.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_error_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_error_trace_attributes.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_error_trace_collector_json.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_external_node_params.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_external_node_params.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_function_called.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_function_called.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_internal_metrics.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_internal_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_log_event_collector_json.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_log_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_log_event_count.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_log_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_log_event_count_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_log_events.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_log_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_log_events_outside_transaction.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_log_events_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_messagebroker_headers.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_messagebroker_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_metric_payload.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_metric_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_non_transaction_error_event.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_non_transaction_error_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_outbound_headers.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_outbound_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_serverless_data.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_serverless_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_serverless_metadata.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_serverless_metadata.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_serverless_payload.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_serverless_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_slow_sql_collector_json.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_slow_sql_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_span_events.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_sql_obfuscation.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_sql_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_synthetics_event.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_synthetics_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_synthetics_transaction_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_time_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_transaction_count.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_error_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_transaction_errors.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_transaction_event_attributes.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_event_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_transaction_event_collector_json.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_transaction_metrics.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_slow_sql_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_transaction_trace_attributes.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.0/tests/testing_support/validators/validate_tt_collector_json.py` & `newrelic-8.8.1/tests/testing_support/validators/validate_tt_collector_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 assert "exclusive_duration_millis" in params
                 assert isinstance(params["exclusive_duration_millis"], float)
 
                 segment_name = _lookup_string_table(node[2], string_table, default=node[2])
                 if segment_name.startswith("Datastore"):
                     for key in datastore_params:
                         assert key in params, key
-                        assert params[key] == datastore_params[key]
+                        assert params[key] == datastore_params[key], "Expected %s. Got %s." % (datastore_params[key], params[key])
                     for key in datastore_forgone_params:
                         assert key not in params, key
 
                     # if host is reported, it cannot be localhost
                     if "host" in params:
                         assert params["host"] not in LOCALHOST_EQUIVALENTS
```

### Comparing `newrelic-8.8.0/tox.ini` & `newrelic-8.8.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ;           framework_aiohttp: tests/framework_aiohttp
 ;        deps =
 ;           adapter_gunicorn-gunicornlatest: gunicorn
 ;           datastore_asyncpg: asyncpg
 ;           framework_aiohttp-aiohttp01: aiohttp<2
 ;           framework_aiohttp-aiohttp0202: aiohttp<2.3
 ; 3. Python version required. Uses the standard tox definitions. (https://tox.readthedocs.io/en/latest/config.html#tox-environments)
-;    Examples: py27,py37,py38,py39,pypy,pypy37
+;    Examples: py27,py37,py38,py39,pypy27,pypy37
 ; 4. Library and version (Optional). Used when testing multiple versions of the library, and may be omitted when only testing a single version.
 ;    Versions should be specified with 2 digits per version number, so <3 becomes 02 and <3.5 becomes 0304. latest and master are also acceptable versions.
 ;    Examples: uvicorn03, CherryPy0302, uvicornlatest
 ;       deps =
 ;           adapter_uvicorn-uvicorn03: uvicorn<0.4
 ;           adapter_uvicorn-uvicornlatest: uvicorn
 ;           framework_cherrypy-CherryPy0302: CherryPy<3.3.0
@@ -36,145 +36,147 @@
 ;
 ; Full Examples:
 ;   - memcached-datastore_bmemcached-py37-memcached030
 ;   - python-agent_unittests-py38-with_extensions
 ;   - python-adapter_gevent-py27
 
 [tox]
+requires = virtualenv<20.22.0
 setupdir = {toxinidir}
 envlist =
     python-adapter_cheroot-{py27,py37,py38,py39,py310,py311},
     python-adapter_daphne-{py37,py38,py39,py310,py311}-daphnelatest,
     python-adapter_daphne-py38-daphne{0204,0205},
     python-adapter_gevent-{py27,py37,py38,py310,py311},
     python-adapter_gunicorn-{py37,py38,py39,py310,py311}-aiohttp3-gunicornlatest,
     python-adapter_hypercorn-{py37,py38,py39,py310,py311}-hypercornlatest,
     python-adapter_hypercorn-py38-hypercorn{0010,0011,0012,0013},
     python-adapter_uvicorn-py37-uvicorn03,
     python-adapter_uvicorn-{py37,py38,py39,py310,py311}-uvicornlatest,
+    python-adapter_waitress-{py37,py38,py39}-waitress010404,
+    python-adapter_waitress-{py37,py38,py39,py310}-waitress02,
+    python-adapter_waitress-{py37,py38,py39,py310,py311}-waitresslatest,
     python-agent_features-{py27,py37,py38,py39,py310,py311}-{with,without}_extensions,
-    python-agent_features-{pypy,pypy37}-without_extensions,
+    python-agent_features-{pypy27,pypy37}-without_extensions,
     python-agent_streaming-py27-grpc0125-{with,without}_extensions,
     python-agent_streaming-{py37,py38,py39,py310,py311}-protobuf04-{with,without}_extensions,
     python-agent_streaming-py39-protobuf{03,0319}-{with,without}_extensions,
     python-agent_unittests-{py27,py37,py38,py39,py310,py311}-{with,without}_extensions,
-    python-agent_unittests-{pypy,pypy37}-without_extensions,
-    python-application_celery-{py27,py37,py38,py39,py310,py311,pypy,pypy37},
-    gearman-application_gearman-{py27,pypy},
+    python-agent_unittests-{pypy27,pypy37}-without_extensions,
+    python-application_celery-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    gearman-application_gearman-{py27,pypy27},
     python-component_djangorestframework-py27-djangorestframework0300,
     python-component_djangorestframework-{py37,py38,py39,py310,py311}-djangorestframeworklatest,
     python-component_flask_rest-{py37,py38,py39,pypy37}-flaskrestxlatest,
-    python-component_flask_rest-{py27,pypy}-flaskrestx051,
+    python-component_flask_rest-{py27,pypy27}-flaskrestx051,
     python-component_graphqlserver-{py37,py38,py39,py310,py311},
-    python-component_tastypie-{py27,pypy}-tastypie0143,
+    python-component_tastypie-{py27,pypy27}-tastypie0143,
     python-component_tastypie-{py37,py38,py39,pypy37}-tastypie{0143,latest},
     python-coroutines_asyncio-{py37,py38,py39,py310,py311,pypy37},
     python-cross_agent-{py27,py37,py38,py39,py310,py311}-{with,without}_extensions,
-    python-cross_agent-pypy-without_extensions,
+    python-cross_agent-pypy27-without_extensions,
     postgres-datastore_asyncpg-{py37,py38,py39,py310,py311},
-    memcached-datastore_bmemcached-{pypy,py27,py37,py38,py39,py310,py311}-memcached030,
-    elasticsearchserver07-datastore_elasticsearch-{py27,py37,py38,py39,py310,py311,pypy,pypy37}-elasticsearch07,
+    memcached-datastore_bmemcached-{pypy27,py27,py37,py38,py39,py310,py311}-memcached030,
+    elasticsearchserver07-datastore_elasticsearch-{py27,py37,py38,py39,py310,py311,pypy27,pypy37}-elasticsearch07,
     elasticsearchserver08-datastore_elasticsearch-{py37,py38,py39,py310,py311,pypy37}-elasticsearch08,
-    memcached-datastore_memcache-{py27,py37,py38,py39,py310,py311,pypy,pypy37}-memcached01,
+    memcached-datastore_memcache-{py27,py37,py38,py39,py310,py311,pypy27,pypy37}-memcached01,
     mysql-datastore_mysql-mysql080023-py27,
     mysql-datastore_mysql-mysqllatest-{py37,py38,py39,py310,py311},
     postgres-datastore_postgresql-{py37,py38,py39},
     postgres-datastore_psycopg2-{py27,py37,py38,py39,py310,py311}-psycopg2latest
-    postgres-datastore_psycopg2cffi-{py27,pypy,py37,py38,py39,py310,py311}-psycopg2cffilatest,
+    postgres-datastore_psycopg2cffi-{py27,pypy27,py37,py38,py39,py310,py311}-psycopg2cffilatest,
+    postgres-datastore_pyodbc-{py27,py37,py311}-pyodbclatest
     memcached-datastore_pylibmc-{py27,py37},
-    memcached-datastore_pymemcache-{py27,py37,py38,py39,py310,py311,pypy,pypy37},
-    mongodb-datastore_pymongo-{py27,py37,py38,py39,py310,py311,pypy}-pymongo{03},
-    mongodb-datastore_pymongo-{py37,py38,py39,py310,py311,pypy,pypy37}-pymongo04,
-    mysql-datastore_pymysql-{py27,py37,py38,py39,py310,py311,pypy,pypy37},
-    solr-datastore_pysolr-{py27,py37,py38,py39,py310,py311,pypy,pypy37},
-    redis-datastore_redis-{py27,py37,py38,pypy,pypy37}-redis03,
+    memcached-datastore_pymemcache-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    mongodb-datastore_pymongo-{py27,py37,py38,py39,py310,py311,pypy27}-pymongo{03},
+    mongodb-datastore_pymongo-{py37,py38,py39,py310,py311,pypy27,pypy37}-pymongo04,
+    mysql-datastore_pymysql-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    solr-datastore_pysolr-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    redis-datastore_redis-{py27,py37,py38,pypy27,pypy37}-redis03,
     redis-datastore_redis-{py37,py38,py39,py310,py311,pypy37}-redis{0400,latest},
     redis-datastore_aioredis-{py37,py38,py39,py310,pypy37}-aioredislatest,
-    redis-datastore_aioredis-{py37,py310}-aioredis01,
     redis-datastore_aioredis-{py37,py38,py39,py310,py311,pypy37}-redislatest,
     redis-datastore_aredis-{py37,py38,py39,pypy37}-aredislatest,
-    solr-datastore_solrpy-{py27,pypy}-solrpy{00,01},
-    python-datastore_sqlite-{py27,py37,py38,py39,py310,py311,pypy,pypy37},
-    memcached-datastore_umemcache-{py27,pypy},
+    solr-datastore_solrpy-{py27,pypy27}-solrpy{00,01},
+    python-datastore_sqlite-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
     python-external_boto3-{py27,py37,py38,py39,py310,py311}-boto01,
     python-external_botocore-{py37,py38,py39,py310,py311}-botocorelatest,
     python-external_botocore-{py311}-botocore128,
     python-external_botocore-py310-botocore0125,
     python-external_feedparser-py27-feedparser{05,06},
-    python-external_http-{py27,py37,py38,py39,py310,py311,pypy},
-    python-external_httplib-{py27,py37,py38,py39,py310,py311,pypy,pypy37},
-    python-external_httplib2-{py27,py37,py38,py39,py310,py311,pypy,pypy37},
+    python-external_http-{py27,py37,py38,py39,py310,py311,pypy27},
+    python-external_httplib-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    python-external_httplib2-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
     python-external_httpx-{py37,py38,py39,py310,py311},
-    python-external_requests-{py27,py37,py38,py39,py310,py311,pypy,pypy37},
-    python-external_urllib3-{py27,py37,pypy}-urllib3{0109},
-    python-external_urllib3-{py27,py37,py38,py39,py310,py311,pypy,pypy37}-urllib3latest,
+    python-external_requests-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    python-external_urllib3-{py27,py37,pypy27}-urllib3{0109},
+    python-external_urllib3-{py27,py37,py38,py39,py310,py311,pypy27,pypy37}-urllib3latest,
     python-framework_aiohttp-{py37,py38,py39,py310,py311,pypy37}-aiohttp03,
     python-framework_ariadne-{py37,py38,py39,py310,py311}-ariadnelatest,
     python-framework_ariadne-py37-ariadne{0011,0012,0013},
     python-framework_bottle-py27-bottle{0008,0009,0010},
     python-framework_bottle-{py27,py37,py38,py39,pypy37}-bottle{0011,0012},
     python-framework_bottle-{py310,py311}-bottle0012,
-    python-framework_bottle-pypy-bottle{0008,0009,0010,0011,0012},
+    python-framework_bottle-pypy27-bottle{0008,0009,0010,0011,0012},
     ; CherryPy still uses inspect.getargspec, deprecated in favor of inspect.getfullargspec.  Not supported in 3.11
-    python-framework_cherrypy-{py37,py38,py39,py310,pypy37}-CherryPy18,
-    python-framework_cherrypy-{py37}-CherryPy0302,
-    python-framework_cherrypy-pypy37-CherryPy0303,
-    python-framework_django-{pypy,py27}-Django0103,
-    python-framework_django-{pypy,py27,py37}-Django0108,
+    python-framework_cherrypy-{py37,py38,py39,py310,py311,pypy37}-CherryPylatest,
+    python-framework_django-{pypy27,py27}-Django0103,
+    python-framework_django-{pypy27,py27,py37}-Django0108,
     python-framework_django-{py39}-Django{0200,0201,0202,0300,0301,latest},
     python-framework_django-{py37,py38,py39,py310,py311}-Django0302,
-    python-framework_falcon-{py27,py37,py38,py39,pypy,pypy37}-falcon0103,
+    python-framework_falcon-{py27,py37,py38,py39,pypy27,pypy37}-falcon0103,
     python-framework_falcon-{py37,py38,py39,py310,pypy37}-falcon{0200,master},
     # Falcon master branch failing on 3.11 currently.
     python-framework_falcon-py311-falcon0200,
     python-framework_fastapi-{py37,py38,py39,py310,py311},
-    python-framework_flask-{pypy,py27}-flask0012,
-    python-framework_flask-{pypy,py27,py37,py38,py39,py310,py311,pypy37}-flask0101,
+    python-framework_flask-{pypy27,py27}-flask0012,
+    python-framework_flask-{pypy27,py27,py37,py38,py39,py310,py311,pypy37}-flask0101,
     ; temporarily disabling flaskmaster tests
     python-framework_flask-{py37,py38,py39,py310,py311,pypy37}-flask{latest},
     python-framework_graphene-{py37,py38,py39,py310,py311}-graphenelatest,
-    python-framework_graphene-{py27,py37,py38,py39,pypy,pypy37}-graphene{0200,0201},
+    python-framework_graphene-{py27,py37,py38,py39,pypy27,pypy37}-graphene{0200,0201},
     python-framework_graphene-{py310,py311}-graphene0201,
-    python-framework_graphql-{py27,py37,py38,py39,py310,py311,pypy,pypy37}-graphql02,
+    python-framework_graphql-{py27,py37,py38,py39,py310,py311,pypy27,pypy37}-graphql02,
     python-framework_graphql-{py37,py38,py39,py310,py311,pypy37}-graphql03,
     ; temporarily disabling graphqlmaster tests
     python-framework_graphql-py37-graphql{0202,0203,0300,0301,0302},
     grpc-framework_grpc-py27-grpc0125,
     grpc-framework_grpc-{py37,py38,py39,py310,py311}-grpclatest,
-    python-framework_pyramid-{pypy,py27,py38}-Pyramid0104,
-    python-framework_pyramid-{pypy,py27,pypy37,py37,py38,py39,py310,py311}-Pyramid0110-cornice,
+    python-framework_pyramid-{pypy27,py27,py38}-Pyramid0104,
+    python-framework_pyramid-{pypy27,py27,pypy37,py37,py38,py39,py310,py311}-Pyramid0110-cornice,
     python-framework_pyramid-{py37,py38,py39,py310,py311,pypy37}-Pyramidlatest,
     python-framework_sanic-{py38,pypy37}-sanic{190301,1906,1912,200904,210300,2109,2112,2203,2290},
     python-framework_sanic-{py37,py38,py39,py310,py311,pypy37}-saniclatest,
     python-framework_starlette-{py310,pypy37}-starlette{0014,0015,0019},
     python-framework_starlette-{py37,py38}-starlette{002001},
     python-framework_starlette-{py37,py38,py39,py310,py311,pypy37}-starlettelatest,
     python-framework_strawberry-{py37,py38,py39,py310,py311}-strawberrylatest,
-    python-logger_logging-{py27,py37,py38,py39,py310,py311,pypy,pypy37},
+    python-logger_logging-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
     python-logger_loguru-{py37,py38,py39,py310,py311,pypy37}-logurulatest,
     python-logger_loguru-py39-loguru{06,05,04,03},
-    libcurl-framework_tornado-{py37,py38,py39,py310,py311,pypy37}-tornado0600,
-    libcurl-framework_tornado-{py38,py39,py310,py311}-tornadomaster,
-    rabbitmq-messagebroker_pika-{py27,py37,py38,py39,pypy,pypy37}-pika0.13,
+    python-framework_tornado-{py37,py38,py39,py310,py311,pypy37}-tornado0600,
+    python-framework_tornado-{py38,py39,py310,py311}-tornadomaster,
+    rabbitmq-messagebroker_pika-{py27,py37,py38,py39,pypy27,pypy37}-pika0.13,
     rabbitmq-messagebroker_pika-{py37,py38,py39,py310,py311,pypy37}-pikalatest,
     kafka-messagebroker_confluentkafka-{py27,py37,py38,py39,py310,py311}-confluentkafkalatest,
     kafka-messagebroker_confluentkafka-{py27,py39}-confluentkafka{0107,0106},
     ; confluent-kafka had a bug in 1.8.2's setup.py file which was incompatible with 2.7.
     kafka-messagebroker_confluentkafka-{py39}-confluentkafka{0108},
-    kafka-messagebroker_kafkapython-{pypy,py27,py37,py38,pypy37}-kafkapythonlatest,
+    kafka-messagebroker_kafkapython-{pypy27,py27,py37,py38,pypy37}-kafkapythonlatest,
     kafka-messagebroker_kafkapython-{py27,py38}-kafkapython{020001,020000,0104},
-    python-template_mako-{py27,py37,py38,py39,py310,py311}
+    python-template_genshi-{py27,py37,py311}-genshilatest
+    python-template_mako-{py27,py37,py310,py311}
 
 [testenv]
 deps =
     # Base Dependencies
-    {py37,py38,py39,py310,py311,pypy37}: pytest==6.2.5
-    {py27,pypy}: pytest==4.6.11
+    {py37,py38,py39,py310,py311,pypy37}: pytest==7.2.2
+    {py27,pypy27}: pytest==4.6.11
     iniconfig
-    pytest-cov
+    coverage
     WebTest==2.0.35
 
     # Test Suite Dependencies
     adapter_cheroot: cheroot
     adapter_daphne-daphnelatest: daphne
     adapter_daphne-daphne0205: daphne<2.6
     adapter_daphne-daphne0204: daphne<2.5
@@ -189,17 +191,21 @@
     adapter_hypercorn-hypercorn0013: hypercorn<0.14
     adapter_hypercorn-hypercorn0012: hypercorn<0.13
     adapter_hypercorn-hypercorn0011: hypercorn<0.12
     adapter_hypercorn-hypercorn0010: hypercorn<0.11
     adapter_uvicorn-uvicorn03: uvicorn<0.4
     adapter_uvicorn-uvicorn014: uvicorn<0.15
     adapter_uvicorn-uvicornlatest: uvicorn
+    adapter_waitress: WSGIProxy2
+    adapter_waitress-waitress010404: waitress<1.4.5
+    adapter_waitress-waitress02: waitress<2.1
+    adapter_waitress-waitresslatest: waitress
     agent_features: beautifulsoup4
     application_celery: celery<6.0
-    application_celery-py{py37,37}: importlib-metadata<5.0
+    application_celery-{py37,pypy37}: importlib-metadata<5.0
     application_gearman: gearman<3.0.0
     component_djangorestframework-djangorestframework0300: Django<1.9
     component_djangorestframework-djangorestframework0300: djangorestframework<3.1
     component_djangorestframework-djangorestframeworklatest: Django
     component_djangorestframework-djangorestframeworklatest: djangorestframework
     component_flask_rest: flask
     component_flask_rest: flask-restful
@@ -209,18 +215,20 @@
     component_flask_rest-flaskrestx051: flask-restx<1.0
     component_graphqlserver: graphql-server[sanic,flask]==3.0.0b5
     component_graphqlserver: sanic>20
     component_graphqlserver: Flask
     component_graphqlserver: markupsafe<2.1
     component_graphqlserver: jinja2<3.1
     component_tastypie-tastypie0143: django-tastypie<0.14.4
-    component_tastypie-{py27,pypy}-tastypie0143: django<1.12
+    component_tastypie-{py27,pypy27}-tastypie0143: django<1.12
     component_tastypie-{py37,py38,py39,py310,py311,pypy37}-tastypie0143: django<3.0.1
+    component_tastypie-{py37,py38,py39,py310,py311,pypy37}-tastypie0143: asgiref<3.7.1  # asgiref==3.7.1 only suppport Python 3.10+
     component_tastypie-tastypielatest: django-tastypie
     component_tastypie-tastypielatest: django<4.1
+    component_tastypie-tastypielatest: asgiref<3.7.1  # asgiref==3.7.1 only suppport Python 3.10+
     coroutines_asyncio-{py37,py38,py39,py310,py311}: uvloop
     cross_agent: mock==1.0.1
     cross_agent: requests
     datastore_asyncpg: asyncpg
     datastore_bmemcached-memcached030: python-binary-memcached<0.31
     datastore_bmemcached-memcached030: uhashring<2.0
     datastore_elasticsearch: requests
@@ -229,32 +237,30 @@
     datastore_memcache-memcached01: python-memcached<2
     datastore_mysql-mysqllatest: mysql-connector-python
     datastore_mysql-mysql080023: mysql-connector-python<8.0.24
     datastore_mysql: protobuf<4
     datastore_postgresql: py-postgresql<1.3
     datastore_psycopg2-psycopg2latest: psycopg2-binary
     datastore_psycopg2cffi-psycopg2cffilatest: psycopg2cffi
-    datastore_pyelasticsearch: pyelasticsearch<2.0
+    datastore_pyodbc-pyodbclatest: pyodbc
     datastore_pylibmc: pylibmc
     datastore_pymemcache: pymemcache
     datastore_pymongo-pymongo03: pymongo<4.0
     datastore_pymongo-pymongo04: pymongo<5.0
     datastore_pymysql: PyMySQL<0.11
     datastore_pysolr: pysolr<4.0
     datastore_redis-redislatest: redis
     datastore_redis-redis0400: redis<4.1
     datastore_redis-redis03: redis<4.0
-    datastore_redis-{py27,pypy}: rb
+    datastore_redis-{py27,pypy27}: rb
     datastore_aioredis-redislatest: redis
     datastore_aioredis-aioredislatest: aioredis
-    datastore_aioredis-aioredis01: aioredis<2
     datastore_aredis-aredislatest: aredis
     datastore_solrpy-solrpy00: solrpy<1.0
     datastore_solrpy-solrpy01: solrpy<2.0
-    datastore_umemcache: umemcache<1.7
     external_boto3-boto01: boto3<2.0
     external_boto3-boto01: moto<2.0
     external_boto3-py27: rsa<4.7.1
     external_botocore-botocorelatest: botocore
     external_botocore-botocore128: botocore<1.29
     external_botocore-botocore0125: botocore<1.26
     external_botocore-{py37,py38,py39,py310,py311}: moto[awslambda,ec2,iam]<3.0
@@ -277,17 +283,15 @@
     framework_bottle-bottle0009: bottle<0.10.0
     framework_bottle-bottle0010: bottle<0.11.0
     framework_bottle-bottle0011: bottle<0.12.0
     framework_bottle-bottle0012: bottle<0.13.0
     framework_bottle: jinja2<3.1
     framework_bottle: markupsafe<2.1
     framework_cherrypy: routes
-    framework_cherrypy-CherryPy0302: CherryPy<3.3.0
-    framework_cherrypy-CherryPy0303: CherryPy<3.4.0
-    framework_cherrypy-CherryPy18: CherryPy<18.6.0
+    framework_cherrypy-CherryPylatest: CherryPy
     framework_django-Django0103: Django<1.4
     framework_django-Django0108: Django<1.9
     framework_django-Django0200: Django<2.1
     framework_django-Django0201: Django<2.2
     framework_django-Django0202: Django<2.3
     framework_django-Django0300: Django<3.1
     framework_django-Django0301: Django<3.2
@@ -340,14 +344,15 @@
     framework_sanic-sanic210300: sanic<21.3.1
     framework_sanic-sanic2109: sanic<21.10
     framework_sanic-sanic2112: sanic<21.13
     framework_sanic-sanic2203: sanic<22.4
     framework_sanic-sanic2290: sanic<22.9.1
     framework_sanic-saniclatest: sanic
     framework_sanic-sanic{1812,190301,1906}: aiohttp
+    framework_sanic-sanic{1812,190301,1906,1912,200904,210300,2109,2112,2203,2290}: websockets<11
     framework_starlette: graphene<3
     framework_starlette-starlette0014: starlette<0.15
     framework_starlette-starlette0015: starlette<0.16
     framework_starlette-starlette0019: starlette<0.20
     framework_starlette-starlette002001: starlette==0.20.1
     framework_starlette-starlettelatest: starlette
     framework_strawberry: starlette
@@ -359,71 +364,71 @@
     logger_loguru-loguru06: loguru<0.7
     logger_loguru-loguru05: loguru<0.6
     logger_loguru-loguru04: loguru<0.5
     logger_loguru-loguru03: loguru<0.4
     messagebroker_pika-pika0.13: pika<0.14
     messagebroker_pika-pikalatest: pika
     messagebroker_pika: tornado<5
-    messagebroker_pika-{py27,pypy}: enum34
+    messagebroker_pika-{py27,pypy27}: enum34
     messagebroker_confluentkafka-confluentkafkalatest: confluent-kafka
     messagebroker_confluentkafka-confluentkafka0108: confluent-kafka<1.9
     messagebroker_confluentkafka-confluentkafka0107: confluent-kafka<1.8
     messagebroker_confluentkafka-confluentkafka0106: confluent-kafka<1.7
     messagebroker_kafkapython-kafkapythonlatest: kafka-python
     messagebroker_kafkapython-kafkapython020001: kafka-python<2.0.2
     messagebroker_kafkapython-kafkapython020000: kafka-python<2.0.1
     messagebroker_kafkapython-kafkapython0104: kafka-python<1.5
-    template_mako: mako<1.2
+    template_genshi-genshilatest: genshi
+    template_mako: mako
 
 setenv =
     PYTHONPATH={toxinidir}/tests
     TOX_ENV_DIR={envdir}
     COVERAGE_FILE={envdir}/.coverage.{envname}
     COVERAGE_RCFILE={toxinidir}/tox.ini
     with_extensions: NEW_RELIC_EXTENSIONS = true
     without_extensions: NEW_RELIC_EXTENSIONS = false
     agent_features: NEW_RELIC_APDEX_T = 1000
-    datastore_umemcache: CFLAGS="-Wno-error"
     framework_grpc: PYTHONPATH={toxinidir}/tests/:{toxinidir}/tests/framework_grpc/sample_application
-    libcurl: PYCURL_SSL_LIBRARY=openssl
-    libcurl: LDFLAGS=-L/usr/local/opt/openssl/lib
-    libcurl: CPPFLAGS=-I/usr/local/opt/openssl/include
+    framework_tornado: PYCURL_SSL_LIBRARY=openssl
+    framework_tornado: LDFLAGS=-L/usr/local/opt/openssl/lib
+    framework_tornado: CPPFLAGS=-I/usr/local/opt/openssl/include
 
 passenv =
     NEW_RELIC_DEVELOPER_MODE
     NEW_RELIC_LICENSE_KEY
     NEW_RELIC_HOST
     GITHUB_ACTIONS
 
 commands =
     framework_grpc: python -m grpc_tools.protoc \
     framework_grpc:     --proto_path={toxinidir}/tests/framework_grpc/sample_application \
     framework_grpc:     --python_out={toxinidir}/tests/framework_grpc/sample_application \
     framework_grpc:     --grpc_python_out={toxinidir}/tests/framework_grpc/sample_application \
     framework_grpc:     /{toxinidir}/tests/framework_grpc/sample_application/sample_application.proto
 
-    libcurl: pip install --ignore-installed --install-option="--with-openssl" pycurl
+    framework_tornado: pip install --ignore-installed --config-settings="--build-option=--with-openssl" pycurl
+    coverage run -m pytest -v []
 
-    py.test -v []
+allowlist_externals={toxinidir}/.github/scripts/*
 
 install_command=
-    # Older pip versions that support python 2 have issues with using the cache directory and cause crashes on GitHub Actions
-    {py27,pypy}: {toxinidir}/.github/scripts/retry.sh 3 pip install --no-cache-dir {opts} {packages}
-    !{py27,pypy}: {toxinidir}/.github/scripts/retry.sh 3 pip install {opts} {packages}
+    {toxinidir}/.github/scripts/retry.sh 3 pip install {opts} {packages}
 
 extras =
     agent_streaming: infinite-tracing
 
 changedir =
     adapter_cheroot: tests/adapter_cheroot
     adapter_daphne: tests/adapter_daphne
     adapter_gevent: tests/adapter_gevent
     adapter_gunicorn: tests/adapter_gunicorn
     adapter_hypercorn: tests/adapter_hypercorn
     adapter_uvicorn: tests/adapter_uvicorn
+    adapter_waitress: tests/adapter_waitress
     agent_features: tests/agent_features
     agent_streaming: tests/agent_streaming
     agent_unittests: tests/agent_unittests
     application_celery: tests/application_celery
     application_gearman: tests/application_gearman
     component_djangorestframework: tests/component_djangorestframework
     component_flask_rest: tests/component_flask_rest
@@ -434,27 +439,26 @@
     datastore_asyncpg: tests/datastore_asyncpg
     datastore_bmemcached: tests/datastore_bmemcached
     datastore_elasticsearch: tests/datastore_elasticsearch
     datastore_memcache: tests/datastore_memcache
     datastore_mysql: tests/datastore_mysql
     datastore_postgresql: tests/datastore_postgresql
     datastore_psycopg2: tests/datastore_psycopg2
+    datastore_pyodbc: tests/datastore_pyodbc
     datastore_psycopg2cffi: tests/datastore_psycopg2cffi
-    datastore_pyelasticsearch: tests/datastore_pyelasticsearch
     datastore_pylibmc: tests/datastore_pylibmc
     datastore_pymemcache: tests/datastore_pymemcache
     datastore_pymongo: tests/datastore_pymongo
     datastore_pymysql: tests/datastore_pymysql
     datastore_pysolr: tests/datastore_pysolr
     datastore_redis: tests/datastore_redis
     datastore_aioredis: tests/datastore_aioredis
     datastore_aredis: tests/datastore_aredis
     datastore_solrpy: tests/datastore_solrpy
     datastore_sqlite: tests/datastore_sqlite
-    datastore_umemcache: tests/datastore_umemcache
     external_boto3: tests/external_boto3
     external_botocore: tests/external_botocore
     external_feedparser: tests/external_feedparser
     external_http: tests/external_http
     external_httplib: tests/external_httplib
     external_httplib2: tests/external_httplib2
     external_httpx: tests/external_httpx
@@ -477,31 +481,31 @@
     framework_strawberry: tests/framework_strawberry
     framework_tornado: tests/framework_tornado
     logger_logging: tests/logger_logging
     logger_loguru: tests/logger_loguru
     messagebroker_pika: tests/messagebroker_pika
     messagebroker_confluentkafka: tests/messagebroker_confluentkafka
     messagebroker_kafkapython: tests/messagebroker_kafkapython
+    template_genshi: tests/template_genshi
     template_mako: tests/template_mako
 
 [pytest]
-addopts = --cov="newrelic" --cov-report=html --cov-report=xml
 usefixtures =
     collector_available_fixture
     collector_agent_registration
 
 [coverage:run]
 branch = True
-omit = "newrelic/packages/**/*.py"
-parallel = True
 disable_warnings = couldnt-parse
+source = newrelic 
 
 [coverage:paths]
 source = 
     newrelic/
     .tox/**/site-packages/newrelic/
+    /__w/**/site-packages/newrelic/
 
 [coverage:html]
 directory = ${TOX_ENV_DIR-.}/htmlcov
 
 [coverage:xml]
 output = ${TOX_ENV_DIR-.}/coverage.xml
```

