# Comparing `tmp/flexmeasures-0.9.3.tar.gz` & `tmp/flexmeasures-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexmeasures-0.9.3.tar", last modified: Fri Apr 15 09:01:46 2022, max compression
+gzip compressed data, was "flexmeasures-0.9.4.tar", last modified: Thu Apr 28 14:16:50 2022, max compression
```

## Comparing `flexmeasures-0.9.3.tar` & `flexmeasures-0.9.4.tar`

### file list

```diff
@@ -1,542 +1,542 @@
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.405070 flexmeasures-0.9.3/
--rw-r--r--   0 felix     (1000) felix     (1000)       36 2021-08-24 11:36:33.000000 flexmeasures-0.9.3/.coveragerc
--rw-r--r--   0 felix     (1000) felix     (1000)       34 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/.flaskenv
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.669076 flexmeasures-0.9.3/.github/
--rw-r--r--   0 felix     (1000) felix     (1000)      210 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 felix     (1000) felix     (1000)       39 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/.github/issue-branch.yml
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.669076 flexmeasures-0.9.3/.github/workflows/
--rw-r--r--   0 felix     (1000) felix     (1000)     1071 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/.github/workflows/deploy.yml
--rw-r--r--   0 felix     (1000) felix     (1000)     2252 2022-02-15 16:41:20.000000 flexmeasures-0.9.3/.github/workflows/lint-and-test.yml
--rw-r--r--   0 felix     (1000) felix     (1000)      390 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/.gitignore
--rw-r--r--   0 felix     (1000) felix     (1000)      637 2021-12-01 15:26:39.000000 flexmeasures-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0 felix     (1000) felix     (1000)      485 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/.readthedocs.yaml
--rw-r--r--   0 felix     (1000) felix     (1000)    10141 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/LICENSE
--rw-r--r--   0 felix     (1000) felix     (1000)      106 2021-10-05 10:00:02.000000 flexmeasures-0.9.3/MANIFEST.in
--rw-r--r--   0 felix     (1000) felix     (1000)     2619 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/Makefile
--rw-r--r--   0 felix     (1000) felix     (1000)       77 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/NOTICE
--rw-r--r--   0 felix     (1000) felix     (1000)     2709 2022-04-15 09:01:46.405070 flexmeasures-0.9.3/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)     4047 2022-04-15 08:50:38.000000 flexmeasures-0.9.3/Readme.md
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.685076 flexmeasures-0.9.3/ci/
--rwxr-xr-x   0 felix     (1000) felix     (1000)      472 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/ci/DEPLOY.sh
--rw-r--r--   0 felix     (1000) felix     (1000)       25 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/ci/Readme.md
--rwxr-xr-x   0 felix     (1000) felix     (1000)      996 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/ci/SETUP.sh
--rwxr-xr-x   0 felix     (1000) felix     (1000)      707 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/ci/install-cbc.sh
--rwxr-xr-x   0 felix     (1000) felix     (1000)      823 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/ci/run_mypy.sh
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.701076 flexmeasures-0.9.3/documentation/
--rw-r--r--   0 felix     (1000) felix     (1000)      643 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/documentation/Makefile
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.601077 flexmeasures-0.9.3/documentation/_static/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.701076 flexmeasures-0.9.3/documentation/_static/css/
--rw-r--r--   0 felix     (1000) felix     (1000)      401 2021-08-24 11:36:33.000000 flexmeasures-0.9.3/documentation/_static/css/custom.css
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.729076 flexmeasures-0.9.3/documentation/api/
--rw-r--r--   0 felix     (1000) felix     (1000)     1822 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/api/aggregator.rst
--rw-r--r--   0 felix     (1000) felix     (1000)    13064 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/api/change_log.rst
--rw-r--r--   0 felix     (1000) felix     (1000)      528 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/documentation/api/dev.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     2957 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/api/introduction.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1021 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/api/mdc.rst
--rw-r--r--   0 felix     (1000) felix     (1000)    12255 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/api/notation.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     2095 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/api/prosumer.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1082 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/api/supplier.rst
--rw-r--r--   0 felix     (1000) felix     (1000)      447 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/api/v1.rst
--rw-r--r--   0 felix     (1000) felix     (1000)      453 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/api/v1_1.rst
--rw-r--r--   0 felix     (1000) felix     (1000)      453 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/api/v1_2.rst
--rw-r--r--   0 felix     (1000) felix     (1000)      453 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/api/v1_3.rst
--rw-r--r--   0 felix     (1000) felix     (1000)      453 2022-03-14 09:49:11.000000 flexmeasures-0.9.3/documentation/api/v2_0.rst
--rw-r--r--   0 felix     (1000) felix     (1000)      499 2022-03-24 14:48:18.000000 flexmeasures-0.9.3/documentation/api/v3_0.rst
--rw-r--r--   0 felix     (1000) felix     (1000)    26340 2022-04-15 08:59:05.000000 flexmeasures-0.9.3/documentation/changelog.rst
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.729076 flexmeasures-0.9.3/documentation/cli/
--rw-r--r--   0 felix     (1000) felix     (1000)     2095 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/cli/change_log.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     5693 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/documentation/cli/commands.rst
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.737076 flexmeasures-0.9.3/documentation/concepts/
--rw-r--r--   0 felix     (1000) felix     (1000)     8489 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/concepts/algorithms.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1064 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/concepts/assets.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1755 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/concepts/benefits.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     9434 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/concepts/benefits_of_flex.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1718 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/concepts/inbuilt-smart-functionality.rst
--rw-r--r--   0 felix     (1000) felix     (1000)      319 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/documentation/concepts/markets.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     5612 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/concepts/security_auth.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     2059 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/concepts/users.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     7267 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/conf.py
--rw-r--r--   0 felix     (1000) felix     (1000)    15062 2022-03-07 13:48:34.000000 flexmeasures-0.9.3/documentation/configuration.rst
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.753075 flexmeasures-0.9.3/documentation/dev/
--rw-r--r--   0 felix     (1000) felix     (1000)     4895 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/dev/api.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     4005 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/dev/auth.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     5942 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/dev/ci.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     6100 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/dev/introduction.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     6758 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/dev/note-on-datamodel-transition.rst
--rw-r--r--   0 felix     (1000) felix     (1000)      590 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/get-in-touch.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1746 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/getting-started.rst
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.757075 flexmeasures-0.9.3/documentation/host/
--rw-r--r--   0 felix     (1000) felix     (1000)    14047 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/host/data.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     2153 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/host/deployment.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     2206 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/host/error-monitoring.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     2262 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/host/modes.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     6164 2022-04-15 08:58:03.000000 flexmeasures-0.9.3/documentation/index.rst
--rwxr-xr-x   0 felix     (1000) felix     (1000)      982 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/documentation/make.bat
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.761075 flexmeasures-0.9.3/documentation/plugin/
--rw-r--r--   0 felix     (1000) felix     (1000)     6461 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/plugin/customisation.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1737 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/plugin/introduction.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     6099 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/plugin/showcase.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1254 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/source.rst
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.765075 flexmeasures-0.9.3/documentation/tut/
--rw-r--r--   0 felix     (1000) felix     (1000)    11143 2022-03-24 12:50:49.000000 flexmeasures-0.9.3/documentation/tut/building_uis.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     8671 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/tut/forecasting_scheduling.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     9439 2022-03-27 22:05:32.000000 flexmeasures-0.9.3/documentation/tut/installation.rst
--rw-r--r--   0 felix     (1000) felix     (1000)    12960 2022-03-24 13:16:39.000000 flexmeasures-0.9.3/documentation/tut/posting_data.rst
--rw-r--r--   0 felix     (1000) felix     (1000)    13544 2022-03-24 15:42:10.000000 flexmeasures-0.9.3/documentation/tut/toy-example-from-scratch.rst
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.777075 flexmeasures-0.9.3/documentation/views/
--rw-r--r--   0 felix     (1000) felix     (1000)      720 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/views/admin.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1783 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/views/analytics.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     2190 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/views/control.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     1187 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/views/dashboard.rst
--rw-r--r--   0 felix     (1000) felix     (1000)     4660 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/documentation/views/portfolio.rst
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.785075 flexmeasures-0.9.3/flexmeasures/
--rw-r--r--   0 felix     (1000) felix     (1000)      100 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/Readme.md
--rw-r--r--   0 felix     (1000) felix     (1000)      737 2022-02-09 12:55:22.000000 flexmeasures-0.9.3/flexmeasures/__init__.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.789075 flexmeasures-0.9.3/flexmeasures/api/
--rw-r--r--   0 felix     (1000) felix     (1000)      112 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/api/Readme.md
--rw-r--r--   0 felix     (1000) felix     (1000)     4860 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/__init__.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.793075 flexmeasures-0.9.3/flexmeasures/api/common/
--rw-r--r--   0 felix     (1000) felix     (1000)      465 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/common/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3574 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/api/common/implementations.py
--rw-r--r--   0 felix     (1000) felix     (1000)    11623 2022-03-31 14:05:27.000000 flexmeasures-0.9.3/flexmeasures/api/common/responses.py
--rw-r--r--   0 felix     (1000) felix     (1000)      606 2022-03-08 10:55:51.000000 flexmeasures-0.9.3/flexmeasures/api/common/routes.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.797075 flexmeasures-0.9.3/flexmeasures/api/common/schemas/
--rw-r--r--   0 felix     (1000) felix     (1000)      687 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/common/schemas/generic_assets.py
--rw-r--r--   0 felix     (1000) felix     (1000)    13421 2022-04-04 15:10:35.000000 flexmeasures-0.9.3/flexmeasures/api/common/schemas/sensor_data.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3394 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/common/schemas/sensors.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.797075 flexmeasures-0.9.3/flexmeasures/api/common/schemas/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)     1715 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/common/schemas/tests/test_sensor_data_schema.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2772 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/api/common/schemas/tests/test_sensors.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1636 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/common/schemas/users.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.801075 flexmeasures-0.9.3/flexmeasures/api/common/utils/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/common/utils/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    19020 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/common/utils/api_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1654 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/api/common/utils/args_parsing.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2189 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/common/utils/decorators.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1309 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/common/utils/migration_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)    35302 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/api/common/utils/validators.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.801075 flexmeasures-0.9.3/flexmeasures/api/dev/
--rw-r--r--   0 felix     (1000) felix     (1000)      253 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/api/dev/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3089 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/dev/sensors.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.801075 flexmeasures-0.9.3/flexmeasures/api/dev/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/dev/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)      844 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/dev/tests/conftest.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.805075 flexmeasures-0.9.3/flexmeasures/api/play/
--rw-r--r--   0 felix     (1000) felix     (1000)      454 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/play/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1973 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/api/play/implementations.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1305 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/play/routes.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.809075 flexmeasures-0.9.3/flexmeasures/api/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)     1455 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)      193 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/tests/test_ping.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3848 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/tests/test_task_runs.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3274 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/api/tests/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.809075 flexmeasures-0.9.3/flexmeasures/api/v1/
--rw-r--r--   0 felix     (1000) felix     (1000)      459 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/v1/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    12603 2022-02-15 16:41:31.000000 flexmeasures-0.9.3/flexmeasures/api/v1/implementations.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5782 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v1/routes.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.821075 flexmeasures-0.9.3/flexmeasures/api/v1/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/v1/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4466 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v1/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10389 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v1/tests/test_api_v1.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4079 2022-02-02 13:05:12.000000 flexmeasures-0.9.3/flexmeasures/api/v1/tests/test_api_v1_fresh_db.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4914 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v1/tests/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.829075 flexmeasures-0.9.3/flexmeasures/api/v1_1/
--rw-r--r--   0 felix     (1000) felix     (1000)      459 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/v1_1/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10643 2022-03-31 14:05:27.000000 flexmeasures-0.9.3/flexmeasures/api/v1_1/implementations.py
--rw-r--r--   0 felix     (1000) felix     (1000)    14098 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/api/v1_1/routes.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.829075 flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4286 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10892 2022-03-10 13:40:14.000000 flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/test_api_v1_1.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3240 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/test_api_v1_1_fresh_db.py
--rw-r--r--   0 felix     (1000) felix     (1000)     6321 2022-03-10 13:40:14.000000 flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.833075 flexmeasures-0.9.3/flexmeasures/api/v1_2/
--rw-r--r--   0 felix     (1000) felix     (1000)      459 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/v1_2/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8055 2022-04-04 15:10:35.000000 flexmeasures-0.9.3/flexmeasures/api/v1_2/implementations.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7498 2022-03-15 16:24:48.000000 flexmeasures-0.9.3/flexmeasures/api/v1_2/routes.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.837075 flexmeasures-0.9.3/flexmeasures/api/v1_2/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)      248 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/api/v1_2/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7928 2022-02-03 10:29:36.000000 flexmeasures-0.9.3/flexmeasures/api/v1_2/tests/test_api_v1_2.py
--rw-r--r--   0 felix     (1000) felix     (1000)      829 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v1_2/tests/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.841075 flexmeasures-0.9.3/flexmeasures/api/v1_3/
--rw-r--r--   0 felix     (1000) felix     (1000)      459 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/api/v1_3/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    15103 2022-04-04 15:10:35.000000 flexmeasures-0.9.3/flexmeasures/api/v1_3/implementations.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7944 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v1_3/routes.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.845075 flexmeasures-0.9.3/flexmeasures/api/v1_3/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)      415 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/api/v1_3/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8818 2022-03-07 12:57:47.000000 flexmeasures-0.9.3/flexmeasures/api/v1_3/tests/test_api_v1_3.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3567 2022-03-07 12:57:47.000000 flexmeasures-0.9.3/flexmeasures/api/v1_3/tests/test_api_v1_3_fresh_db.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1315 2022-03-24 12:50:49.000000 flexmeasures-0.9.3/flexmeasures/api/v1_3/tests/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.845075 flexmeasures-0.9.3/flexmeasures/api/v2_0/
--rw-r--r--   0 felix     (1000) felix     (1000)      428 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/__init__.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.853075 flexmeasures-0.9.3/flexmeasures/api/v2_0/implementations/
--rw-r--r--   0 felix     (1000) felix     (1000)       50 2022-03-14 08:50:45.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/implementations/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5407 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/implementations/assets.py
--rw-r--r--   0 felix     (1000) felix     (1000)    13418 2022-02-15 16:41:31.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/implementations/sensors.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3232 2022-03-14 09:57:51.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/implementations/users.py
--rw-r--r--   0 felix     (1000) felix     (1000)    28391 2022-03-14 09:59:07.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/routes.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.857075 flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)      403 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)    11836 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/test_api_v2_0_assets.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1123 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/test_api_v2_0_sensors.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2228 2022-03-10 13:40:14.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/test_api_v2_0_sensors_fresh_db.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4881 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.861075 flexmeasures-0.9.3/flexmeasures/api/v3_0/
--rw-r--r--   0 felix     (1000) felix     (1000)      506 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7353 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/assets.py
--rw-r--r--   0 felix     (1000) felix     (1000)    19568 2022-03-24 15:44:18.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/sensors.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.881074 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2158 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5863 2022-03-24 12:50:49.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_api_v3_0_users.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1931 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_api_v3_0_users_fresh_db.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8894 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_assets_api.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2925 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_assets_api_fresh_db.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3549 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_sensor_data.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1857 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_sensor_data_fresh_db.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5671 2022-03-24 15:43:26.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_sensor_schedules.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1658 2022-03-31 12:23:27.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8410 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/api/v3_0/users.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5074 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/app.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.885074 flexmeasures-0.9.3/flexmeasures/auth/
--rw-r--r--   0 felix     (1000) felix     (1000)     1563 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/auth/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5420 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/auth/decorators.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4298 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/auth/error_handling.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7624 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/auth/policy.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.889074 flexmeasures-0.9.3/flexmeasures/auth/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)     2914 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/auth/tests/test_principal_matching.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.905074 flexmeasures-0.9.3/flexmeasures/cli/
--rw-r--r--   0 felix     (1000) felix     (1000)      578 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/cli/Readme.md
--rw-r--r--   0 felix     (1000) felix     (1000)     1474 2022-04-15 08:51:19.000000 flexmeasures-0.9.3/flexmeasures/cli/__init__.py
--rwxr-xr-x   0 felix     (1000) felix     (1000)    33167 2022-03-24 15:42:10.000000 flexmeasures-0.9.3/flexmeasures/cli/data_add.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10923 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/cli/data_delete.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7655 2022-03-07 12:57:47.000000 flexmeasures-0.9.3/flexmeasures/cli/data_edit.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9822 2022-03-24 21:01:57.000000 flexmeasures-0.9.3/flexmeasures/cli/data_show.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4642 2022-03-07 12:57:47.000000 flexmeasures-0.9.3/flexmeasures/cli/db_ops.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2982 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/cli/jobs.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3027 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/cli/monitor.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4883 2022-02-02 13:05:12.000000 flexmeasures-0.9.3/flexmeasures/cli/testing.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.913074 flexmeasures-0.9.3/flexmeasures/cli/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-02-12 13:47:15.000000 flexmeasures-0.9.3/flexmeasures/cli/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2679 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/cli/tests/test_data_add.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4055 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/cli/tests/test_data_edit.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3734 2022-04-09 09:14:37.000000 flexmeasures-0.9.3/flexmeasures/cli/tests/test_data_show.py
--rw-r--r--   0 felix     (1000) felix     (1000)      300 2022-04-15 08:51:19.000000 flexmeasures-0.9.3/flexmeasures/cli/tests/test_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)      914 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/cli/tests/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.913074 flexmeasures-0.9.3/flexmeasures/config/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-02-09 12:55:22.000000 flexmeasures-0.9.3/flexmeasures/config/__init__.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.917074 flexmeasures-0.9.3/flexmeasures/config/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-02-09 12:55:22.000000 flexmeasures-0.9.3/flexmeasures/config/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)      395 2022-02-09 12:55:22.000000 flexmeasures-0.9.3/flexmeasures/config/tests/test_package.py
--rw-r--r--   0 felix     (1000) felix     (1000)    24728 2022-03-31 14:05:27.000000 flexmeasures-0.9.3/flexmeasures/conftest.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.925074 flexmeasures-0.9.3/flexmeasures/data/
--rw-r--r--   0 felix     (1000) felix     (1000)      114 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/Readme.md
--rw-r--r--   0 felix     (1000) felix     (1000)      605 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2447 2022-01-06 18:46:11.000000 flexmeasures-0.9.3/flexmeasures/data/config.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.929074 flexmeasures-0.9.3/flexmeasures/data/migrations/
--rwxr-xr-x   0 felix     (1000) felix     (1000)       38 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/README
--rw-r--r--   0 felix     (1000) felix     (1000)      770 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/alembic.ini
--rwxr-xr-x   0 felix     (1000) felix     (1000)     2808 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/env.py
--rwxr-xr-x   0 felix     (1000) felix     (1000)      494 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/script.py.mako
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.977074 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/
--rw-r--r--   0 felix     (1000) felix     (1000)     2255 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/01fe99da5716_initial.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1840 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/02ddbbff29a7_naming_conventions.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1281 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/038bab973c40_add_unique_constraint_for_sensor_names_.py
--rw-r--r--   0 felix     (1000) felix     (1000)      882 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/04f0e2d2924a_add_source_id_as_primary_key_for_timed_beliefs.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1685 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/11b735abebe7_create_power_table_and_drop_measurement_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)      657 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1a4f0e5c4b86_unique_userids_in_ds.py
--rw-r--r--   0 felix     (1000) felix     (1000)      846 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1ae32ffc8c3f_rename_data_source_unique_constraint.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1156 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1b64acf01809_forecasting_job_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)      637 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1bcccdf0c3e1_unique_usernames.py
--rw-r--r--   0 felix     (1000) felix     (1000)      925 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1e8d27922f56_create_price_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7089 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/22ce09690d23_mix_in_timely_beliefs_sensor_with_asset_market_and_weather_sensor.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1287 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/26373d8266db_owner_deletion_deletes_assets_and_power.py
--rw-r--r--   0 felix     (1000) felix     (1000)      828 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/2c9a32614784_rename_data_source_columns_in_power_price_and_weather_tables.py
--rw-r--r--   0 felix     (1000) felix     (1000)      738 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/30f7b63069e1_delete_asset_if_sensor_is_deleted.py
--rw-r--r--   0 felix     (1000) felix     (1000)      952 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/30fe2267e7d5_add_optional_DataSource_columns_for_model_and_version.py
--rw-r--r--   0 felix     (1000) felix     (1000)      328 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/31f251554682_merge.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1504 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/3d56402cde15_drop_login_columns_in_bvp_users_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4335 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/3db3e71d101d_make_datasource_a_subclass_of_timely_beliefs_beliefsource.py
--rw-r--r--   0 felix     (1000) felix     (1000)      683 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/3e43d3274d16_Asset_soc_udi_event_id.py
--rw-r--r--   0 felix     (1000) felix     (1000)      939 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/45d937300b0f_create_measurement_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1672 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/4b6cebbdf473_create_weather_sensor_type_and_weather_sensor_and_weather_tables.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4183 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/50cf294e007d_complete_adding_units_to_all_generic_asset_tables_and_display_names_to_all_generic_asset_tables_and_generic_asset_type_tables.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1159 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/550a9020f1bf_default_resolution_for_existing_sensors.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2504 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/564e8df4e3a9_stop_using_bvp_in_table_names.py
--rw-r--r--   0 felix     (1000) felix     (1000)     6376 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/565e092a6c5e_introduce_the_GenericAssetType_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1788 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/5d39829d91af_create_data_sources_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)      884 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/61bfc6e45c4d_add_soc_columns_in_asset_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)    17209 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/6cf5b241b85f_copy_attributes_from_old_data_models_to_GenericAsset.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3373 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/7113b0f00678_drop_forecasting_jobs_table_and_make_display_names_nullable.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3326 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/7987667dbd43_add_asset_type_hover_label.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5399 2022-03-07 12:57:47.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/7f8b8920355f_create_annotation_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3120 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/830e72a8b218_migrate_sensor_relationships_for_power_price_weather.py
--rw-r--r--   0 felix     (1000) felix     (1000)      809 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/8abe32ffa204_add_owner_id_column_in_asset_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1674 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/8fcc5fec67bc_make_data_source_id_columns_primary_keys.py
--rw-r--r--   0 felix     (1000) felix     (1000)      328 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/919dc9f1dc1f_merge.py
--rw-r--r--   0 felix     (1000) felix     (1000)      954 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/91a938bfa5a8_add_horizon_columns_to_power_price_and_weather_tables.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1381 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/9254559dcac2_create_market_type_and_market_tables.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1631 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/96f2db5bed30_add_account_roles.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9632 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/994170c26bc6_add_account_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1306 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/9c7fc8e46f1e_add_location_columns_to_weather_sensor_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)      710 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/a328412b4623_add_timezone_column_in_bvp_users_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)    12186 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/a528c3c81506_unique_generic_sensor_ids.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1459 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/a5b970eadb3b_time_series_indexes.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1042 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/a918360f7d63_add_unique_contraints_on_.py
--rw-r--r--   0 felix     (1000) felix     (1000)      807 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/ac2613fffc74_add_market_id_column_to_asset_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)      879 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/b087ce8b529f_create_latest_task_run_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)      790 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/b2b43f0eec40_weathersensors_unique_type_location.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9722 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/b6d49ed7cceb_introduce_the_GenericAsset_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1853 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/b797328ac32d_add_user_fs_uniquifier_for_faster_auth_.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1316 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/bddc5e9f72a3_add_event_resolution_field_to_asset_.py
--rw-r--r--   0 felix     (1000) felix     (1000)      328 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/c1d316c60985_merge.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2243 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/d3440de27ab9_create_bvp_roles_and_bvp_users_and_bvp_roles_users_tables.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2127 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/db00b66be82c_add_horizon_columns_as_primary_keys.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1356 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/db1f67336324_add_price_unit_and_display_name_columns_to_market_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1304 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/e0c2f9aff251_rename_source_id_column_in_data_sources_table.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1172 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/e4c9cf837311_sensor_generic_asset_id_should_not_be_.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1494 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/e62ac5f519d7_create_table_for_timed_beliefs.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3019 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/migrations/versions/e690d373a3d9_copy_Power_Price_Weather_time_series_data_to_TimedBeliefs_table.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.993073 flexmeasures-0.9.3/flexmeasures/data/models/
--rw-r--r--   0 felix     (1000) felix     (1000)      448 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/models/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7816 2022-03-07 12:57:47.000000 flexmeasures-0.9.3/flexmeasures/data/models/annotations.py
--rw-r--r--   0 felix     (1000) felix     (1000)    15082 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/data/models/assets.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.001073 flexmeasures-0.9.3/flexmeasures/data/models/charts/
--rw-r--r--   0 felix     (1000) felix     (1000)     1319 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/models/charts/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1351 2022-04-05 14:35:25.000000 flexmeasures-0.9.3/flexmeasures/data/models/charts/belief_charts.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2121 2022-04-15 08:58:03.000000 flexmeasures-0.9.3/flexmeasures/data/models/charts/defaults.py
--rw-r--r--   0 felix     (1000) felix     (1000)      450 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/models/charts/readme.md
--rw-r--r--   0 felix     (1000) felix     (1000)      329 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/models/charts/test_chart_defaults.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3049 2022-03-03 13:12:25.000000 flexmeasures-0.9.3/flexmeasures/data/models/data_sources.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.005073 flexmeasures-0.9.3/flexmeasures/data/models/forecasting/
--rw-r--r--   0 felix     (1000) felix     (1000)     2271 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/models/forecasting/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)      103 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/models/forecasting/exceptions.py
--rw-r--r--   0 felix     (1000) felix     (1000)    12063 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/data/models/forecasting/model_spec_factory.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.009073 flexmeasures-0.9.3/flexmeasures/data/models/forecasting/model_specs/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/models/forecasting/model_specs/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)      777 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/models/forecasting/model_specs/linear_regression.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1731 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/models/forecasting/model_specs/naive.py
--rw-r--r--   0 felix     (1000) felix     (1000)     6782 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/models/forecasting/utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)    11743 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/data/models/generic_assets.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2575 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/models/legacy_migration_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8960 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/data/models/markets.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1494 2022-02-15 16:41:31.000000 flexmeasures-0.9.3/flexmeasures/data/models/parsing_utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.033073 flexmeasures-0.9.3/flexmeasures/data/models/planning/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/models/planning/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5652 2022-03-14 16:07:16.000000 flexmeasures-0.9.3/flexmeasures/data/models/planning/battery.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5965 2022-03-14 16:07:16.000000 flexmeasures-0.9.3/flexmeasures/data/models/planning/charging_station.py
--rw-r--r--   0 felix     (1000) felix     (1000)      214 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/models/planning/exceptions.py
--rw-r--r--   0 felix     (1000) felix     (1000)    12905 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/models/planning/solver.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.033073 flexmeasures-0.9.3/flexmeasures/data/models/planning/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/models/planning/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)      268 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/models/planning/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9035 2022-02-03 10:29:47.000000 flexmeasures-0.9.3/flexmeasures/data/models/planning/tests/test_solver.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7498 2022-03-14 16:07:16.000000 flexmeasures-0.9.3/flexmeasures/data/models/planning/utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1263 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/data/models/task_runs.py
--rw-r--r--   0 felix     (1000) felix     (1000)    33075 2022-04-09 09:14:37.000000 flexmeasures-0.9.3/flexmeasures/data/models/time_series.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8833 2022-02-15 16:41:31.000000 flexmeasures-0.9.3/flexmeasures/data/models/user.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2347 2022-02-03 12:41:27.000000 flexmeasures-0.9.3/flexmeasures/data/models/validation_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10289 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/data/models/weather.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.045073 flexmeasures-0.9.3/flexmeasures/data/queries/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/queries/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    17284 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/data/queries/analytics.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1331 2022-04-05 14:36:01.000000 flexmeasures-0.9.3/flexmeasures/data/queries/annotations.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1731 2022-03-16 16:30:44.000000 flexmeasures-0.9.3/flexmeasures/data/queries/data_sources.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3562 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/data/queries/generic_assets.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5074 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/queries/portfolio.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2719 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/data/queries/sensors.py
--rw-r--r--   0 felix     (1000) felix     (1000)    12459 2022-04-08 14:06:07.000000 flexmeasures-0.9.3/flexmeasures/data/queries/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.053073 flexmeasures-0.9.3/flexmeasures/data/schemas/
--rw-r--r--   0 felix     (1000) felix     (1000)      191 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)      894 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/account.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2965 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/assets.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3955 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/generic_assets.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2399 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/sensors.py
--rw-r--r--   0 felix     (1000) felix     (1000)      805 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/sources.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.053073 flexmeasures-0.9.3/flexmeasures/data/schemas/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2972 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/tests/test_times.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2875 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/times.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1920 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/units.py
--rw-r--r--   0 felix     (1000) felix     (1000)      951 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/users.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1300 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/data/schemas/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.061073 flexmeasures-0.9.3/flexmeasures/data/scripts/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/scripts/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1919 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/scripts/_test_simulation.py
--rw-r--r--   0 felix     (1000) felix     (1000)    15907 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/data/scripts/data_gen.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3883 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/data/scripts/simulation_utils.py
--rwxr-xr-x   0 felix     (1000) felix     (1000)     9114 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/data/scripts/visualize_data_model.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.069073 flexmeasures-0.9.3/flexmeasures/data/services/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/services/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5560 2022-03-31 14:05:27.000000 flexmeasures-0.9.3/flexmeasures/data/services/asset_grouping.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10532 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/data/services/forecasting.py
--rw-r--r--   0 felix     (1000) felix     (1000)    26457 2022-03-15 16:24:48.000000 flexmeasures-0.9.3/flexmeasures/data/services/resources.py
--rw-r--r--   0 felix     (1000) felix     (1000)     6620 2022-03-24 12:50:49.000000 flexmeasures-0.9.3/flexmeasures/data/services/scheduling.py
--rw-r--r--   0 felix     (1000) felix     (1000)      806 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/data/services/sensors.py
--rw-r--r--   0 felix     (1000) felix     (1000)    14506 2022-04-10 08:08:31.000000 flexmeasures-0.9.3/flexmeasures/data/services/time_series.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7551 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/data/services/users.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.073073 flexmeasures-0.9.3/flexmeasures/data/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8513 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/data/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2064 2022-02-15 16:41:31.000000 flexmeasures-0.9.3/flexmeasures/data/tests/test_annotations.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8257 2022-03-31 14:05:27.000000 flexmeasures-0.9.3/flexmeasures/data/tests/test_forecasting_jobs.py
--rw-r--r--   0 felix     (1000) felix     (1000)     6590 2022-03-31 14:05:27.000000 flexmeasures-0.9.3/flexmeasures/data/tests/test_forecasting_jobs_fresh_db.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9709 2022-03-14 16:07:16.000000 flexmeasures-0.9.3/flexmeasures/data/tests/test_queries.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1683 2022-02-03 10:29:41.000000 flexmeasures-0.9.3/flexmeasures/data/tests/test_scheduling_jobs.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2721 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/tests/test_scheduling_jobs_fresh_db.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1183 2022-03-31 14:05:27.000000 flexmeasures-0.9.3/flexmeasures/data/tests/test_sensor_queries.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3835 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/tests/test_time_series_services.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4219 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/data/tests/test_user_services.py
--rw-r--r--   0 felix     (1000) felix     (1000)      668 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/data/tests/utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5511 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/data/transactional.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5688 2022-02-23 15:14:53.000000 flexmeasures-0.9.3/flexmeasures/data/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.637076 flexmeasures-0.9.3/flexmeasures/templates/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.637076 flexmeasures-0.9.3/flexmeasures/templates/security/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.077073 flexmeasures-0.9.3/flexmeasures/templates/security/email/
--rw-r--r--   0 felix     (1000) felix     (1000)      143 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/templates/security/email/reset_instructions.html
--rw-r--r--   0 felix     (1000) felix     (1000)      134 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/templates/security/email/reset_instructions.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       83 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/templates/security/email/reset_notice.html
--rw-r--r--   0 felix     (1000) felix     (1000)       66 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/templates/security/email/reset_notice.txt
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.077073 flexmeasures-0.9.3/flexmeasures/ui/
--rw-r--r--   0 felix     (1000) felix     (1000)     5847 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/__init__.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.077073 flexmeasures-0.9.3/flexmeasures/ui/charts/
--rw-r--r--   0 felix     (1000) felix     (1000)     3997 2022-03-03 13:12:25.000000 flexmeasures-0.9.3/flexmeasures/ui/charts/latest_state.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.085073 flexmeasures-0.9.3/flexmeasures/ui/crud/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/crud/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3460 2022-01-04 10:42:40.000000 flexmeasures-0.9.3/flexmeasures/ui/crud/api_wrapper.py
--rw-r--r--   0 felix     (1000) felix     (1000)    15225 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/ui/crud/assets.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5413 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/ui/crud/users.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2932 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/error_handlers.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.085073 flexmeasures-0.9.3/flexmeasures/ui/static/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.085073 flexmeasures-0.9.3/flexmeasures/ui/static/css/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.101072 flexmeasures-0.9.3/flexmeasures/ui/static/css/external/
--rw-r--r--   0 felix     (1000) felix     (1000)    81017 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/external/rq-dashboard-bootstrap.min.css
--rw-r--r--   0 felix     (1000) felix     (1000)    26681 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/external/weather-icons.min.css
--rw-r--r--   0 felix     (1000) felix     (1000)    24270 2022-04-15 08:58:03.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/flexmeasures.css
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.109072 flexmeasures-0.9.3/flexmeasures/ui/static/css/font/
--rw-r--r--   0 felix     (1000) felix     (1000)    99774 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.eot
--rw-r--r--   0 felix     (1000) felix     (1000)   184969 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.svg
--rw-r--r--   0 felix     (1000) felix     (1000)    99564 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.ttf
--rw-r--r--   0 felix     (1000) felix     (1000)    56468 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.woff
--rw-r--r--   0 felix     (1000) felix     (1000)    44720 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.woff2
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.141072 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/
--rw-r--r--   0 felix     (1000) felix     (1000)   134808 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/FontAwesome.otf
--rw-r--r--   0 felix     (1000) felix     (1000)   165742 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 felix     (1000) felix     (1000)   444379 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 felix     (1000) felix     (1000)   165548 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 felix     (1000) felix     (1000)    98024 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 felix     (1000) felix     (1000)    77160 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 felix     (1000) felix     (1000)    20127 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 felix     (1000) felix     (1000)   108738 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 felix     (1000) felix     (1000)    45404 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 felix     (1000) felix     (1000)    23424 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 felix     (1000) felix     (1000)    18028 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 felix     (1000) felix     (1000)     4352 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-white.png
--rw-r--r--   0 felix     (1000) felix     (1000)     4352 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings.png
--rw-r--r--   0 felix     (1000) felix     (1000)      866 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/favicon.ico
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.149072 flexmeasures-0.9.3/flexmeasures/ui/static/font/
--rw-r--r--   0 felix     (1000) felix     (1000)     9632 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.eot
--rw-r--r--   0 felix     (1000) felix     (1000)    18348 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.svg
--rw-r--r--   0 felix     (1000) felix     (1000)     9444 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.ttf
--rw-r--r--   0 felix     (1000) felix     (1000)     6024 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.woff
--rw-r--r--   0 felix     (1000) felix     (1000)     4952 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.woff2
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.157072 flexmeasures-0.9.3/flexmeasures/ui/static/images/
--rw-r--r--   0 felix     (1000) felix     (1000)   106674 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/images/chase-lewis-506404-unsplash.jpg
--rw-r--r--   0 felix     (1000) felix     (1000)   143119 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/images/flexmeasures-preview.jpg
--rw-r--r--   0 felix     (1000) felix     (1000)   121868 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/images/tj-k-349056-unsplash.jpg
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.165072 flexmeasures-0.9.3/flexmeasures/ui/static/js/
--rw-r--r--   0 felix     (1000) felix     (1000)     1467 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/ui/static/js/daterange-utils.js
--rw-r--r--   0 felix     (1000) felix     (1000)     1818 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/js/daterangepicker-init.js
--rw-r--r--   0 felix     (1000) felix     (1000)    10156 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/static/js/flexmeasures.js
--rw-r--r--   0 felix     (1000) felix     (1000)     1379 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/static/js/map-init.js
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.169072 flexmeasures-0.9.3/flexmeasures/ui/templates/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.173072 flexmeasures-0.9.3/flexmeasures/ui/templates/admin/
--rw-r--r--   0 felix     (1000) felix     (1000)      848 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/admin/forgot_password.html
--rw-r--r--   0 felix     (1000) felix     (1000)     3533 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/admin/logged_in_user.html
--rw-r--r--   0 felix     (1000) felix     (1000)     4676 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/admin/login_user.html
--rw-r--r--   0 felix     (1000) felix     (1000)      941 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/admin/reset_password.html
--rw-r--r--   0 felix     (1000) felix     (1000)    28779 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/admin/upload.html
--rw-r--r--   0 felix     (1000) felix     (1000)    20926 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/base.html
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.181072 flexmeasures-0.9.3/flexmeasures/ui/templates/crud/
--rw-r--r--   0 felix     (1000) felix     (1000)     8305 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/crud/asset.html
--rw-r--r--   0 felix     (1000) felix     (1000)     5114 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/crud/asset_new.html
--rw-r--r--   0 felix     (1000) felix     (1000)     2985 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/crud/assets.html
--rw-r--r--   0 felix     (1000) felix     (1000)     3849 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/crud/user.html
--rw-r--r--   0 felix     (1000) felix     (1000)     2860 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/crud/users.html
--rw-r--r--   0 felix     (1000) felix     (1000)     2626 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/defaults.jinja
--rw-r--r--   0 felix     (1000) felix     (1000)      636 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/error.html
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.185072 flexmeasures-0.9.3/flexmeasures/ui/templates/rq_dashboard/
--rw-r--r--   0 felix     (1000) felix     (1000)     1632 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/rq_dashboard/base.html
--rw-r--r--   0 felix     (1000) felix     (1000)     9353 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/rq_dashboard/dashboard.html
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.189072 flexmeasures-0.9.3/flexmeasures/ui/templates/views/
--rw-r--r--   0 felix     (1000) felix     (1000)    17179 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/views/analytics.html
--rw-r--r--   0 felix     (1000) felix     (1000)    12426 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/views/control.html
--rw-r--r--   0 felix     (1000) felix     (1000)    15750 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/views/dashboard.html
--rw-r--r--   0 felix     (1000) felix     (1000)    10729 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/views/new_dashboard.html
--rw-r--r--   0 felix     (1000) felix     (1000)    13760 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/views/portfolio.html
--rw-r--r--   0 felix     (1000) felix     (1000)     6131 2022-04-15 08:58:03.000000 flexmeasures-0.9.3/flexmeasures/ui/templates/views/sensors.html
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.193072 flexmeasures-0.9.3/flexmeasures/ui/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/ui/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2358 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/ui/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4338 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/ui/tests/test_asset_crud.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2027 2022-02-11 09:51:55.000000 flexmeasures-0.9.3/flexmeasures/ui/tests/test_error_handling.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3200 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/ui/tests/test_user_crud.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2274 2022-03-24 14:48:03.000000 flexmeasures-0.9.3/flexmeasures/ui/tests/test_views.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1982 2022-03-19 14:58:40.000000 flexmeasures-0.9.3/flexmeasures/ui/tests/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.193072 flexmeasures-0.9.3/flexmeasures/ui/utils/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/flexmeasures/ui/utils/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)      179 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/utils/chart_defaults.py
--rw-r--r--   0 felix     (1000) felix     (1000)    25135 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/utils/plotting_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)    14177 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/ui/utils/view_utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.377070 flexmeasures-0.9.3/flexmeasures/ui/views/
--rw-r--r--   0 felix     (1000) felix     (1000)     1014 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/views/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    27869 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/ui/views/analytics.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4652 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/views/charts.py
--rw-r--r--   0 felix     (1000) felix     (1000)      806 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/views/control.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2048 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/ui/views/dashboard.py
--rw-r--r--   0 felix     (1000) felix     (1000)      720 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/views/logged_in_user.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2330 2022-03-03 13:12:25.000000 flexmeasures-0.9.3/flexmeasures/ui/views/new_dashboard.py
--rw-r--r--   0 felix     (1000) felix     (1000)    12639 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/views/portfolio.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2417 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/views/sensors.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3650 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/ui/views/state.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.397070 flexmeasures-0.9.3/flexmeasures/utils/
--rw-r--r--   0 felix     (1000) felix     (1000)       46 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/utils/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5918 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/utils/app_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2853 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/utils/calculations.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3552 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/flexmeasures/utils/coding_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8260 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/utils/config_defaults.py
--rw-r--r--   0 felix     (1000) felix     (1000)     6865 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/flexmeasures/utils/config_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)    14541 2022-03-14 16:07:16.000000 flexmeasures-0.9.3/flexmeasures/utils/entity_address_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4317 2022-02-08 16:32:58.000000 flexmeasures-0.9.3/flexmeasures/utils/error_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1601 2022-02-03 14:57:57.000000 flexmeasures-0.9.3/flexmeasures/utils/flexmeasures_inflection.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2111 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/utils/geo_utils.py
--rwxr-xr-x   0 felix     (1000) felix     (1000)     9926 2022-03-14 16:07:16.000000 flexmeasures-0.9.3/flexmeasures/utils/grid_cells.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7495 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/flexmeasures/utils/plugin_utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.397070 flexmeasures-0.9.3/flexmeasures/utils/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/flexmeasures/utils/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9116 2021-11-16 09:21:26.000000 flexmeasures-0.9.3/flexmeasures/utils/tests/test_entity_address_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3533 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/utils/tests/test_time_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5080 2022-04-15 08:58:03.000000 flexmeasures-0.9.3/flexmeasures/utils/tests/test_unit_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10783 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/flexmeasures/utils/time_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9061 2022-04-15 08:58:03.000000 flexmeasures-0.9.3/flexmeasures/utils/unit_utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:45.789075 flexmeasures-0.9.3/flexmeasures.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)     2709 2022-04-15 09:01:44.000000 flexmeasures-0.9.3/flexmeasures.egg-info/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)    20731 2022-04-15 09:01:45.000000 flexmeasures-0.9.3/flexmeasures.egg-info/SOURCES.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        1 2022-04-15 09:01:44.000000 flexmeasures-0.9.3/flexmeasures.egg-info/dependency_links.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       80 2022-04-15 09:01:44.000000 flexmeasures-0.9.3/flexmeasures.egg-info/entry_points.txt
--rw-r--r--   0 felix     (1000) felix     (1000)     2114 2022-04-15 09:01:44.000000 flexmeasures-0.9.3/flexmeasures.egg-info/requires.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       13 2022-04-15 09:01:44.000000 flexmeasures-0.9.3/flexmeasures.egg-info/top_level.txt
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-15 09:01:46.405070 flexmeasures-0.9.3/requirements/
--rw-r--r--   0 felix     (1000) felix     (1000)      751 2021-10-22 14:22:50.000000 flexmeasures-0.9.3/requirements/Readme.md
--rw-r--r--   0 felix     (1000) felix     (1000)     1120 2022-04-15 08:58:03.000000 flexmeasures-0.9.3/requirements/app.in
--rw-r--r--   0 felix     (1000) felix     (1000)     7813 2022-04-15 08:58:03.000000 flexmeasures-0.9.3/requirements/app.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      110 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/requirements/dev.in
--rw-r--r--   0 felix     (1000) felix     (1000)     1911 2022-03-27 22:13:19.000000 flexmeasures-0.9.3/requirements/dev.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       99 2022-03-22 10:33:46.000000 flexmeasures-0.9.3/requirements/docs.in
--rw-r--r--   0 felix     (1000) felix     (1000)     2492 2022-03-27 22:07:03.000000 flexmeasures-0.9.3/requirements/docs.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      273 2022-03-04 20:51:54.000000 flexmeasures-0.9.3/requirements/test.in
--rw-r--r--   0 felix     (1000) felix     (1000)     2732 2022-03-27 22:07:03.000000 flexmeasures-0.9.3/requirements/test.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      438 2021-10-23 08:38:38.000000 flexmeasures-0.9.3/run-local.py
--rw-r--r--   0 felix     (1000) felix     (1000)      389 2022-04-15 09:01:46.409070 flexmeasures-0.9.3/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)     3683 2022-01-29 15:27:56.000000 flexmeasures-0.9.3/setup.py
--rwxr-xr-x   0 felix     (1000) felix     (1000)     3113 2021-11-01 13:04:25.000000 flexmeasures-0.9.3/to_pypi.sh
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.635150 flexmeasures-0.9.4/
+-rw-r--r--   0 felix     (1000) felix     (1000)       36 2021-08-24 11:36:33.000000 flexmeasures-0.9.4/.coveragerc
+-rw-r--r--   0 felix     (1000) felix     (1000)       34 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/.flaskenv
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.343153 flexmeasures-0.9.4/.github/
+-rw-r--r--   0 felix     (1000) felix     (1000)      210 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 felix     (1000) felix     (1000)       39 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/.github/issue-branch.yml
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.347153 flexmeasures-0.9.4/.github/workflows/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1071 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/.github/workflows/deploy.yml
+-rw-r--r--   0 felix     (1000) felix     (1000)     2252 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/.github/workflows/lint-and-test.yml
+-rw-r--r--   0 felix     (1000) felix     (1000)      390 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/.gitignore
+-rw-r--r--   0 felix     (1000) felix     (1000)      637 2021-12-01 15:26:39.000000 flexmeasures-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 felix     (1000) felix     (1000)      485 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/.readthedocs.yaml
+-rw-r--r--   0 felix     (1000) felix     (1000)    10141 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/LICENSE
+-rw-r--r--   0 felix     (1000) felix     (1000)      106 2021-10-05 10:00:02.000000 flexmeasures-0.9.4/MANIFEST.in
+-rw-r--r--   0 felix     (1000) felix     (1000)     2619 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/Makefile
+-rw-r--r--   0 felix     (1000) felix     (1000)       77 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/NOTICE
+-rw-r--r--   0 felix     (1000) felix     (1000)     2709 2022-04-28 14:16:50.635150 flexmeasures-0.9.4/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     4047 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/Readme.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.347153 flexmeasures-0.9.4/ci/
+-rwxr-xr-x   0 felix     (1000) felix     (1000)      472 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/ci/DEPLOY.sh
+-rw-r--r--   0 felix     (1000) felix     (1000)       25 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/ci/Readme.md
+-rwxr-xr-x   0 felix     (1000) felix     (1000)      996 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/ci/SETUP.sh
+-rwxr-xr-x   0 felix     (1000) felix     (1000)      707 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/ci/install-cbc.sh
+-rwxr-xr-x   0 felix     (1000) felix     (1000)      823 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/ci/run_mypy.sh
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.351153 flexmeasures-0.9.4/documentation/
+-rw-r--r--   0 felix     (1000) felix     (1000)      643 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/documentation/Makefile
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.311153 flexmeasures-0.9.4/documentation/_static/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.351153 flexmeasures-0.9.4/documentation/_static/css/
+-rw-r--r--   0 felix     (1000) felix     (1000)      401 2021-08-24 11:36:33.000000 flexmeasures-0.9.4/documentation/_static/css/custom.css
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.359153 flexmeasures-0.9.4/documentation/api/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1822 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/api/aggregator.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)    13064 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/api/change_log.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)      528 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/documentation/api/dev.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     2957 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/api/introduction.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1021 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/api/mdc.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)    12255 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/api/notation.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     2095 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/api/prosumer.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1082 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/api/supplier.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)      447 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/api/v1.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)      453 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/api/v1_1.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)      453 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/api/v1_2.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)      453 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/api/v1_3.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)      453 2022-03-14 09:49:11.000000 flexmeasures-0.9.4/documentation/api/v2_0.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)      499 2022-03-24 14:48:18.000000 flexmeasures-0.9.4/documentation/api/v3_0.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)    26567 2022-04-28 14:14:00.000000 flexmeasures-0.9.4/documentation/changelog.rst
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.363153 flexmeasures-0.9.4/documentation/cli/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2095 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/cli/change_log.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     5693 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/documentation/cli/commands.rst
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.371152 flexmeasures-0.9.4/documentation/concepts/
+-rw-r--r--   0 felix     (1000) felix     (1000)     8489 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/concepts/algorithms.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1064 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/concepts/assets.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1755 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/concepts/benefits.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     9434 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/concepts/benefits_of_flex.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1718 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/concepts/inbuilt-smart-functionality.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)      319 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/documentation/concepts/markets.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     5612 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/concepts/security_auth.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     2059 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/concepts/users.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     7267 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/documentation/conf.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    15062 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/documentation/configuration.rst
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.371152 flexmeasures-0.9.4/documentation/dev/
+-rw-r--r--   0 felix     (1000) felix     (1000)     4895 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/dev/api.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     4005 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/dev/auth.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     5942 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/documentation/dev/ci.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     6100 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/dev/introduction.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     6758 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/dev/note-on-datamodel-transition.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)      590 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/get-in-touch.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1746 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/getting-started.rst
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.371152 flexmeasures-0.9.4/documentation/host/
+-rw-r--r--   0 felix     (1000) felix     (1000)    14047 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/documentation/host/data.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     2153 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/documentation/host/deployment.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     2206 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/host/error-monitoring.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     2262 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/host/modes.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     6164 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/documentation/index.rst
+-rwxr-xr-x   0 felix     (1000) felix     (1000)      982 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/documentation/make.bat
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.375152 flexmeasures-0.9.4/documentation/plugin/
+-rw-r--r--   0 felix     (1000) felix     (1000)     6461 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/plugin/customisation.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1737 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/plugin/introduction.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     6099 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/plugin/showcase.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1254 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/source.rst
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.375152 flexmeasures-0.9.4/documentation/tut/
+-rw-r--r--   0 felix     (1000) felix     (1000)    11143 2022-03-24 12:50:49.000000 flexmeasures-0.9.4/documentation/tut/building_uis.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     8671 2022-03-27 22:05:32.000000 flexmeasures-0.9.4/documentation/tut/forecasting_scheduling.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     9439 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/documentation/tut/installation.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)    12960 2022-03-24 13:16:39.000000 flexmeasures-0.9.4/documentation/tut/posting_data.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)    13544 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/documentation/tut/toy-example-from-scratch.rst
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.383152 flexmeasures-0.9.4/documentation/views/
+-rw-r--r--   0 felix     (1000) felix     (1000)      720 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/views/admin.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1783 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/views/analytics.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     2190 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/views/control.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     1187 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/views/dashboard.rst
+-rw-r--r--   0 felix     (1000) felix     (1000)     4660 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/documentation/views/portfolio.rst
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.387152 flexmeasures-0.9.4/flexmeasures/
+-rw-r--r--   0 felix     (1000) felix     (1000)      100 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/Readme.md
+-rw-r--r--   0 felix     (1000) felix     (1000)      737 2022-02-09 12:55:22.000000 flexmeasures-0.9.4/flexmeasures/__init__.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.387152 flexmeasures-0.9.4/flexmeasures/api/
+-rw-r--r--   0 felix     (1000) felix     (1000)      112 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/api/Readme.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     4860 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/__init__.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.391152 flexmeasures-0.9.4/flexmeasures/api/common/
+-rw-r--r--   0 felix     (1000) felix     (1000)      465 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/common/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3574 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/api/common/implementations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    11623 2022-03-31 14:05:27.000000 flexmeasures-0.9.4/flexmeasures/api/common/responses.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      606 2022-04-28 14:11:28.000000 flexmeasures-0.9.4/flexmeasures/api/common/routes.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.391152 flexmeasures-0.9.4/flexmeasures/api/common/schemas/
+-rw-r--r--   0 felix     (1000) felix     (1000)      687 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/common/schemas/generic_assets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    13421 2022-04-04 15:10:35.000000 flexmeasures-0.9.4/flexmeasures/api/common/schemas/sensor_data.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3394 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/common/schemas/sensors.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.391152 flexmeasures-0.9.4/flexmeasures/api/common/schemas/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1715 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/common/schemas/tests/test_sensor_data_schema.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2772 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/api/common/schemas/tests/test_sensors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1636 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/common/schemas/users.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.395152 flexmeasures-0.9.4/flexmeasures/api/common/utils/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/common/utils/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    19020 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/common/utils/api_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1654 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/api/common/utils/args_parsing.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2189 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/common/utils/decorators.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1309 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/common/utils/migration_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    35302 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/api/common/utils/validators.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.395152 flexmeasures-0.9.4/flexmeasures/api/dev/
+-rw-r--r--   0 felix     (1000) felix     (1000)      253 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/api/dev/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3089 2022-04-28 14:11:28.000000 flexmeasures-0.9.4/flexmeasures/api/dev/sensors.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.395152 flexmeasures-0.9.4/flexmeasures/api/dev/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/dev/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      844 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/dev/tests/conftest.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.395152 flexmeasures-0.9.4/flexmeasures/api/play/
+-rw-r--r--   0 felix     (1000) felix     (1000)      454 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/play/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1973 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/api/play/implementations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1305 2022-04-28 14:11:28.000000 flexmeasures-0.9.4/flexmeasures/api/play/routes.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.399152 flexmeasures-0.9.4/flexmeasures/api/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1455 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      193 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/tests/test_ping.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3848 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/tests/test_task_runs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3274 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/api/tests/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.399152 flexmeasures-0.9.4/flexmeasures/api/v1/
+-rw-r--r--   0 felix     (1000) felix     (1000)      459 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/v1/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    12603 2022-02-15 16:41:31.000000 flexmeasures-0.9.4/flexmeasures/api/v1/implementations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5782 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v1/routes.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.403152 flexmeasures-0.9.4/flexmeasures/api/v1/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/v1/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4466 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v1/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10389 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v1/tests/test_api_v1.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4079 2022-02-02 13:05:12.000000 flexmeasures-0.9.4/flexmeasures/api/v1/tests/test_api_v1_fresh_db.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4914 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v1/tests/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.403152 flexmeasures-0.9.4/flexmeasures/api/v1_1/
+-rw-r--r--   0 felix     (1000) felix     (1000)      459 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/v1_1/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10643 2022-03-31 14:05:27.000000 flexmeasures-0.9.4/flexmeasures/api/v1_1/implementations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    14098 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/api/v1_1/routes.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.403152 flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4286 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10892 2022-03-10 13:40:14.000000 flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/test_api_v1_1.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3240 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/test_api_v1_1_fresh_db.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     6321 2022-03-10 13:40:14.000000 flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.407152 flexmeasures-0.9.4/flexmeasures/api/v1_2/
+-rw-r--r--   0 felix     (1000) felix     (1000)      459 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/v1_2/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8055 2022-04-04 15:10:35.000000 flexmeasures-0.9.4/flexmeasures/api/v1_2/implementations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7498 2022-03-15 16:24:48.000000 flexmeasures-0.9.4/flexmeasures/api/v1_2/routes.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.411152 flexmeasures-0.9.4/flexmeasures/api/v1_2/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)      248 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/api/v1_2/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7928 2022-02-03 10:29:36.000000 flexmeasures-0.9.4/flexmeasures/api/v1_2/tests/test_api_v1_2.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      829 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v1_2/tests/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.415152 flexmeasures-0.9.4/flexmeasures/api/v1_3/
+-rw-r--r--   0 felix     (1000) felix     (1000)      459 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/api/v1_3/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    15103 2022-04-04 15:10:35.000000 flexmeasures-0.9.4/flexmeasures/api/v1_3/implementations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7944 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v1_3/routes.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.415152 flexmeasures-0.9.4/flexmeasures/api/v1_3/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)      415 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/api/v1_3/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8818 2022-03-07 12:57:47.000000 flexmeasures-0.9.4/flexmeasures/api/v1_3/tests/test_api_v1_3.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3567 2022-03-07 12:57:47.000000 flexmeasures-0.9.4/flexmeasures/api/v1_3/tests/test_api_v1_3_fresh_db.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1315 2022-03-24 12:50:49.000000 flexmeasures-0.9.4/flexmeasures/api/v1_3/tests/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.415152 flexmeasures-0.9.4/flexmeasures/api/v2_0/
+-rw-r--r--   0 felix     (1000) felix     (1000)      428 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/__init__.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.419152 flexmeasures-0.9.4/flexmeasures/api/v2_0/implementations/
+-rw-r--r--   0 felix     (1000) felix     (1000)       50 2022-03-14 08:50:45.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/implementations/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5407 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/implementations/assets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    13418 2022-02-15 16:41:31.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/implementations/sensors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3232 2022-03-14 09:57:51.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/implementations/users.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    28391 2022-03-14 09:59:07.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/routes.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.423152 flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)      403 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    11836 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/test_api_v2_0_assets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1123 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/test_api_v2_0_sensors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2228 2022-03-10 13:40:14.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/test_api_v2_0_sensors_fresh_db.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4881 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.423152 flexmeasures-0.9.4/flexmeasures/api/v3_0/
+-rw-r--r--   0 felix     (1000) felix     (1000)      506 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7353 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/assets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    19568 2022-03-24 15:44:18.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/sensors.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.427152 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2158 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5863 2022-03-24 12:50:49.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_api_v3_0_users.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1931 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_api_v3_0_users_fresh_db.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8894 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_assets_api.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2925 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_assets_api_fresh_db.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3549 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_sensor_data.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1857 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_sensor_data_fresh_db.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5671 2022-03-24 15:43:26.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_sensor_schedules.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1658 2022-03-31 12:23:27.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8410 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/api/v3_0/users.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5074 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/app.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.427152 flexmeasures-0.9.4/flexmeasures/auth/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1563 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/auth/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5420 2022-04-28 14:11:28.000000 flexmeasures-0.9.4/flexmeasures/auth/decorators.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4298 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/auth/error_handling.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7624 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/auth/policy.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.431152 flexmeasures-0.9.4/flexmeasures/auth/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2914 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/auth/tests/test_principal_matching.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.431152 flexmeasures-0.9.4/flexmeasures/cli/
+-rw-r--r--   0 felix     (1000) felix     (1000)      578 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/cli/Readme.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     1474 2022-04-15 08:51:19.000000 flexmeasures-0.9.4/flexmeasures/cli/__init__.py
+-rwxr-xr-x   0 felix     (1000) felix     (1000)    33167 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/flexmeasures/cli/data_add.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10923 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/cli/data_delete.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7655 2022-03-07 12:57:47.000000 flexmeasures-0.9.4/flexmeasures/cli/data_edit.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9822 2022-03-24 21:01:57.000000 flexmeasures-0.9.4/flexmeasures/cli/data_show.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4642 2022-03-07 12:57:47.000000 flexmeasures-0.9.4/flexmeasures/cli/db_ops.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2982 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/cli/jobs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3027 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/cli/monitor.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4883 2022-02-02 13:05:12.000000 flexmeasures-0.9.4/flexmeasures/cli/testing.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.435152 flexmeasures-0.9.4/flexmeasures/cli/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-02-12 13:47:15.000000 flexmeasures-0.9.4/flexmeasures/cli/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2679 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/cli/tests/test_data_add.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4055 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/cli/tests/test_data_edit.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3734 2022-04-09 09:14:37.000000 flexmeasures-0.9.4/flexmeasures/cli/tests/test_data_show.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      300 2022-04-15 08:51:19.000000 flexmeasures-0.9.4/flexmeasures/cli/tests/test_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      914 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/cli/tests/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.435152 flexmeasures-0.9.4/flexmeasures/config/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-02-09 12:55:22.000000 flexmeasures-0.9.4/flexmeasures/config/__init__.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.435152 flexmeasures-0.9.4/flexmeasures/config/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2022-02-09 12:55:22.000000 flexmeasures-0.9.4/flexmeasures/config/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      395 2022-02-09 12:55:22.000000 flexmeasures-0.9.4/flexmeasures/config/tests/test_package.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    24728 2022-03-31 14:05:27.000000 flexmeasures-0.9.4/flexmeasures/conftest.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.439152 flexmeasures-0.9.4/flexmeasures/data/
+-rw-r--r--   0 felix     (1000) felix     (1000)      114 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/Readme.md
+-rw-r--r--   0 felix     (1000) felix     (1000)      605 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2447 2022-01-06 18:46:11.000000 flexmeasures-0.9.4/flexmeasures/data/config.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.439152 flexmeasures-0.9.4/flexmeasures/data/migrations/
+-rwxr-xr-x   0 felix     (1000) felix     (1000)       38 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/README
+-rw-r--r--   0 felix     (1000) felix     (1000)      770 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/alembic.ini
+-rwxr-xr-x   0 felix     (1000) felix     (1000)     2808 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/env.py
+-rwxr-xr-x   0 felix     (1000) felix     (1000)      494 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/script.py.mako
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.483151 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2255 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/01fe99da5716_initial.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1840 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/02ddbbff29a7_naming_conventions.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1281 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/038bab973c40_add_unique_constraint_for_sensor_names_.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      882 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/04f0e2d2924a_add_source_id_as_primary_key_for_timed_beliefs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1685 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/11b735abebe7_create_power_table_and_drop_measurement_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      657 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1a4f0e5c4b86_unique_userids_in_ds.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      846 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1ae32ffc8c3f_rename_data_source_unique_constraint.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1156 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1b64acf01809_forecasting_job_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      637 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1bcccdf0c3e1_unique_usernames.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      925 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1e8d27922f56_create_price_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7089 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/22ce09690d23_mix_in_timely_beliefs_sensor_with_asset_market_and_weather_sensor.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1287 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/26373d8266db_owner_deletion_deletes_assets_and_power.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      828 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/2c9a32614784_rename_data_source_columns_in_power_price_and_weather_tables.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      738 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/30f7b63069e1_delete_asset_if_sensor_is_deleted.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      952 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/30fe2267e7d5_add_optional_DataSource_columns_for_model_and_version.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      328 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/31f251554682_merge.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1504 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/3d56402cde15_drop_login_columns_in_bvp_users_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4335 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/3db3e71d101d_make_datasource_a_subclass_of_timely_beliefs_beliefsource.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      683 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/3e43d3274d16_Asset_soc_udi_event_id.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      939 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/45d937300b0f_create_measurement_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1672 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/4b6cebbdf473_create_weather_sensor_type_and_weather_sensor_and_weather_tables.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4183 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/50cf294e007d_complete_adding_units_to_all_generic_asset_tables_and_display_names_to_all_generic_asset_tables_and_generic_asset_type_tables.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1159 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/550a9020f1bf_default_resolution_for_existing_sensors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2504 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/564e8df4e3a9_stop_using_bvp_in_table_names.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     6376 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/565e092a6c5e_introduce_the_GenericAssetType_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1788 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/5d39829d91af_create_data_sources_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      884 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/61bfc6e45c4d_add_soc_columns_in_asset_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    17209 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/6cf5b241b85f_copy_attributes_from_old_data_models_to_GenericAsset.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3373 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/7113b0f00678_drop_forecasting_jobs_table_and_make_display_names_nullable.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3326 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/7987667dbd43_add_asset_type_hover_label.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5399 2022-03-07 12:57:47.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/7f8b8920355f_create_annotation_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3120 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/830e72a8b218_migrate_sensor_relationships_for_power_price_weather.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      809 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/8abe32ffa204_add_owner_id_column_in_asset_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1674 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/8fcc5fec67bc_make_data_source_id_columns_primary_keys.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      328 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/919dc9f1dc1f_merge.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      954 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/91a938bfa5a8_add_horizon_columns_to_power_price_and_weather_tables.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1381 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/9254559dcac2_create_market_type_and_market_tables.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1631 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/96f2db5bed30_add_account_roles.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9632 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/994170c26bc6_add_account_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1306 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/9c7fc8e46f1e_add_location_columns_to_weather_sensor_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      710 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/a328412b4623_add_timezone_column_in_bvp_users_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    12186 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/a528c3c81506_unique_generic_sensor_ids.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1459 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/a5b970eadb3b_time_series_indexes.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1042 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/a918360f7d63_add_unique_contraints_on_.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      807 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/ac2613fffc74_add_market_id_column_to_asset_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      879 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/b087ce8b529f_create_latest_task_run_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      790 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/b2b43f0eec40_weathersensors_unique_type_location.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9722 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/b6d49ed7cceb_introduce_the_GenericAsset_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1853 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/b797328ac32d_add_user_fs_uniquifier_for_faster_auth_.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1316 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/bddc5e9f72a3_add_event_resolution_field_to_asset_.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      328 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/c1d316c60985_merge.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2243 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/d3440de27ab9_create_bvp_roles_and_bvp_users_and_bvp_roles_users_tables.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2127 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/db00b66be82c_add_horizon_columns_as_primary_keys.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1356 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/db1f67336324_add_price_unit_and_display_name_columns_to_market_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1304 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/e0c2f9aff251_rename_source_id_column_in_data_sources_table.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1172 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/e4c9cf837311_sensor_generic_asset_id_should_not_be_.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1494 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/e62ac5f519d7_create_table_for_timed_beliefs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3019 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/migrations/versions/e690d373a3d9_copy_Power_Price_Weather_time_series_data_to_TimedBeliefs_table.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.495151 flexmeasures-0.9.4/flexmeasures/data/models/
+-rw-r--r--   0 felix     (1000) felix     (1000)      448 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/models/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7816 2022-03-07 12:57:47.000000 flexmeasures-0.9.4/flexmeasures/data/models/annotations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    15082 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/data/models/assets.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.499151 flexmeasures-0.9.4/flexmeasures/data/models/charts/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1319 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/models/charts/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1351 2022-04-05 14:35:25.000000 flexmeasures-0.9.4/flexmeasures/data/models/charts/belief_charts.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2121 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/flexmeasures/data/models/charts/defaults.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      450 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/models/charts/readme.md
+-rw-r--r--   0 felix     (1000) felix     (1000)      329 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/models/charts/test_chart_defaults.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3049 2022-03-03 13:12:25.000000 flexmeasures-0.9.4/flexmeasures/data/models/data_sources.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.503151 flexmeasures-0.9.4/flexmeasures/data/models/forecasting/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2271 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/models/forecasting/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      103 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/models/forecasting/exceptions.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    12063 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/data/models/forecasting/model_spec_factory.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.503151 flexmeasures-0.9.4/flexmeasures/data/models/forecasting/model_specs/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/models/forecasting/model_specs/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      777 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/models/forecasting/model_specs/linear_regression.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1731 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/models/forecasting/model_specs/naive.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     6782 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/models/forecasting/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    11743 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/data/models/generic_assets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2575 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/models/legacy_migration_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8960 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/data/models/markets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1494 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/flexmeasures/data/models/parsing_utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.507151 flexmeasures-0.9.4/flexmeasures/data/models/planning/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/models/planning/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5652 2022-03-14 16:07:16.000000 flexmeasures-0.9.4/flexmeasures/data/models/planning/battery.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5965 2022-03-14 16:07:16.000000 flexmeasures-0.9.4/flexmeasures/data/models/planning/charging_station.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      214 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/models/planning/exceptions.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    12905 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/models/planning/solver.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.511151 flexmeasures-0.9.4/flexmeasures/data/models/planning/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/models/planning/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      268 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/models/planning/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9035 2022-02-03 10:29:47.000000 flexmeasures-0.9.4/flexmeasures/data/models/planning/tests/test_solver.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7498 2022-03-14 16:07:16.000000 flexmeasures-0.9.4/flexmeasures/data/models/planning/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1263 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/data/models/task_runs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    33075 2022-04-09 09:14:37.000000 flexmeasures-0.9.4/flexmeasures/data/models/time_series.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8833 2022-02-15 16:41:31.000000 flexmeasures-0.9.4/flexmeasures/data/models/user.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2347 2022-02-03 12:41:27.000000 flexmeasures-0.9.4/flexmeasures/data/models/validation_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10289 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/data/models/weather.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.515151 flexmeasures-0.9.4/flexmeasures/data/queries/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/queries/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    17284 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/data/queries/analytics.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1331 2022-04-05 14:36:01.000000 flexmeasures-0.9.4/flexmeasures/data/queries/annotations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1731 2022-03-16 16:30:44.000000 flexmeasures-0.9.4/flexmeasures/data/queries/data_sources.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3562 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/data/queries/generic_assets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5074 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/queries/portfolio.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2719 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/data/queries/sensors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    12459 2022-04-08 14:06:07.000000 flexmeasures-0.9.4/flexmeasures/data/queries/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.523151 flexmeasures-0.9.4/flexmeasures/data/schemas/
+-rw-r--r--   0 felix     (1000) felix     (1000)      191 2022-04-21 09:44:15.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      894 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/account.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2965 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/assets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3955 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/generic_assets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2399 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/sensors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      805 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/sources.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.523151 flexmeasures-0.9.4/flexmeasures/data/schemas/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2972 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/tests/test_times.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2875 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/times.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1920 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/units.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      951 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/users.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1300 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/data/schemas/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.523151 flexmeasures-0.9.4/flexmeasures/data/scripts/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/scripts/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1919 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/scripts/_test_simulation.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    15907 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/data/scripts/data_gen.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3883 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/data/scripts/simulation_utils.py
+-rwxr-xr-x   0 felix     (1000) felix     (1000)     9114 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/data/scripts/visualize_data_model.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.531151 flexmeasures-0.9.4/flexmeasures/data/services/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/services/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5560 2022-03-31 14:05:27.000000 flexmeasures-0.9.4/flexmeasures/data/services/asset_grouping.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10532 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/data/services/forecasting.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    26457 2022-03-15 16:24:48.000000 flexmeasures-0.9.4/flexmeasures/data/services/resources.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     6620 2022-03-24 12:50:49.000000 flexmeasures-0.9.4/flexmeasures/data/services/scheduling.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      806 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/data/services/sensors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    14506 2022-04-10 08:08:31.000000 flexmeasures-0.9.4/flexmeasures/data/services/time_series.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7551 2022-03-22 10:33:46.000000 flexmeasures-0.9.4/flexmeasures/data/services/users.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.535151 flexmeasures-0.9.4/flexmeasures/data/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8513 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/data/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2064 2022-02-15 16:41:31.000000 flexmeasures-0.9.4/flexmeasures/data/tests/test_annotations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8257 2022-03-31 14:05:27.000000 flexmeasures-0.9.4/flexmeasures/data/tests/test_forecasting_jobs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     6590 2022-03-31 14:05:27.000000 flexmeasures-0.9.4/flexmeasures/data/tests/test_forecasting_jobs_fresh_db.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9709 2022-03-14 16:07:16.000000 flexmeasures-0.9.4/flexmeasures/data/tests/test_queries.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1683 2022-02-03 10:29:41.000000 flexmeasures-0.9.4/flexmeasures/data/tests/test_scheduling_jobs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2721 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/tests/test_scheduling_jobs_fresh_db.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1183 2022-03-31 14:05:27.000000 flexmeasures-0.9.4/flexmeasures/data/tests/test_sensor_queries.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3835 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/tests/test_time_series_services.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4219 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/data/tests/test_user_services.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      668 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/data/tests/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5511 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/data/transactional.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5688 2022-02-23 15:14:53.000000 flexmeasures-0.9.4/flexmeasures/data/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.323153 flexmeasures-0.9.4/flexmeasures/templates/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.323153 flexmeasures-0.9.4/flexmeasures/templates/security/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.535151 flexmeasures-0.9.4/flexmeasures/templates/security/email/
+-rw-r--r--   0 felix     (1000) felix     (1000)      143 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/templates/security/email/reset_instructions.html
+-rw-r--r--   0 felix     (1000) felix     (1000)      134 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/templates/security/email/reset_instructions.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       83 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/templates/security/email/reset_notice.html
+-rw-r--r--   0 felix     (1000) felix     (1000)       66 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/templates/security/email/reset_notice.txt
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.539151 flexmeasures-0.9.4/flexmeasures/ui/
+-rw-r--r--   0 felix     (1000) felix     (1000)     5847 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/__init__.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.539151 flexmeasures-0.9.4/flexmeasures/ui/charts/
+-rw-r--r--   0 felix     (1000) felix     (1000)     3997 2022-03-03 13:12:25.000000 flexmeasures-0.9.4/flexmeasures/ui/charts/latest_state.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.543151 flexmeasures-0.9.4/flexmeasures/ui/crud/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/crud/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3460 2022-01-04 10:42:40.000000 flexmeasures-0.9.4/flexmeasures/ui/crud/api_wrapper.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    15225 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/ui/crud/assets.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5413 2022-04-28 14:11:28.000000 flexmeasures-0.9.4/flexmeasures/ui/crud/users.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2932 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/error_handlers.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.543151 flexmeasures-0.9.4/flexmeasures/ui/static/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.543151 flexmeasures-0.9.4/flexmeasures/ui/static/css/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.547151 flexmeasures-0.9.4/flexmeasures/ui/static/css/external/
+-rw-r--r--   0 felix     (1000) felix     (1000)    81017 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/external/rq-dashboard-bootstrap.min.css
+-rw-r--r--   0 felix     (1000) felix     (1000)    26681 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/external/weather-icons.min.css
+-rw-r--r--   0 felix     (1000) felix     (1000)    24270 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/flexmeasures.css
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.551151 flexmeasures-0.9.4/flexmeasures/ui/static/css/font/
+-rw-r--r--   0 felix     (1000) felix     (1000)    99774 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.eot
+-rw-r--r--   0 felix     (1000) felix     (1000)   184969 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.svg
+-rw-r--r--   0 felix     (1000) felix     (1000)    99564 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.ttf
+-rw-r--r--   0 felix     (1000) felix     (1000)    56468 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.woff
+-rw-r--r--   0 felix     (1000) felix     (1000)    44720 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.woff2
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.579150 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/
+-rw-r--r--   0 felix     (1000) felix     (1000)   134808 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/FontAwesome.otf
+-rw-r--r--   0 felix     (1000) felix     (1000)   165742 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 felix     (1000) felix     (1000)   444379 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 felix     (1000) felix     (1000)   165548 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 felix     (1000) felix     (1000)    98024 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 felix     (1000) felix     (1000)    77160 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 felix     (1000) felix     (1000)    20127 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 felix     (1000) felix     (1000)   108738 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 felix     (1000) felix     (1000)    45404 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 felix     (1000) felix     (1000)    23424 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 felix     (1000) felix     (1000)    18028 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 felix     (1000) felix     (1000)     4352 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-white.png
+-rw-r--r--   0 felix     (1000) felix     (1000)     4352 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings.png
+-rw-r--r--   0 felix     (1000) felix     (1000)      866 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/favicon.ico
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.579150 flexmeasures-0.9.4/flexmeasures/ui/static/font/
+-rw-r--r--   0 felix     (1000) felix     (1000)     9632 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.eot
+-rw-r--r--   0 felix     (1000) felix     (1000)    18348 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.svg
+-rw-r--r--   0 felix     (1000) felix     (1000)     9444 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.ttf
+-rw-r--r--   0 felix     (1000) felix     (1000)     6024 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.woff
+-rw-r--r--   0 felix     (1000) felix     (1000)     4952 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.woff2
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.583150 flexmeasures-0.9.4/flexmeasures/ui/static/images/
+-rw-r--r--   0 felix     (1000) felix     (1000)   106674 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/images/chase-lewis-506404-unsplash.jpg
+-rw-r--r--   0 felix     (1000) felix     (1000)   143119 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/images/flexmeasures-preview.jpg
+-rw-r--r--   0 felix     (1000) felix     (1000)   121868 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/images/tj-k-349056-unsplash.jpg
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.587150 flexmeasures-0.9.4/flexmeasures/ui/static/js/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1467 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/ui/static/js/daterange-utils.js
+-rw-r--r--   0 felix     (1000) felix     (1000)     1818 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/js/daterangepicker-init.js
+-rw-r--r--   0 felix     (1000) felix     (1000)    10156 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/static/js/flexmeasures.js
+-rw-r--r--   0 felix     (1000) felix     (1000)     1379 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/static/js/map-init.js
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.591150 flexmeasures-0.9.4/flexmeasures/ui/templates/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.595150 flexmeasures-0.9.4/flexmeasures/ui/templates/admin/
+-rw-r--r--   0 felix     (1000) felix     (1000)      848 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/admin/forgot_password.html
+-rw-r--r--   0 felix     (1000) felix     (1000)     3533 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/admin/logged_in_user.html
+-rw-r--r--   0 felix     (1000) felix     (1000)     4676 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/admin/login_user.html
+-rw-r--r--   0 felix     (1000) felix     (1000)      941 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/admin/reset_password.html
+-rw-r--r--   0 felix     (1000) felix     (1000)    28779 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/admin/upload.html
+-rw-r--r--   0 felix     (1000) felix     (1000)    20926 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/base.html
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.595150 flexmeasures-0.9.4/flexmeasures/ui/templates/crud/
+-rw-r--r--   0 felix     (1000) felix     (1000)     8305 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/crud/asset.html
+-rw-r--r--   0 felix     (1000) felix     (1000)     5114 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/crud/asset_new.html
+-rw-r--r--   0 felix     (1000) felix     (1000)     2985 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/crud/assets.html
+-rw-r--r--   0 felix     (1000) felix     (1000)     3849 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/crud/user.html
+-rw-r--r--   0 felix     (1000) felix     (1000)     2860 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/crud/users.html
+-rw-r--r--   0 felix     (1000) felix     (1000)     2626 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/defaults.jinja
+-rw-r--r--   0 felix     (1000) felix     (1000)      636 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/error.html
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.595150 flexmeasures-0.9.4/flexmeasures/ui/templates/rq_dashboard/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1632 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/rq_dashboard/base.html
+-rw-r--r--   0 felix     (1000) felix     (1000)     9353 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/rq_dashboard/dashboard.html
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.603150 flexmeasures-0.9.4/flexmeasures/ui/templates/views/
+-rw-r--r--   0 felix     (1000) felix     (1000)    17179 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/views/analytics.html
+-rw-r--r--   0 felix     (1000) felix     (1000)    12426 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/views/control.html
+-rw-r--r--   0 felix     (1000) felix     (1000)    15750 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/views/dashboard.html
+-rw-r--r--   0 felix     (1000) felix     (1000)    10729 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/views/new_dashboard.html
+-rw-r--r--   0 felix     (1000) felix     (1000)    13760 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/views/portfolio.html
+-rw-r--r--   0 felix     (1000) felix     (1000)     6131 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/flexmeasures/ui/templates/views/sensors.html
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.607150 flexmeasures-0.9.4/flexmeasures/ui/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/ui/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2358 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/ui/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4338 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/ui/tests/test_asset_crud.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2027 2022-02-11 09:51:55.000000 flexmeasures-0.9.4/flexmeasures/ui/tests/test_error_handling.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3200 2022-04-28 14:11:28.000000 flexmeasures-0.9.4/flexmeasures/ui/tests/test_user_crud.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2274 2022-03-24 14:48:03.000000 flexmeasures-0.9.4/flexmeasures/ui/tests/test_views.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1982 2022-03-19 14:58:40.000000 flexmeasures-0.9.4/flexmeasures/ui/tests/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.611150 flexmeasures-0.9.4/flexmeasures/ui/utils/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/flexmeasures/ui/utils/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      179 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/utils/chart_defaults.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    25135 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/utils/plotting_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    14177 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/ui/utils/view_utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.615150 flexmeasures-0.9.4/flexmeasures/ui/views/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1014 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/views/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    27869 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/ui/views/analytics.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4652 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/views/charts.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      806 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/views/control.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2048 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/ui/views/dashboard.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      720 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/views/logged_in_user.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2330 2022-03-03 13:12:25.000000 flexmeasures-0.9.4/flexmeasures/ui/views/new_dashboard.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    12639 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/views/portfolio.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2417 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/views/sensors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3650 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/ui/views/state.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.631150 flexmeasures-0.9.4/flexmeasures/utils/
+-rw-r--r--   0 felix     (1000) felix     (1000)       46 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/utils/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5918 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/utils/app_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2853 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/utils/calculations.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3552 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/flexmeasures/utils/coding_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8260 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/utils/config_defaults.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     6865 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/flexmeasures/utils/config_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    14541 2022-04-21 09:44:15.000000 flexmeasures-0.9.4/flexmeasures/utils/entity_address_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4317 2022-02-08 16:32:58.000000 flexmeasures-0.9.4/flexmeasures/utils/error_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1601 2022-02-03 14:57:57.000000 flexmeasures-0.9.4/flexmeasures/utils/flexmeasures_inflection.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2111 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/utils/geo_utils.py
+-rwxr-xr-x   0 felix     (1000) felix     (1000)     9926 2022-03-14 16:07:16.000000 flexmeasures-0.9.4/flexmeasures/utils/grid_cells.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7495 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/flexmeasures/utils/plugin_utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.635150 flexmeasures-0.9.4/flexmeasures/utils/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/flexmeasures/utils/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9116 2021-11-16 09:21:26.000000 flexmeasures-0.9.4/flexmeasures/utils/tests/test_entity_address_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3533 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/utils/tests/test_time_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5102 2022-04-28 14:13:30.000000 flexmeasures-0.9.4/flexmeasures/utils/tests/test_unit_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10783 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/flexmeasures/utils/time_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9179 2022-04-28 14:13:30.000000 flexmeasures-0.9.4/flexmeasures/utils/unit_utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.387152 flexmeasures-0.9.4/flexmeasures.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2709 2022-04-28 14:16:49.000000 flexmeasures-0.9.4/flexmeasures.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)    20731 2022-04-28 14:16:50.000000 flexmeasures-0.9.4/flexmeasures.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2022-04-28 14:16:49.000000 flexmeasures-0.9.4/flexmeasures.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       80 2022-04-28 14:16:49.000000 flexmeasures-0.9.4/flexmeasures.egg-info/entry_points.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)     2114 2022-04-28 14:16:49.000000 flexmeasures-0.9.4/flexmeasures.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       13 2022-04-28 14:16:49.000000 flexmeasures-0.9.4/flexmeasures.egg-info/top_level.txt
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-04-28 14:16:50.635150 flexmeasures-0.9.4/requirements/
+-rw-r--r--   0 felix     (1000) felix     (1000)      751 2021-10-22 14:22:50.000000 flexmeasures-0.9.4/requirements/Readme.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     1120 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/requirements/app.in
+-rw-r--r--   0 felix     (1000) felix     (1000)     7813 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/requirements/app.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      110 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/requirements/dev.in
+-rw-r--r--   0 felix     (1000) felix     (1000)     1911 2022-03-27 22:13:19.000000 flexmeasures-0.9.4/requirements/dev.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       99 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/requirements/docs.in
+-rw-r--r--   0 felix     (1000) felix     (1000)     2492 2022-04-28 14:13:21.000000 flexmeasures-0.9.4/requirements/docs.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      273 2022-03-04 20:51:54.000000 flexmeasures-0.9.4/requirements/test.in
+-rw-r--r--   0 felix     (1000) felix     (1000)     2732 2022-03-27 22:07:03.000000 flexmeasures-0.9.4/requirements/test.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      438 2021-10-23 08:38:38.000000 flexmeasures-0.9.4/run-local.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      389 2022-04-28 14:16:50.639150 flexmeasures-0.9.4/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)     3683 2022-01-29 15:27:56.000000 flexmeasures-0.9.4/setup.py
+-rwxr-xr-x   0 felix     (1000) felix     (1000)     3113 2021-11-01 13:04:25.000000 flexmeasures-0.9.4/to_pypi.sh
```

### Comparing `flexmeasures-0.9.3/.github/workflows/deploy.yml` & `flexmeasures-0.9.4/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/.github/workflows/lint-and-test.yml` & `flexmeasures-0.9.4/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/.pre-commit-config.yaml` & `flexmeasures-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/LICENSE` & `flexmeasures-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/Makefile` & `flexmeasures-0.9.4/Makefile`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/PKG-INFO` & `flexmeasures-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexmeasures
-Version: 0.9.3
+Version: 0.9.4
 Summary: The *FlexMeasures Platform* is the intelligent backend to support real-time energy flexibility apps, rapidly and scalable.
 Home-page: https://github.com/seitabv/flexmeasures
 Author: Seita BV
 Author-email: nicolas@seita.nl
 License: Apache2.0
 Keywords: smart grid,renewables,balancing,forecasting,scheduling
 Platform: UNKNOWN
```

