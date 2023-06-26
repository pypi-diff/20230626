# Comparing `tmp/django-query-builder-3.0.1.tar.gz` & `tmp/django-query-builder-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-query-builder-3.0.1.tar", last modified: Tue Aug 23 02:25:40 2022, max compression
+gzip compressed data, was "django-query-builder-3.1.0.tar", last modified: Mon Jun 26 21:11:41 2023, max compression
```

## Comparing `django-query-builder-3.0.1.tar` & `django-query-builder-3.1.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 02:25:40.611305 django-query-builder-3.0.1/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/LICENSE
--rw-rw-r--   0 wes       (1000) wes       (1000)      109 2022-08-22 19:30:11.000000 django-query-builder-3.0.1/MANIFEST.in
--rw-rw-r--   0 wes       (1000) wes       (1000)     3448 2022-08-23 02:25:40.611305 django-query-builder-3.0.1/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     2063 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/README.rst
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 02:25:40.603305 django-query-builder-3.0.1/django_query_builder.egg-info/
--rw-rw-r--   0 wes       (1000) wes       (1000)     3448 2022-08-23 02:25:40.000000 django-query-builder-3.0.1/django_query_builder.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1522 2022-08-23 02:25:40.000000 django-query-builder-3.0.1/django_query_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2022-08-23 02:25:40.000000 django-query-builder-3.0.1/django_query_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       44 2022-08-23 02:25:40.000000 django-query-builder-3.0.1/django_query_builder.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       13 2022-08-23 02:25:40.000000 django-query-builder-3.0.1/django_query_builder.egg-info/top_level.txt
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 02:25:40.603305 django-query-builder-3.0.1/docs/
--rw-rw-r--   0 wes       (1000) wes       (1000)     4392 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/docs/conf.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      235 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/manage.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      408 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/publish.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 02:25:40.607305 django-query-builder-3.0.1/querybuilder/
--rw-rw-r--   0 wes       (1000) wes       (1000)      109 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      141 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    27702 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/fields.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/groups.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1461 2022-08-19 20:19:29.000000 django-query-builder-3.0.1/querybuilder/helpers.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1670 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/logger.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      560 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/paginator.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    78700 2022-08-22 21:56:03.000000 django-query-builder-3.0.1/querybuilder/query.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    13535 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tables.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 02:25:40.611305 django-query-builder-3.0.1/querybuilder/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)       70 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     7461 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/aggregate_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      182 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      125 2022-08-19 22:01:44.000000 django-query-builder-3.0.1/querybuilder/tests/base.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     7342 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/date_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     6838 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/field_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1765 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/group_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4080 2022-08-19 22:02:02.000000 django-query-builder-3.0.1/querybuilder/tests/helper_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2643 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/insert_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     7750 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/join_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4632 2022-08-22 19:14:13.000000 django-query-builder-3.0.1/querybuilder/tests/json_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1212 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/limit_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     5606 2022-08-19 22:04:11.000000 django-query-builder-3.0.1/querybuilder/tests/logger_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 02:25:40.611305 django-query-builder-3.0.1/querybuilder/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     3519 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1679 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1804 2022-08-19 21:59:14.000000 django-query-builder-3.0.1/querybuilder/tests/order_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     8012 2022-08-19 22:03:07.000000 django-query-builder-3.0.1/querybuilder/tests/query_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    19400 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/select_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     6766 2022-08-19 22:04:26.000000 django-query-builder-3.0.1/querybuilder/tests/table_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     6323 2022-08-22 20:38:36.000000 django-query-builder-3.0.1/querybuilder/tests/update_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     8203 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/upsert_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      655 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/utils.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    14133 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/where_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    14211 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/tests/window_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      114 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/querybuilder/urls.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       22 2022-08-22 19:27:59.000000 django-query-builder-3.0.1/querybuilder/version.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 02:25:40.611305 django-query-builder-3.0.1/requirements/
--rw-rw-r--   0 wes       (1000) wes       (1000)       31 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/requirements/docs.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      105 2022-08-22 19:14:13.000000 django-query-builder-3.0.1/requirements/requirements-testing.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       44 2022-08-19 21:08:15.000000 django-query-builder-3.0.1/requirements/requirements.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      840 2021-04-21 17:36:07.000000 django-query-builder-3.0.1/run_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2267 2022-08-22 19:14:13.000000 django-query-builder-3.0.1/settings.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      264 2022-08-23 02:25:40.611305 django-query-builder-3.0.1/setup.cfg
--rw-rw-r--   0 wes       (1000) wes       (1000)     1930 2022-08-19 20:00:11.000000 django-query-builder-3.0.1/setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:11:41.478762 django-query-builder-3.1.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)      109 2022-08-22 19:30:11.000000 django-query-builder-3.1.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2960 2023-06-26 21:11:41.478762 django-query-builder-3.1.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2056 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:11:41.478762 django-query-builder-3.1.0/django_query_builder.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2960 2023-06-26 21:11:41.000000 django-query-builder-3.1.0/django_query_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1580 2023-06-26 21:11:41.000000 django-query-builder-3.1.0/django_query_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-26 21:11:41.000000 django-query-builder-3.1.0/django_query_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       40 2023-06-26 21:11:41.000000 django-query-builder-3.1.0/django_query_builder.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       13 2023-06-26 21:11:41.000000 django-query-builder-3.1.0/django_query_builder.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:11:41.478762 django-query-builder-3.1.0/docs/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4392 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/docs/conf.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      604 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/manage.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      408 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/publish.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:11:41.478762 django-query-builder-3.1.0/querybuilder/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      141 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6547 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/cursor.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    27702 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/fields.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/groups.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1461 2022-08-19 20:19:29.000000 django-query-builder-3.1.0/querybuilder/helpers.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1670 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/logger.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      560 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/paginator.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    78870 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/query.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    13475 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/tables.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:11:41.478762 django-query-builder-3.1.0/querybuilder/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7461 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/aggregate_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      182 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      125 2022-08-19 22:01:44.000000 django-query-builder-3.1.0/querybuilder/tests/base.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      559 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/tests/cursor_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7342 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/date_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6838 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/field_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1765 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/group_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4080 2022-08-19 22:02:02.000000 django-query-builder-3.1.0/querybuilder/tests/helper_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2643 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/insert_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7750 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/join_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4288 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/tests/json_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1212 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/limit_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     5606 2022-08-19 22:04:11.000000 django-query-builder-3.1.0/querybuilder/tests/logger_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:11:41.478762 django-query-builder-3.1.0/querybuilder/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3188 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1681 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1804 2022-08-19 21:59:14.000000 django-query-builder-3.1.0/querybuilder/tests/order_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     8012 2022-08-19 22:03:07.000000 django-query-builder-3.1.0/querybuilder/tests/query_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    19400 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/select_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6766 2022-08-19 22:04:26.000000 django-query-builder-3.1.0/querybuilder/tests/table_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6323 2022-08-22 20:38:36.000000 django-query-builder-3.1.0/querybuilder/tests/update_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     8203 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/upsert_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      655 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/utils.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    14133 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/where_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    14211 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/querybuilder/tests/window_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       37 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/querybuilder/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:11:41.478762 django-query-builder-3.1.0/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       31 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/requirements/docs.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       82 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       40 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      840 2021-04-21 17:36:07.000000 django-query-builder-3.1.0/run_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2293 2023-06-26 21:11:01.000000 django-query-builder-3.1.0/settings.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      268 2023-06-26 21:11:41.482762 django-query-builder-3.1.0/setup.cfg
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1930 2022-08-19 20:00:11.000000 django-query-builder-3.1.0/setup.py
```

### Comparing `django-query-builder-3.0.1/LICENSE` & `django-query-builder-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/PKG-INFO` & `django-query-builder-3.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,83 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-query-builder
-Version: 3.0.1
+Version: 3.1.0
 Summary: Build complex nested queries
 Home-page: https://github.com/ambitioninc/django-query-builder
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/ambitioninc/django-query-builder.png
-           :target: https://travis-ci.org/ambitioninc/django-query-builder
-        
-        .. image:: https://coveralls.io/repos/ambitioninc/django-query-builder/badge.png?branch=develop
-            :target: https://coveralls.io/r/ambitioninc/django-query-builder?branch=develop
-        
-        .. image:: https://pypip.in/v/django-query-builder/badge.png
-            :target: https://crate.io/packages/django-query-builder/
-            :alt: Latest PyPI version
-        
-        .. image:: https://pypip.in/d/django-query-builder/badge.png
-            :target: https://crate.io/packages/django-query-builder/
-        
-        django-query-builder
-        ====================
-        querybuilder is a django library for assisting with the construction and
-        execution of sql. This is not meant to replace django querysets; it is meant
-        for managing complex queries and helping perform database operations that
-        django doesn't handle.
-        
-        Why use querybuilder?
-        ---------------------
-        The django querybuilder allows you to control all parts of the query
-        construction. This is happens more clearly because the function calls more
-        closely represent the actual sql keywords.
-        
-        Why not just use django's .raw() function?
-        ------------------------------------------
-        While the raw function lets you execute custom sql, it doesn't provide any way
-        for the developer to build the query dynamically. Users lacking experience
-        writing "raw" sql should avoid using querybuilder and stick with django's
-        querysets. The querybuilder's query construction closely mirrors writing sql,
-        where django querysets simplify the sql generation process for simple queries.
-        
-        Requirements
-        ------------
-        * Python 2.7
-        * Python 3.3, 3.4
-        * Django 1.7+
-        * Postgres 9.3+
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install django-query-builder
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/django-query-builder.git
-        
-        Documentation
-        -------------
-        
-        Full documentation is available at http://django-query-builder.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-        
 Keywords: django,database,query,sql,postgres,upsert
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/django-query-builder.png
+   :target: https://travis-ci.org/ambitioninc/django-query-builder
+
+.. image:: https://coveralls.io/repos/ambitioninc/django-query-builder/badge.png?branch=develop
+    :target: https://coveralls.io/r/ambitioninc/django-query-builder?branch=develop
+
+.. image:: https://pypip.in/v/django-query-builder/badge.png
+    :target: https://crate.io/packages/django-query-builder/
+    :alt: Latest PyPI version
+
+.. image:: https://pypip.in/d/django-query-builder/badge.png
+    :target: https://crate.io/packages/django-query-builder/
+
+django-query-builder
+====================
+querybuilder is a django library for assisting with the construction and
+execution of sql. This is not meant to replace django querysets; it is meant
+for managing complex queries and helping perform database operations that
+django doesn't handle.
+
+Why use querybuilder?
+---------------------
+The django querybuilder allows you to control all parts of the query
+construction. This is happens more clearly because the function calls more
+closely represent the actual sql keywords.
+
+Why not just use django's .raw() function?
+------------------------------------------
+While the raw function lets you execute custom sql, it doesn't provide any way
+for the developer to build the query dynamically. Users lacking experience
+writing "raw" sql should avoid using querybuilder and stick with django's
+querysets. The querybuilder's query construction closely mirrors writing sql,
+where django querysets simplify the sql generation process for simple queries.
+
+Requirements
+------------
+* Python 3.7 - 3.9
+* Django 2.2 - 4.1
+* Postgres 9.3+
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install django-query-builder
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/django-query-builder.git
+
+Documentation
+-------------
+
+Full documentation is available at http://django-query-builder.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

