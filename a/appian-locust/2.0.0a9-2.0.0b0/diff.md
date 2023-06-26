# Comparing `tmp/appian-locust-2.0.0a9.tar.gz` & `tmp/appian-locust-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.0.0a9.tar", last modified: Tue Jun 13 21:44:15 2023, max compression
+gzip compressed data, was "appian-locust-2.0.0b0.tar", last modified: Mon Jun 26 16:49:14 2023, max compression
```

## Comparing `appian-locust-2.0.0a9.tar` & `appian-locust-2.0.0b0.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.768547 appian-locust-2.0.0a9/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5449 2023-06-13 21:44:15.768547 appian-locust-2.0.0a9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4875 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.763548 appian-locust-2.0.0a9/appian_locust/
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9592 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2498 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_design.py
--rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_feature_toggle_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7849 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_grid_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)    52246 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)     5177 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_locust_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7747 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_portals.py
--rw-rw-rw-   0 root         (0) root         (0)    16611 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_records.py
--rw-rw-rw-   0 root         (0) root         (0)     7390 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_records_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7474 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_save_request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     9939 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_sites.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_task_opener.py
--rw-rw-rw-   0 root         (0) root         (0)     7653 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_ui_reconciler.py
--rw-rw-rw-   0 root         (0) root         (0)    16940 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/appianclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.764547 appian-locust-2.0.0a9/appian_locust/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/exceptions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/exceptions/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/feature_flag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.765547 appian-locust-2.0.0a9/appian_locust/info/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/actions_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/news_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/records_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/reports_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1258 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/sites_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/tasks_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.766548 appian-locust-2.0.0a9/appian_locust/objects/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/application.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/design_object.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/page.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/site.py
--rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/system_operator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.767547 appian-locust-2.0.0a9/appian_locust/uiform/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/application_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/design_object_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/design_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/record_list_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1322 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/record_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)    73478 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/uiform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.768547 appian-locust-2.0.0a9/appian_locust/utilities/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16347 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/utilities/helper.py
--rwxrwxrwx   0 root         (0) root         (0)     1393 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/utilities/loadDriverUtils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/utilities/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    14863 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.764547 appian-locust-2.0.0a9/appian_locust.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5449 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1786 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-13 21:44:15.768547 appian-locust-2.0.0a9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.510967 appian-locust-2.0.0b0/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5449 2023-06-26 16:49:14.510967 appian-locust-2.0.0b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.505967 appian-locust-2.0.0b0/appian_locust/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9592 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2498 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_design.py
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_feature_toggle_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7849 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_grid_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)    52958 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5177 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_locust_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7747 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_portals.py
+-rw-rw-rw-   0 root         (0) root         (0)    15240 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     7390 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_records_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7474 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_save_request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9939 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_sites.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_task_opener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_ui_reconciler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7334 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/appian_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/appian_task_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.506967 appian-locust-2.0.0b0/appian_locust/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/exceptions/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/feature_flag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.507967 appian-locust-2.0.0b0/appian_locust/info/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/actions_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/news_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/records_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/reports_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/sites_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/tasks_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.508967 appian-locust-2.0.0b0/appian_locust/objects/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/application.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/design_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/page.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/site.py
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/system_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.509967 appian-locust-2.0.0b0/appian_locust/uiform/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/application_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/design_object_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/design_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4395 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/record_list_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/record_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)    73472 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/uiform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.510967 appian-locust-2.0.0b0/appian_locust/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)    16347 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1393 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/loadDriverUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    14525 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.506967 appian-locust-2.0.0b0/appian_locust.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5449 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-26 16:49:14.511968 appian-locust-2.0.0b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/setup.py
```

### Comparing `appian-locust-2.0.0a9/LICENSE` & `appian-locust-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/PKG-INFO` & `appian-locust-2.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a9
+Version: 2.0.0b0
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a9/README.rst` & `appian-locust-2.0.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_actions.py` & `appian-locust-2.0.0b0/appian_locust/_actions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_admin.py` & `appian-locust-2.0.0b0/appian_locust/_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_base.py` & `appian-locust-2.0.0b0/appian_locust/_base.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_design.py` & `appian-locust-2.0.0b0/appian_locust/_design.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.0.0b0/appian_locust/_feature_toggle_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_grid_interactor.py` & `appian-locust-2.0.0b0/appian_locust/_grid_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_interactor.py` & `appian-locust-2.0.0b0/appian_locust/_interactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,14 +421,16 @@
             site_name: name of site for link in starting process model.
             page_name: name of page for link in starting process model.
             is_mobile: indicates if it should hit the mobile endpoint.
             locust_request_label: label to be used within locust
 
         Returns: the response of get Start Process Link operation as json
         '''
+        if self.url_pattern_version == 1:
+            page_name = f"p.{page_name}"
         if is_mobile:
             spl_link_url = f"/suite/rest/a/model/latest/startProcess/{process_model_opaque_id}?cacheKey={cache_key}"
         else:
             spl_link_url = f"/suite/rest/a/sites/latest/{site_name}/page/{page_name}/startProcess/{process_model_opaque_id}?cacheKey={cache_key}"
 
         headers = self.setup_sail_headers()
         locust_label = locust_request_label or "Clicking StartProcessLink: " + component["label"]
@@ -479,14 +481,25 @@
                 resp = self.post_page(
                     self.host + related_action_link_url, payload={}, headers=headers, label=locust_label
                 )
             else:
                 return json_response
         return resp.json()
 
+    def click_record_list_action(self, component: Dict[str, Any], process_model_uuid: str,
+                                 cache_key: str, locust_request_label: Optional[str] = None) -> Dict[str, Any]:
+        record_list_action_url = f"/suite/rest/a/model/latest/{process_model_uuid}/forminternal?cacheKey={cache_key}"
+
+        headers = self.setup_sail_headers()
+        locust_label = locust_request_label or "Clicking RecordListAction: " + component["label"]
+        resp = self.post_page(
+            self.host + record_list_action_url, payload={}, headers=headers, label=locust_label
+        )
+        return resp.json()
+
     # COMPONENT RELATED METHODS
 
     def click_component(self, post_url: str, component: Dict[str, Any], context: Dict[str, Any],
                         uuid: str, label: Optional[str] = None, headers: Optional[Dict[str, Any]] = None,
                         client_mode: Optional[str] = None) -> Dict[str, Any]:
         '''
             Calls the post operation to click certain SAIL components such as Buttons and Dynamic Links