### Comparing `flexmeasures-0.9.3/Readme.md` & `flexmeasures-0.9.4/Readme.md`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/ci/SETUP.sh` & `flexmeasures-0.9.4/ci/SETUP.sh`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/ci/install-cbc.sh` & `flexmeasures-0.9.4/ci/install-cbc.sh`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/ci/run_mypy.sh` & `flexmeasures-0.9.4/ci/run_mypy.sh`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/Makefile` & `flexmeasures-0.9.4/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/api/aggregator.rst` & `flexmeasures-0.9.4/documentation/api/aggregator.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/api/change_log.rst` & `flexmeasures-0.9.4/documentation/api/change_log.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/api/dev.rst` & `flexmeasures-0.9.4/documentation/api/dev.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/api/introduction.rst` & `flexmeasures-0.9.4/documentation/api/introduction.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/api/mdc.rst` & `flexmeasures-0.9.4/documentation/api/mdc.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/api/notation.rst` & `flexmeasures-0.9.4/documentation/api/notation.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/api/prosumer.rst` & `flexmeasures-0.9.4/documentation/api/prosumer.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/api/supplier.rst` & `flexmeasures-0.9.4/documentation/api/supplier.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/changelog.rst` & `flexmeasures-0.9.4/documentation/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 **********************
 FlexMeasures Changelog
 **********************
 
