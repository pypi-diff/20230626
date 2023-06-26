# Comparing `tmp/ewah-0.8.84.tar.gz` & `tmp/ewah-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewah-0.8.84.tar", last modified: Mon Jun 26 07:26:16 2023, max compression
+gzip compressed data, was "ewah-0.8.9.tar", last modified: Sun Jan 16 21:03:09 2022, max compression
```

## Comparing `ewah-0.8.84.tar` & `ewah-0.8.9.tar`

### file list

```diff
@@ -1,125 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:26:16.641318 ewah-0.8.84/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 07:25:53.000000 ewah-0.8.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19612 2023-06-26 07:26:16.641318 ewah-0.8.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-26 07:25:53.000000 ewah-0.8.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:26:16.625318 ewah-0.8.84/ewah/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/cleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:26:16.625318 ewah-0.8.84/ewah/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:26:16.625318 ewah-0.8.84/ewah/dag_factories/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/dag_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/dag_factories/dag_factory_atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)    17844 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/dag_factories/dag_factory_idempotent.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/dag_factories/dag_factory_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/dag_factories/dbt_dag_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:26:16.633318 ewah-0.8.84/ewah/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/aircall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/airtable.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/amazon_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)    32285 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/amazon_seller_central.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/braze.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/dbt_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/google_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/google_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/google_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/hubspot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/infigo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/linkedin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/metabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/mssql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/personio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/pipedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/plentymarkets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/rapidmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/recurly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/sevdesk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/shopify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/hooks/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:26:16.641318 ewah-0.8.84/ewah/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/aircall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/airtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/amazon_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/amazon_seller_central.py
--rw-r--r--   0 runner    (1001) docker     (123)    25319 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/braze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/google_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/google_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/google_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/google_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/google_sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/hubspot.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/infigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/linkedin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/linkedin_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/mailingwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/personio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/pipedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/plentymarkets.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/rapidmail.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/recurly.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/sevdesk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/shopify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/sql_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/sql_mssql.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/sql_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/sql_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/sql_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/operators/zendesk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:26:16.641318 ewah-0.8.84/ewah/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/uploaders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21566 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/uploaders/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/uploaders/google_sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/uploaders/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/uploaders/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:26:16.641318 ewah-0.8.84/ewah/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/airflow_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/dbt_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/email_data_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/git_pull_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/log_cleanup_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/run_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-26 07:25:53.000000 ewah-0.8.84/ewah/utils/yml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:26:16.625318 ewah-0.8.84/ewah.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19612 2023-06-26 07:26:15.000000 ewah-0.8.84/ewah.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-26 07:26:16.000000 ewah-0.8.84/ewah.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:26:15.000000 ewah-0.8.84/ewah.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 07:26:15.000000 ewah-0.8.84/ewah.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-26 07:26:15.000000 ewah-0.8.84/ewah.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 07:26:15.000000 ewah-0.8.84/ewah.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 07:26:16.645318 ewah-0.8.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-26 07:25:53.000000 ewah-0.8.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:09.983773 ewah-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-01-16 21:03:00.000000 ewah-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    19644 2022-01-16 21:03:09.983773 ewah-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    16351 2022-01-16 21:03:00.000000 ewah-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:09.975773 ewah-0.8.9/ewah/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9707 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/cleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:09.975773 ewah-0.8.9/ewah/constants/
+-rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:09.975773 ewah-0.8.9/ewah/dag_factories/
+-rw-r--r--   0 runner    (1001) docker     (121)     5334 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/dag_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5925 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/dag_factories/dag_factory_atomic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17842 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/dag_factories/dag_factory_idempotent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12967 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/dag_factories/dag_factory_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7513 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/dag_factories/dbt_dag_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:09.979773 ewah-0.8.9/ewah/hooks/
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/aircall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/aws.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4591 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6562 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/braze.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5015 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5114 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/google_ads.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8116 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/google_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/google_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11067 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/hubspot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/infigo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6482 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/pipedrive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9226 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/plentymarkets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/rapidmail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/recurly.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7892 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4341 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3405 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5507 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/hooks/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:09.983773 ewah-0.8.9/ewah/operators/
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/aircall.py
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23227 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/braze.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/fx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/google_ads.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3894 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/google_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/google_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/google_maps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4935 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/google_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/hubspot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/infigo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4844 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/mailingwork.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3643 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/pipedrive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/plentymarkets.py
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/rapidmail.py
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/recurly.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12081 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15884 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/shopify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4037 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      783 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/sql_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/sql_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/sql_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/sql_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6773 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/operators/zendesk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:09.983773 ewah-0.8.9/ewah/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11526 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/uploaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18080 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/uploaders/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5360 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/uploaders/google_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9703 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/uploaders/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12084 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/uploaders/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:09.983773 ewah-0.8.9/ewah/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/airflow_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11981 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/dbt_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2947 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/email_data_dag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/git_pull_dag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4402 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/log_cleanup_dag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/run_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-01-16 21:03:00.000000 ewah-0.8.9/ewah/utils/yml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 21:03:09.975773 ewah-0.8.9/ewah.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    19644 2022-01-16 21:03:09.000000 ewah-0.8.9/ewah.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2532 2022-01-16 21:03:09.000000 ewah-0.8.9/ewah.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-16 21:03:09.000000 ewah-0.8.9/ewah.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-01-16 21:03:09.000000 ewah-0.8.9/ewah.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-01-16 21:03:09.000000 ewah-0.8.9/ewah.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-16 21:03:09.000000 ewah-0.8.9/ewah.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-01-16 21:03:09.983773 ewah-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-01-16 21:03:00.000000 ewah-0.8.9/setup.py
```

### Comparing `ewah-0.8.84/LICENSE` & `ewah-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/PKG-INFO` & `ewah-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: ewah
-Version: 0.8.84
+Version: 0.8.9
 Summary: An ELT with airflow helper module: Ewah
 Home-page: https://gemmaanalytics.com/
 Author: Bijan Soltani
 Author-email: bijan.soltani+ewah@gemmaanalytics.com
 License: UNKNOWN
 Description: # ewah
         Ewah: ELT With Airflow Helper - Classes and functions to make apache airflow life easier.
         
         Functions to create all DAGs required for ELT using only a simple config file.
         
         ## DWHs Implemented
         - Snowflake
         - PostgreSQL
+        
+        ## DWHs Planned
         - Bigquery
         
         ## Operators
         
         EWAH currently supports the following operators:
         
         - Aircall
```

### Comparing `ewah-0.8.84/README.md` & `ewah-0.8.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Ewah: ELT With Airflow Helper - Classes and functions to make apache airflow life easier.
 
 Functions to create all DAGs required for ELT using only a simple config file.
 
 ## DWHs Implemented
 - Snowflake
 - PostgreSQL
+
+## DWHs Planned
 - Bigquery
 
 ## Operators
 
 EWAH currently supports the following operators:
 
 - Aircall
```

### Comparing `ewah-0.8.84/ewah/cleaner.py` & `ewah-0.8.9/ewah/cleaner.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,79 +101,61 @@
     Derive from this class to extend functionalities.
     """
 
     def __init__(
         self,
         default_row: Optional[Dict[str, Any]] = None,
         add_metadata: bool = False,
-        include_columns: Optional[List[str]] = None,
         exclude_columns: Optional[List[str]] = None,
         hash_columns: Optional[List[str]] = None,
-        hash_salt: Optional[str] = None,
         rename_columns: Optional[Dict[str, str]] = None,
         additional_callables: Optional[Union[List[Callable], Callable]] = None,
         json_encoder: type = EWAHJSONEncoder,
     ):
         super().__init__()
 
         cleaning_steps = []
 
-        if include_columns:
-            cleaning_steps.append(self._include_columns)
-            self.include_columns = include_columns
-
-        if include_columns and exclude_columns:
-            _msg = "Don't use include and exclude columns config at the same time!"
-            raise Exception(_msg)
-
         if exclude_columns:
             cleaning_steps.append(self._exclude_columns)
             self.exclude_columns = exclude_columns
 
         if rename_columns:
             cleaning_steps.append(self._rename_columns)
             self.rename_columns = rename_columns
 
         if hash_columns:
             cleaning_steps.append(self._hash_row)
             self.hash_columns = hash_columns
 
         if add_metadata:
             cleaning_steps.append(self._add_metadata)
-        self.add_metadata = add_metadata
+            self.add_metadata = add_metadata
 
         if additional_callables:
             if callable(additional_callables):
                 cleaning_steps.append(additional_callables)
             else:
                 cleaning_steps += additional_callables
 
         # Clean values right at the end
         cleaning_steps.append(self.clean_values)
 
         self.cleaning_steps = cleaning_steps
-        self.hash_salt = hash_salt or ""
         self.default_row = default_row or {}
         self.json_encoder = json_encoder
 
         if default_row:
             # initialize with defaults
             self.fields_definition = {
                 field: type(value) for field, value in default_row.items()
             }
         else:
             self.fields_definition = {}
 
-    def _include_columns(self, row):
-        tmp_row = {}
-        for column in self.include_columns:
-            if column in row:
-                tmp_row[column] = row[column]
-        return tmp_row
-
     def _exclude_columns(self, row):
         for column in self.exclude_columns:
             row.pop(column, None)
         return row
 
     def _add_metadata(self, row):
         row.update(self.metadata)
@@ -185,19 +167,20 @@
         return row
 
     def _hash_row(self, row):
         for column in self.hash_columns:
             row[column] = self._hash_value(row.get(column))
         return row
 
-    def _hash_value(self, value):
+    @staticmethod
+    def _hash_value(value):
         # Overwrite function for any other desired hashing behavior
         if value is None:
             return None
-        return sha256((str(value) + str(self.hash_salt)).encode()).hexdigest()
+        return sha256(str(value).encode()).hexdigest()
 
     def clean_rows(
         self, rows: List[Dict[str, Any]], metadata: Optional[Dict[str, Any]] = None
     ) -> List[Dict[str, Any]]:
         cleaned_rows = []
         self.log.info("Cleaning {0} rows of data!".format(str(len(rows))))
         if self.add_metadata:
@@ -210,15 +193,15 @@
         row = deepcopy(self.default_row)
         # Note: Destructive iteration using raw_row.popitem() causes a reversed order!
         # --> create a list of tuples first and then destructively iterate over it.
         key_value_pairs = list(raw_row.items())
         while key_value_pairs:
             key, value = key_value_pairs.pop(0)
             if not value is None:
-                value_type = None  # May be set during the type change below
+                value_type = None # May be set during the type change below
                 if isinstance(value, str):
                     if value == "\0":
                         # This is a null value -> treat as None
                         value = row.get(key)  # Use default, if exists
                     else:
                         # Some database systems don't handle this character well
                         # Thus, remove it
@@ -236,15 +219,15 @@
                         # Refactor this, PLEASE!
                         value = dumps(value)
                 elif isinstance(value, Decimal):
                     value = float(value)
                 row[key] = value
 
                 # Set the fields_definition for the key
-                value_type = value_type or type(value)  # set now if not done above
+                value_type = value_type or type(value) # set now if not done above
                 current_type_set = self.fields_definition.get(key)
                 if current_type_set:
                     if (
                         not current_type_set == value_type
                         and not current_type_set == str
                     ):
                         # TODO: make this flexible
```

### Comparing `ewah-0.8.84/ewah/constants/__init__.py` & `ewah-0.8.9/ewah/constants/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,37 +77,35 @@
             frozenset: "jsonb",
             bool: "boolean",
             datetime: "timestamp with time zone",
             date: "date",
             timedelta: "interval",
         },
         DWH_ENGINE_SNOWFLAKE: {
-            str: "TEXT",
-            int: "FLOAT",  # Temporary fix - need to implement dynamic data type changes
-            float: "FLOAT",
+            str: "VARCHAR",
+            int: "NUMBER",
+            float: "NUMBER",
             dict: "OBJECT",
             list: "ARRAY",
             tuple: "ARRAY",
             set: "ARRAY",
             frozenset: "ARRAY",
             bool: "BOOLEAN",
             datetime: "TIMESTAMP_TZ",
             date: "DATE",
         },
         DWH_ENGINE_BIGQUERY: {
             str: "STRING",
             int: "INT64",
-            float: "FLOAT64",
-            # Cannot use struct as data type because if there is any difference
-            # in the structure of the mapping types, BigQuery loading will fail
-            dict: "STRING",  # "STRUCT",
-            list: "STRING",  # "STRUCT",
-            tuple: "STRING",  # "STRUCT",
-            set: "STRING",  # "STRUCT",
-            frozenset: "STRING",  # "STRUCT",
+            float: "NUMERIC",
+            dict: "STRUCT",
+            list: "STRUCT",
+            tuple: "STRUCT",
+            set: "STRUCT",
+            frozenset: "STRUCT",
             bool: "BOOL",
             datetime: "TIMESTAMP",
             date: "DATE",
             bytes: "BYTES",
         },
         # DWH_ENGINE_REDSHIFT: {},
         # DWH_ENGINE_S3: {},
```

### Comparing `ewah-0.8.84/ewah/dag_factories/__init__.py` & `ewah-0.8.9/ewah/dag_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/dag_factories/dag_factory_atomic.py` & `ewah-0.8.9/ewah/dag_factories/dag_factory_atomic.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from ewah.constants import EWAHConstants as EC
 from ewah.utils.airflow_utils import datetime_utcnow_with_tz
 from ewah.operators.base import EWAHBaseOperator
 from ewah.uploaders import get_uploader
 
 from collections.abc import Iterable
 from copy import deepcopy
-from croniter import croniter
 from datetime import datetime, timedelta
 from typing import Optional, Type, Callable, List, Tuple, Union
 
 import re
 
 
 def dag_factory_atomic(
@@ -21,15 +20,15 @@
     start_date: datetime,
     el_operator: Type[EWAHBaseOperator],
     operator_config: dict,
     target_schema_name: str,
     target_schema_suffix: str = "_next",
     target_database_name: Optional[str] = None,
     default_args: Optional[dict] = None,
-    schedule_interval: Union[str, timedelta] = timedelta(days=1),
+    schedule_interval: timedelta = timedelta(days=1),
     end_date: Optional[datetime] = None,
     read_right_users: Optional[Union[List[str], str]] = None,
     additional_dag_args: Optional[dict] = None,
     additional_task_args: Optional[dict] = None,
     logging_func: Optional[Callable] = None,
     dagrun_timeout_factor: Optional[float] = None,
     task_timeout_factor: Optional[float] = None,
@@ -49,48 +48,32 @@
 
     if not read_right_users is None:
         if isinstance(read_right_users, str):
             read_right_users = [u.strip() for u in read_right_users.split(",")]
         if not isinstance(read_right_users, Iterable):
             raise_exception("read_right_users must be an iterable or string!")
 
-    if isinstance(schedule_interval, str):
-        # Allow using cron-style schedule intervals
-        catchup = False
-        assert croniter.is_valid(
-            schedule_interval
-        ), "schedule_interval is neither timedelta nor not valid cron!"
+    # fake catchup = True: between start_date and end_date is only one schedule_interval
+    # --> run the full refreshs every schedule_interval at the same time instead of
+    # having a drift in execution time!
+    if end_date:
+        end_date = min(end_date, datetime_utcnow_with_tz())
     else:
-        assert isinstance(
-            schedule_interval, timedelta
-        ), "schedule_interval must be cron-string or timedelta!"
-
-        catchup = True
-        # fake catchup = True: between start_date and end_date is one schedule_interval
-        # --> run the full refreshs every schedule_interval at the same time instead of
-        # having a drift in execution time!
-        if end_date:
-            end_date = min(end_date, datetime_utcnow_with_tz())
-        else:
-            end_date = datetime_utcnow_with_tz()
-
-        start_date += (
-            int((end_date - start_date) / schedule_interval) - 1
-        ) * schedule_interval
-
-        # case 1: end_date = start_date + schedule_interval
+        end_date = datetime_utcnow_with_tz()
+    start_date += int((end_date - start_date) / schedule_interval) * schedule_interval
+    if start_date == end_date:
         # if the division result is a precise integer, that implies a definite end_date
         # --> adjust to get exactly one schedule_interval delta between start_date and
         # end_date to have one last run available (that should have run before end_date)
-
-        # case 2: end_date > (start_date + schedule_interval)
+        start_date -= schedule_interval
+    else:
         # Airflow executes after data_interval_end - start_date has to be
         # between exactly 1 and below 2 time schedule_interval before end_date!
         # end_date - 2*schedule_interval < start_date <= end_date - schedule_interval
-
+        start_date -= schedule_interval
         # Make sure only one execution every runs scheduled but manual triggers work!
         end_date = start_date + 2 * schedule_interval - timedelta(seconds=1)
 
     if dagrun_timeout_factor:
         _msg = "dagrun_timeout_factor must be a number between 0 and 1!"
         assert isinstance(dagrun_timeout_factor, (int, float)) and (
             0 < dagrun_timeout_factor <= 1
@@ -102,15 +85,15 @@
     if task_timeout_factor:
         additional_task_args["execution_timeout"] = additional_task_args.get(
             "execution_timeout", task_timeout_factor * schedule_interval
         )
 
     dag = DAG(
         dag_name,
-        catchup=catchup,
+        catchup=True,  # See above
         default_args=default_args,
         max_active_runs=1,
         schedule_interval=schedule_interval,
         start_date=start_date,
         end_date=end_date,
         **additional_dag_args,
     )
@@ -134,17 +117,16 @@
             table_config.update(operator_config["tables"][table] or {})
             table_config.update(
                 {
                     "task_id": "extract_load_" + re.sub(r"[^a-zA-Z0-9_]", "", table),
                     "dwh_engine": dwh_engine,
                     "dwh_conn_id": dwh_conn_id,
                     "extract_strategy": table_config.get(  # Default to full refresh
-                        "extract_strategy", None
-                    )
-                    or EC.ES_FULL_REFRESH,  # value can be given as None in table conf
+                        "extract_strategy", EC.ES_FULL_REFRESH
+                    ),
                     "target_table_name": operator_config["tables"][table].get(
                         "target_table_name", table
                     ),
                     "target_schema_name": target_schema_name,
                     "target_schema_suffix": target_schema_suffix,
                     "target_database_name": target_database_name,
                 }
```

### Comparing `ewah-0.8.84/ewah/dag_factories/dag_factory_idempotent.py` & `ewah-0.8.9/ewah/dag_factories/dag_factory_idempotent.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             "execution_timeout", task_timeout_factor * schedule_interval_future
         )
         execution_timeout_backfill = additional_task_args.pop(
             "execution_timeout", task_timeout_factor * schedule_interval_backfill
         )
     else:
         execution_timeout = additional_task_args.get("execution_timeout")
-        execution_timeout_backfill = additional_task_args.pop("execution_timeout", None)
+        execution_timeout_backfill = additional_task_args.pop(execution_timeout, None)
 
     dags = (
         DAG(  # Current DAG
             dag_name + "_Idempotent",
             start_date=switch_absolute_date,
             end_date=end_date,
             schedule_interval=schedule_interval_future,
```

### Comparing `ewah-0.8.84/ewah/dag_factories/dag_factory_mixed.py` & `ewah-0.8.9/ewah/dag_factories/dag_factory_mixed.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/dag_factories/dbt_dag_factory.py` & `ewah-0.8.9/ewah/dag_factories/dbt_dag_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,78 @@
 from airflow import DAG
 
 from ewah.constants import EWAHConstants as EC
 from ewah.utils.airflow_utils import EWAHSqlSensor, datetime_utcnow_with_tz
 from ewah.utils.dbt_operator import EWAHdbtOperator
 
-from croniter import croniter
 from datetime import datetime, timedelta
-from typing import Union
 
 import pytz
 
 
 def dbt_dags_factory(
     airflow_conn_id,
     repo_type,
     dwh_engine,
     dwh_conn_id,
     database_name=None,
     git_conn_id=None,  # if provided, expecting private SSH key in conn extra
     local_path=None,
-    dbt_version=None,  # Defaults to require-dbt-version in dbt_project.yml
+    dbt_version="0.18.1",
     subfolder=None,  # optional: supply if dbt project is in a subfolder
     threads=4,  # see https://docs.getdbt.com/dbt-cli/configure-your-profile/#understanding-threads
     schema_name="analytics",  # see https://docs.getdbt.com/dbt-cli/configure-your-profile/#understanding-target-schemas
     keepalives_idle=0,  # see https://docs.getdbt.com/reference/warehouse-profiles/postgres-profile/
     dag_base_name="T_dbt_run",
-    schedule_interval: Union[str, timedelta] = timedelta(hours=1),
+    schedule_interval=timedelta(hours=1),
     start_date=datetime(2019, 1, 1),
     default_args=None,
     run_flags=None,  # e.g. --model tag:base
-    seed_flags=None,
     project=None,  # BigQuery alias
     dataset=None,  # BigQuery alias
     dagrun_timeout_factor=None,  # doesn't apply to full refresh
     task_timeout_factor=0.8,  # doesn't apply to full refresh
     metabase_conn_id=None,  # push docs to Metabase after full refresh run if exists
-    env_var_conn_ids=None,
 ):
     run_flags = run_flags or ""  # use empty string instead of None
-    seed_flags = seed_flags or ""
 
     # only PostgreSQL & Snowflake implemented as of now!
     assert dwh_engine in (
         EC.DWH_ENGINE_POSTGRES,
         EC.DWH_ENGINE_SNOWFLAKE,
         EC.DWH_ENGINE_BIGQUERY,
     )
 
-    if isinstance(schedule_interval, str):
-        # Allow using cron-style schedule intervals
-        assert croniter.is_valid(
-            schedule_interval
-        ), "schedule_interval is neither timedelta nor not valid cron!"
-        catchup = False
-        end_date = None
-    else:
-        # if start_date is timezone offset-naive, assume utc and turn into offset-aware
-        catchup = True
-        if not start_date.tzinfo:
-            start_date = start_date.replace(tzinfo=pytz.utc)
-
-        start_date += (
-            int((datetime_utcnow_with_tz() - start_date) / schedule_interval) - 1
-        ) * schedule_interval
-        end_date = start_date + 2 * schedule_interval - timedelta(seconds=1)
+    # if start_date is timezone offset-naive, assume utc and turn into offset-aware
+    if not start_date.tzinfo:
+        start_date = start_date.replace(tzinfo=pytz.utc)
+
+    start_date += (
+        int((datetime_utcnow_with_tz() - start_date) / schedule_interval) - 1
+    ) * schedule_interval
+    end_date = start_date + 2 * schedule_interval - timedelta(seconds=1)
 
     dag_kwargs = {
-        "catchup": catchup,
+        "catchup": True,
         "start_date": start_date,
         "end_date": end_date,
         "default_args": default_args,
         "max_active_runs": 1,
     }
 
-    if dagrun_timeout_factor and isinstance(schedule_interval, timedelta):
+    if dagrun_timeout_factor:
         _msg = "dagrun_timeout_factor must be a number between 0 and 1!"
         assert isinstance(dagrun_timeout_factor, (int, float)) and (
             0 < dagrun_timeout_factor <= 1
         ), _msg
         dagrun_timeout = dagrun_timeout_factor * schedule_interval
     else:
         dagrun_timeout = None
 
-    if task_timeout_factor and isinstance(schedule_interval, timedelta):
+    if task_timeout_factor:
         _msg = "task_timeout_factor must be a number between 0 and 1!"
         assert isinstance(task_timeout_factor, (int, float)) and (
             0 < task_timeout_factor <= 1
         ), _msg
         execution_timeout = task_timeout_factor * schedule_interval
     else:
         execution_timeout = None
@@ -103,22 +89,19 @@
         SELECT
             -- only succeed if there is no other running DagRun
             CASE WHEN COUNT(*) = 0 THEN 1 ELSE 0 END
         FROM public.dag_run
         WHERE dag_id IN ('{0}', '{1}')
           AND state = 'running'
           AND data_interval_end < '{2}' -- DagRun's data_interval_end
-          AND NOT (run_id = '{3}' AND dag_id = '{4}')
           -- Note: data_interval_end = data_interval_start if run_type = 'manual'
     """.format(
         dag_1._dag_id,
         dag_2._dag_id,
         "{{ data_interval_end }}",
-        "{{ run_id }}",
-        "{{ dag._dag_id }}",
     )
 
     snsr_1 = EWAHSqlSensor(
         task_id="sense_dbt_conflict_avoided",
         conn_id=airflow_conn_id,
         sql=sensor_sql,
         poke_interval=5 * 60,
@@ -144,50 +127,41 @@
         "threads": threads,
         "schema_name": schema_name,
         "keepalives_idle": 0,
         "dwh_engine": dwh_engine,
         "database_name": database_name,
         "project": project,
         "dataset": dataset,
-        "env_var_conn_ids": env_var_conn_ids,
     }
 
     run_1 = EWAHdbtOperator(
         task_id="dbt_run",
-        dbt_commands=[f"seed {seed_flags}", f"run {run_flags}"],
+        dbt_commands=["seed", f"run {run_flags}"],
         dag=dag_1,
         execution_timeout=execution_timeout,
         **dbt_kwargs,
     )
     run_2 = EWAHdbtOperator(
         task_id="dbt_run",
-        dbt_commands=[
-            f"seed --full-refresh {seed_flags}",
-            f"run --full-refresh {run_flags}",
-        ],
+        dbt_commands=["seed --full-refresh", f"run --full-refresh {run_flags}"],
         dag=dag_2,
         # If metabase_conn_id exists, push dbt docs to Metabase after full refresh run
         metabase_conn_id=metabase_conn_id,
         **dbt_kwargs,
     )
 