### Comparing `django-query-builder-3.0.1/README.rst` & `django-query-builder-3.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,16 @@
 for the developer to build the query dynamically. Users lacking experience
 writing "raw" sql should avoid using querybuilder and stick with django's
 querysets. The querybuilder's query construction closely mirrors writing sql,
 where django querysets simplify the sql generation process for simple queries.
 
 Requirements
 ------------
-* Python 2.7
-* Python 3.3, 3.4
-* Django 1.7+
+* Python 3.7 - 3.9
+* Django 2.2 - 4.1
 * Postgres 9.3+
 
 Installation
 ------------
 To install the latest release, type::
 
     pip install django-query-builder
```

### Comparing `django-query-builder-3.0.1/django_query_builder.egg-info/PKG-INFO` & `django-query-builder-3.1.0/django_query_builder.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,83 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-query-builder
-Version: 3.0.1
+Version: 3.1.0
 Summary: Build complex nested queries
 Home-page: https://github.com/ambitioninc/django-query-builder
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/ambitioninc/django-query-builder.png
-           :target: https://travis-ci.org/ambitioninc/django-query-builder
-        
-        .. image:: https://coveralls.io/repos/ambitioninc/django-query-builder/badge.png?branch=develop
-            :target: https://coveralls.io/r/ambitioninc/django-query-builder?branch=develop
-        
-        .. image:: https://pypip.in/v/django-query-builder/badge.png
-            :target: https://crate.io/packages/django-query-builder/
-            :alt: Latest PyPI version
-        
-        .. image:: https://pypip.in/d/django-query-builder/badge.png
-            :target: https://crate.io/packages/django-query-builder/
-        
-        django-query-builder
-        ====================
-        querybuilder is a django library for assisting with the construction and
-        execution of sql. This is not meant to replace django querysets; it is meant
-        for managing complex queries and helping perform database operations that
-        django doesn't handle.
-        
-        Why use querybuilder?
-        ---------------------
-        The django querybuilder allows you to control all parts of the query
-        construction. This is happens more clearly because the function calls more
-        closely represent the actual sql keywords.
-        
-        Why not just use django's .raw() function?
-        ------------------------------------------
-        While the raw function lets you execute custom sql, it doesn't provide any way
-        for the developer to build the query dynamically. Users lacking experience
-        writing "raw" sql should avoid using querybuilder and stick with django's
-        querysets. The querybuilder's query construction closely mirrors writing sql,
-        where django querysets simplify the sql generation process for simple queries.
-        
-        Requirements
-        ------------
-        * Python 2.7
-        * Python 3.3, 3.4
-        * Django 1.7+
-        * Postgres 9.3+
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install django-query-builder
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/django-query-builder.git
-        
-        Documentation
-        -------------
-        
-        Full documentation is available at http://django-query-builder.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-        
 Keywords: django,database,query,sql,postgres,upsert
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/django-query-builder.png
+   :target: https://travis-ci.org/ambitioninc/django-query-builder
+
+.. image:: https://coveralls.io/repos/ambitioninc/django-query-builder/badge.png?branch=develop
+    :target: https://coveralls.io/r/ambitioninc/django-query-builder?branch=develop
+
+.. image:: https://pypip.in/v/django-query-builder/badge.png
+    :target: https://crate.io/packages/django-query-builder/
+    :alt: Latest PyPI version
+
+.. image:: https://pypip.in/d/django-query-builder/badge.png
+    :target: https://crate.io/packages/django-query-builder/
+
+django-query-builder
+====================
+querybuilder is a django library for assisting with the construction and
+execution of sql. This is not meant to replace django querysets; it is meant
+for managing complex queries and helping perform database operations that
+django doesn't handle.
+
+Why use querybuilder?
+---------------------
+The django querybuilder allows you to control all parts of the query
+construction. This is happens more clearly because the function calls more
+closely represent the actual sql keywords.
+
+Why not just use django's .raw() function?
+------------------------------------------
+While the raw function lets you execute custom sql, it doesn't provide any way
+for the developer to build the query dynamically. Users lacking experience
+writing "raw" sql should avoid using querybuilder and stick with django's
+querysets. The querybuilder's query construction closely mirrors writing sql,
+where django querysets simplify the sql generation process for simple queries.
+
+Requirements
+------------
+* Python 3.7 - 3.9
+* Django 2.2 - 4.1
+* Postgres 9.3+
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install django-query-builder
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/django-query-builder.git
+
+Documentation
+-------------
+
+Full documentation is available at http://django-query-builder.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