+v0.9.4 | April 28, 2022
+===========================
+
+Bugfixes
+--------
+* Support checking validity of custom units (i.e. non-SI, non-currency units) [see `PR #424 <http://www.github.com/FlexMeasures/flexmeasures/pull/424>`_]
+
+
 v0.9.3 | April 15, 2022
 ===========================
 
 Bugfixes
 --------
 * Let registered plugins use CLI authorization [see `PR #411 <http://www.github.com/FlexMeasures/flexmeasures/pull/411>`_]
```

### Comparing `flexmeasures-0.9.3/documentation/cli/change_log.rst` & `flexmeasures-0.9.4/documentation/cli/change_log.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/cli/commands.rst` & `flexmeasures-0.9.4/documentation/cli/commands.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/concepts/algorithms.rst` & `flexmeasures-0.9.4/documentation/concepts/algorithms.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/concepts/assets.rst` & `flexmeasures-0.9.4/documentation/concepts/assets.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/concepts/benefits.rst` & `flexmeasures-0.9.4/documentation/concepts/benefits.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/concepts/benefits_of_flex.rst` & `flexmeasures-0.9.4/documentation/concepts/benefits_of_flex.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/concepts/inbuilt-smart-functionality.rst` & `flexmeasures-0.9.4/documentation/concepts/inbuilt-smart-functionality.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/concepts/security_auth.rst` & `flexmeasures-0.9.4/documentation/concepts/security_auth.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/concepts/users.rst` & `flexmeasures-0.9.4/documentation/concepts/users.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/conf.py` & `flexmeasures-0.9.4/documentation/conf.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/configuration.rst` & `flexmeasures-0.9.4/documentation/configuration.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/dev/api.rst` & `flexmeasures-0.9.4/documentation/dev/api.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/dev/auth.rst` & `flexmeasures-0.9.4/documentation/dev/auth.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/dev/ci.rst` & `flexmeasures-0.9.4/documentation/dev/ci.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/dev/introduction.rst` & `flexmeasures-0.9.4/documentation/dev/introduction.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/dev/note-on-datamodel-transition.rst` & `flexmeasures-0.9.4/documentation/dev/note-on-datamodel-transition.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/get-in-touch.rst` & `flexmeasures-0.9.4/documentation/get-in-touch.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/getting-started.rst` & `flexmeasures-0.9.4/documentation/getting-started.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/host/data.rst` & `flexmeasures-0.9.4/documentation/host/data.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/host/deployment.rst` & `flexmeasures-0.9.4/documentation/host/deployment.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/host/error-monitoring.rst` & `flexmeasures-0.9.4/documentation/host/error-monitoring.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/host/modes.rst` & `flexmeasures-0.9.4/documentation/host/modes.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/index.rst` & `flexmeasures-0.9.4/documentation/index.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/make.bat` & `flexmeasures-0.9.4/documentation/make.bat`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/plugin/customisation.rst` & `flexmeasures-0.9.4/documentation/plugin/customisation.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/plugin/introduction.rst` & `flexmeasures-0.9.4/documentation/plugin/introduction.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/plugin/showcase.rst` & `flexmeasures-0.9.4/documentation/plugin/showcase.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/source.rst` & `flexmeasures-0.9.4/documentation/source.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/tut/building_uis.rst` & `flexmeasures-0.9.4/documentation/tut/building_uis.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/tut/forecasting_scheduling.rst` & `flexmeasures-0.9.4/documentation/tut/forecasting_scheduling.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/tut/installation.rst` & `flexmeasures-0.9.4/documentation/tut/installation.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/tut/posting_data.rst` & `flexmeasures-0.9.4/documentation/tut/posting_data.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/tut/toy-example-from-scratch.rst` & `flexmeasures-0.9.4/documentation/tut/toy-example-from-scratch.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/views/admin.rst` & `flexmeasures-0.9.4/documentation/views/admin.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/views/analytics.rst` & `flexmeasures-0.9.4/documentation/views/analytics.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/views/control.rst` & `flexmeasures-0.9.4/documentation/views/control.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/views/dashboard.rst` & `flexmeasures-0.9.4/documentation/views/dashboard.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/documentation/views/portfolio.rst` & `flexmeasures-0.9.4/documentation/views/portfolio.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/__init__.py` & `flexmeasures-0.9.4/flexmeasures/__init__.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/__init__.py` & `flexmeasures-0.9.4/flexmeasures/api/__init__.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/implementations.py` & `flexmeasures-0.9.4/flexmeasures/api/common/implementations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/responses.py` & `flexmeasures-0.9.4/flexmeasures/api/common/responses.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/routes.py` & `flexmeasures-0.9.4/flexmeasures/api/common/routes.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/schemas/generic_assets.py` & `flexmeasures-0.9.4/flexmeasures/api/common/schemas/generic_assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/schemas/sensor_data.py` & `flexmeasures-0.9.4/flexmeasures/api/common/schemas/sensor_data.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/schemas/sensors.py` & `flexmeasures-0.9.4/flexmeasures/api/common/schemas/sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/schemas/tests/test_sensor_data_schema.py` & `flexmeasures-0.9.4/flexmeasures/api/common/schemas/tests/test_sensor_data_schema.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/schemas/tests/test_sensors.py` & `flexmeasures-0.9.4/flexmeasures/api/common/schemas/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/schemas/users.py` & `flexmeasures-0.9.4/flexmeasures/api/common/schemas/users.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/utils/api_utils.py` & `flexmeasures-0.9.4/flexmeasures/api/common/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/utils/args_parsing.py` & `flexmeasures-0.9.4/flexmeasures/api/common/utils/args_parsing.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/utils/decorators.py` & `flexmeasures-0.9.4/flexmeasures/api/common/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/utils/migration_utils.py` & `flexmeasures-0.9.4/flexmeasures/api/common/utils/migration_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/common/utils/validators.py` & `flexmeasures-0.9.4/flexmeasures/api/common/utils/validators.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/dev/sensors.py` & `flexmeasures-0.9.4/flexmeasures/api/dev/sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/dev/tests/conftest.py` & `flexmeasures-0.9.4/flexmeasures/api/dev/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/play/implementations.py` & `flexmeasures-0.9.4/flexmeasures/api/play/implementations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/play/routes.py` & `flexmeasures-0.9.4/flexmeasures/api/play/routes.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/tests/conftest.py` & `flexmeasures-0.9.4/flexmeasures/api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/tests/test_task_runs.py` & `flexmeasures-0.9.4/flexmeasures/api/tests/test_task_runs.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/api/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1/implementations.py` & `flexmeasures-0.9.4/flexmeasures/api/v1/implementations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1/routes.py` & `flexmeasures-0.9.4/flexmeasures/api/v1/routes.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1/tests/conftest.py` & `flexmeasures-0.9.4/flexmeasures/api/v1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1/tests/test_api_v1.py` & `flexmeasures-0.9.4/flexmeasures/api/v1/tests/test_api_v1.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1/tests/test_api_v1_fresh_db.py` & `flexmeasures-0.9.4/flexmeasures/api/v1/tests/test_api_v1_fresh_db.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/api/v1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_1/implementations.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_1/implementations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_1/routes.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_1/routes.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/conftest.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/test_api_v1_1.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/test_api_v1_1.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/test_api_v1_1_fresh_db.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/test_api_v1_1_fresh_db.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_1/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_2/implementations.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_2/implementations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_2/routes.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_2/routes.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_2/tests/test_api_v1_2.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_2/tests/test_api_v1_2.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_2/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_3/implementations.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_3/implementations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_3/routes.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_3/routes.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_3/tests/test_api_v1_3.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_3/tests/test_api_v1_3.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_3/tests/test_api_v1_3_fresh_db.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_3/tests/test_api_v1_3_fresh_db.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v1_3/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/api/v1_3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v2_0/implementations/assets.py` & `flexmeasures-0.9.4/flexmeasures/api/v2_0/implementations/assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v2_0/implementations/sensors.py` & `flexmeasures-0.9.4/flexmeasures/api/v2_0/implementations/sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v2_0/implementations/users.py` & `flexmeasures-0.9.4/flexmeasures/api/v2_0/implementations/users.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v2_0/routes.py` & `flexmeasures-0.9.4/flexmeasures/api/v2_0/routes.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/test_api_v2_0_assets.py` & `flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/test_api_v2_0_assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/test_api_v2_0_sensors.py` & `flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/test_api_v2_0_sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/test_api_v2_0_sensors_fresh_db.py` & `flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/test_api_v2_0_sensors_fresh_db.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v2_0/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/api/v2_0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/assets.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/sensors.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/conftest.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_api_v3_0_users.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_api_v3_0_users.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_api_v3_0_users_fresh_db.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_api_v3_0_users_fresh_db.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_assets_api.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_assets_api.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_assets_api_fresh_db.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_assets_api_fresh_db.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_sensor_data.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_sensor_data.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_sensor_data_fresh_db.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_sensor_data_fresh_db.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/test_sensor_schedules.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/test_sensor_schedules.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/api/v3_0/users.py` & `flexmeasures-0.9.4/flexmeasures/api/v3_0/users.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/app.py` & `flexmeasures-0.9.4/flexmeasures/app.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/auth/__init__.py` & `flexmeasures-0.9.4/flexmeasures/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/auth/decorators.py` & `flexmeasures-0.9.4/flexmeasures/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/auth/error_handling.py` & `flexmeasures-0.9.4/flexmeasures/auth/error_handling.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/auth/policy.py` & `flexmeasures-0.9.4/flexmeasures/auth/policy.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/auth/tests/test_principal_matching.py` & `flexmeasures-0.9.4/flexmeasures/auth/tests/test_principal_matching.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/Readme.md` & `flexmeasures-0.9.4/flexmeasures/cli/Readme.md`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/__init__.py` & `flexmeasures-0.9.4/flexmeasures/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/data_add.py` & `flexmeasures-0.9.4/flexmeasures/cli/data_add.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/data_delete.py` & `flexmeasures-0.9.4/flexmeasures/cli/data_delete.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/data_edit.py` & `flexmeasures-0.9.4/flexmeasures/cli/data_edit.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/data_show.py` & `flexmeasures-0.9.4/flexmeasures/cli/data_show.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/db_ops.py` & `flexmeasures-0.9.4/flexmeasures/cli/db_ops.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/jobs.py` & `flexmeasures-0.9.4/flexmeasures/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/monitor.py` & `flexmeasures-0.9.4/flexmeasures/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/testing.py` & `flexmeasures-0.9.4/flexmeasures/cli/testing.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/tests/test_data_add.py` & `flexmeasures-0.9.4/flexmeasures/cli/tests/test_data_add.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/tests/test_data_edit.py` & `flexmeasures-0.9.4/flexmeasures/cli/tests/test_data_edit.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/tests/test_data_show.py` & `flexmeasures-0.9.4/flexmeasures/cli/tests/test_data_show.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/cli/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/cli/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/conftest.py` & `flexmeasures-0.9.4/flexmeasures/conftest.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/__init__.py` & `flexmeasures-0.9.4/flexmeasures/data/__init__.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/config.py` & `flexmeasures-0.9.4/flexmeasures/data/config.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/alembic.ini` & `flexmeasures-0.9.4/flexmeasures/data/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/env.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/env.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/01fe99da5716_initial.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/01fe99da5716_initial.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/02ddbbff29a7_naming_conventions.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/02ddbbff29a7_naming_conventions.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/038bab973c40_add_unique_constraint_for_sensor_names_.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/038bab973c40_add_unique_constraint_for_sensor_names_.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/04f0e2d2924a_add_source_id_as_primary_key_for_timed_beliefs.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/04f0e2d2924a_add_source_id_as_primary_key_for_timed_beliefs.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/11b735abebe7_create_power_table_and_drop_measurement_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/11b735abebe7_create_power_table_and_drop_measurement_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1a4f0e5c4b86_unique_userids_in_ds.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1a4f0e5c4b86_unique_userids_in_ds.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1ae32ffc8c3f_rename_data_source_unique_constraint.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1ae32ffc8c3f_rename_data_source_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1b64acf01809_forecasting_job_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1b64acf01809_forecasting_job_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1bcccdf0c3e1_unique_usernames.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1bcccdf0c3e1_unique_usernames.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/1e8d27922f56_create_price_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/1e8d27922f56_create_price_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/22ce09690d23_mix_in_timely_beliefs_sensor_with_asset_market_and_weather_sensor.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/22ce09690d23_mix_in_timely_beliefs_sensor_with_asset_market_and_weather_sensor.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/26373d8266db_owner_deletion_deletes_assets_and_power.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/26373d8266db_owner_deletion_deletes_assets_and_power.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/2c9a32614784_rename_data_source_columns_in_power_price_and_weather_tables.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/2c9a32614784_rename_data_source_columns_in_power_price_and_weather_tables.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/30f7b63069e1_delete_asset_if_sensor_is_deleted.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/30f7b63069e1_delete_asset_if_sensor_is_deleted.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/30fe2267e7d5_add_optional_DataSource_columns_for_model_and_version.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/30fe2267e7d5_add_optional_DataSource_columns_for_model_and_version.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/3d56402cde15_drop_login_columns_in_bvp_users_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/3d56402cde15_drop_login_columns_in_bvp_users_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/3db3e71d101d_make_datasource_a_subclass_of_timely_beliefs_beliefsource.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/3db3e71d101d_make_datasource_a_subclass_of_timely_beliefs_beliefsource.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/3e43d3274d16_Asset_soc_udi_event_id.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/3e43d3274d16_Asset_soc_udi_event_id.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/45d937300b0f_create_measurement_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/45d937300b0f_create_measurement_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/4b6cebbdf473_create_weather_sensor_type_and_weather_sensor_and_weather_tables.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/4b6cebbdf473_create_weather_sensor_type_and_weather_sensor_and_weather_tables.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/50cf294e007d_complete_adding_units_to_all_generic_asset_tables_and_display_names_to_all_generic_asset_tables_and_generic_asset_type_tables.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/50cf294e007d_complete_adding_units_to_all_generic_asset_tables_and_display_names_to_all_generic_asset_tables_and_generic_asset_type_tables.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/550a9020f1bf_default_resolution_for_existing_sensors.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/550a9020f1bf_default_resolution_for_existing_sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/564e8df4e3a9_stop_using_bvp_in_table_names.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/564e8df4e3a9_stop_using_bvp_in_table_names.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/565e092a6c5e_introduce_the_GenericAssetType_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/565e092a6c5e_introduce_the_GenericAssetType_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/5d39829d91af_create_data_sources_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/5d39829d91af_create_data_sources_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/61bfc6e45c4d_add_soc_columns_in_asset_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/61bfc6e45c4d_add_soc_columns_in_asset_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/6cf5b241b85f_copy_attributes_from_old_data_models_to_GenericAsset.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/6cf5b241b85f_copy_attributes_from_old_data_models_to_GenericAsset.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/7113b0f00678_drop_forecasting_jobs_table_and_make_display_names_nullable.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/7113b0f00678_drop_forecasting_jobs_table_and_make_display_names_nullable.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/7987667dbd43_add_asset_type_hover_label.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/7987667dbd43_add_asset_type_hover_label.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/7f8b8920355f_create_annotation_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/7f8b8920355f_create_annotation_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/830e72a8b218_migrate_sensor_relationships_for_power_price_weather.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/830e72a8b218_migrate_sensor_relationships_for_power_price_weather.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/8abe32ffa204_add_owner_id_column_in_asset_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/8abe32ffa204_add_owner_id_column_in_asset_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/8fcc5fec67bc_make_data_source_id_columns_primary_keys.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/8fcc5fec67bc_make_data_source_id_columns_primary_keys.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/91a938bfa5a8_add_horizon_columns_to_power_price_and_weather_tables.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/91a938bfa5a8_add_horizon_columns_to_power_price_and_weather_tables.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/9254559dcac2_create_market_type_and_market_tables.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/9254559dcac2_create_market_type_and_market_tables.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/96f2db5bed30_add_account_roles.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/96f2db5bed30_add_account_roles.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/994170c26bc6_add_account_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/994170c26bc6_add_account_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/9c7fc8e46f1e_add_location_columns_to_weather_sensor_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/9c7fc8e46f1e_add_location_columns_to_weather_sensor_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/a328412b4623_add_timezone_column_in_bvp_users_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/a328412b4623_add_timezone_column_in_bvp_users_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/a528c3c81506_unique_generic_sensor_ids.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/a528c3c81506_unique_generic_sensor_ids.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/a5b970eadb3b_time_series_indexes.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/a5b970eadb3b_time_series_indexes.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/a918360f7d63_add_unique_contraints_on_.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/a918360f7d63_add_unique_contraints_on_.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/ac2613fffc74_add_market_id_column_to_asset_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/ac2613fffc74_add_market_id_column_to_asset_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/b087ce8b529f_create_latest_task_run_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/b087ce8b529f_create_latest_task_run_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/b2b43f0eec40_weathersensors_unique_type_location.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/b2b43f0eec40_weathersensors_unique_type_location.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/b6d49ed7cceb_introduce_the_GenericAsset_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/b6d49ed7cceb_introduce_the_GenericAsset_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/b797328ac32d_add_user_fs_uniquifier_for_faster_auth_.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/b797328ac32d_add_user_fs_uniquifier_for_faster_auth_.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/bddc5e9f72a3_add_event_resolution_field_to_asset_.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/bddc5e9f72a3_add_event_resolution_field_to_asset_.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/d3440de27ab9_create_bvp_roles_and_bvp_users_and_bvp_roles_users_tables.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/d3440de27ab9_create_bvp_roles_and_bvp_users_and_bvp_roles_users_tables.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/db00b66be82c_add_horizon_columns_as_primary_keys.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/db00b66be82c_add_horizon_columns_as_primary_keys.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/db1f67336324_add_price_unit_and_display_name_columns_to_market_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/db1f67336324_add_price_unit_and_display_name_columns_to_market_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/e0c2f9aff251_rename_source_id_column_in_data_sources_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/e0c2f9aff251_rename_source_id_column_in_data_sources_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/e4c9cf837311_sensor_generic_asset_id_should_not_be_.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/e4c9cf837311_sensor_generic_asset_id_should_not_be_.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/e62ac5f519d7_create_table_for_timed_beliefs.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/e62ac5f519d7_create_table_for_timed_beliefs.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/migrations/versions/e690d373a3d9_copy_Power_Price_Weather_time_series_data_to_TimedBeliefs_table.py` & `flexmeasures-0.9.4/flexmeasures/data/migrations/versions/e690d373a3d9_copy_Power_Price_Weather_time_series_data_to_TimedBeliefs_table.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/annotations.py` & `flexmeasures-0.9.4/flexmeasures/data/models/annotations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/assets.py` & `flexmeasures-0.9.4/flexmeasures/data/models/assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/charts/__init__.py` & `flexmeasures-0.9.4/flexmeasures/data/models/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/charts/belief_charts.py` & `flexmeasures-0.9.4/flexmeasures/data/models/charts/belief_charts.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/charts/defaults.py` & `flexmeasures-0.9.4/flexmeasures/data/models/charts/defaults.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/data_sources.py` & `flexmeasures-0.9.4/flexmeasures/data/models/data_sources.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/forecasting/__init__.py` & `flexmeasures-0.9.4/flexmeasures/data/models/forecasting/__init__.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/forecasting/model_spec_factory.py` & `flexmeasures-0.9.4/flexmeasures/data/models/forecasting/model_spec_factory.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/forecasting/model_specs/linear_regression.py` & `flexmeasures-0.9.4/flexmeasures/data/models/forecasting/model_specs/linear_regression.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/forecasting/model_specs/naive.py` & `flexmeasures-0.9.4/flexmeasures/data/models/forecasting/model_specs/naive.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/forecasting/utils.py` & `flexmeasures-0.9.4/flexmeasures/data/models/forecasting/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/generic_assets.py` & `flexmeasures-0.9.4/flexmeasures/data/models/generic_assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/legacy_migration_utils.py` & `flexmeasures-0.9.4/flexmeasures/data/models/legacy_migration_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/markets.py` & `flexmeasures-0.9.4/flexmeasures/data/models/markets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/parsing_utils.py` & `flexmeasures-0.9.4/flexmeasures/data/models/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/planning/battery.py` & `flexmeasures-0.9.4/flexmeasures/data/models/planning/battery.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/planning/charging_station.py` & `flexmeasures-0.9.4/flexmeasures/data/models/planning/charging_station.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/planning/solver.py` & `flexmeasures-0.9.4/flexmeasures/data/models/planning/solver.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/planning/tests/test_solver.py` & `flexmeasures-0.9.4/flexmeasures/data/models/planning/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/planning/utils.py` & `flexmeasures-0.9.4/flexmeasures/data/models/planning/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/task_runs.py` & `flexmeasures-0.9.4/flexmeasures/data/models/task_runs.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/time_series.py` & `flexmeasures-0.9.4/flexmeasures/data/models/time_series.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/user.py` & `flexmeasures-0.9.4/flexmeasures/data/models/user.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/validation_utils.py` & `flexmeasures-0.9.4/flexmeasures/data/models/validation_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/models/weather.py` & `flexmeasures-0.9.4/flexmeasures/data/models/weather.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/queries/analytics.py` & `flexmeasures-0.9.4/flexmeasures/data/queries/analytics.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/queries/annotations.py` & `flexmeasures-0.9.4/flexmeasures/data/queries/annotations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/queries/data_sources.py` & `flexmeasures-0.9.4/flexmeasures/data/queries/data_sources.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/queries/generic_assets.py` & `flexmeasures-0.9.4/flexmeasures/data/queries/generic_assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/queries/portfolio.py` & `flexmeasures-0.9.4/flexmeasures/data/queries/portfolio.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/queries/sensors.py` & `flexmeasures-0.9.4/flexmeasures/data/queries/sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/queries/utils.py` & `flexmeasures-0.9.4/flexmeasures/data/queries/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/account.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/account.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/assets.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/generic_assets.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/generic_assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/sensors.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/sources.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/sources.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/tests/test_times.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/tests/test_times.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/times.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/times.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/units.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/units.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/users.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/users.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/schemas/utils.py` & `flexmeasures-0.9.4/flexmeasures/data/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/scripts/_test_simulation.py` & `flexmeasures-0.9.4/flexmeasures/data/scripts/_test_simulation.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/scripts/data_gen.py` & `flexmeasures-0.9.4/flexmeasures/data/scripts/data_gen.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/scripts/simulation_utils.py` & `flexmeasures-0.9.4/flexmeasures/data/scripts/simulation_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/scripts/visualize_data_model.py` & `flexmeasures-0.9.4/flexmeasures/data/scripts/visualize_data_model.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/services/asset_grouping.py` & `flexmeasures-0.9.4/flexmeasures/data/services/asset_grouping.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/services/forecasting.py` & `flexmeasures-0.9.4/flexmeasures/data/services/forecasting.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/services/resources.py` & `flexmeasures-0.9.4/flexmeasures/data/services/resources.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/services/scheduling.py` & `flexmeasures-0.9.4/flexmeasures/data/services/scheduling.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/services/sensors.py` & `flexmeasures-0.9.4/flexmeasures/data/services/sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/services/time_series.py` & `flexmeasures-0.9.4/flexmeasures/data/services/time_series.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/services/users.py` & `flexmeasures-0.9.4/flexmeasures/data/services/users.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/conftest.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/test_annotations.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/test_forecasting_jobs.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/test_forecasting_jobs.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/test_forecasting_jobs_fresh_db.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/test_forecasting_jobs_fresh_db.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/test_queries.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/test_scheduling_jobs.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/test_scheduling_jobs.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/test_scheduling_jobs_fresh_db.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/test_scheduling_jobs_fresh_db.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/test_sensor_queries.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/test_sensor_queries.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/test_time_series_services.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/test_time_series_services.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/test_user_services.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/test_user_services.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/data/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/transactional.py` & `flexmeasures-0.9.4/flexmeasures/data/transactional.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/data/utils.py` & `flexmeasures-0.9.4/flexmeasures/data/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/__init__.py` & `flexmeasures-0.9.4/flexmeasures/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/charts/latest_state.py` & `flexmeasures-0.9.4/flexmeasures/ui/charts/latest_state.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/crud/api_wrapper.py` & `flexmeasures-0.9.4/flexmeasures/ui/crud/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/crud/assets.py` & `flexmeasures-0.9.4/flexmeasures/ui/crud/assets.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/crud/users.py` & `flexmeasures-0.9.4/flexmeasures/ui/crud/users.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/error_handlers.py` & `flexmeasures-0.9.4/flexmeasures/ui/error_handlers.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/external/rq-dashboard-bootstrap.min.css` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/external/rq-dashboard-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/external/weather-icons.min.css` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/external/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/flexmeasures.css` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/flexmeasures.css`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.eot` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.svg` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.ttf` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.woff` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/font/weathericons-regular-webfont.woff2` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/font/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/FontAwesome.otf` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.eot` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.svg` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.ttf` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.woff` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/fontawesome-webfont.woff2` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.eot` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.svg` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.ttf` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.woff` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.woff2` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings-white.png` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/css/fonts/glyphicons-halflings.png` & `flexmeasures-0.9.4/flexmeasures/ui/static/css/fonts/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/favicon.ico` & `flexmeasures-0.9.4/flexmeasures/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.eot` & `flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.eot`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.svg` & `flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.svg`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.ttf` & `flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.ttf`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.woff` & `flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.woff`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/font/seita-webfont.woff2` & `flexmeasures-0.9.4/flexmeasures/ui/static/font/seita-webfont.woff2`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/images/chase-lewis-506404-unsplash.jpg` & `flexmeasures-0.9.4/flexmeasures/ui/static/images/chase-lewis-506404-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/images/flexmeasures-preview.jpg` & `flexmeasures-0.9.4/flexmeasures/ui/static/images/flexmeasures-preview.jpg`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/images/tj-k-349056-unsplash.jpg` & `flexmeasures-0.9.4/flexmeasures/ui/static/images/tj-k-349056-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/js/daterange-utils.js` & `flexmeasures-0.9.4/flexmeasures/ui/static/js/daterange-utils.js`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/js/daterangepicker-init.js` & `flexmeasures-0.9.4/flexmeasures/ui/static/js/daterangepicker-init.js`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/js/flexmeasures.js` & `flexmeasures-0.9.4/flexmeasures/ui/static/js/flexmeasures.js`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/static/js/map-init.js` & `flexmeasures-0.9.4/flexmeasures/ui/static/js/map-init.js`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/admin/forgot_password.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/admin/forgot_password.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/admin/logged_in_user.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/admin/logged_in_user.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/admin/login_user.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/admin/login_user.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/admin/reset_password.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/admin/reset_password.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/admin/upload.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/admin/upload.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/base.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/base.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/crud/asset.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/crud/asset.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/crud/asset_new.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/crud/asset_new.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/crud/assets.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/crud/assets.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/crud/user.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/crud/user.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/crud/users.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/crud/users.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/defaults.jinja` & `flexmeasures-0.9.4/flexmeasures/ui/templates/defaults.jinja`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/error.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/error.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/rq_dashboard/base.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/rq_dashboard/base.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/rq_dashboard/dashboard.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/rq_dashboard/dashboard.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/views/analytics.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/views/analytics.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/views/control.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/views/control.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/views/dashboard.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/views/dashboard.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/views/new_dashboard.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/views/new_dashboard.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/views/portfolio.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/views/portfolio.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/templates/views/sensors.html` & `flexmeasures-0.9.4/flexmeasures/ui/templates/views/sensors.html`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/tests/conftest.py` & `flexmeasures-0.9.4/flexmeasures/ui/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/tests/test_asset_crud.py` & `flexmeasures-0.9.4/flexmeasures/ui/tests/test_asset_crud.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/tests/test_error_handling.py` & `flexmeasures-0.9.4/flexmeasures/ui/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/tests/test_user_crud.py` & `flexmeasures-0.9.4/flexmeasures/ui/tests/test_user_crud.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/tests/test_views.py` & `flexmeasures-0.9.4/flexmeasures/ui/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/tests/utils.py` & `flexmeasures-0.9.4/flexmeasures/ui/tests/utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/utils/plotting_utils.py` & `flexmeasures-0.9.4/flexmeasures/ui/utils/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/utils/view_utils.py` & `flexmeasures-0.9.4/flexmeasures/ui/utils/view_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/__init__.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/__init__.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/analytics.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/analytics.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/charts.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/charts.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/control.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/control.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/dashboard.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/logged_in_user.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/logged_in_user.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/new_dashboard.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/new_dashboard.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/portfolio.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/portfolio.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/sensors.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/sensors.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/ui/views/state.py` & `flexmeasures-0.9.4/flexmeasures/ui/views/state.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/app_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/app_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/calculations.py` & `flexmeasures-0.9.4/flexmeasures/utils/calculations.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/coding_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/coding_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/config_defaults.py` & `flexmeasures-0.9.4/flexmeasures/utils/config_defaults.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/config_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/entity_address_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/entity_address_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/error_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/error_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/flexmeasures_inflection.py` & `flexmeasures-0.9.4/flexmeasures/utils/flexmeasures_inflection.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/geo_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/geo_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/grid_cells.py` & `flexmeasures-0.9.4/flexmeasures/utils/grid_cells.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/plugin_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/tests/test_entity_address_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/tests/test_entity_address_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/tests/test_time_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/tests/test_unit_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/tests/test_unit_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
         ("KRW/kWh", False),
         ("kWh", False),
         ("kW", True),
         ("watt", True),
         ("°C", False),
         ("", False),
         ("not-a-unit", False),
+        ("#", False),
     ],
 )
 def test_is_power_unit(unit: str, power_unit: bool):
     assert is_power_unit(unit) is power_unit
 
 
 @pytest.mark.parametrize(
```

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/time_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures/utils/unit_utils.py` & `flexmeasures-0.9.4/flexmeasures/utils/unit_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     return x
 
 
 def is_valid_unit(unit: str) -> bool:
     """Return True if the pint library can work with this unit identifier."""
     try:
         ur.Quantity(unit)
