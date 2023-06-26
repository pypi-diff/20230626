# Comparing `tmp/sdc_dp_helpers-1.3.8.tar.gz` & `tmp/sdc_dp_helpers-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdc_dp_helpers-1.3.8.tar", last modified: Mon Jan 16 12:26:35 2023, max compression
+gzip compressed data, was "sdc_dp_helpers-1.3.9.tar", last modified: Fri Jan 20 06:27:53 2023, max compression
```

## Comparing `sdc_dp_helpers-1.3.8.tar` & `sdc_dp_helpers-1.3.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.793841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.793841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/__init_.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/data_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17377 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/date_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/file_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/retry_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/tracking_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.793841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/azure/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/azure/writers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/base_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/base_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.793841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/facebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/facebook/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/facebook/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.793841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/falcon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/falcon/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/falcon/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.793841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_ads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_ads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_ads/generate_refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_ads/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_ads/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.793841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/config_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.793841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics_v4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics_v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics_v4/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics_v4/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_big_query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_big_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_big_query/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_big_query/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_knowledge_graph/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_knowledge_graph/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/old_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/old_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/onesignal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/onesignal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/onesignal/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/onesignal/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/pyspark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/pyspark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/pyspark/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/sailthru/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/sailthru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/sailthru/config_magagers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/sailthru/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/sailthru/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/sailthru/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xero/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xero/auth_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xero/config_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xero/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xero/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xml/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/xml/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/sdc_dp_helpers/zoho/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/zoho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/zoho/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-01-16 12:26:33.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers/zoho/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:26:35.793841 sdc_dp_helpers-1.3.8/sdc_dp_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-01-16 12:26:35.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-01-16 12:26:35.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 12:26:35.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-16 12:26:35.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-16 12:26:35.000000 sdc_dp_helpers-1.3.8/sdc_dp_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-16 12:26:35.797841 sdc_dp_helpers-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-01-16 12:26:35.000000 sdc_dp_helpers-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.089048 sdc_dp_helpers-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-01-20 06:27:53.089048 sdc_dp_helpers-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.081047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/__init_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/data_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17377 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/date_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/file_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/retry_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/tracking_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/azure/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/azure/writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/base_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/base_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/facebook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/facebook/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/facebook/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/falcon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/falcon/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/falcon/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_ads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_ads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_ads/generate_refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_ads/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_ads/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/config_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics_v4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics_v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics_v4/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics_v4/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_big_query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_big_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_big_query/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_big_query/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_knowledge_graph/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_knowledge_graph/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/old_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/old_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.085047 sdc_dp_helpers-1.3.9/sdc_dp_helpers/onesignal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/onesignal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/onesignal/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/onesignal/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.089048 sdc_dp_helpers-1.3.9/sdc_dp_helpers/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/pyspark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/pyspark/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.089048 sdc_dp_helpers-1.3.9/sdc_dp_helpers/sailthru/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/sailthru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/sailthru/config_magagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/sailthru/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/sailthru/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/sailthru/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.089048 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xero/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xero/auth_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xero/config_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xero/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xero/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.089048 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xml/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/xml/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.089048 sdc_dp_helpers-1.3.9/sdc_dp_helpers/zoho/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/zoho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/zoho/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-01-20 06:27:50.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers/zoho/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 06:27:53.081047 sdc_dp_helpers-1.3.9/sdc_dp_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-01-20 06:27:52.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-01-20 06:27:53.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 06:27:52.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-20 06:27:52.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-20 06:27:52.000000 sdc_dp_helpers-1.3.9/sdc_dp_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-20 06:27:53.089048 sdc_dp_helpers-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-01-20 06:27:52.000000 sdc_dp_helpers-1.3.9/setup.py
```

### Comparing `sdc_dp_helpers-1.3.8/README.md` & `sdc_dp_helpers-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/data_managers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/data_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/date_managers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/date_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/exceptions.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/file_managers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/file_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/retry_managers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/retry_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/api_utilities/tracking_metadata.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/api_utilities/tracking_metadata.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/azure/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/azure/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/azure/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/azure/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/base_readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/base_readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/base_writer.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/base_writer.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/base_writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/base_writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/facebook/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/facebook/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/facebook/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/facebook/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/falcon/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/falcon/readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
             f"&statuses=published"
             f"&networks={network}"
             f"&{date_filters}"
         )
         content_ids_by_channel_id = {}
         while endpoint_url is not None:
             url = f"{self.base_url}{endpoint_url}"
-            response = self.request_session.get(url=url, params={"limit": "9999"})
+            response = self.request_session.get(url=url)
             response_data = response.json()
             if response.status_code != 200:
                 raise ConnectionError(
                     f"Falcon API failed to return content ids. "
                     f"Status code: {response.status_code}, Reason: {response.reason}."
                 )
             for item in response_data.get("items"):
@@ -410,33 +410,35 @@
         raise ConnectionError(
             f"Falcon API failed to return content ids. "
             f"Status code: {response.status_code}, Reason: {response.reason}."
         )
 
     @staticmethod
     def _normalize_data(dataset: dict, network: str, channel_ids: dict):