-    run_flags_freshness = (
-        run_flags.replace("--models", "--select")
-        .replace("--model", "--select")
-        .replace("-m ", "-s ")
-    )
     test_1 = EWAHdbtOperator(
         task_id="dbt_test",
-        dbt_commands=[f"test {run_flags}", f"source freshness {run_flags_freshness}"],
+        dbt_commands="test",
         dag=dag_1,
         execution_timeout=execution_timeout,
         **dbt_kwargs,
     )
     test_2 = EWAHdbtOperator(
-        task_id="dbt_test", dbt_commands=f"test {run_flags}", dag=dag_2, **dbt_kwargs
+        task_id="dbt_test", dbt_commands="test", dag=dag_2, **dbt_kwargs
     )
 
     snsr_1 >> run_1 >> test_1
     snsr_2 >> run_2 >> test_2
 
     return (dag_1, dag_2)
 
@@ -195,49 +169,39 @@
 def dbt_snapshot_dag(
     dwh_engine,
     dwh_conn_id,
     repo_type="git",
     database_name=None,
     git_conn_id=None,
     local_path=None,
-    dbt_version=None,
+    dbt_version="0.18.1",
     subfolder=None,
     threads=4,
     schema_name="analytics",  # for the profiles.yml
     keepalives_idle=0,
     dag_name="T_dbt_snapshots",
-    schedule_interval: Union[str, timedelta] = timedelta(hours=1),
+    schedule_interval=timedelta(hours=1),
     start_date=None,
     default_args=None,
     dagrun_timeout_factor=None,
     task_timeout_factor=0.8,
-    project=None,  # BigQuery alias
-    dataset=None,  # BigQuery alias
-    run_flags=None,
-    env_var_conn_ids=None,
 ):
-    run_flags = run_flags or ""
-
     # only PostgreSQL & Snowflake implemented as of now!
-    assert dwh_engine in (
-        EC.DWH_ENGINE_POSTGRES,
-        EC.DWH_ENGINE_SNOWFLAKE,
-        EC.DWH_ENGINE_BIGQUERY,
-    )
+    assert dwh_engine in (EC.DWH_ENGINE_POSTGRES, EC.DWH_ENGINE_SNOWFLAKE)
 
-    if dagrun_timeout_factor and isinstance(schedule_interval, timedelta):
+    if dagrun_timeout_factor:
         _msg = "dagrun_timeout_factor must be a number between 0 and 1!"
         assert isinstance(dagrun_timeout_factor, (int, float)) and (
             0 < dagrun_timeout_factor <= 1
         ), _msg
         dagrun_timeout = dagrun_timeout_factor * schedule_interval
     else:  # In case of 0 set to None
         dagrun_timeout = None
 
-    if task_timeout_factor and isinstance(schedule_interval, timedelta):
+    if task_timeout_factor:
         _msg = "dagrun_timeout_factor must be a number between 0 and 1!"
         assert isinstance(task_timeout_factor, (int, float)) and (
             0 < task_timeout_factor <= 1
         ), _msg
         execution_timeout = task_timeout_factor * schedule_interval
     else:
         execution_timeout = None
@@ -251,26 +215,23 @@
         default_args=default_args,
         dagrun_timeout=dagrun_timeout,
     )
 
     task = EWAHdbtOperator(
         dag=dag,
         task_id="dbt_snapshot",
-        dbt_commands=[f"snapshot {run_flags}"],
+        dbt_commands=["snapshot"],
         repo_type=repo_type,
         dwh_engine=dwh_engine,
         dwh_conn_id=dwh_conn_id,
         git_conn_id=git_conn_id,
         local_path=local_path,
         database_name=database_name,
         dbt_version=dbt_version,
         subfolder=subfolder,
         threads=threads,
         schema_name=schema_name,
         keepalives_idle=keepalives_idle,
         execution_timeout=execution_timeout,
-        project=project,
-        dataset=dataset,
-        env_var_conn_ids=env_var_conn_ids,
     )
 
     return dag
```

### Comparing `ewah-0.8.84/ewah/hooks/__init__.py` & `ewah-0.8.9/ewah/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/aircall.py` & `ewah-0.8.9/ewah/hooks/aircall.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     @staticmethod
     def get_ui_field_behaviour():
         return {
             "hidden_fields": ["port", "schema", "extra", "host"],
             "relabeling": {
                 "login": "Basic Auth API ID",
-                "password": "Basic Auth API Token",
+                "password": "Baisc Auth API Token",
             },
         }
 
     def get_data_in_batches(
         self,
         resource,
         data_from=None,
```

### Comparing `ewah-0.8.84/ewah/hooks/airflow.py` & `ewah-0.8.9/ewah/hooks/airflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
     conn_name_attr = "ewah_airflow_conn_id"
     default_conn_name = "ewah_airflow_default"
     conn_type = "ewah_airflow"
     hook_name = "EWAH Airflow Connection"
 
     # Resolve some more complex endpoints
-    _ENDPOINT_DAGRUNS = "dags/~/dagRuns"
     _ENDPOINTS = {
         "dagRuns": "dags/~/dagRuns",
         "taskInstance": "dags/~/dagRuns/~/taskInstances",
         "taskInstances": "dags/~/dagRuns/~/taskInstances",
     }
 
     _BASE_URL = "{0}/api/v1/{1}"
@@ -48,29 +47,19 @@
             "extra__ewah_airflow__ssh_conn_id": StringField(
                 "SSH Connection ID to Airflow Server (optional)",
                 widget=BS3TextFieldWidget(),
             ),
             "extra__ewah_airflow__protocol": StringField(
                 # Note: must not use SelectField
                 "Connection protocol (if using SSH or not specified in URL; one of: http, https)",
-                widget=BS3TextFieldWidget(),
                 default="http",
             ),
         }
 
-    def get_data_in_batches(
-        self, endpoint, page_size=100, batch_size=10000, data_from=None
-    ):
-        endpoint = self._ENDPOINTS.get(endpoint, endpoint)
-        params = {}
-        if data_from:
-            assert endpoint == self._ENDPOINT_DAGRUNS
-            # get DagRuns that ended since data_from
-            params["end_date_gte"] = data_from.isoformat()
-            params["order_by"] = "end_date"
+    def get_data_in_batches(self, endpoint, page_size=100, batch_size=10000):
         auth = requests.auth.HTTPBasicAuth(self.conn.login, self.conn.password)
         if self.conn.ssh_conn_id:
             ssh_hook = EWAHBaseHook.get_hook_from_conn_id(conn_id=self.conn.ssh_conn_id)
             ssh_host = self.conn.host or "localhost"
             ssh_host = ssh_host.replace("https://", "").replace("http://", "")
             ssh_port = self.conn.port
             if not ssh_port:
@@ -86,17 +75,16 @@
                 str(local_bind_address[1]),
                 self.conn.protocol or "http",
             )
         else:
             host = self.conn.host
             if not host.startswith("http"):
                 host = self.conn.protocol + "://" + host
-        url = self._BASE_URL.format(host, endpoint)
-        params["limit"] = page_size
-        params["offset"] = 0
+        url = self._BASE_URL.format(host, self._ENDPOINTS.get(endpoint, endpoint))
+        params = {"limit": page_size, "offset": 0}
         data = []
         i = 0
         while True:
             i += 1
             self.log.info("Making request {0} to {1}...".format(i, url))
             request = requests.get(url, params=params, auth=auth)
             assert request.status_code == 200, request.text
```

### Comparing `ewah-0.8.84/ewah/hooks/amazon_ads.py` & `ewah-0.8.9/ewah/hooks/hubspot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,336 +1,294 @@
 from ewah.hooks.base import EWAHBaseHook
-from ewah.constants import EWAHConstants as EC
 
-# from datetime import datetime, date, timedelta
-import pendulum
 import requests
-import gzip
 import json
+import urllib
 import time
 
+from typing import List, Optional, Dict, Any
+from collections import defaultdict
+from time import sleep
 
-class EWAHAmazonAdsHook(EWAHBaseHook):
-    """
-    Implements the Amazon Ads API.
-    """
-
-    _ENDPOINTS_ADS_API = {  # TODO: validate in operator
-        "NA": "https://advertising-api.amazon.com",
-        "EU": "https://advertising-api-eu.amazon.com",
-        "FE": "https://advertising-api-fe.amazon.com",
-    }
-
-    _ENDPOINTS_TOKENS = {
-        "NA": "https://api.amazon.com/auth/o2/token",
-        "EU": "https://api.amazon.co.uk/auth/o2/token",
-        "FE": "https://api.amazon.co.jp/auth/o2/token",
-    }
 
-    _ADS_TYPES = ["sp", "sb", "sd"]  # TODO: validate in operator
+class EWAHHubspotHook(EWAHBaseHook):
 
-    _ATTR_RELABEL = {}
+    _ATTR_RELABEL = {
+        "api_key": "password",
+    }
 
-    conn_name_attr = "ewah_amazon_ads_conn_id"
-    default_conn_name = "ewah_amazon_ads_default"
-    conn_type = "ewah_amazon_ads"
-    hook_name = "EWAH Amazon Ads API Connection"
+    conn_name_attr = "ewah_hubspot_conn_id"
+    default_conn_name = "ewah_hubspot_default"
+    conn_type = "ewah_hubspot"
+    hook_name = "EWAH Hubspot Connection"
+
+    BASE_URL = "https://api.hubapi.com/crm/v3/objects/{0}"
+    PROPERTIES_URL = "https://api.hubapi.com/crm/v3/properties/{0}"
+    PIPELINES_URL = "https://api.hubapi.com/crm/v3/pipelines/{0}"
+    ASSOC_URL = "https://api.hubapi.com/crm/v3/associations/{fromObjectType}/{toObjectType}/batch/read"
+    OWNERS_URL = "https://api.hubapi.com/crm/v3/owners/"
+
+    ACCEPTED_OBJECTS = [
+        "companies",
+        "contacts",
+        "deals",
+        "feedback_submissions",
+        "line_items",
+        "products",
+        "tickets",
+        "quotes",
+        "properties",
+        "owners",
+        "pipelines",
+        # special cases - see get_data_in_batches function
+        "engagement",
+        "engagements",
+        "activity",
+        "activities",
+    ]
 
     @staticmethod
     def get_ui_field_behaviour():
-        # Hide all and use custom fields only
         return {
-            "hidden_fields": ["port", "schema", "extra", "host", "login", "password"],
-            "relabeling": {},
+            "hidden_fields": ["port", "schema", "extra", "host", "login"],
+            "relabeling": {
+                "password": "API Key",
+            },
         }
 