```

### Comparing `appian-locust-2.0.0a9/appian_locust/_locust_error_handler.py` & `appian-locust-2.0.0b0/appian_locust/_locust_error_handler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_news.py` & `appian-locust-2.0.0b0/appian_locust/_news.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_portals.py` & `appian-locust-2.0.0b0/appian_locust/_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_records.py` & `appian-locust-2.0.0b0/appian_locust/_records.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,32 +20,34 @@
 RECORDS_NAV_PATH = ["/suite/rest/a/sites/latest/D6JMim/page/", "records", "/nav"]
 RECORDS_MOBILE_PATH = "/suite/rest/a/applications/latest/legacy/tempo/records/type/"
 RECORD_TYPE_VIEW_PATH = "/suite/rest/a/sites/latest/D6JMim/pages/records/recordType/"
 RECORD_VIEW_PATH = ["/suite/rest/a/sites/latest/", "/page/records/record/", "/view/"]
 
 
 class _Records(_Base):
-    def __init__(self, interactor: _Interactor) -> None:
+    def __init__(self, interactor: _Interactor, is_mobile_client: bool = False) -> None:
         """
         Records class wrapping list of possible activities can be performed with Appian-Tempo-Records.
 
         Warnings: This class is internal and should not be accessed by tests directly. It can be accessed via the "appian" object
 
         Note: "appian" is created as part of ``AppianTaskSet``'s ``on_start`` function
 
         Args:
             session: Locust session/client object
             host (str): Host URL
+            is_mobile_client(bool): If we are running from a mobile client
         """
         self.interactor = interactor
 
         # When Get All functions called, these variables will be used to cache the values
         self._record_types: Dict[str, Any] = dict()
         self._records: Dict[str, Any] = dict()
         self._errors: int = 0
+        self._is_mobile_client = is_mobile_client
 
     def get_records_interface(self, locust_request_label: Optional[str] = "Records") -> Dict[str, Any]:
         uri = self.interactor.host + RECORDS_INTERFACE_PATH
         headers = self.interactor.setup_sail_headers()
         resp = self.interactor.get_page(uri, headers, f'{locust_request_label}.Interface')
         return resp.json()
 