### Comparing `django-query-builder-3.0.1/django_query_builder.egg-info/SOURCES.txt` & `django-query-builder-3.1.0/django_query_builder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 django_query_builder.egg-info/SOURCES.txt
 django_query_builder.egg-info/dependency_links.txt
 django_query_builder.egg-info/requires.txt
 django_query_builder.egg-info/top_level.txt
 docs/conf.py
 querybuilder/__init__.py
 querybuilder/apps.py
+querybuilder/cursor.py
 querybuilder/fields.py
 querybuilder/groups.py
 querybuilder/helpers.py
 querybuilder/logger.py
 querybuilder/paginator.py
 querybuilder/query.py
 querybuilder/tables.py
 querybuilder/urls.py
 querybuilder/version.py
 querybuilder/tests/__init__.py
 querybuilder/tests/aggregate_tests.py
 querybuilder/tests/apps.py
 querybuilder/tests/base.py
+querybuilder/tests/cursor_tests.py
 querybuilder/tests/date_tests.py
 querybuilder/tests/field_tests.py
 querybuilder/tests/group_tests.py
 querybuilder/tests/helper_tests.py
 querybuilder/tests/insert_tests.py
 querybuilder/tests/join_tests.py
 querybuilder/tests/json_tests.py
```

### Comparing `django-query-builder-3.0.1/docs/conf.py` & `django-query-builder-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/fields.py` & `django-query-builder-3.1.0/querybuilder/fields.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/helpers.py` & `django-query-builder-3.1.0/querybuilder/helpers.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/logger.py` & `django-query-builder-3.1.0/querybuilder/logger.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/paginator.py` & `django-query-builder-3.1.0/querybuilder/paginator.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/query.py` & `django-query-builder-3.1.0/querybuilder/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from django.db.models import Q, AutoField
 from django.db.models.query import QuerySet
 from django.db.models.constants import LOOKUP_SEP
 from django.apps import apps
 get_model = apps.get_model
 import six
 