-    except ValueError:
-        return False
-    except pint.errors.UndefinedUnitError:
+    except Exception:  # noqa B902
+        # in practice, we encountered pint.errors.UndefinedUnitError, ValueError and AttributeError,
+        # but since there may be more, here we simply catch them all
         return False
     return True
 
 
 def determine_unit_conversion_multiplier(
     from_unit: str, to_unit: str, duration: Optional[timedelta] = None
 ):
```

### Comparing `flexmeasures-0.9.3/flexmeasures.egg-info/PKG-INFO` & `flexmeasures-0.9.4/flexmeasures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexmeasures
-Version: 0.9.3
+Version: 0.9.4
 Summary: The *FlexMeasures Platform* is the intelligent backend to support real-time energy flexibility apps, rapidly and scalable.
 Home-page: https://github.com/seitabv/flexmeasures
 Author: Seita BV
 Author-email: nicolas@seita.nl
 License: Apache2.0
 Keywords: smart grid,renewables,balancing,forecasting,scheduling
 Platform: UNKNOWN
```

### Comparing `flexmeasures-0.9.3/flexmeasures.egg-info/SOURCES.txt` & `flexmeasures-0.9.4/flexmeasures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/flexmeasures.egg-info/requires.txt` & `flexmeasures-0.9.4/flexmeasures.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/requirements/Readme.md` & `flexmeasures-0.9.4/requirements/Readme.md`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/requirements/app.in` & `flexmeasures-0.9.4/requirements/app.in`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/requirements/app.txt` & `flexmeasures-0.9.4/requirements/app.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/requirements/dev.txt` & `flexmeasures-0.9.4/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/requirements/docs.txt` & `flexmeasures-0.9.4/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/requirements/test.txt` & `flexmeasures-0.9.4/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/setup.py` & `flexmeasures-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-0.9.3/to_pypi.sh` & `flexmeasures-0.9.4/to_pypi.sh`

 * *Files identical despite different names*