@@ -123,60 +125,23 @@
 
         Examples:
 
             >>> self.appian.records.get_all_records_of_record_type("record_type_name")
         """
         self._records[record_type] = dict()
 
-        json_response = self._record_type_list_request(record_type, search_string=search_string)
+        json_response = self._record_type_list_request(record_type, search_string=search_string, is_mobile=self._is_mobile_client)
 
         if column_index is not None:
             self._records[record_type], self._errors = get_records_from_json_by_column(json_response, column_index)
         else:
             self._records[record_type], self._errors = get_all_records_from_json(json_response)
 
         return self._records
 
-    def get_all_records_of_record_type_mobile(self, record_type: str, search_string: Optional[str] = None) -> Dict[str, Any]:
-        """
-        Retrieves all the available "records" for the given record type for a mobile device.
-
-        Todo: Partial match functionality is not yet implemented
-
-        Returns (dict): List of records and associated metadata
-
-        Examples:
-
-            >>> self.appian.records.get_all_records_of_record_type_mobile("record_type_name")
-        """
-        json_response = self._record_type_list_request(record_type, is_mobile=True, search_string=search_string)
-
-        self._records[record_type], self._errors = get_all_records_from_json(json_response)
-
-        return self._records
-
-    def get_all_mobile(self, search_string: Optional[str] = None) -> Dict[str, Any]:
-        """
-        Retrieves all available "records types" and "records" and associated metadata from "Appian-Tempo-Records"
-
-        Note: All the retrieved data about record types and records is stored in the private variables
-        self._record_types and self._records respectively
-
-        Returns (dict): List of records and associated metadata
-        """
-
-        if search_string:
-            # Format search string to be compatible with URLs
-            search_string = quote(search_string)
-
-        self.get_all_record_types()
-        for record_type in self._record_types:
-            self.get_all_records_of_record_type_mobile(record_type, search_string=search_string)
-        return self._records
-
     def fetch_record_instance(self, record_type: str, record_name: str, exact_match: bool = True) -> Dict[str, Any]:
         """
         Get the information about a specific record by specifying its name and its record type.
 
         Args:
             record_type (str): Name of the record type.
             record_name (str): Name of the record which should be available in the given record type
@@ -290,15 +255,15 @@
         uri = f"{RECORD_VIEW_PATH[0]}{tempo_site_url_stub}{RECORD_VIEW_PATH[1]}{opaque_id}{RECORD_VIEW_PATH[2]}{view_url_stub}"
         resp = self.interactor.get_page(uri=uri, headers=headers, label=locust_label)
         return resp.json()
 
     # Alias for the above function to allow backwards compatability
     visit = visit_record_instance
 