-    @staticmethod
-    def get_connection_form_widgets():
-        """Returns connection widgets to add to connection form"""
-        from flask_appbuilder.fieldwidgets import (
-            BS3TextFieldWidget,
-            BS3PasswordFieldWidget,
+    def get_properties_for_object(self, object: str):
+        if object == "properties":
+            return []
+        request = requests.get(
+            url=self.PROPERTIES_URL.format(object),
+            params={"hapikey": self.conn.api_key},
+            headers={"accept": "application/json"},
         )
-        from wtforms import StringField
+        assert request.status_code == 200, request.text
+        return [property["name"] for property in request.json()["results"]]
 
-        return {
-            "extra__ewah_amazon_ads__lwa_client_id": StringField(
-                "AWS LWA Client ID", widget=BS3TextFieldWidget()
-            ),
-            "extra__ewah_amazon_ads__lwa_client_secret": StringField(
-                "AWS LWA CLient Secret", widget=BS3PasswordFieldWidget()
-            ),
-            "extra__ewah_amazon_ads__region": StringField(
-                "Amazon Ads Region (one of: NA, EU, FE)", widget=BS3TextFieldWidget()
-            ),
-            "extra__ewah_amazon_ads__refresh_token": StringField(
-                "Refresh Token", widget=BS3PasswordFieldWidget()
-            ),
-        }
-
-    @property
-    def access_token(self):
-        if (
-            not hasattr(self, "_access_token")
-            or pendulum.now() > self._access_token_expires_at
-        ):
-            self.log.info("Requesting new access token...")
-            requested_at = pendulum.now()
-            url = self._ENDPOINTS_TOKENS[self.conn.region]
-            payload = {
-                "grant_type": "refresh_token",
-                "client_id": self.conn.lwa_client_id,
-                "client_secret": self.conn.lwa_client_secret,
-                "refresh_token": self.conn.refresh_token,
-            }
-            response = requests.post(url, data=payload)
-            assert response.status_code == 200, response.text
-            self._access_token = response.json()["access_token"]
-            self._access_token_expires_at = requested_at.add(
-                seconds=response.json()["expires_in"] * 0.85
-            )
+    def retry_request(
+        self,
+        url: str,
+        params: dict,
+        headers: Optional[dict] = None,
+        expected_status_code: int = 200,
+        retries: int = 3,
+        wait_for_seconds: int = 60,
+    ):
+        # Every once in a while, the HubSpot API returns a 502 Bad Gateway
+        # error. This appears to be random and related to HubSpot's server
+        # infrastructure. To avoid failing DAGs due to this error, try
+        # again in case of errors, but never more than 3 times.
+        try_number = 0
+        while try_number < retries:
+            try_number += 1
+            request = requests.get(url, params=params, headers=headers)
+            if request.status_code == expected_status_code:
+                break
             self.log.info(
-                "New Amazon oauth access token is valid until {0}...".format(
-                    self._access_token_expires_at.isoformat()
+                "Status {0} - Waiting {2}s and trying again. Response:\n\n{1}".format(
+                    request.status_code, request.text, wait_for_seconds
                 )
             )
-        return self._access_token
+            sleep(60)
+        return request
 
-    def get_profile_ids(self):
-        url = "/".join([self._ENDPOINTS_ADS_API[self.conn.region], "v2", "profiles"])
-        headers = {
-            "Amazon-Advertising-API-ClientId": self.conn.lwa_client_id,
-            "Authorization": f"Bearer {self.access_token}",
-            "Content-Type": "application/json",
-        }
-        response = requests.get(url, headers=headers)
-        assert response.status_code == 200, response.text
-        return response.json()
-
-    def get_report(
-        self,
-        date,
-        ads_type,
-        report_type,
-        profile_id,
-        additional_params=None,
-    ):
-        # profile_id - the account id to be used
-        # ads_type - sp, sb, sd for sponsored products, brands, or display
-        # report_type - e.g. keywords, targets
-
-        self.log.info("Requesting report creation...")
-        url = "/".join(
-            [
-                self._ENDPOINTS_ADS_API[self.conn.region],
-                "v2",
-                ads_type,
-                report_type,
-                "report",
-            ]
-        )
-        headers = {
-            "Amazon-Advertising-API-ClientId": self.conn.lwa_client_id,
-            "Authorization": f"Bearer {self.access_token}",
-            "Amazon-Advertising-API-Scope": str(profile_id),
-            "Content-Type": "application/json",
-        }
+    def get_engagements_in_batches(self, batch_size: int):
+        url = "https://api.hubapi.com/engagements/v1/engagements/paged"
+        limit = 250
         params = {
-            "reportDate": date.isoformat().replace("-", ""),
-            "metrics": "cost,clicks,keywordId,keywordText",  # TODO: make kwarg
-            **(additional_params or {})
-            # "segment": "query",  # TODO: make kwarg
+            "hapikey": self.conn.api_key,
+            "limit": limit,
         }
-        self.log.info(f"Creating report at {url}")
-        response = requests.post(url, data=json.dumps(params), headers=headers)
-        assert response.status_code == 202, response.text
-        report_id = response.json()["reportId"]
-
-        # Loop for report status
-        wait_for = 1
+        data = []
+        i = 0
         while True:
-            url = "/".join(
-                [self._ENDPOINTS_ADS_API[self.conn.region], "v2", "reports", report_id]
+            # paginate
+            i += 1
+            self.log.info("Getting page {0} of data...".format(str(i)))
+            request = self.retry_request(
+                url=url, params=params, expected_status_code=200, retries=3
+            )
+            assert request.status_code == 200, "\nStatus: {0}\nResponse: {1}".format(
+                request.status_code, request.text
             )
-            self.log.info(f"Pinging report status at {url}")
-            response = requests.get(url, headers=headers)
-            assert response.status_code == 200, response.text
-            report_status = response.json()["status"]
-            if report_status == "SUCCESS":
+            response = request.json()
+            result = response.pop("results")
+            while result:
+                # column id is expected as primary key!
+                datum = result.pop(0)
+                datum["id"] = datum["engagement"]["id"]
+                data.append(datum)
+            if response.get("hasMore"):
+                params["offset"] = response["offset"]
+                if len(data) >= batch_size:
+                    yield data
+                    data = []
+            else:
                 break
-            if report_status == "FAILURE":
-                raise Exception(
-                    f"Report failure!\n\nFull status request response:"
-                    f"\n\n{response.text}\n\n"
-                )
-            if not report_status == "IN_PROGRESS":
-                raise Exception(f"Invalid report status: {report_status}")
-            self.log.info(f"In progress. Trying again in {wait_for}s...")
-            time.sleep(wait_for)
-            wait_for *= 2
-
-        # Download data
-        url = "/".join(
-            [
-                self._ENDPOINTS_ADS_API[self.conn.region],
-                "v2",
-                "reports",
-                report_id,
-                "download",
-            ]
-        )
-        self.log.info(f"Downloading report from {url}")
-        response = requests.get(url, headers=headers)
-        assert response.status_code == 200, response.text
-        report_data = json.loads(gzip.decompress(response.content).decode())
+        if data:
+            yield data
 
-        return report_data
-
-    def get_report_v3(
+    def get_data_in_batches(
         self,
-        date,
-        ad_product,
-        report_type,
-        profile_id,
-        additional_params=None,
-    ):
-        # profile_id - the account id to be used
-        # ad_product - e.g. SPONSORED_PRODUCTS (sp), for now only sp
-        # report_type - e.g. spCampaign, spAdvertisedProduct
-        # additional_params - contains configuration params for API v3 like groupBy, columns, filters, etc.
-
-        self.log.info("Requesting report creation...")
-        url = "/".join(
-            [
-                self._ENDPOINTS_ADS_API[self.conn.region],
-                "reporting",
-                "reports",
+        object: str,
+        properties: Optional[List[str]] = None,
+        exclude_properties: Optional[List[str]] = None,
+        associations: Optional[List[str]] = None,
+        batch_size: int = 10000,
+    ) -> List[Dict[str, Any]]:
+
+        self.log.info("Loading data for CRM object {0}!".format(object))
+        params_auth = {"hapikey": self.conn.api_key}
+        params_object = {"hapikey": self.conn.api_key, "limit": 100}
+
+        if object in ("properties", "pipelines"):
+            # Special case: not a normal object
+            assert not associations
+            assert not properties
+            assert not exclude_properties
+
+            if object == "properties":
+                url_object_raw = self.PROPERTIES_URL
+                object_list = [  # engagements is OK! but only get them once
+                    o
+                    for o in self.ACCEPTED_OBJECTS
+                    if not o
+                    in (
+                        "properties",
+                        "owners",
+                        "engagement",
+                        "activity",
+                        "activities",
+                        "pipelines",
+                    )
+                ]
+            elif object == "pipelines":
+                url_object_raw = self.PIPELINES_URL
+                object_list = ["tickets", "deals"]
+
+            params_object["objectType"] = object_list.pop(0)
+            url_object = url_object_raw.format(params_object["objectType"])
+        elif object in ("engagement", "engagements", "activity", "activities"):
+            # As of 2021-07-28, engagements are not part of the v3 of the API.
+            # Thus, they need special treatment.
+            # Also a special case and not a normal object.
+            assert not associations
+            assert not properties
+            assert not exclude_properties
+            for batch in self.get_engagements_in_batches(batch_size):
+                yield batch
+            return
+        elif object == "owners":
+            assert not associations
+            assert not properties
+            assert not exclude_properties
+            url_object = self.OWNERS_URL
+        else:
+            url_object = self.BASE_URL.format(object)
+            properties = [
+                property
+                for property in (properties or self.get_properties_for_object(object))
+                if not property in (exclude_properties or [])
             ]
-        )
-        headers = {
-            "Amazon-Advertising-API-ClientId": self.conn.lwa_client_id,
-            "Authorization": f"Bearer {self.access_token}",
-            "Amazon-Advertising-API-Scope": str(profile_id),
-            "Content-Type": "application/json",
-        }
-        params = {
-            "startDate": date.isoformat(),
-            "endDate": date.isoformat(),
-            "configuration": {
-                "adProduct": ad_product,
-                "reportTypeId": report_type,
-                "timeUnit": "DAILY",
-                "format": "GZIP_JSON",
-                **(additional_params),
-            },
-        }
-        self.log.info(f"Creating report at {url}")
-        response = requests.post(url, data=json.dumps(params), headers=headers)
-        assert response.status_code == 200, response.text
-        report_id = response.json()["reportId"]
+            params_object["properties"] = properties
 
-        # Loop for report status
-        wait_for = 1
-        while True:
-            url = "/".join(
-                [
-                    self._ENDPOINTS_ADS_API[self.conn.region],
-                    "reporting",
-                    "reports",
-                    report_id,
-                ]
+            self.log.info(
+                "Loading these properties:\n\n\t- {0}\n\n".format(
+                    "\n\t- ".join(properties)
+                )
             )
-            self.log.info(f"Pinging report status at {url}")
-            response = requests.get(url, headers=headers)
-            assert response.status_code == 200, response.text
-            report_status = response.json()["status"]
-            if report_status == "COMPLETED":
-                break
-            if report_status == "FAILURE":
-                raise Exception(
-                    f"Report failure!\n\nFull status request response:"
-                    f"\n\n{response.text}\n\n"
+            if associations:
+                self.log.info(
+                    "Also loading these associations:\n\n\t- {0}".format(
+                        "\n\t- ".join(associations)
+                    )
                 )
-            if not report_status in ("PROCESSING", "PENDING"):
-                raise Exception(f"Invalid report status: {report_status}")
-            self.log.info(f"In progress. Trying again in {wait_for}s...")
-            time.sleep(wait_for)
-            wait_for *= 2
-
-        # Download data
-        download_url = response.json()["url"]
-        self.log.info(f"Downloading report from {download_url}")
-        download = requests.get(download_url)
-        report_data = json.loads(gzip.decompress(download.content).decode())
 
-        return report_data
-
-    def get_report_dsp(
-        self,
-        account_id,
-        report_date_start,
-        report_date_end,
-        report_type,
-        metrics=None,
-        dimensions=None,
-    ):
-        self.log.info("Requesting report creation...")
-        url = "/".join(
-            [
-                self._ENDPOINTS_ADS_API[self.conn.region],
-                "accounts",
-                account_id,
-                "dsp",
-                "reports",
-            ]
-        )
-        headers = {
-            "User-Agent": "EWAH",
-            "Accept": "application/vnd.dspcreatereports.v3+json",
-            "Amazon-Advertising-API-ClientId": self.conn.lwa_client_id,
-            "Authorization": f"Bearer {self.access_token}",
-            "Content-Type": "application/json",
-        }
-        body = {
-            "startDate": report_date_start,
-            "endDate": report_date_end,
-            "format": "JSON",
-            "type": report_type,
-            "timeUnit": "DAILY",
-        }
-        if metrics:
-            body["metrics"] = metrics
-        if dimensions:
-            body["dimensions"] = dimensions
-
-        response = requests.post(url, headers=headers, json=body)
-        assert response.status_code == 202, response.text
-        report_id = response.json()["reportId"]
-
-        # Wait until report is ready
-        url = "/".join([url, report_id])
-        headers["Accept"] = "application/vnd.dspgetreports.v3+json"
-        # Loop for report status
-        wait_for = 1
-        while True:
-            self.log.info(f"Pinging report status at {url}")
-            response = requests.get(url, headers=headers)
-            assert response.status_code == 200, response.text
-            report_status = response.json()["status"]
-            if report_status == "SUCCESS":
-                break
-            if report_status == "FAILURE":
-                raise Exception(
-                    f"Report failure!\n\nFull status request response:"
-                    f"\n\n{response.text}\n\n"
+        keepgoing = True
+        i = 0
+        batch_data = []
+        while keepgoing:
+            # Get next page of object data
+            time.sleep(0.2)  # Avoid hitting API rate limits
+            i += 1
+            self.log.info("Getting page {0} of data...".format(str(i)))
+            request = self.retry_request(
+                url=url_object,
+                params=params_object,
+                headers={"accept": "application/json"},
+                expected_status_code=200,
+                retries=3,
+            )
+            if request.status_code == 414:
+                _msg = (
+                    "Error: Too many properties. Please use a smaller, custom set of"
+                    " properties.\n\nUsed properties in this call:\n\t"
+                )
+                _msg += "\n\t".join(properties) + "\n\n"
+                raise Exception(_msg)
+            assert request.status_code == 200, "Status {0}: {1}".format(
+                request.status_code, request.text
+            )
+            response = request.json()
+            response_data = response["results"] or []
+            # Keep going as long as a link is shipped in the response
+            keepgoing = response.get("paging", {}).get("next", {}).get("after")
+            params_object["after"] = keepgoing
+
+            # If applicable: get associations for all relevant objects
+            if associations and response_data:
+                associations_data = defaultdict(dict)
+                payload = json.dumps(
+                    {"inputs": [{"id": str(datum["id"])} for datum in response_data]}
                 )
-            if not report_status == "IN_PROGRESS":
-                raise Exception(f"Invalid report status: {report_status}")
-            self.log.info(f"In progress. Trying again in {wait_for}s...")
-            time.sleep(wait_for)
-            wait_for *= 2
-
-        url = response.json()["location"]
-        self.log.info("Downloading report...")
-        response = requests.get(url)
-        assert response.status_code == 200, response.text
-        return json.loads(response.content.decode())
+                for association in associations:
+                    request = requests.post(
+                        self.ASSOC_URL.format(
+                            fromObjectType=object,
+                            toObjectType=association,
+                        ),
+                        params=params_auth,
+                        headers={
+                            "accept": "application/json",
+                            "content-type": "application/json",
+                        },
+                        data=payload,
+                    )
+                    assert request.status_code < 300, request.text
+                    assert request.status_code >= 200, request.text
+                    associations_data[association].update(
+                        {
+                            datum["from"]["id"]: datum["to"]
+                            for datum in request.json()["results"]
+                        }
+                    )
+
+            # Clean up data:
+            # 1) expand the properties field into individual fields
+            # 2) add any available associations
+            # 3) if getting properties or pipelines: add object metadata
+            for datum in response_data:
+                datum.update(datum.pop("properties", {}))  # 1)
+                for association in associations or []:  # 2)
+                    datum[
+                        "ewah_associations_to_{0}".format(association)
+                    ] = associations_data[association].get(datum["id"])
+                if object in ("properties", "pipelines"):  # 3)
+                    datum["object_type"] = params_object["objectType"]
+
+            # batch_data saves all data until it is yielded
+            batch_data += response_data
+
+            if not keepgoing and object in ("properties", "pipelines"):
+                # Iterate through list of all objects
+                if object_list:
+                    params_object["objectType"] = object_list.pop(0)
+                    # tbd
+                    url_object = url_object_raw.format(params_object["objectType"])
+                    keepgoing = True
+
+            # Yield data when appropriate
+            if (len(batch_data) >= batch_size) or (not keepgoing and batch_data):
+                yield batch_data
+                batch_data = []
```

### Comparing `ewah-0.8.84/ewah/hooks/aws.py` & `ewah-0.8.9/ewah/hooks/aws.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/base.py` & `ewah-0.8.9/ewah/hooks/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from typing import Type, Optional
 
 
 class EWAHConnection(Connection):
     """Extension of airflow's native Connection."""
 
     @classmethod
+    def get_cleaner_callables(cls):
+        # overwrite me for cleaner callables that are always called
+        return []
+
+    @classmethod
     def get_connection_from_secrets(cls, conn_id):
         """Save the calling hook class as provided when called."""
         conn = super().get_connection_from_secrets(conn_id)
         # conn is returned as airflow.hooks.base.BaseHook, return as cls instead
         conn = cls(
             conn_id=conn.conn_id,
             conn_type=conn.conn_type,
@@ -104,19 +109,14 @@
             setattr(self, self.conn_name_attr, self.default_conn_name)
         else:
             setattr(self, self.conn_name_attr, kwargs[self.conn_name_attr])
 
         return super().__init__()
 
     @classmethod
-    def get_cleaner_callables(cls):
-        # overwrite me for cleaner callables that are always called
-        return []
-
-    @classmethod
     def get_connection(cls, conn_id: str) -> EWAHConnection:
         """
         Overwrite classmethod to use extended Connection object.
 
         Get connection, given connection id.
         :param conn_id: connection id
         :return: connection
```

### Comparing `ewah-0.8.84/ewah/hooks/bigquery.py` & `ewah-0.8.9/ewah/hooks/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,14 @@
             return_dict: bool = True,
         ):
             self.client = client
             self.outer = outer_class  # access outer class
             self.return_dict = return_dict
             self.latest_query = None
 
-        def close(self):
-            self.outer.log.info("Warning: BigQuery cursors cannot be closed!")
-
         def execute(self, sql, params=None, commit=True):
             if not commit:
                 self.outer.log.info("Warning: BigQuery always auto-commits!")
 
             # params have to be supplied via a job_config object!
             # only scalar implemented - array and structs are TODO!
             if params:
```

### Comparing `ewah-0.8.84/ewah/hooks/braze.py` & `ewah-0.8.9/ewah/hooks/braze.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,19 +59,15 @@
         self, object: str, data_from: Optional[datetime] = None
     ) -> List[Dict[str, Any]]:
         url = "{0}/{1}/list".format(
             self.conn.endpoint, self.OBJECTS[object]["endpoint"]
         )
         self.log.info("Loading objects from {0} ...".format(url))
         page = 0
-        params = {
-            "page": page,
-            "include_archived": "true",  # This needs to be a string, not a bool!
-            # If this is a bool, the API will ignore the value and default to false
-        }
+        params = {"page": page, "include_archived": True}
         if data_from:
             params["last_edit.time[gt]"] = data_from.isoformat()
             self.log.info("Loading data from {0}...".format(data_from.isoformat()))
         while True:
             # pagination
             params["page"] = page
             response = self.make_api_call(url, params=params)[object]
```

### Comparing `ewah-0.8.84/ewah/hooks/facebook.py` & `ewah-0.8.9/ewah/hooks/facebook.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     }
 
     conn_name_attr = "ewah_facebook_conn_id"
     default_conn_name = "ewah_facebook_default"
     conn_type = "ewah_facebook"
     hook_name = "EWAH Facebook Connection"
 
-    _DEFAULT_VERSION = "v13.0"
+    _DEFAULT_VERSION = "v12.0"
 
     @staticmethod
     def get_ui_field_behaviour():
         return {
             "hidden_fields": ["port", "extra"],
             "relabeling": {
                 "host": "[Optional] API Version",
@@ -36,20 +36,19 @@
                 "password": "App Secret",
             },
         }
 
     @staticmethod
     def get_connection_form_widgets() -> dict:
         """Returns connection widgets to add to connection form"""
-        from wtforms import StringField
-        from flask_appbuilder.fieldwidgets import BS3PasswordFieldWidget
+        from wtforms import PasswordField
 
         return {
-            "extra__ewah_facebook__access_token": StringField(
-                "Access Token", widget=BS3PasswordFieldWidget()
+            "extra__ewah_facebook__access_token": PasswordField(
+                "Access Token",
             ),
         }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def fb_init(self, account_id=None):
```

### Comparing `ewah-0.8.84/ewah/hooks/git.py` & `ewah-0.8.9/ewah/hooks/git.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/google_ads.py` & `ewah-0.8.9/ewah/hooks/google_ads.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,24 +33,21 @@
                 "password": "Client Secret",
             },
         }
 
     @staticmethod
     def get_connection_form_widgets() -> dict:
         """Returns connection widgets to add to connection form"""
-        from wtforms import StringField
-        from flask_appbuilder.fieldwidgets import BS3PasswordFieldWidget
+        # from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
+        from ewah.utils.widgets import EWAHTextAreaWidget
+        from wtforms import PasswordField
 
         return {
-            "extra__ewah_google_ads__developer_token": StringField(
-                "Developer Token", widget=BS3PasswordFieldWidget()
-            ),
-            "extra__ewah_google_ads__refresh_token": StringField(
-                "Refresh Token", widget=BS3PasswordFieldWidget()
-            ),
+            "extra__ewah_google_ads__developer_token": PasswordField("Developer Token"),
+            "extra__ewah_google_ads__refresh_token": PasswordField("Refresh Token"),
         }
 
     @property
     def service(self):
         if not hasattr(self, "_service"):
             config_dict = {
                 "developer_token": self.conn.developer_token,
@@ -61,15 +58,15 @@
                 # See here for details : https://github.com/googleads/google-ads-python/issues/486
                 "use_proto_plus": True,
             }
             if self.conn.schema:
                 config_dict["login_customer_id"] = self.conn.schema.replace("-", "")
             self._service = GoogleAdsClient.load_from_dict(
                 config_dict=config_dict,
-                version="v13",
+                version="v8",
             ).get_service("GoogleAdsService")
 
         return self._service
 
     @staticmethod
     def create_query(fields, resource, conditions=None):
         def format_columns(dict_to_format, prefix=None):
```

### Comparing `ewah-0.8.84/ewah/hooks/google_analytics.py` & `ewah-0.8.9/ewah/hooks/google_analytics.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/google_cloud_storage.py` & `ewah-0.8.9/ewah/hooks/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/infigo.py` & `ewah-0.8.9/ewah/hooks/infigo.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/mailchimp.py` & `ewah-0.8.9/ewah/hooks/mailchimp.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/metabase.py` & `ewah-0.8.9/ewah/hooks/metabase.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,21 +31,19 @@
                 "port": "Sync timeout (leave empty for none)",
             },
         }
 
     @staticmethod
     def get_connection_form_widgets() -> dict:
         """Returns connection widgets to add to connection form"""
-        from wtforms import StringField
-        from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
+        from wtforms import StringField, BooleanField
 
         return {
             "extra__ewah_metabase__http_string": StringField(
                 "Use http instead of https?",
-                widget=BS3TextFieldWidget(),
             )
         }
 
     def push_dbt_docs_to_metabase(
         self,
         dbt_project_path: str,
         dbt_database_name: str,
```

### Comparing `ewah-0.8.84/ewah/hooks/mongodb.py` & `ewah-0.8.9/ewah/hooks/mongodb.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,48 +34,37 @@
                 "password": "Uri OR password",
             },
         }
 
     @staticmethod
     def get_connection_form_widgets() -> dict:
         """Returns connection widgets to add to connection form"""
-        from flask_appbuilder.fieldwidgets import (
-            BS3TextFieldWidget,
-            BS3PasswordFieldWidget,
-        )
-        from wtforms import StringField, PasswordField
+        from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
+        from wtforms import StringField, BooleanField, PasswordField
         from ewah.utils.widgets import EWAHTextAreaWidget
 
         return {
             "extra__ewah_mongodb__conn_style": StringField(
                 "Connection Style (one of: uri, credentials)",
                 default="uri",
-                widget=BS3TextFieldWidget(),
             ),
-            "extra__ewah_mongodb__tls": StringField(
-                "SSL / TLS?",
-                default="no",
-                widget=BS3TextFieldWidget(),
-            ),
-            "extra__ewah_mongodb__tls_insecure": StringField(
-                "TLS: Allow insecure connections? Aka 'tlsInsecure'",
-                default="no",
-                widget=BS3TextFieldWidget(),
+            "extra__ewah_mongodb__tls": BooleanField("SSL / TLS?"),
+            "extra__ewah_mongodb__tls_insecure": BooleanField(
+                "TLS: Allow insecure connections? Aka 'tlsInsecure'"
             ),
             "extra__ewah_mongodb__ssl_cert": StringField(
                 "SSL Certificate",
                 widget=EWAHTextAreaWidget(rows=12),
             ),
             "extra__ewah_mongodb__ssl_private": StringField(
                 "SSL Private Key",
                 widget=EWAHTextAreaWidget(rows=12),
             ),
-            "extra__ewah_mongodb__ssl_password": StringField(
+            "extra__ewah_mongodb__ssl_password": PasswordField(
                 "SSL Certificate / Private Key Password",
-                widget=BS3PasswordFieldWidget(),
             ),
             "extra__ewah_mongodb__auth_source": StringField(
                 "Auth Source", widget=BS3TextFieldWidget()
             ),
             "extra__ewah_mongodb__auth_mechanism": StringField(
                 "Auth Mechanism", widget=BS3TextFieldWidget()
             ),
@@ -119,15 +108,15 @@
                 conn_kwargs["port"] = self.local_bind_address[1]
                 if self.conn.username:
                     conn_kwargs["username"] = self.conn.username
                 if self.conn.password:
                     conn_kwargs["password"] = self.conn.password
 
             with TemporaryDirectory() as tmp_dir:
-                if self.conn.tls.lower().startswith(("y", "t")):
+                if self.conn.tls:
                     conn_kwargs["tls"] = True
                 with NamedTemporaryFile(dir=tmp_dir) as ssl_cert:
                     if self.conn.ssl_cert:
                         ssl_cert.write(self.conn.ssl_cert.encode())
                         if self.conn.ssl_private:
                             # Concatenate into the same file
                             ssl_cert.write(self.conn.ssl_private.encode())
@@ -136,15 +125,15 @@
                             ssl_cert.name
                         )
 
                     if self.conn.ssl_password:
                         conn_kwargs[
                             "tlsCertificateKeyFilePassword"
                         ] = self.conn.ssl_password
-                    if self.conn.tls_insecure.lower().startswith(("y", "t")):
+                    if self.conn.tls_insecure:
                         conn_kwargs["tlsInsecure"] = True
                     if self.conn.auth_source:
                         conn_kwargs["authSource"] = self.conn.auth_source
                     if self.conn.auth_mechanism:
                         conn_kwargs["authMechanism"] = self.conn.auth_mechanism
                     self._mc = MongoClient(**conn_kwargs)
```

### Comparing `ewah-0.8.84/ewah/hooks/mssql.py` & `ewah-0.8.9/ewah/hooks/postgres.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,71 @@
 from ewah.hooks.sql_base import EWAHSQLBaseHook
 
-import pymssql
-import uuid
+from psycopg2 import connect as pg_connect
+from psycopg2.extras import RealDictCursor
+from typing import Optional, List, Union, Dict, Any
 
-from typing import Optional, List, Union
 
+class EWAHPostgresHook(EWAHSQLBaseHook):
 
-class EWAHMSSQLHook(EWAHSQLBaseHook):
+    _DEFAULT_PORT = 5432
 
-    _DEFAULT_PORT = 1433
-
-    _ATTR_RELABEL = {
-        "user": "login",
+    _ATTR_RELABEL: dict = {
         "database": "schema",
+        "hostname": "host",
+        "user": "login",
     }
 
-    conn_name_attr = "ewah_mssql_conn_id"
-    default_conn_name = "ewah_mssql_default"
-    conn_type = "ewah_mssql"
-    hook_name = "EWAH MSSQL Connection"
+    conn_name_attr = "ewah_postgres_conn_id"
+    default_conn_name = "ewah_postgres_default"
+    conn_type = "ewah_postgres"
+    hook_name = "EWAH PostgreSQL Connection"
 
     @staticmethod
     def get_ui_field_behaviour() -> dict:
         return {
             "hidden_fields": ["extra"],
             "relabeling": {
                 "password": "Password",
                 "login": "User",
                 "schema": "Database",
                 "host": "Hostname / IP",
-                "port": "Port (default: 1433)",
+                "port": "Port (default: 5432)",
             },
         }
 
     @staticmethod
     def get_connection_form_widgets() -> dict:
         """Returns connection widgets to add to connection form"""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from wtforms import StringField
 
         return {
-            f"extra__ewah_mssql__ssh_conn_id": StringField(
+            f"extra__ewah_postgres__ssh_conn_id": StringField(
                 "SSH Connection ID (optional)",
                 widget=BS3TextFieldWidget(),
             ),
         }
 
-    @staticmethod
-    def get_cleaner_callables():
-        # type UUID needs to be cast into a string!
-        def cast_uuid_to_string(row):
-            for key, value in row.items():
-                if isinstance(value, uuid.UUID):
-                    row[key] = str(value)
-
-            return row
-
-        return [cast_uuid_to_string]
-
     def _get_db_conn(self):
-        conn = pymssql.connect(
-            f"{self.local_bind_address[0]}:{self.local_bind_address[1]}",
-            self.conn.user,
-            self.conn.password,
-            self.conn.database,
+        return pg_connect(
+            "dbname='{0}' user='{1}' host='{2}' password='{3}' port='{4}'".format(
+                self.conn.database,
+                self.conn.user,
+                self.local_bind_address[0],
+                self.conn.password,
+                self.local_bind_address[1],
+            )
         )
-        return conn
 
     def _get_cursor(self):
         return self.dbconn.cursor()
 
     def _get_dictcursor(self):
-        return self.dbconn.cursor(as_dict=True)
+        return self.dbconn.cursor(cursor_factory=RealDictCursor)
 
     def execute(
         self, sql: str, params: Optional[dict] = None, commit: bool = False, cursor=None
     ) -> None:
         self.log.info(
             "Executing SQL:\n\n{0}\n\nWith params:\n{1}".format(
                 sql,
@@ -85,10 +75,17 @@
                         for (key, value) in params.items()
                     ]
                 )
                 if params
                 else "No params!",
             )
         )
-        (cursor or self.cursor).execute(sql.strip(), params)
+        (cursor or self.cursor).execute(sql.strip(), vars=params)
         if commit:
             self.commit()
+
+    def get_data_from_sql(
+        self, sql: str, params: Optional[dict] = None, return_dict: bool = True
+    ) -> Union[List[list], List[dict]]:
+        cur = self.dictcursor if return_dict else self.cursor
+        self.execute(sql, params=params, cursor=cur, commit=False)
+        return cur.fetchall()
```

### Comparing `ewah-0.8.84/ewah/hooks/mysql.py` & `ewah-0.8.9/ewah/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/oracle.py` & `ewah-0.8.9/ewah/hooks/oracle.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/pipedrive.py` & `ewah-0.8.9/ewah/hooks/pipedrive.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/plentymarkets.py` & `ewah-0.8.9/ewah/hooks/plentymarkets.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,47 +22,14 @@
     conn_type = "ewah_plentymarkets"
     hook_name = "EWAH PlentyMarkets Connection"
 
     _INCREMENTAL_FIELDS = {
         "/rest/orders": ["updatedAtFrom", "updatedAtTo"],
         "/rest/orders/status-history": ["createdAtFrom", "createdAtTo"],
         "/rest/accounts/contacts": ["updatedAtAfter", "updatedAtBefore"],
-        # TODO - refactor this hook to not need this dict to begin with
-        "/rest/orders/documents/invoice": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/receipt": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/tillCount": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/posCouponReceipt": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/posInvoice": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/posInvoiceCancellation": [
-            "updatedAtFrom",
-            "updatedAtTo",
-        ],
-        "/rest/orders/documents/cancellation": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/zReport": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/invoiceExternal": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/invoice": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/deliveryNote": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/poDeliveryNote": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/creditNote": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/creditNoteExternal": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/orderConfirmation": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/offer": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/dunningLetter": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/reversalDunningLetter": [
-            "updatedAtFrom",
-            "updatedAtTo",
-        ],
-        "/rest/orders/documents/returnNote": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/successConfirmation": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/correction": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/reversal": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/reversalRefund": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/proFormaInvoice": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/reorder": ["updatedAtFrom", "updatedAtTo"],
-        "/rest/orders/documents/uploaded": ["updatedAtFrom", "updatedAtTo"],
     }
 
     @staticmethod
     def get_ui_field_behaviour():
         return {
             "hidden_fields": ["port", "schema", "extra"],
             "relabeling": {
@@ -71,28 +38,25 @@
                 "host": "URL (e.g. https://myplentyshop.com or https://plentymarkets-cloud-07.com/12345)",
             },
         }
 
     @staticmethod
     def get_connection_form_widgets() -> dict:
         """Returns connection widgets to add to connection form"""
-        from wtforms import StringField
-        from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
+        from wtforms import BooleanField
 
         return {
-            "extra__ewah_plentymarkets__url_is_final": StringField(
-                "Is this the final endpoint?",
-                default="no",
-                widget=BS3TextFieldWidget(),
+            "extra__ewah_plentymarkets__url_is_final": BooleanField(
+                "Is this the final endpoint?"
             )
         }
 
     @property
     def endpoint(self):
-        if self.conn.url_is_final.lower().startswith(("y", "t")):
+        if self.conn.url_is_final:
             return self.conn.url
 
         # get the current endpoint with the correct backend hash
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_argument("--headless")
         chrome_options.add_argument("--no-sandbox")
         chrome_options.add_argument("--disable-dev-shm-usage")
```

### Comparing `ewah-0.8.84/ewah/hooks/postgres.py` & `ewah-0.8.9/ewah/hooks/sql_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,107 @@
-from ewah.hooks.sql_base import EWAHSQLBaseHook
+from ewah.hooks.base import EWAHBaseHook
 
-from psycopg2 import connect as pg_connect
-from psycopg2.extras import RealDictCursor
-from typing import Optional, List, Union, Dict, Any
-
-
-class EWAHPostgresHook(EWAHSQLBaseHook):
-
-    _DEFAULT_PORT = 5432
-
-    _ATTR_RELABEL: dict = {
-        "database": "schema",
-        "hostname": "host",
-        "user": "login",
-    }
-
-    conn_name_attr = "ewah_postgres_conn_id"
-    default_conn_name = "ewah_postgres_default"
-    conn_type = "ewah_postgres"
-    hook_name = "EWAH PostgreSQL Connection"
-
-    @staticmethod
-    def get_ui_field_behaviour() -> dict:
-        return {
-            "hidden_fields": ["extra"],
-            "relabeling": {
-                "password": "Password",
-                "login": "User",
-                "schema": "Database",
-                "host": "Hostname / IP",
-                "port": "Port (default: 5432)",
-            },
-        }
-
-    @staticmethod
-    def get_connection_form_widgets() -> dict:
-        """Returns connection widgets to add to connection form"""
-        from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
-        from wtforms import StringField
-
-        return {
-            f"extra__ewah_postgres__ssh_conn_id": StringField(
-                "SSH Connection ID (optional)",
-                widget=BS3TextFieldWidget(),
-            ),
-        }
-
-    def _get_db_conn(self):
-        return pg_connect(
-            "dbname='{0}' user='{1}' host='{2}' password='{3}' port='{4}'".format(
-                self.conn.database,
-                self.conn.user,
-                self.local_bind_address[0],
-                self.conn.password,
-                self.local_bind_address[1],
-            )
-        )
+from typing import Optional, Dict, Any, Union, List
 
-    def _get_cursor(self):
-        return self.dbconn.cursor()
 
-    def _get_dictcursor(self):
-        return self.dbconn.cursor(cursor_factory=RealDictCursor)
+class EWAHSQLBaseHook(EWAHBaseHook):
+    """Base hook extension for use as parent of various SQL hooks.
 
-    def execute(
-        self, sql: str, params: Optional[dict] = None, commit: bool = False, cursor=None
-    ) -> None:
-        self.log.info(
-            "Executing SQL:\n\n{0}\n\nWith params:\n{1}".format(
-                sql,
-                "\n".join(
-                    [
-                        "{0}: {1}".format(key, str(value))
-                        for (key, value) in params.items()
-                    ]
-                )
-                if params
-                else "No params!",
-            )
+    Children need the following:
+    - _get_db_conn method
+    - _get_cursor property
+    - _get_dictcursor property
+    - execute method
+    - get_data_from_sql method
+    """
+
+    _DEFAULT_PORT = 1234  # overwrite in child
+
+    @property
+    def dbconn(self):
+        if not hasattr(self, "_dbconn"):
+            if hasattr(self.conn, "ssh_conn_id") and self.conn.ssh_conn_id:
+                if not hasattr(self, "_ssh_hook"):
+                    self._ssh_hook = EWAHBaseHook.get_hook_from_conn_id(
+                        conn_id=self.conn.ssh_conn_id
+                    )
+                    self.local_bind_address = self._ssh_hook.start_tunnel(
+                        self.conn.host, self.conn.port or self._DEFAULT_PORT
+                    )
+            else:
+                self.local_bind_address = self.conn.host, self.conn.port
+            self._dbconn = self._get_db_conn()
+        return self._dbconn
+
+    @property
+    def cursor(self):
+        """Cursor that returns lists of lists from the data source."""
+        if not hasattr(self, "_cur"):
+            self._cur = self._get_cursor()
+        return self._cur
+
+    @property
+    def dictcursor(self):
+        """Cursor that returns lists of dictionaries from the data source."""
+        if not hasattr(self, "_dictcur"):
+            self._dictcur = self._get_dictcursor()
+        return self._dictcur
+
+    def get_records(self, sql, parameters=None):
+        """
+        Variant of execute method. Required to work with the SQL sensor.
+        """
+        return self.execute_and_return_result(
+            sql=sql, params=parameters, return_dict=False
         )
-        (cursor or self.cursor).execute(sql.strip(), vars=params)
-        if commit:
-            self.commit()
 
-    def get_data_from_sql(
-        self, sql: str, params: Optional[dict] = None, return_dict: bool = True
+    def execute_and_return_result(
+        self,
+        sql: str,
+        params: Optional[Dict[str, Any]] = None,
+        return_dict: bool = False,
     ) -> Union[List[list], List[dict]]:
+        cursor = self.dictcursor if return_dict else self.cursor
+        self.execute(sql=sql, params=params, commit=False, cursor=cursor)
+        return cursor.fetchall()
+
+    def get_data_in_batches(
+        self,
+        sql: str,
+        params: Optional[dict] = None,
+        return_dict: bool = True,
+        batch_size: int = 10000,
+    ):
         cur = self.dictcursor if return_dict else self.cursor
         self.execute(sql, params=params, cursor=cur, commit=False)
-        return cur.fetchall()
+        while True:
+            self.log.info("Fetching next batch...")
+            data = cur.fetchmany(batch_size)
+            if data:
+                yield data
+            else:
+                break
+
+    def commit(self):
+        self.log.info("Committing changes!")
+        return self.dbconn.commit()
+
+    def rollback(self):
+        self.log.info("Rolling back changes!")
+        return self.dbconn.rollback()
+
+    def close(self):
+        if hasattr(self, "_cur"):
+            self._cur.close()
+            del self._cur
+        if hasattr(self, "_dictcur"):
+            self._dictcur.close()
+            del self._dictcur
+        if hasattr(self, "_dbconn"):
+            if hasattr(self, "_ssh_hook"):
+                self._ssh_hook.stop_tunnel()
+                del self._ssh_hook
+            self._dbconn.close()
+            del self._dbconn
+
+    def __del__(self):
+        self.close()
```

### Comparing `ewah-0.8.84/ewah/hooks/rapidmail.py` & `ewah-0.8.9/ewah/hooks/rapidmail.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class EWAHRapidmailHook(EWAHBaseHook):
 
     _ATTR_RELABEL: {}
 
     conn_name_attr = "ewah_rapidmail_conn_id"
     default_conn_name = "ewah_rapidmail_default"
     conn_type = "ewah_rapidmail"
-    hook_name = "EWAH Rapidmail Connection"
+    hook_name = "EWAH Google Ads Connection"
 
     URL = "https://apiv3.emailsys.net"
     ALLOWED_ENDPOINTS = (
         "apiusers",
         "blacklist",
         "forms",
         "mailings",
```

### Comparing `ewah-0.8.84/ewah/hooks/recurly.py` & `ewah-0.8.9/ewah/hooks/recurly.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     conn_type = "ewah_recurly"
     hook_name = "EWAH Recurly Connection"
 
     @staticmethod
     def get_ui_field_behaviour():
         return {
             "hidden_fields": ["port", "schema", "extra", "host", "login"],
-            "relabeling": {"password": "Basic Auth API Key"},
+            "relabeling": {"password": "Baisc Auth API Key"},
         }
 
     @property
     def client(self):
         if not hasattr(self, "_client"):
             self._client = recurly.Client(self.conn.api_token)
```

### Comparing `ewah-0.8.84/ewah/hooks/salesforce.py` & `ewah-0.8.9/ewah/hooks/salesforce.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/sharepoint.py` & `ewah-0.8.9/ewah/hooks/sharepoint.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/snowflake.py` & `ewah-0.8.9/ewah/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/ssh.py` & `ewah-0.8.9/ewah/hooks/ssh.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/hooks/stripe.py` & `ewah-0.8.9/ewah/hooks/stripe.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/__init__.py` & `ewah-0.8.9/ewah/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/aircall.py` & `ewah-0.8.9/ewah/operators/aircall.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/base.py` & `ewah-0.8.9/ewah/operators/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,35 +131,31 @@
         load_data_from=None,  # set a minimum date e.g. for reloading of data
         reload_data_from=None,  # load data from this date for new tables
         load_data_from_relative=None,  # optional timedelta for incremental
         load_data_until=None,  # set a maximum date
         load_data_until_relative=None,  # optional timedelta for incremental
         load_data_chunking_timedelta=None,  # optional timedelta to chunk by
         primary_key=None,  # either string or list of strings
-        include_columns=None,  # list of columns to explicitly include
         exclude_columns=None,  # list of columns to exclude
         index_columns=[],  # list of columns to create an index on. can be
         # an expression, must be quoted in list if quoting is required.
         hash_columns=None,  # str or list of str - columns to hash pre-upload
-        hash_salt=None,  # string salt part for hashing
         wait_for_seconds=120,  # seconds past data_interval_end to wait until
         # wait_for_seconds only applies for incremental loads
         add_metadata=True,
         rename_columns: Optional[Dict[str, str]] = None,  # Rename columns
         subsequent_field=None,  # field name to use for subsequent extract strategy
         default_timezone=None,  # specify a default time zone for tz-naive datetimes
         use_temp_pickling=True,  # use new upload method if True - use it by default
         pickling_upload_chunk_size=100000,  # default chunk size for pickle upload
         pickle_compression=None,  # data compression algorithm to use for pickles
         default_values=None,  # dict with default values for columns (to avoid nulls)
         cleaner_class=EWAHCleaner,
         cleaner_callables=None,  # callables or list of callables to run during cleaning
         uploader_class=None,  # Future: deprecate dwh_engine and use this kwarg instead
-        additional_uploader_kwargs=None,
-        deduplication_before_upload=False,
         *args,
         **kwargs
     ):
         super().__init__(*args, **kwargs)
 
         if default_values:
             assert isinstance(default_values, dict)
@@ -217,41 +213,20 @@
         _msg = 'param "wait_for_seconds" must be a nonnegative integer!'
         assert isinstance(wait_for_seconds, int) and wait_for_seconds >= 0, _msg
         _msg = "extract_strategy {0} not accepted for this operator!".format(
             extract_strategy,
         )
         assert self._ACCEPTED_EXTRACT_STRATEGIES.get(extract_strategy), _msg
 
-        if isinstance(primary_key, str):
-            primary_key = [primary_key]
-
         if isinstance(hash_columns, str):
             hash_columns = [hash_columns]
 
-        if isinstance(include_columns, str):
-            include_columns = [include_columns]
-
-        if include_columns and primary_key:
-            for col in primary_key:
-                if not col in include_columns:
-                    _msg = """
-                        Primary key {0} is not in the include_columns list.
-                        Make sure all primary keys are included.
-                        """.format(
-                        col
-                    )
-                    raise Exception(_msg)
-
         if exclude_columns and isinstance(exclude_columns, str):
             exclude_columns = [exclude_columns]
 
-        if include_columns and exclude_columns:
-            _msg = "Don't use include and exclude columns config at the same time!"
-            raise Exception(_msg)
-
         if not dwh_engine or not dwh_engine in EC.DWH_ENGINES:
             _msg = "Invalid DWH Engine: {0}\n\nAccepted Engines:\n\t{1}".format(
                 str(dwh_engine),
                 "\n\t".join(EC.DWH_ENGINES),
             )
             raise Exception(_msg)
 
@@ -291,36 +266,34 @@
         self.target_database_name = target_database_name
         self.load_data_from = load_data_from
         self.reload_data_from = reload_data_from
         self.load_data_from_relative = load_data_from_relative
         self.load_data_until = load_data_until
         self.load_data_until_relative = load_data_until_relative
         self.load_data_chunking_timedelta = load_data_chunking_timedelta
+        if isinstance(primary_key, str):
+            primary_key = [primary_key]
         self.primary_key = primary_key  # may be used ...
         #   ... by a child class at execution!
-        self.include_columns = include_columns
         self.exclude_columns = exclude_columns
         self.index_columns = index_columns
         self.hash_columns = hash_columns
-        self.hash_salt = hash_salt
         self.wait_for_seconds = wait_for_seconds
         self.add_metadata = add_metadata
         self.rename_columns = rename_columns
         self.subsequent_field = subsequent_field
         self.default_timezone = default_timezone
         self.use_temp_pickling = use_temp_pickling
         self.pickling_upload_chunk_size = pickling_upload_chunk_size
         self.pickle_compression = pickle_compression
         self.default_values = default_values
         self.cleaner_class = cleaner_class
         self.cleaner_callables = cleaner_callables
-        self.deduplication_before_upload = deduplication_before_upload
 
         self.uploader_class = uploader_class or get_uploader(self.dwh_engine)
-        self.additional_uploader_kwargs = additional_uploader_kwargs or {}
 
         _msg = "DWH hook does not support extract strategy {0}!".format(
             extract_strategy,
         )
         # assert self.uploader._ACCEPTED_EXTRACT_STRATEGIES.get(extract_strategy), _msg
 
     def ewah_execute(self, context):
@@ -358,21 +331,19 @@
 
         cleaner_callables = self.cleaner_callables or []
 
         if self.source_conn_id:
             # resolve conn id here & delete the object to avoid usage elsewhere
             self.source_conn = EWAHBaseHook.get_connection(self.source_conn_id)
             self.source_hook = self.source_conn.get_hook()
-            if callable(getattr(self.source_hook, "get_cleaner_callables", None)):
-                hook_callables = self.source_hook.get_cleaner_callables()
-                if callable(hook_callables):
-                    cleaner_callables.append(hook_callables)
-                elif hook_callables:
-                    # Ought to be list of callables
-                    cleaner_callables += hook_callables
+            hook_callables = self.source_hook.get_cleaner_callables()
+            if callable(hook_callables):
+                cleaner_callables.append(hook_callables)
+            elif hook_callables:
+                cleaner_callables += hook_callables
         del self.source_conn_id
 
         if self._CONN_TYPE:
             assert (
                 self._CONN_TYPE == self.source_conn.conn_type
             ), "Error - connection type must be {0}!".format(self._CONN_TYPE)
 
@@ -382,167 +353,159 @@
         elif uploader_callables:
             cleaner_callables += uploader_callables
 
         self.uploader = self.uploader_class(
             dwh_conn=EWAHBaseHook.get_connection(self.dwh_conn_id),
             cleaner=self.cleaner_class(
                 default_row=self.default_values,
-                include_columns=self.include_columns,
                 exclude_columns=self.exclude_columns,
                 add_metadata=self.add_metadata,
                 rename_columns=self.rename_columns,
                 hash_columns=self.hash_columns,
-                hash_salt=self.hash_salt,
                 additional_callables=cleaner_callables,
             ),
             table_name=self.target_table_name,
             schema_name=self.target_schema_name,
             schema_suffix=self.target_schema_suffix,
             database_name=self.target_database_name,
             primary_key=self.primary_key,
             load_strategy=self.load_strategy,
             use_temp_pickling=self.use_temp_pickling,
             pickling_upload_chunk_size=self.pickling_upload_chunk_size,
             pickle_compression=self.pickle_compression,
-            deduplication_before_upload=self.deduplication_before_upload,
-            **self.additional_uploader_kwargs,
         )
 
-        try:
-            # If applicable: set the session's default time zone
-            if self.default_timezone:
-                self.uploader.dwh_hook.execute(
-                    "SET timezone TO '{0}'".format(self.default_timezone)
-                )
+        # If applicable: set the session's default time zone
+        if self.default_timezone:
+            self.uploader.dwh_hook.execute(
+                "SET timezone TO '{0}'".format(self.default_timezone)
+            )
 
-            # Create a new copy of the target table.
-            # This is so data is loaded into a new table and if data loading
-            # fails, the original data is not corrupted. At a new try or re-run,
-            # the original table is just copied anew.
-            if not self.load_strategy == EC.LS_INSERT_REPLACE:
-                # insert_replace always drops and replaces the tables completely
-                self.uploader.copy_table()
-
-            # set load_data_from and load_data_until as required
-            data_from = ada(self.load_data_from)
-            data_until = ada(self.load_data_until)
-            if self.extract_strategy == EC.ES_INCREMENTAL:
-                _tdz = timedelta(days=0)  # aka timedelta zero
-                _ed = context["data_interval_start"]
-                _ned = context["data_interval_end"]
-
-                # normal incremental load
-                _ed -= self.load_data_from_relative or _tdz
-                data_from = min(_ed, data_from or _ed)
-                if not self.test_if_target_table_exists():
-                    # Load data from scratch!
-                    data_from = ada(self.reload_data_from) or data_from
+        # Create a new copy of the target table.
+        # This is so data is loaded into a new table and if data loading
+        # fails, the original data is not corrupted. At a new try or re-run,
+        # the original table is just copied anew.
+        if not self.load_strategy == EC.LS_INSERT_REPLACE:
+            # insert_replace always drops and replaces the tables completely
+            self.uploader.copy_table()
+
+        # set load_data_from and load_data_until as required
+        data_from = ada(self.load_data_from)
+        data_until = ada(self.load_data_until)
+        if self.extract_strategy == EC.ES_INCREMENTAL:
+            _tdz = timedelta(days=0)  # aka timedelta zero
+            _ed = context["data_interval_start"]
+            _ned = context["data_interval_end"]
+
+            # normal incremental load
+            _ed -= self.load_data_from_relative or _tdz
+            data_from = min(_ed, data_from or _ed)
+            if not self.test_if_target_table_exists():
+                # Load data from scratch!
+                data_from = ada(self.reload_data_from) or data_from
 
-                _ned += self.load_data_until_relative or _tdz
-                data_until = max(_ned, data_until or _ned)
+            _ned += self.load_data_until_relative or _tdz
+            data_until = max(_ned, data_until or _ned)
 
-            elif self.extract_strategy in (EC.ES_FULL_REFRESH, EC.ES_SUBSEQUENT):
-                # Values may still be set as static values
-                data_from = ada(self.reload_data_from) or data_from
+        elif self.extract_strategy in (EC.ES_FULL_REFRESH, EC.ES_SUBSEQUENT):
+            # Values may still be set as static values
+            data_from = ada(self.reload_data_from) or data_from
 
-            else:
-                _msg = "Must define load_data_from etc. behavior for load strategy!"
-                raise Exception(_msg)
-
-            self.data_from = data_from
-            self.data_until = data_until
-            # del variables to make sure they are not used later on
-            del self.load_data_from
-            del self.reload_data_from
-            del self.load_data_until
-            del self.load_data_until_relative
-            if not self.extract_strategy == EC.ES_SUBSEQUENT:
-                # keep this param for subsequent loads
-                del self.load_data_from_relative
-
-            # Have an option to wait until a short period (e.g. 2 minutes) past
-            # the incremental loading range timeframe to ensure that all data is
-            # loaded, useful e.g. if APIs lag or if server timestamps are not
-            # perfectly accurate.
-            # When a DAG is executed as soon as possible, some data sources
-            # may not immediately have up to date data from their API.
-            # E.g. querying all data until 12.30pm only gives all relevant data
-            # after 12.32pm due to some internal delays. In those cases, make
-            # sure the (incremental loading) DAGs don't execute too quickly.
-            if self.wait_for_seconds and self.extract_strategy == EC.ES_INCREMENTAL:
-                wait_until = context.get("data_interval_end")
-                if wait_until:
-                    wait_until += timedelta(seconds=self.wait_for_seconds)
-                    self.log.info(
-                        "Awaiting execution until {0}...".format(
-                            str(wait_until),
-                        )
-                    )
-                while wait_until and datetime_utcnow_with_tz() < wait_until:
-                    # Only sleep a maximum of 5s at a time
-                    wait_for_timedelta = wait_until - datetime_utcnow_with_tz()
-                    time.sleep(max(0, min(wait_for_timedelta.total_seconds(), 5)))
-
-            # execute operator
-            if self.load_data_chunking_timedelta and data_from and data_until:
-                # Chunking to avoid OOM
-                assert data_until > data_from
-                assert self.load_data_chunking_timedelta > timedelta(days=0)
-                while self.data_from < data_until:
-                    self.data_until = min(
-                        self.data_from + self.load_data_chunking_timedelta, data_until
+        else:
+            _msg = "Must define load_data_from etc. behavior for load strategy!"
+            raise Exception(_msg)
+
+        self.data_from = data_from
+        self.data_until = data_until
+        # del variables to make sure they are not used later on
+        del self.load_data_from
+        del self.reload_data_from
+        del self.load_data_until
+        del self.load_data_until_relative
+        if not self.extract_strategy == EC.ES_SUBSEQUENT:
+            # keep this param for subsequent loads
+            del self.load_data_from_relative
+
+        # Have an option to wait until a short period (e.g. 2 minutes) past
+        # the incremental loading range timeframe to ensure that all data is
+        # loaded, useful e.g. if APIs lag or if server timestamps are not
+        # perfectly accurate.
+        # When a DAG is executed as soon as possible, some data sources
+        # may not immediately have up to date data from their API.
+        # E.g. querying all data until 12.30pm only gives all relevant data
+        # after 12.32pm due to some internal delays. In those cases, make
+        # sure the (incremental loading) DAGs don't execute too quickly.
+        if self.wait_for_seconds and self.extract_strategy == EC.ES_INCREMENTAL:
+            wait_until = context.get("data_interval_end")
+            if wait_until:
+                wait_until += timedelta(seconds=self.wait_for_seconds)
+                self.log.info(
+                    "Awaiting execution until {0}...".format(
+                        str(wait_until),
                     )
-                    self.log.info(
-                        "Now loading from {0} to {1}...".format(
-                            str(self.data_from), str(self.data_until)
-                        )
+                )
+            while wait_until and datetime_utcnow_with_tz() < wait_until:
+                # Only sleep a maximum of 5s at a time
+                wait_for_timedelta = wait_until - datetime_utcnow_with_tz()
+                time.sleep(max(0, min(wait_for_timedelta.total_seconds(), 5)))
+
+        # execute operator
+        if self.load_data_chunking_timedelta and data_from and data_until:
+            # Chunking to avoid OOM
+            assert data_until > data_from
+            assert self.load_data_chunking_timedelta > timedelta(days=0)
+            while self.data_from < data_until:
+                self.data_until = min(
+                    self.data_from + self.load_data_chunking_timedelta, data_until
+                )
+                self.log.info(
+                    "Now loading from {0} to {1}...".format(
+                        str(self.data_from), str(self.data_until)
                     )
-                    self.ewah_execute(context)
-                    self.data_from += self.load_data_chunking_timedelta
-            else:
+                )
                 self.ewah_execute(context)
+                self.data_from += self.load_data_chunking_timedelta
+        else:
+            self.ewah_execute(context)
 
-            # Run final scripts
-            # TODO: Include indexes into uploader and then remove this step
-            self.uploader.finalize_upload()
-
-            # if PostgreSQL and arg given: create indices
-            for column in self.index_columns:
-                assert self.dwh_engine == EC.DWH_ENGINE_POSTGRES
-                # Use hashlib to create a unique 63 character string as index
-                # name to avoid breaching index name length limits & accidental
-                # duplicates / missing indices due to name truncation leading to
-                # identical index names.
-                self.uploader.dwh_hook.execute(
-                    self._INDEX_QUERY.format(
-                        "__ewah_"
-                        + hashlib.blake2b(
-                            (
-                                self.target_schema_name
-                                + self.target_schema_suffix
-                                + "."
-                                + self.target_table_name
-                                + "."
-                                + column
-                            ).encode(),
-                            digest_size=28,
-                        ).hexdigest(),
-                        self.target_schema_name + self.target_schema_suffix,
-                        self.target_table_name,
-                        column,
-                    )
+        # Run final scripts
+        # TODO: Include indexes into uploader and then remove this step
+        self.uploader.finalize_upload()
+
+        # if PostgreSQL and arg given: create indices
+        for column in self.index_columns:
+            assert self.dwh_engine == EC.DWH_ENGINE_POSTGRES
+            # Use hashlib to create a unique 63 character string as index
+            # name to avoid breaching index name length limits & accidental
+            # duplicates / missing indices due to name truncation leading to
+            # identical index names.
+            self.uploader.dwh_hook.execute(
+                self._INDEX_QUERY.format(
+                    "__ewah_"
+                    + hashlib.blake2b(
+                        (
+                            temp_schema_name
+                            + "."
+                            + self.target_table_name
+                            + "."
+                            + column
+                        ).encode(),
+                        digest_size=28,
+                    ).hexdigest(),
+                    self.target_schema_name + self.target_schema_suffix,
+                    self.target_table_name,
+                    column,
                 )
+            )
 
-            # commit only at the end, so that no data may be committed before an
-            # error occurs.
-            self.log.info("Now committing changes!")
-            self.uploader.commit()
-        finally:
-            self.uploader.close()
-            del self.uploader
+        # commit only at the end, so that no data may be committed before an
+        # error occurs.
+        self.log.info("Now committing changes!")
+        self.uploader.commit()
+        self.uploader.close()
 
     def test_if_target_table_exists(self):
         # TODO: move this function to uploader
         # Need to use existing hook to work within open transaction
         kwargs = {
             "table_name": self.target_table_name,
             "schema_name": self.target_schema_name + self.target_schema_suffix,
```

### Comparing `ewah-0.8.84/ewah/operators/braze.py` & `ewah-0.8.9/ewah/operators/braze.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/dynamodb.py` & `ewah-0.8.9/ewah/operators/dynamodb.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/facebook.py` & `ewah-0.8.9/ewah/operators/facebook.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class EWAHFBOperator(EWAHBaseOperator):
 
     _NAMES = ["facebook", "fb"]
 
     _ACCEPTED_EXTRACT_STRATEGIES = {
         EC.ES_FULL_REFRESH: True,
-        EC.ES_INCREMENTAL: True,
+        EC.ES_INCREMENTAL: False,
         EC.ES_SUBSEQUENT: True,
     }
 
     class levels:
         ad = "ad"
 
     def __init__(
@@ -86,15 +86,15 @@
                 raise Exception(
                     (
                         "Field {0} is not an accepted value for insight_fields! "
                         + "Accepted field values:\n\t{1}\n"
                     ).format(i_f, "\n\t".join(allowed_insight_fields))
                 )
 
-        assert isinstance(data_since, datetime), "data_since must be of type datetime!"
+        assert isinstance(data_since, datetime), "data_from must be of type datetime!"
 
         if kwargs.get("extract_strategy") == EC.ES_SUBSEQUENT:
             kwargs["subsequent_field"] = "date_start"
 
         super().__init__(*args, **kwargs)
 
         self.data_since = data_since
@@ -105,30 +105,22 @@
         self.refresh_interval = refresh_interval
 
     def ewah_execute(self, context):
         if (
             self.extract_strategy == EC.ES_SUBSEQUENT
             and self.test_if_target_table_exists()
         ):
-            data_since = self.get_max_value_of_column("date_start")
-            if isinstance(data_since, str):
-                # Sometimes the date is saved as string
-                data_since = datetime.strptime(data_since, "%Y-%m-%d").date()
-            data_since = data_since - self.refresh_interval
-            data_until = datetime.now()
-        elif self.extract_strategy == EC.ES_INCREMENTAL:
-            data_since = self.data_from
-            data_until = self.data_until or datetime.now()
+            data_since = (
+                self.get_max_value_of_column("date_start") - self.refresh_interval
+            )
         else:
             data_since = self.data_since
-            data_until = datetime.now()
-
         for account_id in self.account_ids or []:
             for batch in self.source_hook.get_data_in_batches(
                 level=self.level,
                 fields=self.insight_fields,
                 data_from=data_since,
-                data_until=data_until,
+                data_until=datetime.now(),
                 account_id=account_id,
                 breakdowns=self.breakdowns,
             ):
                 self.upload_data(batch)
```

### Comparing `ewah-0.8.84/ewah/operators/fx.py` & `ewah-0.8.9/ewah/operators/fx.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/google_ads.py` & `ewah-0.8.9/ewah/operators/google_ads.py`

 * *Files 13% similar despite different names*

```diff
@@ -83,53 +83,29 @@
     def ewah_execute(self, context):
         # Make sure the correct date conditions are set
         conditions = self.conditions or []
         if (
             self.extract_strategy == EC.ES_SUBSEQUENT
             and self.test_if_target_table_exists()
         ):
-            data_from = self.get_max_value_of_column(self.subsequent_field)
-            if isinstance(data_from, str):
-                data_from = datetime.strptime(data_from, "%Y-%m-%d").date()
-            data_from = data_from - (self.load_data_from_relative or timedelta(days=0))
+            data_from = self.get_max_value_of_column(self.subsequent_field) - (
+                self.load_data_from_relative or timedelta(days=0)
+            )
             data_until = (self.data_until or datetime.now()).date()
         else:
             data_from = self.data_from.date()
             data_until = (self.data_until or datetime.now()).date()
-
-        if self.load_data_chunking_timedelta:
-            batch_from = data_from
-            while batch_from <= data_until:
-                batch_until = min(
-                    data_until, batch_from + self.load_data_chunking_timedelta
-                )
-                conditions.append(
-                    "segments.date BETWEEN '{0}' AND '{1}'".format(
-                        batch_from.isoformat(),
-                        batch_until.isoformat(),
-                    )
-                )
-                self.upload_data(
-                    self.source_hook.get_data(
-                        client_id=self.client_id,
-                        fields=self.fields,
-                        resource=self.resource,
-                        conditions=conditions,
-                    )
-                )
-                del conditions[-1:]  # Re-added in next iteration
-                batch_from = batch_until + timedelta(days=1)
-        else:
+        if data_from and data_until:
             conditions.append(
                 "segments.date BETWEEN '{0}' AND '{1}'".format(
                     data_from.isoformat(),
                     data_until.isoformat(),
                 )
             )
-            self.upload_data(
-                self.source_hook.get_data(
-                    client_id=self.client_id,
-                    fields=self.fields,
-                    resource=self.resource,
-                    conditions=conditions,
-                )
+        self.upload_data(
+            self.source_hook.get_data(
+                client_id=self.client_id,
+                fields=self.fields,
+                resource=self.resource,
+                conditions=conditions,
             )
+        )
```

### Comparing `ewah-0.8.84/ewah/operators/google_analytics.py` & `ewah-0.8.9/ewah/operators/google_analytics.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/google_cloud_storage.py` & `ewah-0.8.9/ewah/operators/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/google_maps.py` & `ewah-0.8.9/ewah/operators/google_maps.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/google_sheets.py` & `ewah-0.8.9/ewah/operators/google_sheets.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                         "Column letter {0} out of bounds!".format(
                             letter,
                         )
                     )
                 column_identifier = column_identifier[:-1]
                 ident_dict.update({i: ord(letter) + 1 - ord("a")})
                 i += 1
-            return sum([v * (26**k) for k, v in ident_dict.items()])
+            return sum([v * (26 ** k) for k, v in ident_dict.items()])
         else:
             return column_identifier
 
     def __init__(
         self,
         workbook_key,  # can be seen in the URL of the workbook
         sheet_key,  # name of the worksheet
```

### Comparing `ewah-0.8.84/ewah/operators/hubspot.py` & `ewah-0.8.9/ewah/operators/hubspot.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,32 +23,32 @@
         exclude_properties=None,
         associations=None,
         **kwargs
     ):
         if object is None:
             object = kwargs.get("target_table_name")
         assert (
-            object in EWAHHubspotHook.ACCEPTED_OBJECTS.keys()
+            object in EWAHHubspotHook.ACCEPTED_OBJECTS
         ), "Object {0} is invalid!".format(object)
         if object == "properties":
             kwargs["primary_key"] = ["name", "object_type"]
         else:
             kwargs["primary_key"] = "id"
         super().__init__(*args, **kwargs)
         self.object = object
         if isinstance(properties, str):
             properties = [properties]
         if isinstance(exclude_properties, str):
             exclude_properties = [exclude_properties]
-        if isinstance(associations, str) and not associations == "all":
+        if isinstance(associations, str):
             associations = [associations]
         nonetype = type(None)
         assert isinstance(properties, (list, nonetype))
         assert isinstance(exclude_properties, (list, nonetype))
-        assert isinstance(associations, (list, nonetype)) or associations == "all"
+        assert isinstance(associations, (list, nonetype))
         self.properties = properties
         self.exclude_properties = exclude_properties
         self.associations = associations
 
     def ewah_execute(self, context):
         for batch in self.source_hook.get_data_in_batches(
             object=self.object,
```

### Comparing `ewah-0.8.84/ewah/operators/infigo.py` & `ewah-0.8.9/ewah/operators/infigo.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/mailchimp.py` & `ewah-0.8.9/ewah/operators/mailchimp.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/mailingwork.py` & `ewah-0.8.9/ewah/operators/mailingwork.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/mongodb.py` & `ewah-0.8.9/ewah/operators/mongodb.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/personio.py` & `ewah-0.8.9/ewah/operators/recurly.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,32 @@
-from ewah.hooks.personio import EWAHPersonioHook
+from ewah.hooks.recurly import EWAHRecurlyHook
 
 from ewah.operators.base import EWAHBaseOperator
 from ewah.constants import EWAHConstants as EC
 
 
-class EWAHPersonioOperator(EWAHBaseOperator):
+class EWAHRecurlyOperator(EWAHBaseOperator):
 
-    _NAMES = ["personio"]
+    _NAMES = ["recurly"]
 
     _ACCEPTED_EXTRACT_STRATEGIES = {
         EC.ES_FULL_REFRESH: True,
-        EC.ES_INCREMENTAL: False,
-        EC.ES_SUBSEQUENT: True,
+        EC.ES_INCREMENTAL: True,
     }
 
-    _CONN_TYPE = EWAHPersonioHook.conn_type
+    _CONN_TYPE = EWAHRecurlyHook.conn_type
 
     def __init__(self, resource=None, *args, **kwargs):
-        resource = resource or kwargs.get("target_table_name", "").lower()
-        assert EWAHPersonioHook.validate_resource(resource)
-        if kwargs.get("extract_strategy") == EC.ES_SUBSEQUENT:
-            assert (
-                resource == "attendances"
-            ), "Only attendances work with subsequent loading!"
-            kwargs["subsequent_field"] = "updated_at"
-            kwargs["primary_key"] = "id"
-
+        kwargs["primary_key"] = "id"
+        resource = resource or kwargs.get("target_table_name")
         super().__init__(*args, **kwargs)
 
+        assert EWAHRecurlyHook.validate_resource(resource)
         self.resource = resource
 
     def ewah_execute(self, context):
-        if (
-            self.extract_strategy == EC.ES_SUBSEQUENT
-            and self.test_if_target_table_exists()
-        ):
-            data_from = self.get_max_value_of_column(self.subsequent_field)
-        else:
-            data_from = None
         for batch in self.source_hook.get_data_in_batches(
             resource=self.resource,
-            data_from=data_from,
+            data_from=self.data_from,
+            data_until=self.data_until,
         ):
             self.upload_data(batch)
```

### Comparing `ewah-0.8.84/ewah/operators/pipedrive.py` & `ewah-0.8.9/ewah/operators/pipedrive.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/plentymarkets.py` & `ewah-0.8.9/ewah/operators/plentymarkets.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,41 +13,32 @@
         EC.ES_FULL_REFRESH: True,
         EC.ES_INCREMENTAL: True,
         EC.ES_SUBSEQUENT: True,
     }
 
     _CONN_TYPE = EWAHPlentyMarketsHook.conn_type
 
-    def __init__(
-        self,
-        resource=None,
-        additional_api_call_params=None,
-        batch_size=10000,
-        *args,
-        **kwargs
-    ):
+    def __init__(self, resource=None, additional_api_call_params=None, *args, **kwargs):
         kwargs["primary_key"] = kwargs.get("primary_key", "id")
         resource = resource or kwargs.get("target_table_name")
         if kwargs["extract_strategy"] == EC.ES_SUBSEQUENT:
             kwargs["subsequent_field"] = kwargs.get("subsequent_field", "updatedAt")
-            assert (
-                EWAHPlentyMarketsHook.format_resource(resource)
-                in EWAHPlentyMarketsHook._INCREMENTAL_FIELDS.keys()
-            ), "{0} is not subsequent loadable!".format(resource)
+            # currently, only the orders and accounts/contacts resource works with subsequent loading
+            assert any(["orders" in resource, "accounts/contacts" in resource])
         if kwargs["extract_strategy"] == EC.ES_INCREMENTAL:
+            # currently, only the orders resource works with incremental loading
             assert (
                 EWAHPlentyMarketsHook.format_resource(resource)
                 in EWAHPlentyMarketsHook._INCREMENTAL_FIELDS.keys()
             ), "{0} is not incrementally loadable!".format(resource)
         super().__init__(*args, **kwargs)
 
         assert isinstance(additional_api_call_params, (type(None), dict))
         self.resource = resource
         self.additional_api_call_params = additional_api_call_params
-        self.batch_size = batch_size
 
     def ewah_execute(self, context):
         if (
             self.extract_strategy == EC.ES_SUBSEQUENT
             and self.test_if_target_table_exists()
         ):
             data_from = self.get_max_value_of_column(self.subsequent_field)
@@ -64,10 +55,9 @@
         else:
             data_from = self.data_from
         for batch in self.source_hook.get_data_in_batches(
             resource=self.resource,
             data_from=data_from,
             data_until=self.data_until,
             additional_params=self.additional_api_call_params,
-            batch_size=self.batch_size,
         ):
             self.upload_data(batch)
```

### Comparing `ewah-0.8.84/ewah/operators/rapidmail.py` & `ewah-0.8.9/ewah/operators/rapidmail.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/recurly.py` & `ewah-0.8.9/ewah/operators/stripe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from ewah.hooks.recurly import EWAHRecurlyHook
-
 from ewah.operators.base import EWAHBaseOperator
 from ewah.constants import EWAHConstants as EC
 
+from ewah.hooks.stripe import EWAHStripeHook
+
 
-class EWAHRecurlyOperator(EWAHBaseOperator):
+class EWAHStripeOperator(EWAHBaseOperator):
 
-    _NAMES = ["recurly"]
+    _NAMES = ["stripe"]
 
     _ACCEPTED_EXTRACT_STRATEGIES = {
         EC.ES_FULL_REFRESH: True,
-        EC.ES_INCREMENTAL: True,
+        EC.ES_INCREMENTAL: False,
     }
 
-    _CONN_TYPE = EWAHRecurlyHook.conn_type
+    _CONN_TYPE = EWAHStripeHook.conn_type
 
-    def __init__(self, resource=None, *args, **kwargs):
+    def __init__(self, *args, resource=None, expand=None, batch_size=10000, **kwargs):
+        if resource is None:
+            resource = kwargs.get("target_table_name")
         kwargs["primary_key"] = "id"
-        resource = resource or kwargs.get("target_table_name")
         super().__init__(*args, **kwargs)
-
-        assert EWAHRecurlyHook.validate_resource(resource)
         self.resource = resource
+        self.expand = expand
+        self.batch_size = batch_size
 
     def ewah_execute(self, context):
         for batch in self.source_hook.get_data_in_batches(
             resource=self.resource,
-            data_from=self.data_from,
-            data_until=self.data_until,
+            expand=self.expand,
+            batch_size=self.batch_size,
         ):
             self.upload_data(batch)
```

### Comparing `ewah-0.8.84/ewah/operators/s3.py` & `ewah-0.8.9/ewah/operators/s3.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/salesforce.py` & `ewah-0.8.9/ewah/operators/salesforce.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/sevdesk.py` & `ewah-0.8.9/ewah/operators/airflow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-from ewah.hooks.sevdesk import EWAHSevDeskHook
-
-from ewah.operators.base import EWAHBaseOperator
 from ewah.constants import EWAHConstants as EC
+from ewah.hooks.airflow import EWAHAirflowHook
+from ewah.operators.base import EWAHBaseOperator
 
 
-class EWAHSevDeskOperator(EWAHBaseOperator):
+class EWAHAirflowOperator(EWAHBaseOperator):
 
-    _NAMES = ["sevdesk"]
+    _NAMES = ["airflow"]
 
     _ACCEPTED_EXTRACT_STRATEGIES = {
         EC.ES_FULL_REFRESH: True,
         EC.ES_INCREMENTAL: False,
-        EC.ES_SUBSEQUENT: False,
     }
 
-    _CONN_TYPE = EWAHSevDeskHook.conn_type
+    _CONN_TYPE = EWAHAirflowHook.conn_type
 
-    def __init__(self, endpoint=None, embed=None, *args, **kwargs):
-        endpoint = endpoint or kwargs.get("target_table_name")
+    def __init__(self, endpoint=None, request_page_size=100, *args, **kwargs):
+        self.endpoint = endpoint or kwargs.get("target_table_name")
+        self.request_page_size = request_page_size
         super().__init__(*args, **kwargs)
 
-        assert EWAHSevDeskHook.validate_endpoint(
-            endpoint
-        ), "Invalid endpoint {0}!".format(endpoint)
-
-        self.endpoint = endpoint
-        self.embed = embed
-
     def ewah_execute(self, context):
         for batch in self.source_hook.get_data_in_batches(
             endpoint=self.endpoint,
-            embed=self.embed,
+            page_size=self.request_page_size,
         ):
             self.upload_data(batch)
```

### Comparing `ewah-0.8.84/ewah/operators/sharepoint.py` & `ewah-0.8.9/ewah/operators/sharepoint.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/sql_base.py` & `ewah-0.8.9/ewah/operators/sql_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         source_schema_name: Optional[str] = None,
         source_table_name: Optional[
             str
         ] = None,  # defaults to same as target_table_name
         source_database_name: Optional[str] = None,  # bigquery: project id
         sql_select_statement: Optional[str] = None,  # Alternative to specifying table
         timestamp_column: Optional[str] = None,
-        subsequent_delta: Optional[Union[timedelta, int]] = None,
         where_clauses: Optional[Union[str, List[str]]] = None,
         extra_params: Optional[dict] = None,
         batch_size: int = 100000,
         *args,
         **kwargs
     ):
         source_table_name = source_table_name or kwargs["target_table_name"]
@@ -68,15 +67,14 @@
             )
 
         self.sql = self._SQL_BASE_SELECT.format(select_sql=sql_select_statement)
         self.extra_params = extra_params
         self.timestamp_column = timestamp_column
         self.where_clauses = where_clauses
         self.batch_size = batch_size
-        self.subsequent_delta = subsequent_delta
 
     def ewah_execute(self, context):
         # called, potentially with a data_from and data_until
 
         params = self.extra_params or {}
         where_clauses = self.where_clauses or []
         if self.data_from and self.timestamp_column:
@@ -92,22 +90,20 @@
                     self.timestamp_column, self._SQL_PARAMS.format("data_until")
                 )
             )
             params["data_until"] = self.data_until
         if self.subsequent_field and self.test_if_target_table_exists():
             where_clauses.append(
                 "{0} > {1}".format(
-                    "{0}{1}{0}".format(self._SQL_COLUMN_QUOTE, self.subsequent_field),
-                    self._SQL_PARAMS.format("previous_max_value"),
+                    self.subsequent_field, self._SQL_PARAMS.format("previous_max_value")
                 )
             )
-            subsequent_value = self.get_max_value_of_column(self.subsequent_field)
-            if self.subsequent_delta:
-                subsequent_value -= self.subsequent_delta
-            params["previous_max_value"] = subsequent_value
+            params["previous_max_value"] = self.get_max_value_of_column(
+                self.subsequent_field
+            )
 
         where_clauses = where_clauses or ["1 = 1"]
         sql = self.sql.format("\n  AND ".join(where_clauses))
         for batch in self.source_hook.get_data_in_batches(
             sql=sql,
             params=params or None,  # Don't supply empty dict as params!
             return_dict=True,
```

### Comparing `ewah-0.8.84/ewah/operators/sql_bigquery.py` & `ewah-0.8.9/ewah/operators/sql_bigquery.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/operators/zendesk.py` & `ewah-0.8.9/ewah/operators/zendesk.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/uploaders/__init__.py` & `ewah-0.8.9/ewah/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/uploaders/base.py` & `ewah-0.8.9/ewah/uploaders/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Optional, Type, Union, Dict, List, Any
 
 
 class EWAHBaseUploader(LoggingMixin):
     """Base class for all EWAH uploader classes aka Uploaders.
 
     Uploaders are classes that can receive data in a standardized format and upload
-    it to a target data storage. Each Uploader uploads data to one type of target.
+    it to a target data storage. Each Uploader is uploads data to one type of target.
     For instance, the EWAHPostgresUploader loads data to PostgreSQL databases.
 
     The base class contains the basic methods shared by all Uploaders for the purpose of
     uploading data. Each target shall have a subclass derived from this class.
     """
 
     upload_call_count = 0
@@ -35,27 +35,21 @@
         schema_name: str,
         schema_suffix: str = "_next",
         database_name: Optional[str] = None,
         primary_key: Optional[List[str]] = None,
         use_temp_pickling: bool = False,
         pickling_upload_chunk_size: int = 100000,
         pickle_compression: Optional[str] = None,
-        deduplication_before_upload: bool = False,
     ) -> None:
         assert pickle_compression is None or pickle_compression in (
             "gzip",
             "bz2",
             "lzma",
         )
 
-        if deduplication_before_upload:
-            assert (
-                primary_key
-            ), "Must set primary key if using deduplication_before_upload!"
-
         if use_temp_pickling:
             # Set a function to use for temporary pickle files
             if pickle_compression is None:
                 self.pickle_file_open = open
             else:
                 self.pickle_file_open = __import__(pickle_compression).open
 
@@ -75,15 +69,14 @@
         self.table_name = table_name
         self.schema_name = schema_name
         self.schema_suffix = schema_suffix
         self.database_name = database_name
         self.primary_key = primary_key
         self.use_temp_pickling = use_temp_pickling
         self.pickling_upload_chunk_size = pickling_upload_chunk_size
-        self.deduplication_before_upload = deduplication_before_upload
 
     @classmethod
     def get_cleaner_callables(cls):
         # overwrite me for cleaner callables that are always called
         return []
 
     @classmethod
@@ -148,30 +141,14 @@
         self.log.info(
             "Chunk {1}: Uploading {0} rows of data.".format(
                 str(len(data)),
                 str(self.upload_call_count),
             )
         )
 
-        if self.deduplication_before_upload:
-            # Some endpoints can't help but return the same record multiple times.
-            # This is needed to deduplicate before uploading data.
-            # It should be avoided whenever possible, however.
-            self.log.info("Deduplicating data...")
-            temp_dict = {}
-            while data:
-                datum = data.pop(0)
-                id_tuple = ()
-                for key in self.primary_key:
-                    id_tuple += (datum.get(key),)
-                temp_dict[id_tuple] = datum
-            while temp_dict:
-                key, value = temp_dict.popitem()
-                data.append(value)
-
         if (self.upload_call_count > 1) or (
             not (self.load_strategy == EC.LS_INSERT_REPLACE)
         ):
             self.log.info("Checking for, and applying schema changes.")
             self.log.info(
                 "Added fields:\n\t{0}\n".format(
                     "\n\t".join(
@@ -237,15 +214,15 @@
 
     def finalize_upload(self):
         if self.use_temp_pickling:
             self._upload_from_pickle()
 
     def close(self):
         self.dwh_hook.close()
-        
+
     def copy_table(self) -> None:
         """Copy the existing version of the table, including all data, if it exists."""
         test_kwargs = {"table_name": self.table_name, "schema_name": self.schema_name}
         if self.database_name:
             test_kwargs["database_name"] = self.database_name
         if self.test_if_table_exists(**test_kwargs):
             if self.database_name:
```

### Comparing `ewah-0.8.84/ewah/uploaders/bigquery.py` & `ewah-0.8.9/ewah/uploaders/bigquery.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,26 @@
 from ewah.uploaders.base import EWAHBaseUploader
 
 from airflow.operators.python import PythonOperator
 from airflow.models import BaseOperator
 
 from google.cloud.bigquery.table import TableReference
 from google.cloud.bigquery import (
-    Table,
     SchemaField,
+    Table,
     LoadJobConfig,
+    SourceFormat,
     CopyJobConfig,
 )
 
 from copy import deepcopy
 from time import sleep
 from tempfile import TemporaryFile, TemporaryDirectory
 from datetime import datetime, date, timedelta
 
-from avro.datafile import DataFileWriter
-from avro.io import DatumWriter
-
-import avro.schema
-import json
-import os
-
 
 class BigqueryOperator(BaseOperator):
     "Operate to execute SQL on BigQuery"
 
     def __init__(
         self, sql, bigquery_conn_id, project=None, params=None, *args, **kwargs
     ):
@@ -54,61 +48,32 @@
 
 class FakeDatasetRef:
     def __init__(self, dataset_id, project_id):
         self.dataset_id = dataset_id
         self.project = project_id
 
 
-def map_bq_data_type_to_avro(data_type):
-    return {
-        "STRING": "string",
-        "INT64": "long",
-        "BOOL": "boolean",
-        # "DATE": "", TODO: Properly deal with datetime types
-        # "TIMESTAMP": "",
-        "BYTES": "bytes",
-        "FLOAT64": "double",
-    }[data_type]
-
-
 class EWAHBigQueryUploader(EWAHBaseUploader):
 
     _QUERY_SCHEMA_CHANGES_COLUMNS = """
         SELECT column_name
         FROM `{project_id}.{schema_name}.INFORMATION_SCHEMA.COLUMNS`
         WHERE table_name = '{table_name}'
     """
     _QUERY_SCHEMA_CHANGES_ADD_COLUMN = """
         ALTER TABLE `{project_id}.{schema_name}.{table_name}`
         ADD COLUMN `{column_name}` {column_type};
     """
 
     _QUERY_TABLE = "SELECT * FROM `{project_id}.{schema_name}.{table_name}`"
 
-    def __init__(
-        self,
-        *args,
-        partition_field=None,
-        partition_type=None,
-        require_partition_filter=False,
-        insert_chunk_size=100,
-        **kwargs,
-    ) -> None:
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(EC.DWH_ENGINE_BIGQUERY, *args, **kwargs)
         # BigQuery project id aka database name may be set in connection
         self.database_name = self.database_name or self.dwh_hook.conn.project
-        if partition_type or partition_field or require_partition_filter:
-            assert (
-                partition_type and partition_field
-            ), "partition_type and partition_field must both be set if either is set or require_partition_filter is true!"
-        self.partition_field = partition_field
-        self.partition_type = partition_type
-        self.insert_chunk_size = insert_chunk_size
-
-        assert self.use_temp_pickling, "BigQuery operator only works with pickling!"
 
     @classmethod
     def get_cleaner_callables(cls):
         def bigquery_data_adjustments(row):
             key_changes = []
             for key, value in row.items():
                 # change date, datetime, timedelta types
@@ -160,15 +125,15 @@
         def kickoff_func(schema_full, schema_suffix, dwh_conn_id):
             # kickoff: create new dataset
             schema = schema_full + schema_suffix
             conn = EWAHBaseHook.get_hook_from_conn_id(dwh_conn_id).dbconn
             # delete dataset first if it already exists
             print("Deleting the dataset {0} if it already exists.".format(schema))
             conn.delete_dataset(schema, delete_contents=True, not_found_ok=True)
-            print("Creating the dataset {0}.".format(schema))
+            print("Creating the dataset {0}.".format(schema_full))
             conn.create_dataset(schema)
             print("Done!")
 
         def final_func(schema_name, schema_suffix, dwh_conn_id):
             # final: move new data into the final dataset
             conn = EWAHBaseHook.get_hook_from_conn_id(dwh_conn_id).dbconn
             # get dataset objects
@@ -268,15 +233,19 @@
 
     def rollback(self):
         raise Exception("Rollback attempted - BigQuery knows no transactions!")
 
     def close(self):
         pass  # nothing to do
 
+    def commit(self):
+        pass  # nothing to do
+
     def test_if_table_exists(self, table_name, schema_name, project_id=None):
+
         if project_id:
             dataset_path = "{0}.{1}".format(project_id, schema_name)
         else:
             dataset_path = schema_name
         if not self.test_if_dataset_exists(dataset_path):
             return False
         return 0 < len(
@@ -350,224 +319,169 @@
             )
             table_new = ds_new.table(self.table_name)
             copy_job = conn.copy_table(
                 table_old,
                 table_new,
                 job_config=CopyJobConfig(write_disposition="WRITE_TRUNCATE"),
             )
+            sleep(1)
 
-            copy_job.result()  # Waits until the job is done
-            assert copy_job.state == "DONE", "Unexpected job state: {0}".format(
-                job.state
-            )
-            self.log.info(
-                "Successfully copied {0}!".format(
-                    copy_job.__dict__["_properties"]["configuration"]["copy"][
-                        "destinationTable"
-                    ]["tableId"]
-                )
-            )
+            while True:
+                copy_job.result()
+                assert copy_job.state in (
+                    "RUNNING",
+                    "DONE",
+                ), "Unexpected job state: {0}".format(job.state)
+                if copy_job.state == "DONE":
+                    self.log.info(
+                        "Successfully copied {0}".format(
+                            copy_job.__dict__["_properties"]["configuration"]["copy"][
+                                "destinationTable"
+                            ]["tableId"]
+                        )
+                    )
+                    break
+                # Wait 5s, try again
+                sleep(5)
 
     def _create_or_update_table(
         self,
         data,
         table_name,
         schema_name,
         schema_suffix,
         columns_definition,
         load_strategy,
         upload_call_count,
         database_name=None,
         primary_key=None,
     ):
-        # This method doesn't actually create or update a table. It just creates
-        # and populates a single .avro file which is used in the data upload.
-        # The actual upload happens when the commit() method is called.
-        if upload_call_count == 1:
-            # Create avro writer and file in temporary folder
-            self.avro_folder = TemporaryDirectory()
-            self.avro_file_name = self.avro_folder.name + os.sep + table_name + ".avro"
-            avro_schema = avro.schema.parse(
-                json.dumps(
-                    {
-                        "type": "record",
-                        "name": table_name,
-                        "namespace": table_name,
-                        "fields": [
-                            {
-                                "name": name,
-                                "type": [
-                                    "null",
-                                    map_bq_data_type_to_avro(field["data_type"]),
-                                ],
-                            }
-                            for name, field in columns_definition.items()
-                        ],
-                    }
-                )
-            )
-            # Create the avro_writer object to be used going forward
-            self.avro_writer = DataFileWriter(
-                open(self.avro_file_name, "wb"), DatumWriter(), avro_schema
-            )
-            # Save the relevant kwargs for later use in the commit() method
-            self.table_creation_config = {
-                "table_name": table_name,
-                "schema_name": schema_name,
-                "schema_suffix": schema_suffix,
-                "columns_definition": columns_definition,
-                "load_strategy": load_strategy,
-                "database_name": database_name,
-                "primary_key": primary_key,
-            }
-
-        self.log.info(
-            "BigQuery Uploader writes data into Avro file for later one-off upload!"
-        )
-        while data:
-            # Write records to .avro file
-            self.avro_writer.append(data.pop(0))
-
-    def commit(self):
-        # The commit is where the upload is actually done for BigQuery (special case).
-        # The _create_or_update_table method can be called multiple times;
-        # each time, data is appended to the .avro file. When "committing",
-        # this .avro file is uploaded and, depending on the load strategy, used.
-        if not hasattr(self, "avro_file_name"):
-            # There was no data ever uploaded
-            # Do nothing
-            self.log.info("Nothing to upload!")
-            return
-
-        # Clean up after yourself first
-        self.avro_writer.close()
-
-        # Fetch the relevant configuration
-        project_id = self.table_creation_config.get("database_name", self.database_name)
-        assert project_id, "Missing Project ID!"
-        load_strategy = self.table_creation_config["load_strategy"]
-        primary_key = self.table_creation_config["primary_key"]
-        schema_name = self.table_creation_config["schema_name"]
-        schema_suffix = self.table_creation_config["schema_suffix"]
-        table_name_final = self.table_creation_config["table_name"]
-        table_suffix = "__ewah_tmp"
-
-        columns_definition = self.table_creation_config["columns_definition"]
-        new_schema_name = schema_name + schema_suffix
-
-        is_full_refresh = (
-            load_strategy == EC.LS_INSERT_REPLACE
-            or not self.test_if_table_exists(
-                table_name=table_name_final,
-                schema_name=new_schema_name,
-                project_id=project_id,
-            )
-        )
-
+        project_id = database_name or self.database_name
         conn = self.dwh_hook.dbconn
+        new_schema_name = schema_name + schema_suffix
         ds_new = conn.get_dataset(new_schema_name)
 
-        # Create temp table with .avro file
-        if is_full_refresh:
-            # temp table is also the final table for full refresh!
-            table_name = table_name_final
-        else:
-            table_name = table_name_final + table_suffix
+        # ensure all fields exist, even if null
+        # otherwise, rarely-populated fields will cause data loading failure
+        upload_data = []
+        while data:
+            datum = data.pop(0)
+            upload_data.append(
+                {field: datum.get(field) for field in columns_definition.keys()}
+            )
 
-        # Drop temp table if it already exists
-        if self.test_if_table_exists(
+        # create table if it does not yet exist / drop if it needs dropping
+        table_exists = self.test_if_table_exists(
             table_name=table_name,
             schema_name=new_schema_name,
             project_id=project_id,
+        )
+
+        # autodetect only works for json, csv
+        # Future: add clustering_fields kwargs
+        # job_config = LoadJobConfig(source_format=SourceFormat.JSON, autodetect=True)
+        job_config = LoadJobConfig(autodetect=True)
+
+        if (load_strategy == EC.LS_INSERT_REPLACE and upload_call_count == 1) or (
+            not table_exists
         ):
-            # Drop table before re-creating it
-            conn.delete_table(
-                conn.get_table(TableReference(dataset_ref=ds_new, table_id=table_name))
-            )
-        # Create temp table with .avro file
-        table_obj = Table(".".join([project_id, new_schema_name, table_name]))
-        if is_full_refresh and self.partition_field:
-            table_obj.time_partitioning = bigquery.TimePartitioning(
-                type_=self.partition_type,
-                field=self.partition_field,
-            )
-            if self.require_partition_filter:
-                table_obj.require_partition_filter = True
-        self.log.info("Uploading data into table now...")
-        with open(self.avro_file_name, "rb") as source_file:
-            job = conn.load_table_from_file(
-                file_obj=source_file,
-                destination=table_obj,
-                job_id_prefix="ewah_",
-                rewind=True,
-                job_config=LoadJobConfig(
-                    autodetect=False,
-                    source_format="AVRO",
-                    schema=[
-                        SchemaField(name=name, field_type=field["data_type"])
-                        for name, field in columns_definition.items()
-                    ],
-                ),
+            if table_exists:
+                # Drop table before re-creating it
+                conn.delete_table(
+                    conn.get_table(
+                        TableReference(dataset_ref=ds_new, table_id=table_name)
+                    )
+                )
+            # create it anew
+            table_obj = Table(".".join([project_id, new_schema_name, table_name]))
+            job = conn.load_table_from_json(
+                json_rows=upload_data, destination=table_obj, job_config=job_config
             )
             try:
                 job.result()
             except:
                 self.log.info("Errors occured - job errors: {0}".format(job.errors))
                 raise
             assert job.state == "DONE", "Invalid job state: {0}".format(job.state)
+        else:
+            # table already exists, use `merge` statement to load data via temp table
 
-        if not is_full_refresh:
-            # Need to merge new rows into the existing table
+            tmp_table_name = table_name + "__tmp"
+            if self.test_if_table_exists(
+                table_name=tmp_table_name,
+                schema_name=new_schema_name,
+                project_id=project_id,
+            ):
+                # Delete temporary table if it exists from a previous run
+                conn.delete_table(
+                    conn.get_table(
+                        TableReference(dataset_ref=ds_new, table_id=tmp_table_name)
+                    )
+                )
 
-            fields_pk = set(primary_key or [])
-            fields_all = set(columns_definition.keys() or [])
-            fields_non_pk = fields_all - fields_pk
+            # create a temp table with new data
+            self.log.info("Uploading data into a temp table...")
+            table_obj = Table(".".join([project_id, new_schema_name, tmp_table_name]))
+            job = conn.load_table_from_json(
+                json_rows=upload_data, destination=table_obj, job_config=job_config
+            )
+            try:
+                job.result()
+            except:
+                self.log.info("Errors occured - job errors: {0}".format(job.errors))
+                raise
+            assert job.state == "DONE", "Invalid job state: {0}".format(job.state)
 
+            # merge it into existing table
             if load_strategy == EC.LS_UPSERT:
-                assert fields_pk
-            elif load_strategy == EC.LS_INSERT_ADD:
-                fields_pk = []  # Ignore if set
+                merge_condition = " AND ".join(
+                    ["TARGET.`{0}` = SOURCE.`{0}`".format(pk) for pk in primary_key]
+                )
+            elif load_strategy in (EC.LS_INSERT_ADD, EC.LS_INSERT_REPLACE):
+                # never matched
+                merge_condition = "FALSE"
             else:
-                raise Exception("Not implemented!")
-
-            merge_statement = """
-                MERGE INTO `{target}` AS TARGET
-                USING `{source}` AS SOURCE
-                ON {condition}
+                raise Exception("Not Implemented!")
 
+            when_clauses = """
                 WHEN MATCHED THEN
-                    UPDATE SET {update_fields}
-
+                    UPDATE SET {set_columns}
                 WHEN NOT MATCHED THEN
-                    INSERT ({insert_fields})
-                    VALUES ({insert_fields})
+                    INSERT ({columns})
+                    VALUES ({columns})
             """.format(
-                target=".".join([project_id, new_schema_name, table_name_final]),
-                source=".".join([project_id, new_schema_name, table_name]),
-                condition=" AND ".join(
-                    ["TARGET.`{0}` = SOURCE.`{0}`".format(field) for field in fields_pk]
-                )
-                or "FALSE",
-                insert_fields="`{0}`".format("`, `".join(fields_all)),
-                update_fields=", ".join(
-                    ["`{0}` = SOURCE.`{0}`".format(field) for field in fields_non_pk]
+                set_columns=",".join(
+                    [
+                        "`{0}` = SOURCE.`{0}`".format(field)
+                        for field in columns_definition.keys()
+                        if not field in (primary_key or [])
+                    ]
+                ),
+                columns=", ".join(
+                    ["`{0}`".format(field) for field in columns_definition.keys()]
                 ),
             )
 
-            self.log.info("Executing query:\n\n{0}\n\n".format(merge_statement))
-            job = conn.query(
-                query=merge_statement,
-                job_id_prefix="ewah_",
+            sql = """
+                MERGE INTO {target_name} AS TARGET
+                USING {source_name} AS SOURCE
+                ON {merge_condition}
+                {when_clauses}
+            """.format(
+                target_name="`{0}.{1}.{2}`".format(
+                    project_id, new_schema_name, table_name
+                ),
+                source_name="`{0}.{1}.{2}`".format(
+                    project_id, new_schema_name, tmp_table_name
+                ),
+                merge_condition=merge_condition,
+                when_clauses=when_clauses,
             )
-            try:
-                job.result()
-            except:
-                self.log.info("Errors occured - job errors: {0}".format(job.errors))
-                raise
-            assert job.state == "DONE", "Invalid job state: {0}".format(job.state)
+            self.dwh_hook.execute(sql=sql)
 
-            # Remove old temp table from dataset
+            self.log.info("Deleting temp table...")
+            # delete temp table
             conn.delete_table(
-                conn.get_table(TableReference(dataset_ref=ds_new, table_id=table_name))
+                conn.get_table(
+                    TableReference(dataset_ref=ds_new, table_id=tmp_table_name)
+                )
             )
-
-        self.log.info("Done!")
```

### Comparing `ewah-0.8.84/ewah/uploaders/google_sheets.py` & `ewah-0.8.9/ewah/uploaders/google_sheets.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/uploaders/postgres.py` & `ewah-0.8.9/ewah/uploaders/postgres.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,30 +19,32 @@
         	JOIN pg_class cl ON cl.OID = f.attrelid
         	LEFT JOIN pg_namespace n ON n.OID = cl.relnamespace
         WHERE cl.relkind = 'r'::CHAR
         	AND n.nspname = %(schema_name)s
         	AND cl.relname = %(table_name)s
         	AND f.attnum > 0;
     """
+    _QUERY_SCHEMA_CHANGES_DROP_COLUMN = """
+        ALTER TABLE "{schema_name}"."{table_name}"
+        DROP COLUMN IF EXISTS "{column_name}" CASCADE;
+    """
     _QUERY_SCHEMA_CHANGES_ADD_COLUMN = """
         ALTER TABLE "{schema_name}"."{table_name}"
         ADD COLUMN "{column_name}" {column_type};
     """
     _QUERY_TABLE = 'SELECT * FROM "{schema_name}"."{table_name}"'
 
     _COPY_TABLE = """
         -- Drop a previous version of the table if it exists
         DROP TABLE IF EXISTS "{new_schema}"."{new_table}";
         CREATE TABLE "{new_schema}"."{new_table}" AS (
             SELECT * FROM "{old_schema}"."{old_table}"
         );
     """
 
-    CONSTRAINTS_SET = False
-
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(EC.DWH_ENGINE_POSTGRES, *args, **kwargs)
 
     @classmethod
     def get_schema_tasks(
         cls,
         dag,
@@ -167,17 +169,16 @@
                     """.format(
                         schema_name=schema_name,
                         table_name=table_name,
                         columns='","'.join(primary_key),
                     )
                 )
 
-        if primary_key and not self.CONSTRAINTS_SET:
+        if primary_key:
             # make sure there is a unique constraint for primary_key
-            self.CONSTRAINTS_SET = True  # Only set it once per DagRun, though
             self.dwh_hook.execute(
                 sql="""
                     ALTER TABLE "{schema_name}"."{table_name}"
                     DROP CONSTRAINT IF EXISTS "{constraint}";
                     ALTER TABLE "{schema_name}"."{table_name}"
                     ADD CONSTRAINT "{constraint}" UNIQUE ("{columns}");
                 """.format(
@@ -196,51 +197,47 @@
             )
 
         set_columns = []
         for column in columns_definition.keys():
             if not (column in (primary_key or [])):
                 set_columns += [column]
 
-        if load_strategy == EC.LS_INSERT_REPLACE:
-            # Ought not be a conflict - just insert
-            do_on_conflict = ""
-        elif load_strategy == EC.LS_INSERT_ADD:
-            # Ought not be a conflict - just insert
-            do_on_conflict = ""
-        elif load_strategy == EC.LS_UPSERT:
-            # Update records as appropriate
-            do_on_conflict = """
-                ON CONFLICT ("{primary_key}") DO UPDATE SET\n\t{sets}
-            """.format(
-                primary_key='", "'.join(primary_key),
-                sets="\n\t,".join(
-                    [
-                        '"{column}" = EXCLUDED."{column}"'.format(column=column)
-                        for column in set_columns
-                    ]
-                ),
-            )
-        else:
-            raise Exception("Not implemented!")
-
         cols_list = list(columns_definition.keys())
         sql = (
             """
             INSERT INTO "{schema_name}"."{table_name}"
             ("{column_names}") VALUES {placeholder}
-            {do_on_conflict};
+            ON CONFLICT {do_on_conflict};
         """.format(
-                schema_name=schema_name,
-                table_name=table_name,
-                placeholder="{placeholder}",
-                column_names='", "'.join(cols_list),
-                do_on_conflict=do_on_conflict,
+                **{
+                    "schema_name": schema_name,
+                    "table_name": table_name,
+                    "placeholder": "{placeholder}",
+                    "column_names": '", "'.join(cols_list),
+                    "do_on_conflict": "DO NOTHING"
+                    if not primary_key
+                    else """
+                ("{primary_key}") DO UPDATE SET\n\t{sets}
+            """.format(
+                        primary_key='", "'.join(primary_key),
+                        sets="\n\t,".join(
+                            [
+                                '"{column}" = EXCLUDED."{column}"'.format(column=column)
+                                for column in set_columns
+                            ]
+                        ),
+                    ),
+                }
             )
             .replace("%", "%%")
-            .format(placeholder="%s")
+            .format(
+                **{
+                    "placeholder": "%s",
+                }
+            )
         )
         self.log.info("Now Uploading! Using SQL:\n\n{0}".format(sql))
         # escape crappy column names by using aliases in the psycopg2 template
         cols_map = {cols_list[i]: "col_" + str(i) for i in range(len(cols_list))}
         template = "(%(" + ")s, %(".join([val for key, val in cols_map.items()]) + ")s)"
         cur = self.dwh_hook.cursor
         upload_data = [
```

### Comparing `ewah-0.8.84/ewah/uploaders/snowflake.py` & `ewah-0.8.9/ewah/uploaders/snowflake.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,24 +4,21 @@
 """
 
 from ewah.uploaders.base import EWAHBaseUploader
 from ewah.constants import EWAHConstants as EC
 from ewah.hooks.base import EWAHBaseHook
 
 import os
-import sys
 import csv
 import pickle
-import pytz
 
 import snowflake.connector
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from airflow.models import BaseOperator
 from copy import deepcopy
-from datetime import datetime
 
 
 class SnowflakeOperator(BaseOperator):
     "Operate to execute SQL on Snowflake"
 
     def __init__(self, sql, snowflake_conn_id, database, params=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -51,14 +48,18 @@
             column_name
         FROM "{database_name}".information_schema.columns
         WHERE table_catalog = %(database_name)s
             AND table_schema = %(schema_name)s
             AND table_name = %(table_name)s
         ORDER BY ordinal_position ASC;
     """
+    _QUERY_SCHEMA_CHANGES_DROP_COLUMN = """
+        ALTER TABLE "{database_name}"."{schema_name}"."{table_name}"
+        DROP COLUMN IF EXISTS "{column_name}" CASCADE;
+    """
     _QUERY_SCHEMA_CHANGES_ADD_COLUMN = """
         ALTER TABLE "{database_name}"."{schema_name}"."{table_name}"
         ADD COLUMN "{column_name}" {column_type};
     """
     _QUERY_TABLE = """
         SELECT * FROM "{database_name}"."{schema_name}"."{table_name}"
     """
@@ -70,28 +71,14 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(EC.DWH_ENGINE_SNOWFLAKE, *args, **kwargs)
         # Snowflake database name may be set in the connection
         self.database_name = self.database_name or self.dwh_hook.conn.database
 
     @classmethod
-    def get_cleaner_callables(cls):
-        def add_timezone(row):
-            # Snowflake uses Pacific Time as default time zone if it receives
-            # a timestamp without a time zone. Overwrite this default by adding
-            # UTC as time zone to every datetime that doesn't have a time zone.
-            for key, value in row.items():
-                if isinstance(value, datetime) and not value.tzinfo:
-                    # add UTC as timezone if there is no timezone for the datetime yet
-                    row[key] = value.replace(tzinfo=pytz.utc)
-            return row
-
-        return [add_timezone]
-
-    @classmethod
     def get_schema_tasks(
         cls,
         dag,
         dwh_engine,
         dwh_conn_id,
         target_schema_name,
         target_schema_suffix="_next",
@@ -172,15 +159,14 @@
         schema_suffix,
         columns_definition,
         load_strategy,
         upload_call_count,
         database_name=None,
         primary_key=None,
     ):
-        primary_key = primary_key or []  # must be empty list, but don't init in kwargs
         database_name = database_name or self.dwh_hook.conn.database
         self.log.info("Preparing DWH Tables...")
         schema_name += schema_suffix
         new_table_name = table_name + "_new"
         self.dwh_hook.execute(
             sql="""CREATE OR REPLACE TABLE
                     "{database_name}"."{schema_name}"."{table_name}"
@@ -210,15 +196,14 @@
             """.format(
                 database_name,
                 schema_name,
                 new_table_name,
             ),
         )
         list_of_columns = [col[0].strip() for col in list_of_columns]
-        python_fix_required = sys.version_info.minor < 10  # See below for reason
 
         self.log.info("Writing data to a temporary .csv file")
         with TemporaryDirectory(prefix="uploadtosnowflake") as tmp_dir:
             with NamedTemporaryFile(
                 dir=tmp_dir,
                 prefix=new_table_name,
                 suffix=".csv",
@@ -232,39 +217,26 @@
                         quoting=csv.QUOTE_MINIMAL,
                     )
 
                     for _ in range(len(data)):
                         datum = data.pop(0)
                         # Make sure order of csv is the same as order of columns
                         csvwriter.writerow(
-                            [
-                                # csv has a bug, which is fixed in Python 3.10,
-                                # which leads to the escape character itself not
-                                # being escaped - Snowflake uploads will fail
-                                # if it is not escaped, hence strings with backslashes
-                                # need double-slashes to "manually" escape it.
-                                # Hotfix can be removed when upgrading to Python >= 3.10
-                                datum[col].replace("\\", "\\\\")
-                                if python_fix_required
-                                and isinstance(datum.get(col), str)
-                                else datum.get(col)
-                                for col in list_of_columns
-                            ],
+                            [datum.get(col) for col in list_of_columns],
                         )
 
                 # now stage and copy into snowflake!
                 sql_upload = """
                     USE DATABASE "{2}";
                     USE SCHEMA "{3}";
                     DROP FILE FORMAT IF EXISTS {1}_format;
                     CREATE FILE FORMAT {1}_format
-                        TYPE = 'CSV'
-                        FIELD_DELIMITER = ','
-                        FIELD_OPTIONALLY_ENCLOSED_BY = '"'
-                        ESCAPE = '\\\\'
+                        type = 'CSV'
+                        field_delimiter = ','
+                        field_optionally_enclosed_by = '"'
                     ;
                     DROP STAGE IF EXISTS {1}_stage;
                     CREATE STAGE {1}_stage
                         file_format = {1}_format;
                     PUT file://{0} @{1}_stage AUTO_COMPRESS = TRUE OVERWRITE = TRUE;
                     COPY INTO "{2}"."{3}"."{1}" FROM '@{1}_stage/{4}.gz';
                 """.format(
@@ -302,31 +274,27 @@
                     database_name,
                     schema_name,
                     table_name,
                     '","'.join(primary_key),
                 )
         else:
             update_set_cols = []
-            if load_strategy == EC.LS_INSERT_ADD:
-                # Even if set, ignore primary key during insert!
-                primary_key = []
-
             for col in columns_definition.keys():
                 if not (col in primary_key):
                     update_set_cols += [col]
 
             sql_final = """
                 USE SCHEMA "{0}"."{1}";
                 MERGE INTO "{0}"."{1}"."{2}" AS a
                     USING "{0}"."{1}"."{3}" AS b
                     ON {4}
                     WHEN MATCHED THEN UPDATE
                         SET {5}
-                    WHEN NOT MATCHED THEN
-                        INSERT  ({6})
+                    WHEN NOT MATCHED THEN INSERT
+                                ({6})
                         VALUES  ({7})
                     ;
                 DROP TABLE "{0}"."{1}"."{3}" CASCADE;
             """.format(
                 database_name,
                 schema_name,
                 table_name,
```

### Comparing `ewah-0.8.84/ewah/utils/airflow_utils.py` & `ewah-0.8.9/ewah/utils/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/utils/dbt_operator.py` & `ewah-0.8.9/ewah/utils/dbt_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,44 +28,43 @@
     _commands = [
         "run",
         "test",
         "snapshot",
         "seed",
         "docs generate",
         "docs serve",
-        "source freshness",
     ]
     # note: dbt deps is always executed first!
 
     def __init__(
         self,
         repo_type,
         dwh_engine,
         dwh_conn_id,
         git_conn_id=None,
         local_path=None,
         dbt_commands=["run"],  # string or list of strings - dbt commands
-        dbt_version=None,
+        dbt_version="0.18.1",
         subfolder=None,  # optional: supply if dbt project is in a subfolder
         threads=4,  # see https://docs.getdbt.com/dbt-cli/configure-your-profile/#understanding-threads
         schema_name="analytics",  # see https://docs.getdbt.com/dbt-cli/configure-your-profile/#understanding-target-schemas
         database_name=None,  # Snowflake & BigQuery only - name of the database / project
         keepalives_idle=0,  # see https://docs.getdbt.com/reference/warehouse-profiles/postgres-profile/
         dataset=None,  # BigQuery alias for schema_name
         project=None,  # BigQuery alias for database_name
         metabase_conn_id=None,  # Push docs to Metabase if exists
-        env_var_conn_ids=None,  # Name of list of names of connections to use as env vars
         *args,
         **kwargs
     ):
         schema_name = dataset or schema_name
         database_name = project or database_name
 
         assert repo_type in ("git", "local")
         assert dbt_commands
+        assert dbt_version
         assert threads
         assert schema_name
 
         if repo_type == "local":
             assert git_conn_id is None
             assert local_path
         else:
@@ -105,20 +104,14 @@
                 )
             )
 
         # Make sure no process command tries to sneak in extra commands
         if not max([1 if "&" in cmd else 0 for cmd in dbt_commands]) == 0:
             raise Exception("Ampersand (&) is an invalid character in dbt_commands!")
 
-        assert isinstance(
-            env_var_conn_ids, (type(None), str, list)
-        ), "env_var_conn_ids must be a string or list of strings!"
-        if env_var_conn_ids and isinstance(env_var_conn_ids, str):
-            env_var_conn_ids = [env_var_conn_ids]
-
         super().__init__(*args, **kwargs)
 
         self.repo_type = repo_type
         self.git_conn_id = git_conn_id
         self.local_path = local_path
         self.dwh_engine = dwh_engine
         self.dwh_conn_id = dwh_conn_id
@@ -126,29 +119,21 @@
         self.dbt_version = dbt_version
         self.subfolder = subfolder
         self.threads = threads
         self.schema_name = schema_name
         self.keepalives_idle = keepalives_idle
         self.database_name = database_name
         self.metabase_conn_id = metabase_conn_id
-        self.env_var_conn_ids = env_var_conn_ids
 
     def execute(self, context):
 
         # env to be used in processes later
         env = os.environ.copy()
         env["PIP_USER"] = "no"
 
-        if self.env_var_conn_ids:
-            for env_var_conn_id in self.env_var_conn_ids:
-                # get name, secret via hook and add to environment
-                # note that the type doesn't matter; just takes login and password
-                hook = EWAHBaseHook.get_hook_from_conn_id(conn_id=env_var_conn_id)
-                env[hook.conn.login] = hook.conn.password
-
         # create a new temp folder, all action happens in here
         with TemporaryDirectory(prefix="__ewah_dbt_operator_") as tmp_dir:
             # clone repo into temp directory
             repo_dir = tmp_dir + os.path.sep + "repo"
             if self.repo_type == "git":
                 # Clone repo into temp folder
                 git_hook = EWAHBaseHook.get_hook_from_conn_id(conn_id=self.git_conn_id)
@@ -163,42 +148,58 @@
             venv_folder = tmp_dir + os.path.sep + "venv"
             self.log.info(
                 "creating a new virtual environment in {0}...".format(
                     venv_folder,
                 )
             )
             venv.create(venv_folder, with_pip=True)
+
+            # install dbt into created venv
+            self.log.info("installing dbt=={0}".format(self.dbt_version))
+            cmd = []
+            cmd.append("source {0}/bin/activate".format(venv_folder))
+            cmd.append("pip install --quiet --upgrade pip setuptools")
+            if self.dbt_version.startswith("1"):
+                # Different pip behavior since dbt 1.0.0
+                cmd.append(
+                    "pip install --quiet --upgrade dbt-{0}=={1}".format(
+                        {
+                            EC.DWH_ENGINE_POSTGRES: "postgres",
+                            EC.DWH_ENGINE_SNOWFLAKE: "snowflake",
+                            EC.DWH_ENGINE_BIGQUERY: "bigquery",
+                        }[self.dwh_engine],
+                        self.dbt_version,
+                    )
+                )
+            else:
+                cmd.append(
+                    "pip install --quiet --upgrade dbt=={0}".format(self.dbt_version)
+                )
+            cmd.append("dbt --version")
+            cmd.append("deactivate")
+            assert run_cmd(cmd, env, self.log.info) == 0
+
             dbt_dir = repo_dir
             if self.subfolder:
                 if not self.subfolder[:1] == os.path.sep:
                     self.subfolder = os.path.sep + self.subfolder
                 dbt_dir += self.subfolder
 
             dwh_hook = EWAHBaseHook.get_hook_from_conn_id(self.dwh_conn_id)
             # in case of SSH: execute a query to create the connection and tunnel
             dwh_hook.execute("SELECT 1 AS a -- Testing the connection")
             dwh_conn = dwh_hook.conn
 
-            # read profile name and dbt version & create temporary profiles.yml
+            # read profile name & create temporary profiles.yml
             project_yml_file = dbt_dir
             if not project_yml_file[-1:] == os.path.sep:
                 project_yml_file += os.path.sep
             project_yml_file += "dbt_project.yml"
             project_yml = yaml.load(open(project_yml_file, "r"), Loader=Loader)
             profile_name = project_yml["profile"]
-            dbt_version = self.dbt_version or project_yml.get("require-dbt-version")
-            del self.dbt_version  # Make sure it can't accidentally be used below
-            assert dbt_version, "Must supply dbt_version or set require-dbt-version!"
-            if isinstance(dbt_version, str):
-                if not dbt_version.startswith(("=", "<", ">")):
-                    dbt_version = "==" + dbt_version
-            elif isinstance(dbt_version, list):
-                dbt_version = ",".join(dbt_version)
-            else:
-                raise Exception("dbt_version must be a string or a list of strings!")
             self.log.info('Creating temp profile "{0}"'.format(profile_name))
             profiles_yml = {
                 "config": {
                     "send_anonymous_usage_stats": False,
                     "use_colors": False,  # colors won't be useful in logs
                 },
             }
@@ -259,46 +260,14 @@
                 if dwh_conn.location:
                     profiles_yml[profile_name]["outputs"]["prod"][
                         "location"
                     ] = dwh_conn.location
             else:
                 raise Exception("DWH Engine not implemented!")
 
-            # install dbt into created venv
-            cmd = []
-            cmd.append("source {0}/bin/activate".format(venv_folder))
-            cmd.append("pip install --quiet --upgrade pip setuptools")
-            if re.search("[^0-9\.]0(\.[0-9]+)?(\.[0-9]+)?$", dbt_version):
-                # regex checks whether the (last) version start with 0
-                # if true, version <1.0.0 required
-                cmd.append(
-                    'pip install --quiet --upgrade "MarkupSafe<=2.0.1" "dbt{0}"'.format(
-                        dbt_version
-                    )
-                )
-            else:
-                # Different pip behavior since dbt 1.0.0
-                cmd.append(
-                    "pip install --quiet --upgrade "
-                    '"MarkupSafe<=2.0.1" '
-                    '"dbt-core{1}" '
-                    '"dbt-{0}{1}"'.format(
-                        {
-                            EC.DWH_ENGINE_POSTGRES: "postgres",
-                            EC.DWH_ENGINE_SNOWFLAKE: "snowflake",
-                            EC.DWH_ENGINE_BIGQUERY: "bigquery",
-                        }[self.dwh_engine],
-                        dbt_version,
-                    )
-                )
-
-            cmd.append("dbt --version")
-            cmd.append("deactivate")
-            assert run_cmd(cmd, env, self.log.info) == 0
-
             # run commands with correct profile in the venv in the temp folder
             profiles_yml_name = tmp_dir + os.path.sep + "profiles.yml"
             env["DBT_PROFILES_DIR"] = os.path.abspath(tmp_dir)
             with open(profiles_yml_name, "w") as profiles_file:
                 # write profile into profiles.yml file
                 yaml.dump(profiles_yml, profiles_file, default_flow_style=False)
```

### Comparing `ewah-0.8.84/ewah/utils/email_data_dag.py` & `ewah-0.8.9/ewah/utils/email_data_dag.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/utils/git_pull_dag.py` & `ewah-0.8.9/ewah/utils/git_pull_dag.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/utils/log_cleanup_dag.py` & `ewah-0.8.9/ewah/utils/log_cleanup_dag.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/utils/run_commands.py` & `ewah-0.8.9/ewah/utils/run_commands.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah/utils/yml_loader.py` & `ewah-0.8.9/ewah/utils/yml_loader.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.84/ewah.egg-info/PKG-INFO` & `ewah-0.8.9/ewah.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: ewah
-Version: 0.8.84
+Version: 0.8.9
 Summary: An ELT with airflow helper module: Ewah
 Home-page: https://gemmaanalytics.com/
 Author: Bijan Soltani
 Author-email: bijan.soltani+ewah@gemmaanalytics.com
 License: UNKNOWN
 Description: # ewah
         Ewah: ELT With Airflow Helper - Classes and functions to make apache airflow life easier.
         
         Functions to create all DAGs required for ELT using only a simple config file.
         
         ## DWHs Implemented
         - Snowflake
         - PostgreSQL
+        
+        ## DWHs Planned
         - Bigquery
         
         ## Operators
         
         EWAH currently supports the following operators:
         
         - Aircall
```

### Comparing `ewah-0.8.84/ewah.egg-info/SOURCES.txt` & `ewah-0.8.9/ewah.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,86 +15,69 @@
 ewah/dag_factories/dag_factory_atomic.py
 ewah/dag_factories/dag_factory_idempotent.py
 ewah/dag_factories/dag_factory_mixed.py
 ewah/dag_factories/dbt_dag_factory.py
 ewah/hooks/__init__.py
 ewah/hooks/aircall.py
 ewah/hooks/airflow.py
-ewah/hooks/airtable.py
-ewah/hooks/amazon_ads.py
-ewah/hooks/amazon_seller_central.py
 ewah/hooks/aws.py
 ewah/hooks/base.py
 ewah/hooks/bigquery.py
 ewah/hooks/braze.py
-ewah/hooks/dbt_env_var.py
 ewah/hooks/facebook.py
 ewah/hooks/git.py
 ewah/hooks/google_ads.py
 ewah/hooks/google_analytics.py
 ewah/hooks/google_cloud_storage.py
 ewah/hooks/hubspot.py
 ewah/hooks/infigo.py
-ewah/hooks/linkedin.py
 ewah/hooks/mailchimp.py
 ewah/hooks/metabase.py
 ewah/hooks/mongodb.py
-ewah/hooks/mssql.py
 ewah/hooks/mysql.py
 ewah/hooks/oracle.py
-ewah/hooks/personio.py
 ewah/hooks/pipedrive.py
 ewah/hooks/plentymarkets.py
 ewah/hooks/postgres.py
 ewah/hooks/rapidmail.py
 ewah/hooks/recurly.py
 ewah/hooks/salesforce.py
-ewah/hooks/sevdesk.py
 ewah/hooks/sharepoint.py
-ewah/hooks/shopify.py
 ewah/hooks/snowflake.py
 ewah/hooks/sql_base.py
 ewah/hooks/ssh.py
 ewah/hooks/stripe.py
 ewah/operators/__init__.py
 ewah/operators/aircall.py
 ewah/operators/airflow.py
-ewah/operators/airtable.py
-ewah/operators/amazon_ads.py
-ewah/operators/amazon_seller_central.py
 ewah/operators/base.py
 ewah/operators/braze.py
 ewah/operators/dynamodb.py
 ewah/operators/facebook.py
 ewah/operators/fx.py
 ewah/operators/google_ads.py
 ewah/operators/google_analytics.py
 ewah/operators/google_cloud_storage.py
 ewah/operators/google_maps.py
 ewah/operators/google_sheets.py
 ewah/operators/hubspot.py
 ewah/operators/infigo.py
-ewah/operators/linkedin.py
-ewah/operators/linkedin_ads.py
 ewah/operators/mailchimp.py
 ewah/operators/mailingwork.py
 ewah/operators/mongodb.py
-ewah/operators/personio.py
 ewah/operators/pipedrive.py
 ewah/operators/plentymarkets.py
 ewah/operators/rapidmail.py
 ewah/operators/recurly.py
 ewah/operators/s3.py
 ewah/operators/salesforce.py
-ewah/operators/sevdesk.py
 ewah/operators/sharepoint.py
 ewah/operators/shopify.py
 ewah/operators/sql_base.py
 ewah/operators/sql_bigquery.py
-ewah/operators/sql_mssql.py
 ewah/operators/sql_mysql.py
 ewah/operators/sql_oracle.py
 ewah/operators/sql_postgres.py
 ewah/operators/stripe.py
 ewah/operators/zendesk.py
 ewah/uploaders/__init__.py
 ewah/uploaders/base.py
```

### Comparing `ewah-0.8.84/setup.py` & `ewah-0.8.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,34 +21,29 @@
         "License :: OSI Approved :: MIT License",
     ],
     python_requires=">=3.6",
     install_requires=[
         "avro",
         "azure-storage-blob>=2.1.0",  # a temporay 2.0.0 bugfix
         "dbt-metabase",
-        "croniter",
         "cx_Oracle",
         "facebook_business",
-        "google-ads>=16.0.0",
+        "google-ads>=13.0.0",
         "google-cloud-bigquery",
         "google-cloud-storage",
         "googlemaps",
         "gspread>=3.6",
         "Jinja2",
         "mailchimp3",
         "oauth2client",
         "Office365-REST-Python-Client",
         "openpyxl",
-        "protobuf",
         "psycopg2",
-        "pyairtable",
         "pymongo",
-        "pymssql",
         "pymysql",
-        "python-dateutil",
         "pytz",
         "pyyaml",
         "recurly",
         "selenium",
         "simple-salesforce",
         "snowflake-connector-python>=2.3.8",  # 2.3.8 vendored urrlib3 and requests
         "sshtunnel>=0.2.2",
```