-
 from querybuilder.fields import FieldFactory, CountField, MaxField, MinField, SumField, AvgField
 from querybuilder.helpers import set_value_for_keypath, copy_instance
 from querybuilder.tables import TableFactory, ModelTable, QueryTable
+from querybuilder.cursor import json_fetch_all_as_dict
+
 
 SERIAL_DTYPES = ['serial', 'bigserial']
 
 
 class Join(object):
     """
     Represents the JOIN clauses of a Query. The join can be of any join type.
@@ -636,15 +637,19 @@
     def get_cursor(self):
         """
         Get a cursor for the Query's connection
 
         :rtype: :class:`CursorDebugWrapper <django:django.db.backends.util.CursorDebugWrapper>`
         :returns: A database cursor
         """
-        return self.connection.cursor()
+        cursor = self.connection.cursor()
+        # Do not set up the cursor in psycopg2 to run json.loads on jsonb columns here. Do it
+        # right before we run a select, and then set it back after that.
+        # jsonify_cursor(cursor)
+        return cursor
 
     def from_table(self, table=None, fields='*', schema=None, **kwargs):
         """
         Adds a ``Table`` and any optional fields to the list of tables
         this query is selecting from.
 
         :type table: str or dict or :class:`Table <querybuilder.tables.Table>`