-    def visit_record_type(self, record_type: str = "", exact_match: bool = True, is_mobile: bool = False, locust_request_label: Optional[str] = None) -> Dict[str, Any]:
+    def visit_record_type(self, record_type: str = "", locust_request_label: Optional[str] = None) -> Dict[str, Any]:
         """
         Navigate into desired record type and retrieve all metadata for associated list of record views.
 
         Returns (dict): List of records and associated metadata
 
         Examples:
 
@@ -311,15 +276,15 @@
 
         # If no record_type is specified, a random one will be assigned
         if not record_type:
             record_type = self._get_random_record_type()
 
         locust_request_label = locust_request_label or f'Records.{record_type}.ListView'
 
-        return self._record_type_list_request(record_type, is_mobile=is_mobile, locust_request_label=locust_request_label)
+        return self._record_type_list_request(record_type, is_mobile=self._is_mobile_client, locust_request_label=locust_request_label)
 
     # ----- Private Functions ----- #
 
     def _is_response_good(self, response_text: str) -> bool:
         return ('"rel":"x-web-bookmark"' in response_text or '"#t":"CardLayout"' in response_text)
 
     def _get_random_record_instance(self, record_type: str = "") -> Tuple[str, str]:
```

### Comparing `appian-locust-2.0.0a9/appian_locust/_records_helper.py` & `appian-locust-2.0.0b0/appian_locust/_records_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_reports.py` & `appian-locust-2.0.0b0/appian_locust/_reports.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_save_request_builder.py` & `appian-locust-2.0.0b0/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_sites.py` & `appian-locust-2.0.0b0/appian_locust/_sites.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_task_opener.py` & `appian-locust-2.0.0b0/appian_locust/_task_opener.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_tasks.py` & `appian-locust-2.0.0b0/appian_locust/_tasks.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/_ui_reconciler.py` & `appian-locust-2.0.0b0/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/exceptions/exceptions.py` & `appian-locust-2.0.0b0/appian_locust/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/feature_flag.py` & `appian-locust-2.0.0b0/appian_locust/feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/info/actions_info.py` & `appian-locust-2.0.0b0/appian_locust/info/actions_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/info/news_info.py` & `appian-locust-2.0.0b0/appian_locust/info/news_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/info/records_info.py` & `appian-locust-2.0.0b0/appian_locust/info/records_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/info/reports_info.py` & `appian-locust-2.0.0b0/appian_locust/info/reports_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/info/sites_info.py` & `appian-locust-2.0.0b0/appian_locust/info/sites_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/info/tasks_info.py` & `appian-locust-2.0.0b0/appian_locust/info/tasks_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/objects/design_object.py` & `appian-locust-2.0.0b0/appian_locust/objects/design_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from enum import Enum
 
+
 class DesignObjectType(Enum):
     DATA_TYPE = 5
     DECISION = 6
     EXPRESSION_RULE = 8
     INTEGRATION = 12
     INTERFACE = 13
     RECORD_TYPE = 17
     SITE = 19
     WEB_API = 20
 
+
 class DesignObject:
     """
     Class representing an Design Object
     """
 
     def __init__(self, name: str, opaque_id: str):
         self.name = name
```

### Comparing `appian-locust-2.0.0a9/appian_locust/objects/page.py` & `appian-locust-2.0.0b0/appian_locust/objects/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 
+
 class PageType(Enum):
     ACTION: str = "action"
     REPORT: str = "report"
     RECORD: str = "recordType"
     INTERFACE: str = "interface"
```

### Comparing `appian-locust-2.0.0a9/appian_locust/system_operator.py` & `appian-locust-2.0.0b0/appian_locust/system_operator.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/uiform/application_uiform.py` & `appian-locust-2.0.0b0/appian_locust/uiform/application_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/uiform/design_object_uiform.py` & `appian-locust-2.0.0b0/appian_locust/uiform/design_object_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/uiform/design_uiform.py` & `appian-locust-2.0.0b0/appian_locust/uiform/design_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/uiform/record_list_uiform.py` & `appian-locust-2.0.0b0/appian_locust/uiform/record_list_uiform.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Dict, Optional
 from urllib.parse import quote
 
 from .._interactor import _Interactor
 from .._records_helper import get_all_records_from_json, get_records_from_json_by_column
-from .uiform import SailUiForm
+from ..utilities.helper import find_component_by_label_and_type_dict
+from .uiform import SailUiForm, START_PROCESS_LINK_TYPE
 
 
 class RecordListUiForm(SailUiForm):
     """
     UiForm representing a Record List from Tempo Records
     """
 
@@ -61,7 +62,31 @@
         Returns: Dictionary with record instance information
         """
         if column_index is not None:
             record_instances, _ = get_records_from_json_by_column(self._state, column_index)
         else:
             record_instances, _ = get_all_records_from_json(self._state)
         return record_instances
+
+    def click_record_list_action(self, label: str, locust_request_label: Optional[str] = None) -> 'RecordListUiForm':
+        """
+        Click on an action in a record list
+        Args:
+            label: The label of the record list action to click
+            locust_request_label: The label locust should associate with this request
+
+        Returns: UiForm with action clicked
+
+        """
+        component = find_component_by_label_and_type_dict('label', label, START_PROCESS_LINK_TYPE, self._state)
+        process_model_uuid = component.get("pmUuid", "")
+        cache_key = component.get("cacheKey", "")
+        if not process_model_uuid:
+            raise Exception(f"Record List Action component does not have process model UUID set.")
+        elif not cache_key:
+            raise Exception(f"Record List Action component does not have cache key set.")
+
+        locust_request_label = locust_request_label or f"RecordListUiform.ClickAction.{label}"
+        new_state = self._interactor.click_record_list_action(component=component, process_model_uuid=process_model_uuid,
+                                                              cache_key=cache_key, locust_request_label=locust_request_label)
+        self._reconcile_state(new_state)
+        return self
```

### Comparing `appian-locust-2.0.0a9/appian_locust/uiform/record_uiform.py` & `appian-locust-2.0.0b0/appian_locust/uiform/record_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/uiform/uiform.py` & `appian-locust-2.0.0b0/appian_locust/uiform/uiform.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 from .._grid_interactor import GridInteractor
 from .._interactor import _Interactor
 from .._locust_error_handler import raises_locust_error
 from .._task_opener import _TaskOpener
 from .._ui_reconciler import UiReconciler
 from ..exceptions import InvalidComponentException, ChoiceNotFoundException
 from ..utilities.helper import (extract_all_by_label, find_component_by_attribute_and_index_in_dict,
-                     find_component_by_attribute_in_dict, find_component_by_index_in_dict,
-                     find_component_by_label_and_type_dict, find_component_by_type_and_attribute_and_index_in_dict)
+                                find_component_by_attribute_in_dict, find_component_by_index_in_dict,
+                                find_component_by_label_and_type_dict, find_component_by_type_and_attribute_and_index_in_dict)
 from .._records_helper import get_url_stub_from_record_list_url_path, _is_grid
 
 if TYPE_CHECKING:
     from ..uiform import RecordInstanceUiForm
 
 KEY_UUID = "uuid"
 KEY_CONTEXT = "context"
 START_PROCESS_LINK_TYPE = 'StartProcessLink'
 PROCESS_TASK_LINK_TYPE = 'ProcessTaskLink'
 COMPONENTS_THAT_CAN_BE_FILLED = ["ParagraphField", "TextField", "SearchBoxWidget"]