-        normalized_data = []
-        for metric, data_items in dataset.items():
-            for data_item in data_items:
-                data_item[f"{metric}"] = data_item.pop("value")
-                data_item["network"] = network
-                data_item["brand"] = channel_ids.get(data_item["channelId"], None)
-                normalized_data.append(data_item)
         temp = {}
-        for _, data in enumerate(normalized_data):
-            check_point = tuple(map(data.get,["channelId", "date", "contentId"]))
-            if not temp.get(check_point):
-                temp[check_point] = data
-            else:
-                missing_keys = set(data).difference(set(temp[check_point]))
-                #flatten
-                for key in missing_keys:
-                    temp[check_point].update({key: data[key]})
-        result = list(temp.values())
-        return result
+
+        for  metric, data_items in dataset.items():
+            if not data_items:
+                #if we have nothing in value
+                continue
+            for data in data_items:
+                data[metric]=data.pop("value")
+                data["network"] = network
+                data["brand"] = channel_ids.get(data["channelId"], None)
+                check_point = tuple(map(data.get,["channelId", "date", "contentId"]))
+                if not temp.get(check_point):
+                    temp[check_point]= data
+                else :
+                    missing_keys = set(data).difference(set(temp[check_point]))
+                    #flatten
+                    for key in missing_keys:
+                        temp[check_point].update({key: data[key]})
+
+        normalized_data = list(temp.values())
+        return normalized_data
 
     def _query_handler(
                         self, start_date: str, end_date: str, network: str, channel_ids: dict
     ) -> dict:
         endpoint_name = self._config.get("endpoint_name", None)
         if not endpoint_name:
             raise KeyError(
@@ -447,15 +449,15 @@
             end_date=end_date,
             network=network,
             channel_ids=channel_ids,
         )
         channels = list(content_ids_by_channel_id.keys())
         channel_id_length = len(channels)
         channel_steps = self._config.get("channel_steps", 10)
-        dataset = {}
+        dataset = []
         data = []
         for _ in range(0, channel_id_length, channel_steps):
             self.curr_channels = channels[self.start : self.start + channel_steps]
             request_content_ids_by_channel_id = {
                 key: value
                 for key, value in content_ids_by_channel_id.items()
                 if key in self.curr_channels
@@ -472,17 +474,17 @@
                     insights_request_id = self._get_insights_request_id(
                         start_date=start_date,
                         end_date=end_date,
                         content_ids_by_channel_id=request_content_ids_by_channel_id,
                     )
                     results = self._get_content_insights(insights_request_id)
                 data = results["data"]["insights"]
-            dataset.update(data)
+                dataset.extend(self._normalize_data(data, network, channel_ids))
             self.start = self.start + channel_steps
-        return self._normalize_data(dataset, network, channel_ids)
+        return dataset
 
     def run_query(self):
         """Handles the query results"""
         channel_ids = self._get_channel_ids()
         print(f"Attempting to gather metrics from {len(channel_ids)} channel ids.")
         network = self._config.get("networks")
         date_iterator = date_range_iterator(
```

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/falcon/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/falcon/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_ads/generate_refresh_token.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_ads/generate_refresh_token.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_ads/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_ads/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_ads/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_ads/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/config_managers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/config_managers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/utils.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics_v4/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics_v4/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_analytics_v4/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_analytics_v4/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_big_query/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_big_query/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_big_query/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_big_query/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_knowledge_graph/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_knowledge_graph/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_knowledge_graph/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_knowledge_graph/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/old_readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/old_readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/old_writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/old_writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/google_search_console/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/google_search_console/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/onesignal/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/onesignal/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/onesignal/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/onesignal/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/pyspark/utils.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/pyspark/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/pyspark/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/pyspark/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/sailthru/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/sailthru/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/sailthru/utils.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/sailthru/utils.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/sailthru/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/sailthru/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/xero/auth_handler.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/xero/auth_handler.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/xero/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/xero/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/xero/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/xero/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/xml/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/xml/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/xml/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/xml/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/zoho/readers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/zoho/readers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers/zoho/writers.py` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers/zoho/writers.py`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/sdc_dp_helpers.egg-info/SOURCES.txt` & `sdc_dp_helpers-1.3.9/sdc_dp_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdc_dp_helpers-1.3.8/setup.py` & `sdc_dp_helpers-1.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,18 +61,18 @@
         "google",
         "google-analytics-data",
         "xmltodict",
     ],
     extras_require={"pyspark": ["pyspark"]},
     cmdclass={"sdist_zip": sdistzip},
     description="A module for developing data pipelines from external api's and on ETL like services",
-    version="1.3.8",
+    version="1.3.9",
     url="http://github.com/RingierIMU/sdc-dataPipeline-helpers",
     author="Ringier South Africa",
     author_email="tools@ringier.co.za",
     keywords=[
         "pip",
         "datapipeline",
         "helpers",
     ],
-    download_url="https://github.com/RingierIMU/sdc-global-dataPipeline-helpers/archive/v1.3.8.zip",
+    download_url="https://github.com/RingierIMU/sdc-global-dataPipeline-helpers/archive/v1.3.9.zip",
 )
```