@@ -1932,19 +1937,15 @@
     def _fetch_all_as_dict(self, cursor):
         """
         Iterates over the result set and converts each row to a dictionary
 
         :return: A list of dictionaries where each row is a dictionary
         :rtype: list of dict
         """
-        desc = cursor.description
-        return [
-            dict(zip([col[0] for col in desc], row))
-            for row in cursor.fetchall()
-        ]
+        return json_fetch_all_as_dict(cursor)
 
 
 class QueryWindow(Query):
     """
     This is a query window that is meant to be used in the OVER clause of
     window functions. It extends ``Query``, but the only methods that will
     be used are ``order_by`` and ``partition_by`` (which just calls ``group_by``)
```

### Comparing `django-query-builder-3.0.1/querybuilder/tables.py` & `django-query-builder-3.1.0/querybuilder/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import abc
+from abc import ABCMeta
 
 from django.db.models.base import ModelBase
-from six import string_types, with_metaclass
 
 import querybuilder
 from querybuilder.fields import FieldFactory
 
 
 class TableFactory(object):
     """
@@ -27,28 +26,28 @@
         """
         # Determine the type of the table
         table_type = type(table)
         if table_type is dict:
             kwargs.update(alias=list(table.keys())[0])
             table = list(table.values())[0]
             table_type = type(table)
-        if isinstance(table, string_types):
+        if isinstance(table, str):
             return SimpleTable(table, **kwargs)
         elif issubclass(table_type, ModelBase):
             return ModelTable(table, **kwargs)
         elif table_type is querybuilder.query.Query:
             return QueryTable(table, **kwargs)
         elif isinstance(table, Table):
             for key, value in kwargs.items():
                 setattr(table, key, value)
             return table
         return None
 
 
-class Table(with_metaclass(abc.ABCMeta, object)):
+class Table(object, metaclass=ABCMeta):
     """
     Abstract table class that all table types extend.
 
     Properties:
 
         name: str
             The name that identifies this table if there is no alias