+TEMPO_SITE_STUB = "D6JMim"
 
 log = logger.getLogger(__name__)
 
 
 class SailUiForm:
     def __init__(self, interactor: _Interactor, state: Dict[str, Any], breadcrumb: str = "SailUi"):
         """
@@ -409,15 +410,15 @@
 
         if not component.get("link"):
             raise Exception(f"CardLayout found at index: {index} does not have a link on it")
 
         link_component = component.get('link')
         locust_label = locust_request_label or f"{self.breadcrumb}.ClickCardLayout.Index.{index}"
         if link_component["#t"] == "StartProcessLink":
-            site_name = link_component["siteUrlStub"] or "D6JMim"
+            site_name = link_component["siteUrlStub"] or TEMPO_SITE_STUB
             page_name = link_component["sitePageUrlStub"]
             new_state = self._click_start_process_link(site_name, page_name, False, link_component, locust_request_label=locust_label)
         else:
             new_state = self._interactor.click_component(self.form_url, link_component, self.context, self.uuid, label=locust_label)
 
         if not new_state:
             raise Exception(f"No response returned when trying to click card layout at index '{index}'")
@@ -508,36 +509,36 @@
         reeval_url = self._get_update_url_for_reeval(self._state)
         new_state = self._interactor.click_record_link(reeval_url, component, self.context, self.uuid,
                                                        locust_label=locust_label)
         from .record_uiform import RecordInstanceUiForm
         return RecordInstanceUiForm(self._interactor, new_state)
 
     @raises_locust_error
-    def click_start_process_link(self, label: str, site_name: str, page_name: str, is_mobile: bool = False, locust_request_label: str = "") -> 'SailUiForm':
+    def click_start_process_link(self, label: str, is_mobile: bool = False, locust_request_label: str = "") -> 'SailUiForm':
         """
         Clicks a start process link on the form by label
         If no link is found, throws a ComponentNotFoundException
 
         Args:
             label(str): Label of the link
-            site_name(str): Name of the site (i.e. the Sites feature)
-            page_name(str): Name of the page within the site
 
         Keyword Args:
             is_mobile(bool): Boolean to use the mobile form of the request
             locust_request_label(str): Label used to identify the request for locust statistics
 
         Returns (SailUiForm): The latest state of the UiForm
 
         Examples:
             >>> form.click_start_process_link('Request upgrade')
 
         """
 
         component = find_component_by_label_and_type_dict('label', label, START_PROCESS_LINK_TYPE, self._state)
+        site_name = component["siteUrlStub"]
+        page_name = component["sitePageUrlStub"]
 
         locust_label = locust_request_label or f"{self.breadcrumb}.ClickStartProcessLink.{label}"
         new_state = self._click_start_process_link(site_name, page_name, is_mobile, component, locust_request_label=locust_label)
 
         return self._reconcile_state(new_state)
 
     @raises_locust_error
@@ -598,15 +599,15 @@
             link_component = component
             link_type = component_type
         else:
             link_component = component.get('link', {})
             link_type = link_component.get('#t')
 
         if link_type == START_PROCESS_LINK_TYPE:
-            site_name = link_component["siteUrlStub"] or "D6JMim"
+            site_name = link_component["siteUrlStub"] or TEMPO_SITE_STUB
             page_name = link_component["sitePageUrlStub"]
             new_state = self._click_start_process_link(site_name, page_name, False, link_component, locust_request_label=locust_label)
         elif link_type == PROCESS_TASK_LINK_TYPE:
             task_name = link_component.get('label') or 'Unnammed Task'
             task_id = link_component.get('opaqueTaskId')
             if not task_id:
                 raise Exception(f"No task id found for task with name '{task_name}'")
```

### Comparing `appian-locust-2.0.0a9/appian_locust/utilities/helper.py` & `appian-locust-2.0.0b0/appian_locust/utilities/helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/utilities/loadDriverUtils.py` & `appian-locust-2.0.0b0/appian_locust/utilities/loadDriverUtils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/utilities/logger.py` & `appian-locust-2.0.0b0/appian_locust/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/appian_locust/visitor.py` & `appian-locust-2.0.0b0/appian_locust/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,30 +157,27 @@
         """
         self.__records.get_records_nav(locust_request_label=locust_request_label)
         form_json = self.__records.visit_record_instance(record_type, record_name, view_url_stub=view_url_stub,
                                                          exact_match=exact_match, locust_request_label=locust_request_label)
         breadcrumb = f'Records.{record_type}.{format_label(record_name, "::", 0)}.SailUi'
         return RecordInstanceUiForm(self.__interactor, form_json, summary_view=summary_view, breadcrumb=breadcrumb)
 
-    def visit_record_type(self, record_type: str = "", exact_match: bool = False, is_mobile: bool = False,
+    def visit_record_type(self, record_type: str = "",
                           locust_request_label: Optional[str] = None) -> RecordListUiForm:
         """
         This function calls the API for the specific record type and returns a SAIL form representing the list of records for that record type.
 
         Args:
             record_type (str): Record Type Name. If not specified, a random record type will be selected.
-            exact_match (bool, optional): Should record type and record name matched exactly as it is or partial match.
-            is_mobile (bool, optional): If this is a mobile record
             locust_request_label (str, optional): Label locust should associate this request with
 
         Returns (SailUiForm): UI representing list of records for that record type
         """
         self.__records.get_records_nav(locust_request_label=locust_request_label)
-        form_json = self.__records.visit_record_type(record_type, exact_match=exact_match, is_mobile=is_mobile,
-                                                     locust_request_label=locust_request_label)
+        form_json = self.__records.visit_record_type(record_type, locust_request_label=locust_request_label)
         breadcrumb = f'Records.{record_type}.RecordListUi'
         return RecordListUiForm(self.__interactor, form_json, breadcrumb=breadcrumb)
 
     def visit_site(self, site_name: str, page_name: str) -> SailUiForm:
         """
         Get a SailUiForm for a Task, Report or Action
```

### Comparing `appian-locust-2.0.0a9/appian_locust.egg-info/PKG-INFO` & `appian-locust-2.0.0b0/appian_locust.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a9
+Version: 2.0.0b0
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a9/appian_locust.egg-info/SOURCES.txt` & `appian-locust-2.0.0b0/appian_locust.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 appian_locust/_records_helper.py
 appian_locust/_reports.py
 appian_locust/_save_request_builder.py
 appian_locust/_sites.py
 appian_locust/_task_opener.py
 appian_locust/_tasks.py
 appian_locust/_ui_reconciler.py
-appian_locust/appianclient.py
+appian_locust/appian_client.py
+appian_locust/appian_task_set.py
 appian_locust/feature_flag.py
 appian_locust/system_operator.py
 appian_locust/visitor.py
 appian_locust.egg-info/PKG-INFO
 appian_locust.egg-info/SOURCES.txt
 appian_locust.egg-info/dependency_links.txt
 appian_locust.egg-info/requires.txt
@@ -48,10 +49,11 @@
 appian_locust/uiform/application_uiform.py
 appian_locust/uiform/design_object_uiform.py
 appian_locust/uiform/design_uiform.py
 appian_locust/uiform/record_list_uiform.py
 appian_locust/uiform/record_uiform.py
 appian_locust/uiform/uiform.py
 appian_locust/utilities/__init__.py
+appian_locust/utilities/credentials.py
 appian_locust/utilities/helper.py
 appian_locust/utilities/loadDriverUtils.py
 appian_locust/utilities/logger.py
```

### Comparing `appian-locust-2.0.0a9/setup.cfg` & `appian-locust-2.0.0b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a9/setup.py` & `appian-locust-2.0.0b0/setup.py`

 * *Files identical despite different names*