@@ -255,15 +254,15 @@
         Adds all of the passed fields to the table's current field list
 
         :param fields: The fields to select from ``table``. This can be
             a single field, a tuple of fields, or a list of fields. Each field can be a string
             or ``Field`` instance
         :type fields: str or tuple or list of str or list of Field or :class:`Field <querybuilder.fields.Field>`
         """
-        if isinstance(fields, string_types):
+        if isinstance(fields, str):
             fields = [fields]
         elif type(fields) is tuple:
             fields = list(fields)
 
         field_objects = [self.add_field(field) for field in fields]
         return field_objects
```

### Comparing `django-query-builder-3.0.1/querybuilder/tests/aggregate_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/aggregate_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/date_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/date_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/field_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/field_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/group_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/group_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/helper_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/helper_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/insert_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/insert_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/join_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/join_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/json_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/json_tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import unittest
-from django import VERSION
 from django.test.utils import override_settings
 from querybuilder.fields import JsonField
 from querybuilder.query import Query, JsonQueryset
 from querybuilder.tests.base import QuerybuilderTestCase
 from querybuilder.tests.models import MetricRecord
 from querybuilder.tests.utils import get_postgres_version
 
@@ -43,55 +42,49 @@
             query.get_sql(),
             (
                 'SELECT querybuilder_tests_metricrecord.data->\'two\' AS "my_two_alias" FROM '
                 'querybuilder_tests_metricrecord WHERE (querybuilder_tests_metricrecord.data->>\'two\' = %(A0)s)'
             )
         )
 
-        # Django 3.1 changes the raw queryset behavior so querybuilder isn't going to change that behavior
-        if self.is_31_or_above():
-            self.assertEqual(query.select(), [{'my_two_alias': '"two"'}])
-        else:
-            self.assertEqual(query.select(), [{'my_two_alias': 'two'}])
+        self.assertEqual(query.select(), [{'my_two_alias': 'two'}])
 
         query = Query().from_table(MetricRecord, fields=[one_field]).where(**{
             one_field.get_where_key(): '1'
         })
         self.assertEqual(
             query.get_sql(),
             (
                 'SELECT querybuilder_tests_metricrecord.data->\'one\' AS "my_one_alias" FROM '
                 'querybuilder_tests_metricrecord WHERE (querybuilder_tests_metricrecord.data->>\'one\' = %(A0)s)'
             )
         )
 
-        # Django 3.1 changes the raw queryset behavior so querybuilder isn't going to change that behavior
-        if self.is_31_or_above():
-            self.assertEqual(query.select(), [{'my_one_alias': '1'}])
-        else:
-            self.assertEqual(query.select(), [{'my_one_alias': 1}])
+        self.assertEqual(query.select(), [{'my_one_alias': 1}])
 
         query = Query().from_table(MetricRecord, fields=[one_field]).where(**{
             one_field.get_where_key(): '2'
         })
         self.assertEqual(
             query.get_sql(),
             (
                 'SELECT querybuilder_tests_metricrecord.data->\'one\' AS "my_one_alias" FROM '
                 'querybuilder_tests_metricrecord WHERE (querybuilder_tests_metricrecord.data->>\'one\' = %(A0)s)'
             )
         )
         self.assertEqual(query.select(), [])
 
-    def is_31_or_above(self):
-        if VERSION[0] == 3 and VERSION[1] >= 1:
-            return True
-        elif VERSION[0] > 3:
-            return True
-        return False
+    # Currently unused (but maybe again sometime) function to check django version for test results
+    # from django import VERSION
+    # def is_31_or_above(self):
+    #     if VERSION[0] == 3 and VERSION[1] >= 1:
+    #         return True
+    #     elif VERSION[0] > 3:
+    #         return True
+    #     return False
 
 
 @override_settings(DEBUG=True)
 class JsonQuerysetTest(QuerybuilderTestCase):
 
     def test_one(self):
         if get_postgres_version() < (9, 4):
```

### Comparing `django-query-builder-3.0.1/querybuilder/tests/limit_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/limit_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/logger_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/logger_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/migrations/0001_initial.py` & `django-query-builder-3.1.0/querybuilder/tests/migrations/0001_initial.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,13 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.9.1 on 2016-02-12 19:03
-from __future__ import unicode_literals
 
 from querybuilder.tests.utils import get_postgres_version
 
 # These migrations should only be run during tests and not in your installed app.
-try:
-    if get_postgres_version() < (9, 4):
-        raise ImportError('Invalid Postgres version')
-    import django.contrib.postgres.fields.jsonb
-    json_field = django.contrib.postgres.fields.jsonb.JSONField()
-except ImportError:
-    import jsonfield.fields
-    json_field = jsonfield.fields.JSONField()
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     initial = True
@@ -34,15 +25,15 @@
             ],
         ),
         migrations.CreateModel(
             name='MetricRecord',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('other_value', models.FloatField(default=0)),
-                ('data', json_field),
+                ('data', models.JSONField()),
             ],
         ),
         migrations.CreateModel(
             name='Order',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('revenue', models.FloatField(null=True)),
@@ -59,15 +50,15 @@
                 ('field1', models.CharField(max_length=16, unique=True)),
                 ('field2', models.CharField(max_length=16, unique=True)),
                 ('field3', models.CharField(max_length=16)),
                 ('field4', models.CharField(default=b'default_value', max_length=16)),
                 ('field5', models.CharField(default=None, max_length=16, null=True)),
                 ('field6', models.CharField(max_length=16)),
                 ('field7', models.CharField(max_length=16)),
-                ('field8', json_field),
+                ('field8', models.JSONField()),
                 ('custom_field_name', models.CharField(max_length=16, null=True, default='foo', db_column='actual_db_column_name')),
             ],
         ),
         migrations.CreateModel(
             name='User',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
```

### Comparing `django-query-builder-3.0.1/querybuilder/tests/models.py` & `django-query-builder-3.1.0/querybuilder/tests/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,14 @@
     field1 = models.CharField(unique=True, max_length=16)
     field2 = models.CharField(unique=True, max_length=16)
     field3 = models.CharField(max_length=16)
     field4 = models.CharField(max_length=16, default='default_value')
     field5 = models.CharField(max_length=16, null=True, default=None)
     field6 = models.CharField(max_length=16)
     field7 = models.CharField(max_length=16)
-    field8 = JSONField(default={})
+    field8 = JSONField(default=dict)
     custom_field_name = models.CharField(
         max_length=16, null=True, default='foo', db_column='actual_db_column_name'
     )
 
     class Meta:
         unique_together = ('field6', 'field7')
```

### Comparing `django-query-builder-3.0.1/querybuilder/tests/order_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/order_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/query_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/query_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/select_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/select_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/table_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/table_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/update_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/update_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/upsert_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/upsert_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/utils.py` & `django-query-builder-3.1.0/querybuilder/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/where_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/where_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/querybuilder/tests/window_tests.py` & `django-query-builder-3.1.0/querybuilder/tests/window_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/run_tests.py` & `django-query-builder-3.1.0/run_tests.py`

 * *Files identical despite different names*

### Comparing `django-query-builder-3.0.1/settings.py` & `django-query-builder-3.1.0/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,22 +47,22 @@
         # Check env for db override (used for github actions)
         if os.environ.get('DB_SETTINGS2'):
             db_config2 = json.loads(os.environ.get('DB_SETTINGS2'))
 
         settings.configure(
             TEST_RUNNER='django_nose.NoseTestSuiteRunner',
             NOSE_ARGS=['--nocapture', '--nologcapture', '--verbosity=1'],
-            MIDDLEWARE_CLASSES=(),
             DATABASES={
                 'default': db_config,
                 'mock-second-database': db_config2,
             },
             INSTALLED_APPS=(
                 'django.contrib.auth',
                 'django.contrib.contenttypes',
                 'querybuilder',
                 'querybuilder.tests',
             ),
             ROOT_URLCONF='querybuilder.urls',
             TIME_ZONE='UTC',
             USE_TZ=False,
+            DEFAULT_AUTO_FIELD='django.db.models.AutoField',
         )
```

### Comparing `django-query-builder-3.0.1/setup.py` & `django-query-builder-3.1.0/setup.py`

 * *Files identical despite different names*

