# Comparing `tmp/mimeograph-0.7.0.tar.gz` & `tmp/mimeograph-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.7.0.tar", last modified: Thu Jun 15 08:33:35 2023, max compression
+gzip compressed data, was "mimeograph-1.0.3.tar", last modified: Mon Jun 26 15:57:24 2023, max compression
```

## Comparing `mimeograph-0.7.0.tar` & `mimeograph-1.0.3.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.7.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-05-11 05:33:09.000000 mimeograph-0.7.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    27826 2023-06-15 08:33:35.192970 mimeograph-0.7.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    25470 2023-06-12 07:59:15.000000 mimeograph-0.7.0/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     3894 2023-06-15 08:31:52.000000 mimeograph-0.7.0/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-06-15 08:33:35.192970 mimeograph-0.7.0/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.184970 mimeograph-0.7.0/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.184970 mimeograph-0.7.0/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1440 2023-06-15 08:31:52.000000 mimeograph-0.7.0/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-05-11 13:41:23.000000 mimeograph-0.7.0/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.184970 mimeograph-0.7.0/src/mimeo/cli/
--rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/cli/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2290 2023-05-17 08:57:29.000000 mimeograph-0.7.0/src/mimeo/cli/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4117 2023-05-27 06:14:50.000000 mimeograph-0.7.0/src/mimeo/cli/job.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    16834 2023-06-15 08:31:52.000000 mimeograph-0.7.0/src/mimeo/cli/parsers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.184970 mimeograph-0.7.0/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)      837 2023-05-27 06:14:50.000000 mimeograph-0.7.0/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5938 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/config/constants.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12311 2023-05-27 06:14:50.000000 mimeograph-0.7.0/src/mimeo/config/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    34682 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1402 2023-05-12 09:42:23.000000 mimeograph-0.7.0/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2131 2023-05-17 08:14:52.000000 mimeograph-0.7.0/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2364 2023-05-12 09:42:23.000000 mimeograph-0.7.0/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3032 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1018 2023-05-12 09:42:23.000000 mimeograph-0.7.0/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/context/decorators.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18138 2023-05-22 07:52:53.000000 mimeograph-0.7.0/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5111 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2888 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-05-16 10:04:29.000000 mimeograph-0.7.0/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5507 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5775 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5613 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/currencies.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6200 2023-05-22 07:52:53.000000 mimeograph-0.7.0/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5471 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/first_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2180 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/last_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10209 2023-05-16 10:04:29.000000 mimeograph-0.7.0/src/mimeo/database/mimeo_db.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1117 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2685 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1654 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    21089 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4033 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      656 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2023-05-12 09:42:23.000000 mimeograph-0.7.0/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)      362 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     1538 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/resources/constants.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     7268 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/currencies.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      783 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/resources/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/forenames.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/surnames.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     1035 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)     2193 2023-05-16 10:04:29.000000 mimeograph-0.7.0/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6224 2023-06-12 07:59:15.000000 mimeograph-0.7.0/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    29122 2023-05-22 07:52:53.000000 mimeograph-0.7.0/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20108 2023-06-12 07:59:15.000000 mimeograph-0.7.0/src/mimeo/utils/renderers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    27826 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1987 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      222 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1848 2023-06-15 08:27:49.000000 mimeograph-0.7.0/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      502 2023-05-22 07:52:53.000000 mimeograph-0.7.0/tests/test_tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.044392 mimeograph-1.0.3/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-1.0.3/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-05-11 05:33:09.000000 mimeograph-1.0.3/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    34465 2023-06-26 15:57:24.044392 mimeograph-1.0.3/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    32079 2023-06-26 13:54:19.000000 mimeograph-1.0.3/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4010 2023-06-26 15:56:55.000000 mimeograph-1.0.3/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-06-26 15:57:24.044392 mimeograph-1.0.3/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1484 2023-06-26 15:56:55.000000 mimeograph-1.0.3/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-06-24 11:03:12.000000 mimeograph-1.0.3/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/cli/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/cli/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2290 2023-05-17 08:57:29.000000 mimeograph-1.0.3/src/mimeo/cli/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4694 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/cli/job.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18152 2023-06-26 15:56:55.000000 mimeograph-1.0.3/src/mimeo/cli/parsers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      837 2023-05-27 06:14:50.000000 mimeograph-1.0.3/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6275 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/config/constants.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12351 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/config/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    35693 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1402 2023-06-24 11:02:10.000000 mimeograph-1.0.3/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2146 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2374 2023-06-24 11:02:23.000000 mimeograph-1.0.3/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3109 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1018 2023-05-12 09:42:23.000000 mimeograph-1.0.3/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/context/decorators.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18276 2023-06-23 11:30:49.000000 mimeograph-1.0.3/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5164 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2911 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-05-16 10:04:29.000000 mimeograph-1.0.3/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5638 2023-06-26 14:29:14.000000 mimeograph-1.0.3/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5885 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5755 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/currencies.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6200 2023-05-22 07:52:53.000000 mimeograph-1.0.3/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5599 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/first_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2235 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/last_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10234 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/mimeo_db.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      702 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/exc.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2023-06-20 06:50:14.000000 mimeograph-1.0.3/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1149 2023-06-20 06:50:14.000000 mimeograph-1.0.3/src/mimeo/generators/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10680 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1852 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    17137 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/generators/json_generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    14857 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-16 15:27:55.000000 mimeograph-1.0.3/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4083 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      656 2023-05-17 13:09:43.000000 mimeograph-1.0.3/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10889 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      362 2023-05-17 13:09:43.000000 mimeograph-1.0.3/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-06-26 14:29:14.000000 mimeograph-1.0.3/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1579 2023-06-20 06:50:14.000000 mimeograph-1.0.3/src/mimeo/resources/constants.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-06-26 14:08:58.000000 mimeograph-1.0.3/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7268 2023-06-26 14:29:14.000000 mimeograph-1.0.3/src/mimeo/resources/currencies.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      783 2023-05-17 13:09:43.000000 mimeograph-1.0.3/src/mimeo/resources/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-06-26 14:05:34.000000 mimeograph-1.0.3/src/mimeo/resources/forenames.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      736 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-06-26 14:05:38.000000 mimeograph-1.0.3/src/mimeo/resources/surnames.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1035 2023-05-17 13:09:43.000000 mimeograph-1.0.3/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.044392 mimeograph-1.0.3/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2193 2023-05-16 10:04:29.000000 mimeograph-1.0.3/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6254 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    29523 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20193 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/utils/renderers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.044392 mimeograph-1.0.3/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    34465 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2043 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      222 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.044392 mimeograph-1.0.3/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16690 2023-06-26 13:54:19.000000 mimeograph-1.0.3/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      502 2023-05-22 07:52:53.000000 mimeograph-1.0.3/tests/test_tools.py
```

### Comparing `mimeograph-0.7.0/LICENSE` & `mimeograph-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/PKG-INFO` & `mimeograph-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,1740 +1,2005 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6d69 6d65  : 2.1.Name: mime
-00000020: 6f67 7261 7068 0a56 6572 7369 6f6e 3a20  ograph.Version: 
-00000030: 302e 372e 300a 5375 6d6d 6172 793a 2047  0.7.0.Summary: G
-00000040: 656e 6572 6174 6520 6461 7461 2062 6173  enerate data bas
-00000050: 6564 206f 6e20 6120 7369 6d70 6c65 2074  ed on a simple t
-00000060: 656d 706c 6174 650a 4175 7468 6f72 2d65  emplate.Author-e
-00000070: 6d61 696c 3a20 2254 2e41 2e20 5072 6f67  mail: "T.A. Prog
-00000080: 7261 6d6d 696e 6720 5376 6373 2e22 203c  ramming Svcs." <
-00000090: 746f 6d61 737a 2e6d 6163 6965 6a2e 616e  tomasz.maciej.an
-000000a0: 696f 6c6f 7773 6b69 4067 6d61 696c 2e63  iolowski@gmail.c
-000000b0: 6f6d 3e0a 4c69 6365 6e73 653a 204d 4954  om>.License: MIT
-000000c0: 204c 6963 656e 7365 0a20 2020 2020 2020   License.       
-000000d0: 200a 2020 2020 2020 2020 436f 7079 7269   .        Copyri
-000000e0: 6768 7420 2863 2920 3230 3233 2054 6f6d  ght (c) 2023 Tom
-000000f0: 6173 7a20 416e 696f c582 6f77 736b 690a  asz Anio..owski.
-00000100: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000110: 2050 6572 6d69 7373 696f 6e20 6973 2068   Permission is h
-00000120: 6572 6562 7920 6772 616e 7465 642c 2066  ereby granted, f
-00000130: 7265 6520 6f66 2063 6861 7267 652c 2074  ree of charge, t
-00000140: 6f20 616e 7920 7065 7273 6f6e 206f 6274  o any person obt
-00000150: 6169 6e69 6e67 2061 2063 6f70 790a 2020  aining a copy.  
-00000160: 2020 2020 2020 6f66 2074 6869 7320 736f        of this so
-00000170: 6674 7761 7265 2061 6e64 2061 7373 6f63  ftware and assoc
-00000180: 6961 7465 6420 646f 6375 6d65 6e74 6174  iated documentat
-00000190: 696f 6e20 6669 6c65 7320 2874 6865 2022  ion files (the "
-000001a0: 536f 6674 7761 7265 2229 2c20 746f 2064  Software"), to d
-000001b0: 6561 6c0a 2020 2020 2020 2020 696e 2074  eal.        in t
-000001c0: 6865 2053 6f66 7477 6172 6520 7769 7468  he Software with
-000001d0: 6f75 7420 7265 7374 7269 6374 696f 6e2c  out restriction,
-000001e0: 2069 6e63 6c75 6469 6e67 2077 6974 686f   including witho
-000001f0: 7574 206c 696d 6974 6174 696f 6e20 7468  ut limitation th
-00000200: 6520 7269 6768 7473 0a20 2020 2020 2020  e rights.       
-00000210: 2074 6f20 7573 652c 2063 6f70 792c 206d   to use, copy, m
-00000220: 6f64 6966 792c 206d 6572 6765 2c20 7075  odify, merge, pu
-00000230: 626c 6973 682c 2064 6973 7472 6962 7574  blish, distribut
-00000240: 652c 2073 7562 6c69 6365 6e73 652c 2061  e, sublicense, a
-00000250: 6e64 2f6f 7220 7365 6c6c 0a20 2020 2020  nd/or sell.     
-00000260: 2020 2063 6f70 6965 7320 6f66 2074 6865     copies of the
-00000270: 2053 6f66 7477 6172 652c 2061 6e64 2074   Software, and t
-00000280: 6f20 7065 726d 6974 2070 6572 736f 6e73  o permit persons
-00000290: 2074 6f20 7768 6f6d 2074 6865 2053 6f66   to whom the Sof
-000002a0: 7477 6172 6520 6973 0a20 2020 2020 2020  tware is.       
-000002b0: 2066 7572 6e69 7368 6564 2074 6f20 646f   furnished to do
-000002c0: 2073 6f2c 2073 7562 6a65 6374 2074 6f20   so, subject to 
-000002d0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-000002e0: 6e64 6974 696f 6e73 3a0a 2020 2020 2020  nditions:.      
-000002f0: 2020 0a20 2020 2020 2020 2054 6865 2061    .        The a
-00000300: 626f 7665 2063 6f70 7972 6967 6874 206e  bove copyright n
-00000310: 6f74 6963 6520 616e 6420 7468 6973 2070  otice and this p
-00000320: 6572 6d69 7373 696f 6e20 6e6f 7469 6365  ermission notice
-00000330: 2073 6861 6c6c 2062 6520 696e 636c 7564   shall be includ
-00000340: 6564 2069 6e20 616c 6c0a 2020 2020 2020  ed in all.      
-00000350: 2020 636f 7069 6573 206f 7220 7375 6273    copies or subs
-00000360: 7461 6e74 6961 6c20 706f 7274 696f 6e73  tantial portions
-00000370: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
-00000380: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00000390: 2020 2054 4845 2053 4f46 5457 4152 4520     THE SOFTWARE 
-000003a0: 4953 2050 524f 5649 4445 4420 2241 5320  IS PROVIDED "AS 
-000003b0: 4953 222c 2057 4954 484f 5554 2057 4152  IS", WITHOUT WAR
-000003c0: 5241 4e54 5920 4f46 2041 4e59 204b 494e  RANTY OF ANY KIN
-000003d0: 442c 2045 5850 5245 5353 204f 520a 2020  D, EXPRESS OR.  
-000003e0: 2020 2020 2020 494d 504c 4945 442c 2049        IMPLIED, I
-000003f0: 4e43 4c55 4449 4e47 2042 5554 204e 4f54  NCLUDING BUT NOT
-00000400: 204c 494d 4954 4544 2054 4f20 5448 4520   LIMITED TO THE 
-00000410: 5741 5252 414e 5449 4553 204f 4620 4d45  WARRANTIES OF ME
-00000420: 5243 4841 4e54 4142 494c 4954 592c 0a20  RCHANTABILITY,. 
-00000430: 2020 2020 2020 2046 4954 4e45 5353 2046         FITNESS F
-00000440: 4f52 2041 2050 4152 5449 4355 4c41 5220  OR A PARTICULAR 
-00000450: 5055 5250 4f53 4520 414e 4420 4e4f 4e49  PURPOSE AND NONI
-00000460: 4e46 5249 4e47 454d 454e 542e 2049 4e20  NFRINGEMENT. IN 
-00000470: 4e4f 2045 5645 4e54 2053 4841 4c4c 2054  NO EVENT SHALL T
-00000480: 4845 0a20 2020 2020 2020 2041 5554 484f  HE.        AUTHO
-00000490: 5253 204f 5220 434f 5059 5249 4748 5420  RS OR COPYRIGHT 
-000004a0: 484f 4c44 4552 5320 4245 204c 4941 424c  HOLDERS BE LIABL
-000004b0: 4520 464f 5220 414e 5920 434c 4149 4d2c  E FOR ANY CLAIM,
-000004c0: 2044 414d 4147 4553 204f 5220 4f54 4845   DAMAGES OR OTHE
-000004d0: 520a 2020 2020 2020 2020 4c49 4142 494c  R.        LIABIL
-000004e0: 4954 592c 2057 4845 5448 4552 2049 4e20  ITY, WHETHER IN 
-000004f0: 414e 2041 4354 494f 4e20 4f46 2043 4f4e  AN ACTION OF CON
-00000500: 5452 4143 542c 2054 4f52 5420 4f52 204f  TRACT, TORT OR O
-00000510: 5448 4552 5749 5345 2c20 4152 4953 494e  THERWISE, ARISIN
-00000520: 4720 4652 4f4d 2c0a 2020 2020 2020 2020  G FROM,.        
-00000530: 4f55 5420 4f46 204f 5220 494e 2043 4f4e  OUT OF OR IN CON
-00000540: 4e45 4354 494f 4e20 5749 5448 2054 4845  NECTION WITH THE
-00000550: 2053 4f46 5457 4152 4520 4f52 2054 4845   SOFTWARE OR THE
-00000560: 2055 5345 204f 5220 4f54 4845 5220 4445   USE OR OTHER DE
-00000570: 414c 494e 4753 2049 4e20 5448 450a 2020  ALINGS IN THE.  
-00000580: 2020 2020 2020 534f 4654 5741 5245 2e0a        SOFTWARE..
-00000590: 2020 2020 2020 2020 0a50 726f 6a65 6374          .Project
-000005a0: 2d55 524c 3a20 4769 7448 7562 2c20 6874  -URL: GitHub, ht
-000005b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000005c0: 2f54 6f6d 6173 7a41 6e69 6f6c 6f77 736b  /TomaszAniolowsk
-000005d0: 692f 6d69 6d65 6f0a 4b65 7977 6f72 6473  i/mimeo.Keywords
-000005e0: 3a20 6d69 6d65 6f67 7261 7068 2c6d 696d  : mimeograph,mim
-000005f0: 656f 2c67 656e 6572 6174 652c 6765 6e65  eo,generate,gene
-00000600: 7261 746f 722c 6461 7461 2c78 6d6c 0a43  rator,data,xml.C
-00000610: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
-00000620: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000630: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-00000640: 650a 436c 6173 7369 6669 6572 3a20 4465  e.Classifier: De
-00000650: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000660: 203a 3a20 3420 2d20 4265 7461 0a43 6c61   :: 4 - Beta.Cla
-00000670: 7373 6966 6965 723a 2045 6e76 6972 6f6e  ssifier: Environ
-00000680: 6d65 6e74 203a 3a20 436f 6e73 6f6c 650a  ment :: Console.
-00000690: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
-000006a0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-000006b0: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
-000006c0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000006d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000006e0: 5079 7468 6f6e 0a43 6c61 7373 6966 6965  Python.Classifie
-000006f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000700: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000710: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
-00000720: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000730: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000740: 6e20 3a3a 2033 203a 3a20 4f6e 6c79 0a43  n :: 3 :: Only.C
-00000750: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000760: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000770: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000780: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000790: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000007a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000007b0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-000007c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000007d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000007e0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
-000007f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000800: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000810: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
-00000820: 6965 723a 2054 6f70 6963 203a 3a20 4461  ier: Topic :: Da
-00000830: 7461 6261 7365 0a43 6c61 7373 6966 6965  tabase.Classifie
-00000840: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
-00000850: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
-00000860: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-00000870: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
-00000880: 6576 656c 6f70 6d65 6e74 203a 3a20 5465  evelopment :: Te
-00000890: 7374 696e 670a 436c 6173 7369 6669 6572  sting.Classifier
-000008a0: 3a20 546f 7069 6320 3a3a 2055 7469 6c69  : Topic :: Utili
-000008b0: 7469 6573 0a52 6571 7569 7265 732d 5079  ties.Requires-Py
-000008c0: 7468 6f6e 3a20 3e3d 332e 380a 4465 7363  thon: >=3.8.Desc
-000008d0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-000008e0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-000008f0: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
-00000900: 7261 3a20 6465 760a 5072 6f76 6964 6573  ra: dev.Provides
-00000910: 2d45 7874 7261 3a20 7465 7374 0a4c 6963  -Extra: test.Lic
-00000920: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-00000930: 5345 0a0a 2320 4d69 6d65 6f20 284d 696d  SE..# Mimeo (Mim
-00000940: 656f 6772 6170 6829 0a0a 5b21 5b4c 6963  eograph)..[![Lic
-00000950: 656e 7365 5d28 6874 7470 733a 2f2f 696d  ense](https://im
-00000960: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00000970: 6875 622f 6c69 6365 6e73 652f 546f 6d61  hub/license/Toma
-00000980: 737a 416e 696f 6c6f 7773 6b69 2f6d 696d  szAniolowski/mim
-00000990: 656f 3f6c 6162 656c 3d4c 6963 656e 7365  eo?label=License
-000009a0: 2673 7479 6c65 3d70 6c61 7374 6963 295d  &style=plastic)]
-000009b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000009c0: 636f 6d2f 546f 6d61 737a 416e 696f 6c6f  com/TomaszAniolo
-000009d0: 7773 6b69 2f6d 696d 656f 2f62 6c6f 622f  wski/mimeo/blob/
-000009e0: 6465 7665 6c6f 702f 4c49 4345 4e53 4529  develop/LICENSE)
-000009f0: 0a5b 215b 5665 7273 696f 6e5d 2868 7474  .[![Version](htt
-00000a00: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000a10: 2e69 6f2f 7079 7069 2f76 2f6d 696d 656f  .io/pypi/v/mimeo
-00000a20: 6772 6170 683f 636f 6c6f 723d 626c 7565  graph?color=blue
-00000a30: 266c 6162 656c 3d50 7950 4926 7374 796c  &label=PyPI&styl
-00000a40: 653d 706c 6173 7469 6329 5d28 6874 7470  e=plastic)](http
-00000a50: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000a60: 6a65 6374 2f6d 696d 656f 6772 6170 682f  ject/mimeograph/
-00000a70: 290a 5b21 5b50 7974 686f 6e5d 2868 7474  ).[![Python](htt
-00000a80: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000a90: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-00000aa0: 6f6e 732f 6d69 6d65 6f67 7261 7068 3f6c  ons/mimeograph?l
-00000ab0: 6162 656c 3d50 7974 686f 6e26 7374 796c  abel=Python&styl
-00000ac0: 653d 706c 6173 7469 6329 5d28 6874 7470  e=plastic)](http
-00000ad0: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
-00000ae0: 7267 2f29 2020 0a5b 215b 4275 696c 645d  rg/)  .[![Build]
-00000af0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000b00: 656c 6473 2e69 6f2f 6769 7468 7562 2f61  elds.io/github/a
-00000b10: 6374 696f 6e73 2f77 6f72 6b66 6c6f 772f  ctions/workflow/
-00000b20: 7374 6174 7573 2f54 6f6d 6173 7a41 6e69  status/TomaszAni
-00000b30: 6f6c 6f77 736b 692f 6d69 6d65 6f2f 7465  olowski/mimeo/te
-00000b40: 7374 2e79 6d6c 3f63 6f6c 6f72 3d62 7269  st.yml?color=bri
-00000b50: 6768 7467 7265 656e 266c 6162 656c 3d54  ghtgreen&label=T
-00000b60: 6573 7425 3230 4d69 6d65 6f26 7374 796c  est%20Mimeo&styl
-00000b70: 653d 706c 6173 7469 6329 5d28 6874 7470  e=plastic)](http
-00000b80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00000b90: 6f6d 6173 7a41 6e69 6f6c 6f77 736b 692f  omaszAniolowski/
-00000ba0: 6d69 6d65 6f2f 6163 7469 6f6e 732f 776f  mimeo/actions/wo
-00000bb0: 726b 666c 6f77 732f 7465 7374 2e79 6d6c  rkflows/test.yml
-00000bc0: 3f71 7565 7279 3d62 7261 6e63 6825 3341  ?query=branch%3A
-00000bd0: 6d61 696e 290a 5b21 5b43 6f64 6520 436f  main).[![Code Co
-00000be0: 7665 7261 6765 5d28 6874 7470 733a 2f2f  verage](https://
-00000bf0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000c00: 6164 6765 2f43 6f64 6525 3230 436f 7665  adge/Code%20Cove
-00000c10: 7261 6765 2d31 3030 2532 352d 6272 6967  rage-100%25-brig
-00000c20: 6874 6772 6565 6e3f 7374 796c 653d 706c  htgreen?style=pl
-00000c30: 6173 7469 6329 5d28 6874 7470 733a 2f2f  astic)](https://
-00000c40: 6769 7468 7562 2e63 6f6d 2f54 6f6d 6173  github.com/Tomas
-00000c50: 7a41 6e69 6f6c 6f77 736b 692f 6d69 6d65  zAniolowski/mime
-00000c60: 6f2f 6163 7469 6f6e 732f 776f 726b 666c  o/actions/workfl
-00000c70: 6f77 732f 636f 7665 7261 6765 5f62 6164  ows/coverage_bad
-00000c80: 6765 2e79 6d6c 3f71 7565 7279 3d62 7261  ge.yml?query=bra
-00000c90: 6e63 6825 3341 6d61 696e 290a 0a5b 4d69  nch%3Amain)..[Mi
-00000ca0: 6d65 6f5d 2868 7474 7073 3a2f 2f67 6974  meo](https://git
-00000cb0: 6875 622e 636f 6d2f 546f 6d61 737a 416e  hub.com/TomaszAn
-00000cc0: 696f 6c6f 7773 6b69 2f6d 696d 656f 2920  iolowski/mimeo) 
-00000cd0: 6973 2061 2063 6f6d 6d61 6e64 206c 696e  is a command lin
-00000ce0: 6520 746f 6f6c 2061 6e64 2070 7974 686f  e tool and pytho
-00000cf0: 6e20 6c69 6272 6172 7920 6765 6e65 7261  n library genera
-00000d00: 7469 6e67 2063 7573 746f 6d20 6461 7461  ting custom data
-00000d10: 2062 6173 6564 206f 6e20 6120 7465 6d70   based on a temp
-00000d20: 6c61 7465 2e0a 4974 2063 616e 2062 6520  late..It can be 
-00000d30: 7573 6564 2062 7920 6465 7665 6c6f 7065  used by develope
-00000d40: 7273 2c20 7465 7374 6572 7320 6f72 2065  rs, testers or e
-00000d50: 7665 6e20 6275 7369 6e65 7373 2061 6e61  ven business ana
-00000d60: 6c79 7374 7320 696e 2074 6865 6972 2064  lysts in their d
-00000d70: 6169 6c79 2077 6f72 6b2e 0a0a 0a23 2320  aily work....## 
-00000d80: 496e 7374 616c 6c61 7469 6f6e 0a0a 496e  Installation..In
-00000d90: 7374 616c 6c20 4d69 6d65 6f20 7769 7468  stall Mimeo with
-00000da0: 2070 6970 0a0a 6060 6073 680a 7069 7020   pip..```sh.pip 
-00000db0: 696e 7374 616c 6c20 6d69 6d65 6f67 7261  install mimeogra
-00000dc0: 7068 0a60 6060 0a0a 0a23 2320 5573 6167  ph.```...## Usag
-00000dd0: 652f 4578 616d 706c 6573 0a0a 2323 2320  e/Examples..### 
-00000de0: 4d69 6d65 6f20 436f 6e66 6967 7572 6174  Mimeo Configurat
-00000df0: 696f 6e0a 0a50 7265 7061 7265 204d 696d  ion..Prepare Mim
-00000e00: 656f 2043 6f6e 6669 6775 7261 7469 6f6e  eo Configuration
-00000e10: 2066 6972 7374 0a2d 2066 6f72 2061 2063   first.- for a c
-00000e20: 6f6d 6d61 6e64 206c 696e 6520 746f 6f6c  ommand line tool
-00000e30: 3a20 696e 2061 204a 534f 4e20 6f72 2058  : in a JSON or X
-00000e40: 4d4c 2066 696c 650a 2d20 666f 7220 6120  ML file.- for a 
-00000e50: 604d 696d 656f 6772 6170 6860 2070 7974  `Mimeograph` pyt
-00000e60: 686f 6e20 636c 6173 733a 2069 6e20 6120  hon class: in a 
-00000e70: 6064 6963 7460 206f 7220 7374 7269 6e67  `dict` or string
-00000e80: 6966 6965 6420 584d 4c0a 0a60 6060 6a73  ified XML..```js
-00000e90: 6f6e 0a7b 0a20 2022 5f74 656d 706c 6174  on.{.  "_templat
-00000ea0: 6573 5f22 3a20 5b0a 2020 2020 7b0a 2020  es_": [.    {.  
-00000eb0: 2020 2020 2263 6f75 6e74 223a 2033 302c      "count": 30,
-00000ec0: 0a20 2020 2020 2022 6d6f 6465 6c22 3a20  .      "model": 
-00000ed0: 7b0a 2020 2020 2020 2020 2253 6f6d 6545  {.        "SomeE
-00000ee0: 6e74 6974 7922 3a20 7b0a 2020 2020 2020  ntity": {.      
-00000ef0: 2020 2020 2240 786d 6c6e 7322 3a20 2268      "@xmlns": "h
-00000f00: 7474 703a 2f2f 6d69 6d65 6f2e 6172 6368  ttp://mimeo.arch
-00000f10: 2e63 6f6d 2f64 6566 6175 6c74 2d6e 616d  .com/default-nam
-00000f20: 6573 7061 6365 222c 0a20 2020 2020 2020  espace",.       
-00000f30: 2020 2022 4078 6d6c 6e73 3a70 6e22 3a20     "@xmlns:pn": 
-00000f40: 2268 7474 703a 2f2f 6d69 6d65 6f2e 6172  "http://mimeo.ar
-00000f50: 6368 2e63 6f6d 2f70 7265 6669 7865 642d  ch.com/prefixed-
-00000f60: 6e61 6d65 7370 6163 6522 2c0a 2020 2020  namespace",.    
-00000f70: 2020 2020 2020 2243 6869 6c64 4e6f 6465        "ChildNode
-00000f80: 3122 3a20 312c 0a20 2020 2020 2020 2020  1": 1,.         
-00000f90: 2022 4368 696c 644e 6f64 6532 223a 2022   "ChildNode2": "
-00000fa0: 7661 6c75 652d 3222 2c0a 2020 2020 2020  value-2",.      
-00000fb0: 2020 2020 2243 6869 6c64 4e6f 6465 3322      "ChildNode3"
-00000fc0: 3a20 7472 7565 0a20 2020 2020 2020 207d  : true.        }
-00000fd0: 0a20 2020 2020 207d 0a20 2020 207d 0a20  .      }.    }. 
-00000fe0: 205d 0a7d 0a60 6060 0a60 6060 786d 6c0a   ].}.```.```xml.
-00000ff0: 3c6d 696d 656f 5f63 6f6e 6669 6775 7261  <mimeo_configura
-00001000: 7469 6f6e 3e0a 2020 2020 3c5f 7465 6d70  tion>.    <_temp
-00001010: 6c61 7465 735f 3e0a 2020 2020 2020 2020  lates_>.        
-00001020: 3c5f 7465 6d70 6c61 7465 5f3e 0a20 2020  <_template_>.   
-00001030: 2020 2020 2020 2020 203c 636f 756e 743e           <count>
-00001040: 3330 3c2f 636f 756e 743e 0a20 2020 2020  30</count>.     
-00001050: 2020 2020 2020 203c 6d6f 6465 6c3e 0a0a         <model>..
-00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 3c53 6f6d 6545 6e74 6974 790a 2020 2020  <SomeEntity.    
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 786d 6c6e 733d 2268 7474 703a 2f2f 6d69  xmlns="http://mi
-000010a0: 6d65 6f2e 6172 6368 2e63 6f6d 2f64 6566  meo.arch.com/def
-000010b0: 6175 6c74 2d6e 616d 6573 7061 6365 220a  ault-namespace".
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 2020 2020 786d 6c6e 733a 706e 3d22 6874      xmlns:pn="ht
-000010e0: 7470 3a2f 2f6d 696d 656f 2e61 7263 682e  tp://mimeo.arch.
-000010f0: 636f 6d2f 7072 6566 6978 6564 2d6e 616d  com/prefixed-nam
-00001100: 6573 7061 6365 223e 0a20 2020 2020 2020  espace">.       
-00001110: 2020 2020 2020 2020 2020 2020 203c 4368               <Ch
-00001120: 696c 644e 6f64 6531 3e31 3c2f 4368 696c  ildNode1>1</Chil
-00001130: 644e 6f64 6531 3e0a 2020 2020 2020 2020  dNode1>.        
-00001140: 2020 2020 2020 2020 2020 2020 3c70 6e3a              <pn:
-00001150: 4368 696c 644e 6f64 6532 3e76 616c 7565  ChildNode2>value
-00001160: 2d32 3c2f 706e 3a43 6869 6c64 4e6f 6465  -2</pn:ChildNode
-00001170: 323e 0a20 2020 2020 2020 2020 2020 2020  2>.             
-00001180: 2020 2020 2020 203c 4368 696c 644e 6f64         <ChildNod
-00001190: 6533 3e74 7275 653c 2f43 6869 6c64 4e6f  e3>true</ChildNo
-000011a0: 6465 333e 0a20 2020 2020 2020 2020 2020  de3>.           
-000011b0: 2020 2020 203c 2f53 6f6d 6545 6e74 6974       </SomeEntit
-000011c0: 793e 0a0a 2020 2020 2020 2020 2020 2020  y>..            
-000011d0: 3c2f 6d6f 6465 6c3e 0a20 2020 2020 2020  </model>.       
-000011e0: 203c 2f5f 7465 6d70 6c61 7465 5f3e 0a20   </_template_>. 
-000011f0: 2020 203c 2f5f 7465 6d70 6c61 7465 735f     </_templates_
-00001200: 3e0a 3c2f 6d69 6d65 6f5f 636f 6e66 6967  >.</mimeo_config
-00001210: 7572 6174 696f 6e3e 0a60 6060 0a5f 596f  uration>.```._Yo
-00001220: 7520 6361 6e20 6669 6e64 206d 6f72 6520  u can find more 
-00001230: 636f 6e66 6967 7572 6174 696f 6e20 6578  configuration ex
-00001240: 616d 706c 6573 2069 6e20 7468 6520 6065  amples in the `e
-00001250: 7861 6d70 6c65 7360 2066 6f6c 6465 722e  xamples` folder.
-00001260: 5f0a 0a23 2323 204d 696d 656f 6772 6170  _..### Mimeograp
-00001270: 680a 0a23 2323 2320 436f 6d6d 616e 6420  h..#### Command 
-00001280: 6c69 6e65 2074 6f6f 6c0a 0a60 6060 7368  line tool..```sh
-00001290: 0a6d 696d 656f 2053 6f6d 6545 6e74 6974  .mimeo SomeEntit
-000012a0: 792d 636f 6e66 6967 2e6a 736f 6e0a 6d69  y-config.json.mi
-000012b0: 6d65 6f20 536f 6d65 456e 7469 7479 2d63  meo SomeEntity-c
-000012c0: 6f6e 6669 672e 786d 6c0a 6060 600a 0a23  onfig.xml.```..#
-000012d0: 2323 2320 5079 7468 6f6e 206c 6962 7261  ### Python libra
-000012e0: 7279 0a0a 6060 6070 7974 686f 6e0a 6672  ry..```python.fr
-000012f0: 6f6d 206d 696d 656f 2069 6d70 6f72 7420  om mimeo import 
-00001300: 4d69 6d65 6f43 6f6e 6669 6746 6163 746f  MimeoConfigFacto
-00001310: 7279 2c20 4d69 6d65 6f67 7261 7068 0a0a  ry, Mimeograph..
-00001320: 636f 6e66 6967 203d 207b 0a20 2020 2023  config = {.    #
-00001330: 2059 6f75 7220 636f 6e66 6967 7572 6174   Your configurat
-00001340: 696f 6e20 696e 2061 2064 6963 740a 7d0a  ion in a dict.}.
-00001350: 636f 6e66 6967 203d 2022 2222 0a20 2020  config = """.   
-00001360: 2059 6f75 7220 636f 6e66 6967 7572 6174   Your configurat
-00001370: 696f 6e20 696e 2061 2073 7472 696e 6769  ion in a stringi
-00001380: 6669 6564 2058 4d4c 206e 6f64 650a 2222  fied XML node.""
-00001390: 220a 636f 6e66 6967 203d 2022 2220 2023  ".config = ""  #
-000013a0: 2041 2066 696c 6520 7061 7468 2074 6f20   A file path to 
-000013b0: 796f 7572 2063 6f6e 6669 6775 7261 7469  your configurati
-000013c0: 6f6e 2028 4a53 4f4e 202f 2058 4d4c 290a  on (JSON / XML).
-000013d0: 6d69 6d65 6f5f 636f 6e66 6967 203d 204d  mimeo_config = M
-000013e0: 696d 656f 436f 6e66 6967 4661 6374 6f72  imeoConfigFactor
-000013f0: 792e 7061 7273 6528 636f 6e66 6967 290a  y.parse(config).
-00001400: 4d69 6d65 6f67 7261 7068 286d 696d 656f  Mimeograph(mimeo
-00001410: 5f63 6f6e 6669 6729 2e70 726f 6365 7373  _config).process
-00001420: 2829 0a60 6060 0a2a 2a2a 0a54 6865 204d  ().```.***.The M
-00001430: 696d 656f 2043 6f6e 6669 6775 7261 7469  imeo Configurati
-00001440: 6f6e 2061 626f 7665 2077 696c 6c20 7072  on above will pr
-00001450: 6f64 7563 6520 3220 6669 6c65 733a 0a0a  oduce 2 files:..
-00001460: 6060 6078 6d6c 0a3c 212d 2d20 6d69 6d65  ```xml.<!-- mime
-00001470: 6f2d 6f75 7470 7574 2f6d 696d 656f 2d6f  o-output/mimeo-o
-00001480: 7574 7075 742d 312e 786d 6c2d 2d3e 0a3c  utput-1.xml-->.<
-00001490: 536f 6d65 456e 7469 7479 2078 6d6c 6e73  SomeEntity xmlns
-000014a0: 3d22 6874 7470 3a2f 2f6d 696d 656f 2e61  ="http://mimeo.a
-000014b0: 7263 682e 636f 6d2f 6465 6661 756c 742d  rch.com/default-
-000014c0: 6e61 6d65 7370 6163 6522 2078 6d6c 6e73  namespace" xmlns
-000014d0: 3a70 6e3d 2268 7474 703a 2f2f 6d69 6d65  :pn="http://mime
-000014e0: 6f2e 6172 6368 2e63 6f6d 2f70 7265 6669  o.arch.com/prefi
-000014f0: 7865 642d 6e61 6d65 7370 6163 6522 3e0a  xed-namespace">.
-00001500: 2020 2020 3c43 6869 6c64 4e6f 6465 313e      <ChildNode1>
-00001510: 313c 2f43 6869 6c64 4e6f 6465 313e 0a20  1</ChildNode1>. 
-00001520: 2020 203c 706e 3a43 6869 6c64 4e6f 6465     <pn:ChildNode
-00001530: 323e 7661 6c75 652d 323c 2f70 6e3a 4368  2>value-2</pn:Ch
-00001540: 696c 644e 6f64 6532 3e0a 2020 2020 3c43  ildNode2>.    <C
-00001550: 6869 6c64 4e6f 6465 333e 7472 7565 3c2f  hildNode3>true</
-00001560: 4368 696c 644e 6f64 6533 3e0a 3c2f 536f  ChildNode3>.</So
-00001570: 6d65 456e 7469 7479 3e0a 6060 600a 6060  meEntity>.```.``
-00001580: 6078 6d6c 0a3c 212d 2d20 6d69 6d65 6f2d  `xml.<!-- mimeo-
-00001590: 6f75 7470 7574 2f6d 696d 656f 2d6f 7574  output/mimeo-out
-000015a0: 7075 742d 322e 786d 6c2d 2d3e 0a3c 536f  put-2.xml-->.<So
-000015b0: 6d65 456e 7469 7479 2078 6d6c 6e73 3d22  meEntity xmlns="
-000015c0: 6874 7470 3a2f 2f6d 696d 656f 2e61 7263  http://mimeo.arc
-000015d0: 682e 636f 6d2f 6465 6661 756c 742d 6e61  h.com/default-na
-000015e0: 6d65 7370 6163 6522 2078 6d6c 6e73 3a70  mespace" xmlns:p
-000015f0: 6e3d 2268 7474 703a 2f2f 6d69 6d65 6f2e  n="http://mimeo.
-00001600: 6172 6368 2e63 6f6d 2f70 7265 6669 7865  arch.com/prefixe
-00001610: 642d 6e61 6d65 7370 6163 6522 3e0a 2020  d-namespace">.  
-00001620: 2020 3c43 6869 6c64 4e6f 6465 313e 313c    <ChildNode1>1<
-00001630: 2f43 6869 6c64 4e6f 6465 313e 0a20 2020  /ChildNode1>.   
-00001640: 203c 706e 3a43 6869 6c64 4e6f 6465 323e   <pn:ChildNode2>
-00001650: 7661 6c75 652d 323c 2f70 6e3a 4368 696c  value-2</pn:Chil
-00001660: 644e 6f64 6532 3e0a 2020 2020 3c43 6869  dNode2>.    <Chi
-00001670: 6c64 4e6f 6465 333e 7472 7565 3c2f 4368  ldNode3>true</Ch
-00001680: 696c 644e 6f64 6533 3e0a 3c2f 536f 6d65  ildNode3>.</Some
-00001690: 456e 7469 7479 3e0a 6060 600a 2a2a 2a0a  Entity>.```.***.
-000016a0: 0a23 2323 204d 696d 656f 2055 7469 6c73  .### Mimeo Utils
-000016b0: 0a0a 4d69 6d65 6f20 6578 706f 7365 7320  ..Mimeo exposes 
-000016c0: 7365 7665 7261 6c20 6675 6e63 7469 6f6e  several function
-000016d0: 7320 666f 7220 6461 7461 2067 656e 6572  s for data gener
-000016e0: 6174 696f 6e20 7468 6174 2077 696c 6c20  ation that will 
-000016f0: 6d61 6b65 2069 7420 6d6f 7265 2075 7365  make it more use
-00001700: 6675 6c20 666f 7220 7465 7374 696e 6720  ful for testing 
-00001710: 7075 7270 6f73 6573 2e0a 0a2a 2a54 656d  purposes...**Tem
-00001720: 706c 6174 652a 2a0a 6060 606a 736f 6e0a  plate**.```json.
-00001730: 7b0a 2020 2263 6f75 6e74 223a 2032 2c0a  {.  "count": 2,.
-00001740: 2020 226d 6f64 656c 223a 207b 0a20 2020    "model": {.   
-00001750: 2022 536f 6d65 456e 7469 7479 223a 207b   "SomeEntity": {
-00001760: 0a20 2020 2020 2022 6964 223a 2022 7b61  .      "id": "{a
-00001770: 7574 6f5f 696e 6372 656d 656e 747d 222c  uto_increment}",
-00001780: 0a20 2020 2020 2022 7261 6e64 6f6d 7374  .      "randomst
-00001790: 7269 6e67 223a 2022 7b72 616e 646f 6d5f  ring": "{random_
-000017a0: 7374 727d 222c 0a20 2020 2020 2022 7261  str}",.      "ra
-000017b0: 6e64 6f6d 696e 7422 3a20 227b 7261 6e64  ndomint": "{rand
-000017c0: 6f6d 5f69 6e74 7d22 0a20 2020 207d 0a20  om_int}".    }. 
-000017d0: 207d 0a7d 0a60 6060 0a60 6060 786d 6c0a   }.}.```.```xml.
-000017e0: 3c5f 7465 6d70 6c61 7465 5f3e 0a20 2020  <_template_>.   
-000017f0: 203c 636f 756e 743e 323c 2f63 6f75 6e74   <count>2</count
-00001800: 3e0a 2020 2020 3c6d 6f64 656c 3e0a 2020  >.    <model>.  
-00001810: 2020 2020 2020 0a20 2020 2020 2020 203c        .        <
-00001820: 536f 6d65 456e 7469 7479 3e0a 2020 2020  SomeEntity>.    
-00001830: 2020 2020 2020 2020 3c69 643e 7b61 7574          <id>{aut
-00001840: 6f5f 696e 6372 656d 656e 747d 3c2f 6964  o_increment}</id
-00001850: 3e0a 2020 2020 2020 2020 2020 2020 3c72  >.            <r
-00001860: 616e 646f 6d73 7472 696e 673e 7b72 616e  andomstring>{ran
-00001870: 646f 6d5f 7374 727d 3c2f 7261 6e64 6f6d  dom_str}</random
-00001880: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
-00001890: 2020 2020 3c72 616e 646f 6d69 6e74 3e7b      <randomint>{
-000018a0: 7261 6e64 6f6d 5f69 6e74 7d3c 2f72 616e  random_int}</ran
-000018b0: 646f 6d69 6e74 3e0a 2020 2020 2020 2020  domint>.        
-000018c0: 3c2f 536f 6d65 456e 7469 7479 3e0a 2020  </SomeEntity>.  
-000018d0: 2020 2020 2020 0a20 2020 203c 2f6d 6f64        .    </mod
-000018e0: 656c 3e0a 3c2f 5f74 656d 706c 6174 655f  el>.</_template_
-000018f0: 3e0a 6060 600a 0a2a 2a58 4d4c 2044 6174  >.```..**XML Dat
-00001900: 612a 2a0a 6060 6078 6d6c 0a3c 536f 6d65  a**.```xml.<Some
-00001910: 456e 7469 7479 3e0a 2020 2020 3c69 643e  Entity>.    <id>
-00001920: 3030 3030 313c 2f69 643e 0a20 2020 203c  00001</id>.    <
-00001930: 7261 6e64 6f6d 7374 7269 6e67 3e6d 4341  randomstring>mCA
-00001940: 7073 595a 7072 6179 596b 6d4b 6e59 5778  psYZprayYkmKnYWx
-00001950: 653c 2f72 616e 646f 6d73 7472 696e 673e  e</randomstring>
-00001960: 0a20 2020 203c 7261 6e64 6f6d 696e 743e  .    <randomint>
-00001970: 383c 2f72 616e 646f 6d69 6e74 3e0a 3c2f  8</randomint>.</
-00001980: 536f 6d65 456e 7469 7479 3e0a 6060 600a  SomeEntity>.```.
-00001990: 6060 6078 6d6c 0a3c 536f 6d65 456e 7469  ```xml.<SomeEnti
-000019a0: 7479 3e0a 2020 2020 3c69 643e 3030 3030  ty>.    <id>0000
-000019b0: 323c 2f69 643e 0a20 2020 203c 7261 6e64  2</id>.    <rand
-000019c0: 6f6d 7374 7269 6e67 3e63 6561 5055 7141  omstring>ceaPUqA
-000019d0: 5255 6b46 756b 5a49 5065 7571 4f3c 2f72  RUkFukZIPeuqO</r
-000019e0: 616e 646f 6d73 7472 696e 673e 0a20 2020  andomstring>.   
-000019f0: 203c 7261 6e64 6f6d 696e 743e 3939 3c2f   <randomint>99</
-00001a00: 7261 6e64 6f6d 696e 743e 0a3c 2f53 6f6d  randomint>.</Som
-00001a10: 6545 6e74 6974 793e 0a60 6060 0a0a 0a23  eEntity>.```...#
-00001a20: 2320 446f 6375 6d65 6e74 6174 696f 6e0a  # Documentation.
-00001a30: 0a23 2323 204d 696d 656f 2043 4c49 0a0a  .### Mimeo CLI..
-00001a40: 2323 2323 204d 696d 656f 2043 6f6e 6669  #### Mimeo Confi
-00001a50: 6775 7261 7469 6f6e 2061 7267 756d 656e  guration argumen
-00001a60: 7473 0a0a 5768 656e 2075 7369 6e67 204d  ts..When using M
-00001a70: 696d 656f 2063 6f6d 6d61 6e64 206c 696e  imeo command lin
-00001a80: 6520 746f 6f6c 2079 6f75 2063 616e 206f  e tool you can o
-00001a90: 7665 7277 7269 7465 204d 696d 656f 2043  verwrite Mimeo C
-00001aa0: 6f6e 6669 6775 7261 7469 6f6e 2070 726f  onfiguration pro
-00001ab0: 7065 7274 6965 733a 0a0a 7c20 5368 6f72  perties:..| Shor
-00001ac0: 7420 6f70 7469 6f6e 207c 204c 6f6e 6720  t option | Long 
-00001ad0: 6f70 7469 6f6e 2020 2020 2020 2020 207c  option         |
-00001ae0: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
-00001af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2020 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d        |.|:------
-00001b30: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
-00001b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d  -------------|:-
-00001b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b90: 2d2d 2d2d 7c0a 7c20 2020 2020 602d 6f60  ----|.|     `-o`
-00001ba0: 2020 2020 207c 2060 2d2d 6f75 7470 7574       | `--output
-00001bb0: 6020 2020 2020 2020 2020 207c 206f 7665  `          | ove
-00001bc0: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
-00001bd0: 7574 2f64 6972 6563 7469 6f6e 6020 7072  ut/direction` pr
-00001be0: 6f70 6572 7479 2020 2020 2020 2020 2020  operty          
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2020 7c0a 7c20 2020 2020 602d 7860 2020    |.|     `-x`  
-00001c10: 2020 207c 2060 2d2d 786d 6c2d 6465 636c     | `--xml-decl
-00001c20: 6172 6174 696f 6e60 207c 206f 7665 7277  aration` | overw
-00001c30: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
-00001c40: 2f78 6d6c 5f64 6563 6c61 7261 7469 6f6e  /xml_declaration
-00001c50: 6020 7072 6f70 6572 7479 2020 2020 2020  ` property      
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 7c0a 7c20 2020 2020 602d 6960 2020 2020  |.|     `-i`    
-00001c80: 207c 2060 2d2d 696e 6465 6e74 6020 2020   | `--indent`   
-00001c90: 2020 2020 2020 207c 206f 7665 7277 7269         | overwri
-00001ca0: 7465 2074 6865 2060 6f75 7470 7574 2f69  te the `output/i
-00001cb0: 6e64 656e 7460 2070 726f 7065 7274 7920  ndent` property 
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00001ce0: 7c20 2020 2020 602d 6460 2020 2020 207c  |     `-d`     |
-00001cf0: 2060 2d2d 6469 7265 6374 6f72 7960 2020   `--directory`  
-00001d00: 2020 2020 207c 206f 7665 7277 7269 7465       | overwrite
-00001d10: 2074 6865 2060 6f75 7470 7574 2f64 6972   the `output/dir
-00001d20: 6563 746f 7279 5f70 6174 6860 2070 726f  ectory_path` pro
-00001d30: 7065 7274 7920 2020 2020 2020 2020 2020  perty           
-00001d40: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00001d50: 2020 2020 602d 6660 2020 2020 207c 2060      `-f`     | `
-00001d60: 2d2d 6669 6c65 6020 2020 2020 2020 2020  --file`         
-00001d70: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
-00001d80: 6865 2060 6f75 7470 7574 2f66 696c 655f  he `output/file_
-00001d90: 6e61 6d65 6020 7072 6f70 6572 7479 2020  name` property  
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001db0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00001dc0: 2020 602d 4860 2020 2020 207c 2060 2d2d    `-H`     | `--
-00001dd0: 6874 7470 2d68 6f73 7460 2020 2020 2020  http-host`      
-00001de0: 207c 206f 7665 7277 7269 7465 2074 6865   | overwrite the
-00001df0: 2060 6f75 7470 7574 2f68 6f73 7460 2070   `output/host` p
-00001e00: 726f 7065 7274 7920 2020 2020 2020 2020  roperty         
-00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e20: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00001e30: 602d 7060 2020 2020 207c 2060 2d2d 6874  `-p`     | `--ht
-00001e40: 7470 2d70 6f72 7460 2020 2020 2020 207c  tp-port`       |
-00001e50: 206f 7665 7277 7269 7465 2074 6865 2060   overwrite the `
-00001e60: 6f75 7470 7574 2f70 6f72 7460 2070 726f  output/port` pro
-00001e70: 7065 7274 7920 2020 2020 2020 2020 2020  perty           
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 2020 2020 2020 7c0a 7c20 2020 2020 602d        |.|     `-
-00001ea0: 4560 2020 2020 207c 2060 2d2d 6874 7470  E`     | `--http
-00001eb0: 2d65 6e64 706f 696e 7460 2020 207c 206f  -endpoint`   | o
-00001ec0: 7665 7277 7269 7465 2074 6865 2060 6f75  verwrite the `ou
-00001ed0: 7470 7574 2f65 6e64 706f 696e 7460 2070  tput/endpoint` p
-00001ee0: 726f 7065 7274 7920 2020 2020 2020 2020  roperty         
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f00: 2020 2020 7c0a 7c20 2020 2020 602d 5560      |.|     `-U`
-00001f10: 2020 2020 207c 2060 2d2d 6874 7470 2d75       | `--http-u
-00001f20: 7365 7260 2020 2020 2020 207c 206f 7665  ser`       | ove
-00001f30: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
-00001f40: 7574 2f75 7365 726e 616d 6560 2070 726f  ut/username` pro
-00001f50: 7065 7274 7920 2020 2020 2020 2020 2020  perty           
+00000000: 2320 4d69 6d65 6f20 284d 696d 656f 6772  # Mimeo (Mimeogr
+00000010: 6170 6829 0a0a 5b21 5b4c 6963 656e 7365  aph)..[![License
+00000020: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000030: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000040: 6c69 6365 6e73 652f 546f 6d61 737a 416e  license/TomaszAn
+00000050: 696f 6c6f 7773 6b69 2f6d 696d 656f 3f6c  iolowski/mimeo?l
+00000060: 6162 656c 3d4c 6963 656e 7365 2673 7479  abel=License&sty
+00000070: 6c65 3d70 6c61 7374 6963 295d 2868 7474  le=plastic)](htt
+00000080: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000090: 546f 6d61 737a 416e 696f 6c6f 7773 6b69  TomaszAniolowski
+000000a0: 2f6d 696d 656f 2f62 6c6f 622f 6465 7665  /mimeo/blob/deve
+000000b0: 6c6f 702f 4c49 4345 4e53 4529 0a5b 215b  lop/LICENSE).[![
+000000c0: 5665 7273 696f 6e5d 2868 7474 7073 3a2f  Version](https:/
+000000d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000000e0: 7079 7069 2f76 2f6d 696d 656f 6772 6170  pypi/v/mimeograp
+000000f0: 683f 636f 6c6f 723d 626c 7565 266c 6162  h?color=blue&lab
+00000100: 656c 3d50 7950 4926 7374 796c 653d 706c  el=PyPI&style=pl
+00000110: 6173 7469 6329 5d28 6874 7470 733a 2f2f  astic)](https://
+00000120: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000130: 2f6d 696d 656f 6772 6170 682f 290a 5b21  /mimeograph/).[!
+00000140: 5b50 7974 686f 6e5d 2868 7474 7073 3a2f  [Python](https:/
+00000150: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000160: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
+00000170: 6d69 6d65 6f67 7261 7068 3f6c 6162 656c  mimeograph?label
+00000180: 3d50 7974 686f 6e26 7374 796c 653d 706c  =Python&style=pl
+00000190: 6173 7469 6329 5d28 6874 7470 733a 2f2f  astic)](https://
+000001a0: 7777 772e 7079 7468 6f6e 2e6f 7267 2f29  www.python.org/)
+000001b0: 2020 0a5b 215b 4275 696c 645d 2868 7474    .[![Build](htt
+000001c0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000001d0: 2e69 6f2f 6769 7468 7562 2f61 6374 696f  .io/github/actio
+000001e0: 6e73 2f77 6f72 6b66 6c6f 772f 7374 6174  ns/workflow/stat
+000001f0: 7573 2f54 6f6d 6173 7a41 6e69 6f6c 6f77  us/TomaszAniolow
+00000200: 736b 692f 6d69 6d65 6f2f 7465 7374 2e79  ski/mimeo/test.y
+00000210: 6d6c 3f63 6f6c 6f72 3d62 7269 6768 7467  ml?color=brightg
+00000220: 7265 656e 266c 6162 656c 3d54 6573 7425  reen&label=Test%
+00000230: 3230 4d69 6d65 6f26 7374 796c 653d 706c  20Mimeo&style=pl
+00000240: 6173 7469 6329 5d28 6874 7470 733a 2f2f  astic)](https://
+00000250: 6769 7468 7562 2e63 6f6d 2f54 6f6d 6173  github.com/Tomas
+00000260: 7a41 6e69 6f6c 6f77 736b 692f 6d69 6d65  zAniolowski/mime
+00000270: 6f2f 6163 7469 6f6e 732f 776f 726b 666c  o/actions/workfl
+00000280: 6f77 732f 7465 7374 2e79 6d6c 3f71 7565  ows/test.yml?que
+00000290: 7279 3d62 7261 6e63 6825 3341 6d61 696e  ry=branch%3Amain
+000002a0: 290a 5b21 5b43 6f64 6520 436f 7665 7261  ).[![Code Covera
+000002b0: 6765 5d28 6874 7470 733a 2f2f 696d 672e  ge](https://img.
+000002c0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000002d0: 2f43 6f64 6525 3230 436f 7665 7261 6765  /Code%20Coverage
+000002e0: 2d31 3030 2532 352d 6272 6967 6874 6772  -100%25-brightgr
+000002f0: 6565 6e3f 7374 796c 653d 706c 6173 7469  een?style=plasti
+00000300: 6329 5d28 6874 7470 733a 2f2f 6769 7468  c)](https://gith
+00000310: 7562 2e63 6f6d 2f54 6f6d 6173 7a41 6e69  ub.com/TomaszAni
+00000320: 6f6c 6f77 736b 692f 6d69 6d65 6f2f 6163  olowski/mimeo/ac
+00000330: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000340: 636f 7665 7261 6765 5f62 6164 6765 2e79  coverage_badge.y
+00000350: 6d6c 3f71 7565 7279 3d62 7261 6e63 6825  ml?query=branch%
+00000360: 3341 6d61 696e 290a 0a5b 4d69 6d65 6f5d  3Amain)..[Mimeo]
+00000370: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000380: 636f 6d2f 546f 6d61 737a 416e 696f 6c6f  com/TomaszAniolo
+00000390: 7773 6b69 2f6d 696d 656f 2920 6973 2061  wski/mimeo) is a
+000003a0: 2063 6f6d 6d61 6e64 206c 696e 6520 746f   command line to
+000003b0: 6f6c 2061 6e64 2061 2070 7974 686f 6e20  ol and a python 
+000003c0: 6c69 6272 6172 7920 6765 6e65 7261 7469  library generati
+000003d0: 6e67 204e 6f53 514c 2064 6174 6120 6261  ng NoSQL data ba
+000003e0: 7365 6420 6f6e 2061 2074 656d 706c 6174  sed on a templat
+000003f0: 652e 0a49 7420 6361 6e20 6265 2075 7365  e..It can be use
+00000400: 6420 6279 2064 6576 656c 6f70 6572 732c  d by developers,
+00000410: 2074 6573 7465 7273 206f 7220 6275 7369   testers or busi
+00000420: 6e65 7373 2061 6e61 6c79 7374 7320 696e  ness analysts in
+00000430: 2074 6865 6972 2064 6169 6c79 2077 6f72   their daily wor
+00000440: 6b2e 0a0a 0a23 2320 496e 7374 616c 6c61  k....## Installa
+00000450: 7469 6f6e 0a0a 496e 7374 616c 6c20 4d69  tion..Install Mi
+00000460: 6d65 6f20 7769 7468 2070 6970 0a0a 6060  meo with pip..``
+00000470: 6073 680a 7069 7020 696e 7374 616c 6c20  `sh.pip install 
+00000480: 6d69 6d65 6f67 7261 7068 0a60 6060 0a0a  mimeograph.```..
+00000490: 0a23 2320 5573 6167 652f 4578 616d 706c  .## Usage/Exampl
+000004a0: 6573 0a0a 2323 2320 4d69 6d65 6f20 436f  es..### Mimeo Co
+000004b0: 6e66 6967 7572 6174 696f 6e0a 0a50 7265  nfiguration..Pre
+000004c0: 7061 7265 204d 696d 656f 2043 6f6e 6669  pare Mimeo Confi
+000004d0: 6775 7261 7469 6f6e 2066 6972 7374 0a0a  guration first..
+000004e0: 3c74 6162 6c65 3e0a 2020 2020 3c74 723e  <table>.    <tr>
+000004f0: 0a20 2020 2020 2020 203c 7468 3e4a 534f  .        <th>JSO
+00000500: 4e3c 2f74 683e 0a20 2020 2020 2020 203c  N</th>.        <
+00000510: 7468 3e58 4d4c 3c2f 7468 3e0a 2020 2020  th>XML</th>.    
+00000520: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+00000530: 2020 2020 2020 203c 7464 2076 616c 6967         <td valig
+00000540: 6e3d 2274 6f70 223e 0a0a 6060 606a 736f  n="top">..```jso
+00000550: 6e0a 7b0a 2020 225f 7465 6d70 6c61 7465  n.{.  "_template
+00000560: 735f 223a 205b 0a20 2020 207b 0a20 2020  s_": [.    {.   
+00000570: 2020 2022 636f 756e 7422 3a20 3330 2c0a     "count": 30,.
+00000580: 2020 2020 2020 226d 6f64 656c 223a 207b        "model": {
+00000590: 0a20 2020 2020 2020 2022 536f 6d65 456e  .        "SomeEn
+000005a0: 7469 7479 223a 207b 0a20 2020 2020 2020  tity": {.       
+000005b0: 2020 2022 4078 6d6c 6e73 223a 2022 6874     "@xmlns": "ht
+000005c0: 7470 3a2f 2f6d 696d 656f 2e61 7263 682e  tp://mimeo.arch.
+000005d0: 636f 6d2f 6465 6661 756c 742d 6e61 6d65  com/default-name
+000005e0: 7370 6163 6522 2c0a 2020 2020 2020 2020  space",.        
+000005f0: 2020 2240 786d 6c6e 733a 706e 223a 2022    "@xmlns:pn": "
+00000600: 6874 7470 3a2f 2f6d 696d 656f 2e61 7263  http://mimeo.arc
+00000610: 682e 636f 6d2f 7072 6566 6978 6564 2d6e  h.com/prefixed-n
+00000620: 616d 6573 7061 6365 222c 0a20 2020 2020  amespace",.     
+00000630: 2020 2020 2022 4368 696c 644e 6f64 6531       "ChildNode1
+00000640: 223a 2031 2c0a 2020 2020 2020 2020 2020  ": 1,.          
+00000650: 2243 6869 6c64 4e6f 6465 3222 3a20 2276  "ChildNode2": "v
+00000660: 616c 7565 2d32 222c 0a20 2020 2020 2020  alue-2",.       
+00000670: 2020 2022 4368 696c 644e 6f64 6533 223a     "ChildNode3":
+00000680: 2074 7275 650a 2020 2020 2020 2020 7d0a   true.        }.
+00000690: 2020 2020 2020 7d0a 2020 2020 7d0a 2020        }.    }.  
+000006a0: 5d0a 7d0a 6060 600a 3c2f 7464 3e0a 2020  ].}.```.</td>.  
+000006b0: 2020 2020 2020 3c74 6420 7661 6c69 676e        <td valign
+000006c0: 3d22 746f 7022 3e0a 0a60 6060 786d 6c0a  ="top">..```xml.
+000006d0: 3c6d 696d 656f 5f63 6f6e 6669 6775 7261  <mimeo_configura
+000006e0: 7469 6f6e 3e0a 2020 2020 3c5f 7465 6d70  tion>.    <_temp
+000006f0: 6c61 7465 735f 3e0a 2020 2020 2020 2020  lates_>.        
+00000700: 3c5f 7465 6d70 6c61 7465 5f3e 0a20 2020  <_template_>.   
+00000710: 2020 2020 2020 2020 203c 636f 756e 743e           <count>
+00000720: 3330 3c2f 636f 756e 743e 0a20 2020 2020  30</count>.     
+00000730: 2020 2020 2020 203c 6d6f 6465 6c3e 0a0a         <model>..
+00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000750: 3c53 6f6d 6545 6e74 6974 790a 2020 2020  <SomeEntity.    
+00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000770: 786d 6c6e 733d 2268 7474 703a 2f2f 6d69  xmlns="http://mi
+00000780: 6d65 6f2e 6172 6368 2e63 6f6d 2f64 6566  meo.arch.com/def
+00000790: 6175 6c74 2d6e 616d 6573 7061 6365 220a  ault-namespace".
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 2020 2020 786d 6c6e 733a 706e 3d22 6874      xmlns:pn="ht
+000007c0: 7470 3a2f 2f6d 696d 656f 2e61 7263 682e  tp://mimeo.arch.
+000007d0: 636f 6d2f 7072 6566 6978 6564 2d6e 616d  com/prefixed-nam
+000007e0: 6573 7061 6365 223e 0a20 2020 2020 2020  espace">.       
+000007f0: 2020 2020 2020 2020 2020 2020 203c 4368               <Ch
+00000800: 696c 644e 6f64 6531 3e31 3c2f 4368 696c  ildNode1>1</Chil
+00000810: 644e 6f64 6531 3e0a 2020 2020 2020 2020  dNode1>.        
+00000820: 2020 2020 2020 2020 2020 2020 3c70 6e3a              <pn:
+00000830: 4368 696c 644e 6f64 6532 3e76 616c 7565  ChildNode2>value
+00000840: 2d32 3c2f 706e 3a43 6869 6c64 4e6f 6465  -2</pn:ChildNode
+00000850: 323e 0a20 2020 2020 2020 2020 2020 2020  2>.             
+00000860: 2020 2020 2020 203c 4368 696c 644e 6f64         <ChildNod
+00000870: 6533 3e74 7275 653c 2f43 6869 6c64 4e6f  e3>true</ChildNo
+00000880: 6465 333e 0a20 2020 2020 2020 2020 2020  de3>.           
+00000890: 2020 2020 203c 2f53 6f6d 6545 6e74 6974       </SomeEntit
+000008a0: 793e 0a0a 2020 2020 2020 2020 2020 2020  y>..            
+000008b0: 3c2f 6d6f 6465 6c3e 0a20 2020 2020 2020  </model>.       
+000008c0: 203c 2f5f 7465 6d70 6c61 7465 5f3e 0a20   </_template_>. 
+000008d0: 2020 203c 2f5f 7465 6d70 6c61 7465 735f     </_templates_
+000008e0: 3e0a 3c2f 6d69 6d65 6f5f 636f 6e66 6967  >.</mimeo_config
+000008f0: 7572 6174 696f 6e3e 0a60 6060 0a3c 2f74  uration>.```.</t
+00000900: 643e 0a20 203c 2f74 723e 0a3c 2f74 6162  d>.  </tr>.</tab
+00000910: 6c65 3e0a 0a0a 5f59 6f75 2063 616e 2066  le>..._You can f
+00000920: 696e 6420 6d6f 7265 2063 6f6e 6669 6775  ind more configu
+00000930: 7261 7469 6f6e 2065 7861 6d70 6c65 7320  ration examples 
+00000940: 696e 2074 6865 2060 6578 616d 706c 6573  in the `examples
+00000950: 6020 666f 6c64 6572 2e5f 0a0a 2323 2320  ` folder._..### 
+00000960: 4461 7461 2067 656e 6572 6174 696f 6e0a  Data generation.
+00000970: 0a54 6865 204d 696d 656f 2043 6f6e 6669  .The Mimeo Confi
+00000980: 6775 7261 7469 6f6e 2061 626f 7665 2077  guration above w
+00000990: 696c 6c20 7072 6f64 7563 6520 3220 6669  ill produce 2 fi
+000009a0: 6c65 733a 0a0a 6060 6078 6d6c 0a3c 212d  les:..```xml.<!-
+000009b0: 2d20 6d69 6d65 6f2d 6f75 7470 7574 2f6d  - mimeo-output/m
+000009c0: 696d 656f 2d6f 7574 7075 742d 312e 786d  imeo-output-1.xm
+000009d0: 6c2d 2d3e 0a3c 536f 6d65 456e 7469 7479  l-->.<SomeEntity
+000009e0: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f6d   xmlns="http://m
+000009f0: 696d 656f 2e61 7263 682e 636f 6d2f 6465  imeo.arch.com/de
+00000a00: 6661 756c 742d 6e61 6d65 7370 6163 6522  fault-namespace"
+00000a10: 2078 6d6c 6e73 3a70 6e3d 2268 7474 703a   xmlns:pn="http:
+00000a20: 2f2f 6d69 6d65 6f2e 6172 6368 2e63 6f6d  //mimeo.arch.com
+00000a30: 2f70 7265 6669 7865 642d 6e61 6d65 7370  /prefixed-namesp
+00000a40: 6163 6522 3e0a 2020 2020 3c43 6869 6c64  ace">.    <Child
+00000a50: 4e6f 6465 313e 313c 2f43 6869 6c64 4e6f  Node1>1</ChildNo
+00000a60: 6465 313e 0a20 2020 203c 706e 3a43 6869  de1>.    <pn:Chi
+00000a70: 6c64 4e6f 6465 323e 7661 6c75 652d 323c  ldNode2>value-2<
+00000a80: 2f70 6e3a 4368 696c 644e 6f64 6532 3e0a  /pn:ChildNode2>.
+00000a90: 2020 2020 3c43 6869 6c64 4e6f 6465 333e      <ChildNode3>
+00000aa0: 7472 7565 3c2f 4368 696c 644e 6f64 6533  true</ChildNode3
+00000ab0: 3e0a 3c2f 536f 6d65 456e 7469 7479 3e0a  >.</SomeEntity>.
+00000ac0: 6060 600a 6060 6078 6d6c 0a3c 212d 2d20  ```.```xml.<!-- 
+00000ad0: 6d69 6d65 6f2d 6f75 7470 7574 2f6d 696d  mimeo-output/mim
+00000ae0: 656f 2d6f 7574 7075 742d 322e 786d 6c2d  eo-output-2.xml-
+00000af0: 2d3e 0a3c 536f 6d65 456e 7469 7479 2078  ->.<SomeEntity x
+00000b00: 6d6c 6e73 3d22 6874 7470 3a2f 2f6d 696d  mlns="http://mim
+00000b10: 656f 2e61 7263 682e 636f 6d2f 6465 6661  eo.arch.com/defa
+00000b20: 756c 742d 6e61 6d65 7370 6163 6522 2078  ult-namespace" x
+00000b30: 6d6c 6e73 3a70 6e3d 2268 7474 703a 2f2f  mlns:pn="http://
+00000b40: 6d69 6d65 6f2e 6172 6368 2e63 6f6d 2f70  mimeo.arch.com/p
+00000b50: 7265 6669 7865 642d 6e61 6d65 7370 6163  refixed-namespac
+00000b60: 6522 3e0a 2020 2020 3c43 6869 6c64 4e6f  e">.    <ChildNo
+00000b70: 6465 313e 313c 2f43 6869 6c64 4e6f 6465  de1>1</ChildNode
+00000b80: 313e 0a20 2020 203c 706e 3a43 6869 6c64  1>.    <pn:Child
+00000b90: 4e6f 6465 323e 7661 6c75 652d 323c 2f70  Node2>value-2</p
+00000ba0: 6e3a 4368 696c 644e 6f64 6532 3e0a 2020  n:ChildNode2>.  
+00000bb0: 2020 3c43 6869 6c64 4e6f 6465 333e 7472    <ChildNode3>tr
+00000bc0: 7565 3c2f 4368 696c 644e 6f64 6533 3e0a  ue</ChildNode3>.
+00000bd0: 3c2f 536f 6d65 456e 7469 7479 3e0a 6060  </SomeEntity>.``
+00000be0: 600a 0a57 6865 6e20 7765 2077 6f75 6c64  `..When we would
+00000bf0: 2063 6f6e 6669 6775 7265 206f 7574 7075   configure outpu
+00000c00: 7420 666f 726d 6174 2061 7320 606a 736f  t format as `jso
+00000c10: 6e60 2074 6865 6e20 6974 2077 6f75 6c64  n` then it would
+00000c20: 2070 726f 6475 6365 204a 534f 4e20 6e6f   produce JSON no
+00000c30: 6465 733a 0a0a 6060 606a 736f 6e0a 7b0a  des:..```json.{.
+00000c40: 2020 2253 6f6d 6545 6e74 6974 7922 3a20    "SomeEntity": 
+00000c50: 7b0a 2020 2020 2240 786d 6c6e 7322 3a20  {.    "@xmlns": 
+00000c60: 2268 7474 703a 2f2f 6d69 6d65 6f2e 6172  "http://mimeo.ar
+00000c70: 6368 2e63 6f6d 2f64 6566 6175 6c74 2d6e  ch.com/default-n
+00000c80: 616d 6573 7061 6365 222c 0a20 2020 2022  amespace",.    "
+00000c90: 4078 6d6c 6e73 3a70 6e22 3a20 2268 7474  @xmlns:pn": "htt
+00000ca0: 703a 2f2f 6d69 6d65 6f2e 6172 6368 2e63  p://mimeo.arch.c
+00000cb0: 6f6d 2f70 7265 6669 7865 642d 6e61 6d65  om/prefixed-name
+00000cc0: 7370 6163 6522 2c0a 2020 2020 2243 6869  space",.    "Chi
+00000cd0: 6c64 4e6f 6465 3122 3a20 312c 0a20 2020  ldNode1": 1,.   
+00000ce0: 2022 706e 3a43 6869 6c64 4e6f 6465 3222   "pn:ChildNode2"
+00000cf0: 3a20 2276 616c 7565 2d32 222c 0a20 2020  : "value-2",.   
+00000d00: 2022 4368 696c 644e 6f64 6533 223a 2074   "ChildNode3": t
+00000d10: 7275 650a 2020 7d0a 7d0a 6060 600a 6060  rue.  }.}.```.``
+00000d20: 606a 736f 6e0a 7b0a 2020 2253 6f6d 6545  `json.{.  "SomeE
+00000d30: 6e74 6974 7922 3a20 7b0a 2020 2020 2240  ntity": {.    "@
+00000d40: 786d 6c6e 7322 3a20 2268 7474 703a 2f2f  xmlns": "http://
+00000d50: 6d69 6d65 6f2e 6172 6368 2e63 6f6d 2f64  mimeo.arch.com/d
+00000d60: 6566 6175 6c74 2d6e 616d 6573 7061 6365  efault-namespace
+00000d70: 222c 0a20 2020 2022 4078 6d6c 6e73 3a70  ",.    "@xmlns:p
+00000d80: 6e22 3a20 2268 7474 703a 2f2f 6d69 6d65  n": "http://mime
+00000d90: 6f2e 6172 6368 2e63 6f6d 2f70 7265 6669  o.arch.com/prefi
+00000da0: 7865 642d 6e61 6d65 7370 6163 6522 2c0a  xed-namespace",.
+00000db0: 2020 2020 2243 6869 6c64 4e6f 6465 3122      "ChildNode1"
+00000dc0: 3a20 312c 0a20 2020 2022 706e 3a43 6869  : 1,.    "pn:Chi
+00000dd0: 6c64 4e6f 6465 3222 3a20 2276 616c 7565  ldNode2": "value
+00000de0: 2d32 222c 0a20 2020 2022 4368 696c 644e  -2",.    "ChildN
+00000df0: 6f64 6533 223a 2074 7275 650a 2020 7d0a  ode3": true.  }.
+00000e00: 7d0a 6060 600a 0a60 6060 7368 0a6d 696d  }.```..```sh.mim
+00000e10: 656f 2053 6f6d 6545 6e74 6974 792d 636f  eo SomeEntity-co
+00000e20: 6e66 6967 2e6a 736f 6e0a 6d69 6d65 6f20  nfig.json.mimeo 
+00000e30: 536f 6d65 456e 7469 7479 2d63 6f6e 6669  SomeEntity-confi
+00000e40: 672e 786d 6c0a 6060 600a 0a0a 2323 2320  g.xml.```...### 
+00000e50: 4d69 6d65 6f20 5574 696c 730a 0a4d 696d  Mimeo Utils..Mim
+00000e60: 656f 2065 7870 6f73 6573 2073 6576 6572  eo exposes sever
+00000e70: 616c 2066 756e 6374 696f 6e73 2066 6f72  al functions for
+00000e80: 2064 6174 6120 6765 6e65 7261 7469 6f6e   data generation
+00000e90: 2074 6861 7420 7769 6c6c 206d 616b 6520   that will make 
+00000ea0: 6974 206d 6f72 6520 7573 6566 756c 2066  it more useful f
+00000eb0: 6f72 2074 6573 7469 6e67 2070 7572 706f  or testing purpo
+00000ec0: 7365 732e 0a54 6f20 7365 6520 616c 6c20  ses..To see all 
+00000ed0: 4d69 6d65 6f20 5574 696c 732c 2067 6f20  Mimeo Utils, go 
+00000ee0: 746f 2074 6865 2064 6f63 756d 656e 7461  to the documenta
+00000ef0: 7469 6f6e 2062 656c 6f77 2e0a 0a2a 2a54  tion below...**T
+00000f00: 656d 706c 6174 652a 2a0a 6060 606a 736f  emplate**.```jso
+00000f10: 6e0a 7b0a 2020 2263 6f75 6e74 223a 2032  n.{.  "count": 2
+00000f20: 2c0a 2020 226d 6f64 656c 223a 207b 0a20  ,.  "model": {. 
+00000f30: 2020 2022 536f 6d65 456e 7469 7479 223a     "SomeEntity":
+00000f40: 207b 0a20 2020 2020 2022 6964 223a 2022   {.      "id": "
+00000f50: 7b61 7574 6f5f 696e 6372 656d 656e 747d  {auto_increment}
+00000f60: 222c 0a20 2020 2020 2022 7261 6e64 6f6d  ",.      "random
+00000f70: 7374 7269 6e67 223a 2022 7b72 616e 646f  string": "{rando
+00000f80: 6d5f 7374 727d 222c 0a20 2020 2020 2022  m_str}",.      "
+00000f90: 7261 6e64 6f6d 696e 7422 3a20 227b 7261  randomint": "{ra
+00000fa0: 6e64 6f6d 5f69 6e74 7d22 0a20 2020 207d  ndom_int}".    }
+00000fb0: 0a20 207d 0a7d 0a60 6060 0a60 6060 786d  .  }.}.```.```xm
+00000fc0: 6c0a 3c5f 7465 6d70 6c61 7465 5f3e 0a20  l.<_template_>. 
+00000fd0: 2020 203c 636f 756e 743e 323c 2f63 6f75     <count>2</cou
+00000fe0: 6e74 3e0a 2020 2020 3c6d 6f64 656c 3e0a  nt>.    <model>.
+00000ff0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001000: 203c 536f 6d65 456e 7469 7479 3e0a 2020   <SomeEntity>.  
+00001010: 2020 2020 2020 2020 2020 3c69 643e 7b61            <id>{a
+00001020: 7574 6f5f 696e 6372 656d 656e 747d 3c2f  uto_increment}</
+00001030: 6964 3e0a 2020 2020 2020 2020 2020 2020  id>.            
+00001040: 3c72 616e 646f 6d73 7472 696e 673e 7b72  <randomstring>{r
+00001050: 616e 646f 6d5f 7374 727d 3c2f 7261 6e64  andom_str}</rand
+00001060: 6f6d 7374 7269 6e67 3e0a 2020 2020 2020  omstring>.      
+00001070: 2020 2020 2020 3c72 616e 646f 6d69 6e74        <randomint
+00001080: 3e7b 7261 6e64 6f6d 5f69 6e74 7d3c 2f72  >{random_int}</r
+00001090: 616e 646f 6d69 6e74 3e0a 2020 2020 2020  andomint>.      
+000010a0: 2020 3c2f 536f 6d65 456e 7469 7479 3e0a    </SomeEntity>.
+000010b0: 2020 2020 2020 2020 0a20 2020 203c 2f6d          .    </m
+000010c0: 6f64 656c 3e0a 3c2f 5f74 656d 706c 6174  odel>.</_templat
+000010d0: 655f 3e0a 6060 600a 0a2a 2a58 4d4c 2044  e_>.```..**XML D
+000010e0: 6174 612a 2a0a 6060 6078 6d6c 0a3c 536f  ata**.```xml.<So
+000010f0: 6d65 456e 7469 7479 3e0a 2020 2020 3c69  meEntity>.    <i
+00001100: 643e 3030 3030 313c 2f69 643e 0a20 2020  d>00001</id>.   
+00001110: 203c 7261 6e64 6f6d 7374 7269 6e67 3e6d   <randomstring>m
+00001120: 4341 7073 595a 7072 6179 596b 6d4b 6e59  CApsYZprayYkmKnY
+00001130: 5778 653c 2f72 616e 646f 6d73 7472 696e  Wxe</randomstrin
+00001140: 673e 0a20 2020 203c 7261 6e64 6f6d 696e  g>.    <randomin
+00001150: 743e 383c 2f72 616e 646f 6d69 6e74 3e0a  t>8</randomint>.
+00001160: 3c2f 536f 6d65 456e 7469 7479 3e0a 6060  </SomeEntity>.``
+00001170: 600a 6060 6078 6d6c 0a3c 536f 6d65 456e  `.```xml.<SomeEn
+00001180: 7469 7479 3e0a 2020 2020 3c69 643e 3030  tity>.    <id>00
+00001190: 3030 323c 2f69 643e 0a20 2020 203c 7261  002</id>.    <ra
+000011a0: 6e64 6f6d 7374 7269 6e67 3e63 6561 5055  ndomstring>ceaPU
+000011b0: 7141 5255 6b46 756b 5a49 5065 7571 4f3c  qARUkFukZIPeuqO<
+000011c0: 2f72 616e 646f 6d73 7472 696e 673e 0a20  /randomstring>. 
+000011d0: 2020 203c 7261 6e64 6f6d 696e 743e 3939     <randomint>99
+000011e0: 3c2f 7261 6e64 6f6d 696e 743e 0a3c 2f53  </randomint>.</S
+000011f0: 6f6d 6545 6e74 6974 793e 0a60 6060 0a0a  omeEntity>.```..
+00001200: 2a2a 4a53 4f4e 2044 6174 612a 2a0a 6060  **JSON Data**.``
+00001210: 606a 736f 6e0a 7b0a 2020 2253 6f6d 6545  `json.{.  "SomeE
+00001220: 6e74 6974 7922 3a20 7b0a 2020 2020 2269  ntity": {.    "i
+00001230: 6422 3a20 2230 3030 3031 222c 0a20 2020  d": "00001",.   
+00001240: 2022 7261 6e64 6f6d 7374 7269 6e67 223a   "randomstring":
+00001250: 2022 6d43 4170 7359 5a70 7261 7959 6b6d   "mCApsYZprayYkm
+00001260: 4b6e 5957 7865 222c 0a20 2020 2022 7261  KnYWxe",.    "ra
+00001270: 6e64 6f6d 696e 7422 3a20 380a 2020 7d0a  ndomint": 8.  }.
+00001280: 7d0a 6060 600a 6060 606a 736f 6e0a 7b0a  }.```.```json.{.
+00001290: 2020 2253 6f6d 6545 6e74 6974 7922 3a20    "SomeEntity": 
+000012a0: 7b0a 2020 2020 2269 6422 3a20 2230 3030  {.    "id": "000
+000012b0: 3032 222c 0a20 2020 2022 7261 6e64 6f6d  02",.    "random
+000012c0: 7374 7269 6e67 223a 2022 6365 6150 5571  string": "ceaPUq
+000012d0: 4152 556b 4675 6b5a 4950 6575 714f 222c  ARUkFukZIPeuqO",
+000012e0: 0a20 2020 2022 7261 6e64 6f6d 696e 7422  .    "randomint"
+000012f0: 3a20 3939 0a20 207d 0a7d 0a60 6060 0a0a  : 99.  }.}.```..
+00001300: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
+00001310: 6e0a 0a23 2323 204d 696d 656f 2043 4c49  n..### Mimeo CLI
+00001320: 0a0a 2323 2323 204d 696d 656f 2043 6f6e  ..#### Mimeo Con
+00001330: 6669 6775 7261 7469 6f6e 2061 7267 756d  figuration argum
+00001340: 656e 7473 0a0a 5768 656e 2075 7369 6e67  ents..When using
+00001350: 204d 696d 656f 2063 6f6d 6d61 6e64 206c   Mimeo command l
+00001360: 696e 6520 746f 6f6c 2079 6f75 2063 616e  ine tool you can
+00001370: 206f 7665 7277 7269 7465 204d 696d 656f   overwrite Mimeo
+00001380: 2043 6f6e 6669 6775 7261 7469 6f6e 2070   Configuration p
+00001390: 726f 7065 7274 6965 733a 0a0a 7c20 5368  roperties:..| Sh
+000013a0: 6f72 7420 6f70 7469 6f6e 207c 204c 6f6e  ort option | Lon
+000013b0: 6720 6f70 7469 6f6e 2020 2020 2020 2020  g option        
+000013c0: 207c 2044 6573 6372 6970 7469 6f6e 2020   | Description  
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001410: 2020 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d    |.|:----------
+00001420: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
+00001430: 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d  ---------|:-----
+00001440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001480: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 2020  ----------|.|   
+00001490: 2020 602d 4660 2020 2020 207c 2060 2d2d    `-F`     | `--
+000014a0: 666f 726d 6174 6020 2020 2020 2020 2020  format`         
+000014b0: 207c 206f 7665 7277 7269 7465 2074 6865   | overwrite the
+000014c0: 2060 6f75 7470 7574 2f66 6f72 6d61 7460   `output/format`
+000014d0: 2070 726f 7065 7274 7920 2020 2020 2020   property       
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001500: 2020 7c0a 7c20 2020 2020 602d 6f60 2020    |.|     `-o`  
+00001510: 2020 207c 2060 2d2d 6f75 7470 7574 6020     | `--output` 
+00001520: 2020 2020 2020 2020 207c 206f 7665 7277           | overw
+00001530: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
+00001540: 2f64 6972 6563 7469 6f6e 6020 7072 6f70  /direction` prop
+00001550: 6572 7479 2020 2020 2020 2020 2020 2020  erty            
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00001580: 2020 602d 7860 2020 2020 207c 2060 2d2d    `-x`     | `--
+00001590: 786d 6c2d 6465 636c 6172 6174 696f 6e60  xml-declaration`
+000015a0: 207c 206f 7665 7277 7269 7465 2074 6865   | overwrite the
+000015b0: 2060 6f75 7470 7574 2f78 6d6c 5f64 6563   `output/xml_dec
+000015c0: 6c61 7261 7469 6f6e 6020 7072 6f70 6572  laration` proper
+000015d0: 7479 2020 2020 2020 2020 2020 2020 2020  ty              
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 7c0a 7c20 2020 2020 602d 6960 2020    |.|     `-i`  
+00001600: 2020 207c 2060 2d2d 696e 6465 6e74 6020     | `--indent` 
+00001610: 2020 2020 2020 2020 207c 206f 7665 7277           | overw
+00001620: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
+00001630: 2f69 6e64 656e 7460 2070 726f 7065 7274  /indent` propert
+00001640: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001660: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00001670: 2020 602d 6460 2020 2020 207c 2060 2d2d    `-d`     | `--
+00001680: 6469 7265 6374 6f72 7960 2020 2020 2020  directory`      
+00001690: 207c 206f 7665 7277 7269 7465 2074 6865   | overwrite the
+000016a0: 2060 6f75 7470 7574 2f64 6972 6563 746f   `output/directo
+000016b0: 7279 5f70 6174 6860 2070 726f 7065 7274  ry_path` propert
+000016c0: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016e0: 2020 7c0a 7c20 2020 2020 602d 6660 2020    |.|     `-f`  
+000016f0: 2020 207c 2060 2d2d 6669 6c65 6020 2020     | `--file`   
+00001700: 2020 2020 2020 2020 207c 206f 7665 7277           | overw
+00001710: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
+00001720: 2f66 696c 655f 6e61 6d65 6020 7072 6f70  /file_name` prop
+00001730: 6572 7479 2020 2020 2020 2020 2020 2020  erty            
+00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001750: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00001760: 2020 602d 4860 2020 2020 207c 2060 2d2d    `-H`     | `--
+00001770: 6874 7470 2d68 6f73 7460 2020 2020 2020  http-host`      
+00001780: 207c 206f 7665 7277 7269 7465 2074 6865   | overwrite the
+00001790: 2060 6f75 7470 7574 2f68 6f73 7460 2070   `output/host` p
+000017a0: 726f 7065 7274 7920 2020 2020 2020 2020  roperty         
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017d0: 2020 7c0a 7c20 2020 2020 602d 7060 2020    |.|     `-p`  
+000017e0: 2020 207c 2060 2d2d 6874 7470 2d70 6f72     | `--http-por
+000017f0: 7460 2020 2020 2020 207c 206f 7665 7277  t`       | overw
+00001800: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
+00001810: 2f70 6f72 7460 2070 726f 7065 7274 7920  /port` property 
+00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001840: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00001850: 2020 602d 4560 2020 2020 207c 2060 2d2d    `-E`     | `--
+00001860: 6874 7470 2d65 6e64 706f 696e 7460 2020  http-endpoint`  
+00001870: 207c 206f 7665 7277 7269 7465 2074 6865   | overwrite the
+00001880: 2060 6f75 7470 7574 2f65 6e64 706f 696e   `output/endpoin
+00001890: 7460 2070 726f 7065 7274 7920 2020 2020  t` property     
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018c0: 2020 7c0a 7c20 2020 2020 602d 5560 2020    |.|     `-U`  
+000018d0: 2020 207c 2060 2d2d 6874 7470 2d75 7365     | `--http-use
+000018e0: 7260 2020 2020 2020 207c 206f 7665 7277  r`       | overw
+000018f0: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
+00001900: 2f75 7365 726e 616d 6560 2070 726f 7065  /username` prope
+00001910: 7274 7920 2020 2020 2020 2020 2020 2020  rty             
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00001940: 2020 602d 5060 2020 2020 207c 2060 2d2d    `-P`     | `--
+00001950: 6874 7470 2d70 6173 7377 6f72 6460 2020  http-password`  
+00001960: 207c 206f 7665 7277 7269 7465 2074 6865   | overwrite the
+00001970: 2060 6f75 7470 7574 2f70 6173 7377 6f72   `output/passwor
+00001980: 6460 2070 726f 7065 7274 7920 2020 2020  d` property     
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019b0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+000019c0: 2020 207c 2060 2d2d 6874 7470 2d6d 6574     | `--http-met
+000019d0: 686f 6460 2020 2020 207c 206f 7665 7277  hod`     | overw
+000019e0: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
+000019f0: 2f6d 6574 686f 6460 2070 726f 7065 7274  /method` propert
+00001a00: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00001a30: 2020 2020 2020 2020 2020 207c 2060 2d2d             | `--
+00001a40: 6874 7470 2d70 726f 746f 636f 6c60 2020  http-protocol`  
+00001a50: 207c 206f 7665 7277 7269 7465 2074 6865   | overwrite the
+00001a60: 2060 6f75 7470 7574 2f70 726f 746f 636f   `output/protoco
+00001a70: 6c60 2070 726f 7065 7274 7920 2020 2020  l` property     
+00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2020 7c0a 7c20 2020 2020 602d 6560 2020    |.|     `-e`  
+00001ab0: 2020 207c 2060 2d2d 6874 7470 2d65 6e76     | `--http-env
+00001ac0: 6020 2020 2020 2020 207c 206f 7665 7277  `        | overw
+00001ad0: 7269 7465 2074 6865 206f 7574 7075 7420  rite the output 
+00001ae0: 6874 7470 2070 726f 7065 7274 6965 7320  http properties 
+00001af0: 7573 696e 6720 6120 6d69 6d65 6f20 656e  using a mimeo en
+00001b00: 7620 636f 6e66 6967 7572 6174 696f 6e20  v configuration 
+00001b10: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00001b20: 2020 2020 2020 2020 2020 207c 2060 2d2d             | `--
+00001b30: 6874 7470 2d65 6e76 732d 6669 6c65 6020  http-envs-file` 
+00001b40: 207c 2075 7365 2061 2063 7573 746f 6d20   | use a custom 
+00001b50: 656e 7669 726f 6e6d 656e 7473 2066 696c  environments fil
+00001b60: 6520 2862 7920 6465 6661 756c 743a 206d  e (by default: m
+00001b70: 696d 656f 2e65 6e76 732e 6a73 6f6e 2920  imeo.envs.json) 
+00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b90: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+00001ba0: 2020 207c 2060 2d2d 7261 7760 2020 2020     | `--raw`    
+00001bb0: 2020 2020 2020 2020 207c 2073 616d 6520           | same 
+00001bc0: 6173 2060 2d6f 2073 7464 6f75 7460 3c62  as `-o stdout`<b
+00001bd0: 7220 2f3e 6f76 6572 7772 6974 6520 7468  r />overwrite th
+00001be0: 6520 606f 7574 7075 742f 6469 7265 6374  e `output/direct
+00001bf0: 696f 6e60 2070 726f 7065 7274 7920 746f  ion` property to
+00001c00: 2060 7374 646f 7574 6020 7c0a 0a23 2323   `stdout` |..###
+00001c10: 2320 4c6f 6767 696e 6720 6172 6775 6d65  # Logging argume
+00001c20: 6e74 730a 0a7c 2053 686f 7274 206f 7074  nts..| Short opt
+00001c30: 696f 6e20 7c20 4c6f 6e67 206f 7074 696f  ion | Long optio
+00001c40: 6e20 7c20 4465 7363 7269 7074 696f 6e20  n | Description 
+00001c50: 2020 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d        |.|:------
+00001c60: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
+00001c70: 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d  -----|:---------
+00001c80: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2020 2020  ---------|.|    
+00001c90: 2020 2020 2020 2020 2020 7c20 602d 2d73            | `--s
+00001ca0: 696c 656e 7460 2020 7c20 6469 7361 626c  ilent`  | disabl
+00001cb0: 6520 494e 464f 206c 6f67 7320 7c0a 7c20  e INFO logs |.| 
+00001cc0: 2020 2020 2020 2020 2020 2020 207c 2060               | `
+00001cd0: 2d2d 6465 6275 6760 2020 207c 2065 6e61  --debug`   | ena
+00001ce0: 626c 6520 4445 4255 4720 6d6f 6465 207c  ble DEBUG mode |
+00001cf0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00001d00: 7c20 602d 2d66 696e 6560 2020 2020 7c20  | `--fine`    | 
+00001d10: 656e 6162 6c65 2046 494e 4520 6d6f 6465  enable FINE mode
+00001d20: 2020 7c0a 0a23 2323 2320 4f74 6865 7220    |..#### Other 
+00001d30: 6172 6775 6d65 6e74 730a 0a7c 2053 686f  arguments..| Sho
+00001d40: 7274 206f 7074 696f 6e20 7c20 4c6f 6e67  rt option | Long
+00001d50: 206f 7074 696f 6e20 2020 2020 207c 2044   option      | D
+00001d60: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001d90: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  .|:------------:
+00001da0: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
+00001db0: 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|:-----------
+00001dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001de0: 2d2d 2d2d 2d7c 0a7c 2020 2020 2020 2020  -----|.|        
+00001df0: 2020 2020 2020 7c20 602d 2d73 6571 7565        | `--seque
+00001e00: 6e74 6961 6c6c 7960 207c 2070 726f 6365  ntially` | proce
+00001e10: 7373 204d 696d 656f 2043 6f6e 6669 6775  ss Mimeo Configu
+00001e20: 7261 7469 6f6e 7320 696e 2061 2073 696e  rations in a sin
+00001e30: 676c 6520 7468 7265 6164 207c 0a0a 2323  gle thread |..##
+00001e40: 2320 4d69 6d65 6f20 436f 6e66 6967 7572  # Mimeo Configur
+00001e50: 6174 696f 6e0a 0a4d 696d 656f 2063 6f6e  ation..Mimeo con
+00001e60: 6669 6775 7261 7469 6f6e 2069 7320 6465  figuration is de
+00001e70: 6669 6e65 6420 696e 2061 204a 534f 4e20  fined in a JSON 
+00001e80: 6669 6c65 2075 7369 6e67 2069 6e74 6572  file using inter
+00001e90: 6e61 6c20 7365 7474 696e 6773 2061 6e64  nal settings and
+00001ea0: 2064 6174 6120 7465 6d70 6c61 7465 732e   data templates.
+00001eb0: 0a0a 7c20 4b65 7920 2020 2020 2020 2020  ..| Key         
+00001ec0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00001ed0: 4c65 7665 6c20 2020 7c20 2020 2020 2052  Level   |      R
+00001ee0: 6571 7569 7265 6420 2020 2020 207c 2020  equired      |  
+00001ef0: 2020 2053 7570 706f 7274 6564 2076 616c     Supported val
+00001f00: 7565 7320 2020 2020 7c20 2020 2044 6566  ues     |    Def
+00001f10: 6175 6c74 2020 2020 207c 2044 6573 6372  ault     | Descr
+00001f20: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f70: 2020 7c0a 7c20 2020 2020 602d 5060 2020    |.|     `-P`  
-00001f80: 2020 207c 2060 2d2d 6874 7470 2d70 6173     | `--http-pas
-00001f90: 7377 6f72 6460 2020 207c 206f 7665 7277  sword`   | overw
-00001fa0: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
-00001fb0: 2f70 6173 7377 6f72 6460 2070 726f 7065  /password` prope
-00001fc0: 7274 7920 2020 2020 2020 2020 2020 2020  rty             
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00001ff0: 207c 2060 2d2d 6874 7470 2d6d 6574 686f   | `--http-metho
-00002000: 6460 2020 2020 207c 206f 7665 7277 7269  d`     | overwri
-00002010: 7465 2074 6865 2060 6f75 7470 7574 2f6d  te the `output/m
-00002020: 6574 686f 6460 2070 726f 7065 7274 7920  ethod` property 
-00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002040: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00002050: 7c20 2020 2020 2020 2020 2020 2020 207c  |              |
-00002060: 2060 2d2d 6874 7470 2d70 726f 746f 636f   `--http-protoco
-00002070: 6c60 2020 207c 206f 7665 7277 7269 7465  l`   | overwrite
-00002080: 2074 6865 2060 6f75 7470 7574 2f70 726f   the `output/pro
-00002090: 746f 636f 6c60 2070 726f 7065 7274 7920  tocol` property 
-000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020b0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-000020c0: 2020 2020 602d 6560 2020 2020 207c 2060      `-e`     | `
-000020d0: 2d2d 6874 7470 2d65 6e76 6020 2020 2020  --http-env`     
-000020e0: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
-000020f0: 6865 206f 7574 7075 7420 6874 7470 2070  he output http p
-00002100: 726f 7065 7274 6965 7320 7573 696e 6720  roperties using 
-00002110: 6120 6d69 6d65 6f20 656e 7620 636f 6e66  a mimeo env conf
-00002120: 6967 7572 6174 696f 6e20 7c0a 7c20 2020  iguration |.|   
-00002130: 2020 2020 2020 2020 2020 207c 2060 2d2d             | `--
-00002140: 6874 7470 2d65 6e76 732d 6669 6c65 6020  http-envs-file` 
-00002150: 207c 2075 7365 2061 2063 7573 746f 6d20   | use a custom 
-00002160: 656e 7669 726f 6e6d 656e 7473 2066 696c  environments fil
-00002170: 6520 2862 7920 6465 6661 756c 743a 206d  e (by default: m
-00002180: 696d 656f 2e65 6e76 732e 6a73 6f6e 2920  imeo.envs.json) 
-00002190: 2020 2020 2020 2020 7c0a 0a23 2323 2320          |..#### 
-000021a0: 4c6f 6767 696e 6720 6172 6775 6d65 6e74  Logging argument
-000021b0: 730a 0a7c 2053 686f 7274 206f 7074 696f  s..| Short optio
-000021c0: 6e20 7c20 4c6f 6e67 206f 7074 696f 6e20  n | Long option 
-000021d0: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
-000021e0: 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d      |.|:--------
-000021f0: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00002200: 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|:-----------
-00002210: 2d2d 2d2d 2d2d 2d7c 0a7c 2020 2020 2020  -------|.|      
-00002220: 2020 2020 2020 2020 7c20 602d 2d73 696c          | `--sil
-00002230: 656e 7460 2020 7c20 6469 7361 626c 6520  ent`  | disable 
-00002240: 494e 464f 206c 6f67 7320 7c0a 7c20 2020  INFO logs |.|   
-00002250: 2020 2020 2020 2020 2020 207c 2060 2d2d             | `--
-00002260: 6465 6275 6760 2020 207c 2065 6e61 626c  debug`   | enabl
-00002270: 6520 4445 4255 4720 6d6f 6465 207c 0a7c  e DEBUG mode |.|
-00002280: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00002290: 602d 2d66 696e 6560 2020 2020 7c20 656e  `--fine`    | en
-000022a0: 6162 6c65 2046 494e 4520 6d6f 6465 2020  able FINE mode  
-000022b0: 7c0a 0a23 2323 204d 696d 656f 2043 6f6e  |..### Mimeo Con
-000022c0: 6669 6775 7261 7469 6f6e 0a0a 4d69 6d65  figuration..Mime
-000022d0: 6f20 636f 6e66 6967 7572 6174 696f 6e20  o configuration 
-000022e0: 6973 2064 6566 696e 6564 2069 6e20 6120  is defined in a 
-000022f0: 4a53 4f4e 2066 696c 6520 7573 696e 6720  JSON file using 
-00002300: 696e 7465 726e 616c 2073 6574 7469 6e67  internal setting
-00002310: 7320 616e 6420 6461 7461 2074 656d 706c  s and data templ
-00002320: 6174 6573 2e0a 0a7c 204b 6579 2020 2020  ates...| Key    
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2020 2020 2020 2020 2020 7c20 204c 6576            |  Lev
-00002350: 656c 2020 207c 2020 2020 2020 5265 7175  el   |      Requ
-00002360: 6972 6564 2020 2020 2020 7c20 2020 2020  ired      |     
-00002370: 5375 7070 6f72 7465 6420 7661 6c75 6573  Supported values
-00002380: 2020 2020 207c 2020 2020 4465 6661 756c       |    Defaul
-00002390: 7420 2020 2020 7c20 4465 7363 7269 7074  t     | Descript
-000023a0: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.|:------------
-00002440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002450: 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d3a  -----|:--------:
-00002460: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-00002470: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00002480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
-00002490: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-000024a0: 3a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|--------------
-000024b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000024c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000024d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000024e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000024f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2060  -----------|.| `
-00002540: 6f75 7470 7574 6020 2020 2020 2020 2020  output`         
-00002550: 2020 2020 2020 2020 7c20 2043 6f6e 6669          |  Confi
-00002560: 6720 207c 2020 2020 2020 2020 3a78 3a20  g  |        :x: 
-00002570: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00002580: 2020 206f 626a 6563 7420 2020 2020 2020     object       
-00002590: 2020 207c 2020 2020 2020 2d2d 2d20 2020     |      ---   
-000025a0: 2020 2020 7c20 4465 6669 6e65 7320 6f75      | Defines ou
-000025b0: 7470 7574 2064 6574 6169 6c73 206f 6e20  tput details on 
-000025c0: 686f 7720 6974 2077 696c 6c20 6265 2063  how it will be c
-000025d0: 6f6e 7375 6d65 6420 2020 2020 2020 2020  onsumed         
-000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00002640: 7c20 606f 7574 7075 742f 6469 7265 6374  | `output/direct
-00002650: 696f 6e60 2020 2020 2020 207c 2020 436f  ion`       |  Co
-00002660: 6e66 6967 2020 7c20 2020 2020 2020 203a  nfig  |        :
-00002670: 783a 2020 2020 2020 2020 207c 2060 6669  x:         | `fi
-00002680: 6c65 602c 2060 7374 646f 7574 602c 2060  le`, `stdout`, `
-00002690: 6874 7470 6020 7c20 2020 2020 6066 696c  http` |     `fil
-000026a0: 6560 2020 2020 207c 2044 6566 696e 6573  e`     | Defines
-000026b0: 2068 6f77 206f 7574 7075 7420 7769 6c6c   how output will
-000026c0: 2062 6520 636f 6e73 756d 6564 2020 2020   be consumed    
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 207c 0a7c 2060 6f75 7470 7574 2f66 6f72   |.| `output/for
-00002750: 6d61 7460 2020 2020 2020 2020 2020 7c20  mat`          | 
-00002760: 2043 6f6e 6669 6720 207c 2020 2020 2020   Config  |      
-00002770: 2020 3a78 3a20 2020 2020 2020 2020 7c20    :x:         | 
-00002780: 2020 2020 2020 2020 2060 786d 6c60 2020           `xml`  
-00002790: 2020 2020 2020 2020 207c 2020 2020 2060           |     `
-000027a0: 786d 6c60 2020 2020 2020 7c20 4465 6669  xml`      | Defi
-000027b0: 6e65 7320 6f75 7470 7574 2064 6174 6120  nes output data 
-000027c0: 666f 726d 6174 2020 2020 2020 2020 2020  format          
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 2020 7c0a 7c20 606f 7574 7075 742f      |.| `output/
-00002850: 696e 6465 6e74 6020 2020 2020 2020 2020  indent`         
-00002860: 207c 2020 436f 6e66 6967 2020 7c20 2020   |  Config  |   
-00002870: 2020 2020 203a 783a 2020 2020 2020 2020       :x:        
-00002880: 207c 2020 2020 2020 2020 2069 6e74 6567   |         integ
-00002890: 6572 2020 2020 2020 2020 2020 7c20 2020  er          |   
-000028a0: 2020 606e 756c 6c60 2020 2020 207c 2044    `null`     | D
-000028b0: 6566 696e 6573 2069 6e64 656e 7420 6170  efines indent ap
-000028c0: 706c 6965 6420 696e 206f 7574 7075 7420  plied in output 
-000028d0: 6461 7461 2020 2020 2020 2020 2020 2020  data            
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002940: 2020 2020 2020 207c 0a7c 2060 6f75 7470         |.| `outp
-00002950: 7574 2f78 6d6c 5f64 6563 6c61 7261 7469  ut/xml_declarati
-00002960: 6f6e 6020 7c20 2043 6f6e 6669 6720 207c  on` |  Config  |
-00002970: 2020 2020 2020 2020 3a78 3a20 2020 2020          :x:     
-00002980: 2020 2020 7c20 2020 2020 2020 2020 626f      |         bo
-00002990: 6f6c 6561 6e20 2020 2020 2020 2020 207c  olean          |
-000029a0: 2020 2020 6066 616c 7365 6020 2020 2020      `false`     
-000029b0: 7c20 496e 6469 6361 7465 7320 7768 6574  | Indicates whet
-000029c0: 6865 7220 616e 2078 6d6c 2064 6563 6c61  her an xml decla
-000029d0: 7261 7469 6f6e 2073 686f 756c 6420 6265  ration should be
-000029e0: 2061 6464 6564 2074 6f20 6f75 7470 7574   added to output
-000029f0: 2064 6174 6120 2020 2020 2020 2020 2020   data           
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 2020 2020 2020 2020 2020 7c0a 7c20 606f            |.| `o
-00002a50: 7574 7075 742f 6469 7265 6374 6f72 795f  utput/directory_
-00002a60: 7061 7468 6020 207c 2020 436f 6e66 6967  path`  |  Config
-00002a70: 2020 7c20 2020 2020 2020 203a 783a 2020    |        :x:  
-00002a80: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00002a90: 2020 7374 7269 6e67 2020 2020 2020 2020    string        
-00002aa0: 2020 7c20 606d 696d 656f 2d6f 7574 7075    | `mimeo-outpu
-00002ab0: 7460 207c 2046 6f72 2060 6669 6c65 6020  t` | For `file` 
-00002ac0: 6469 7265 6374 696f 6e20 2d20 6465 6669  direction - defi
-00002ad0: 6e65 7320 616e 206f 7574 7075 7420 6469  nes an output di
-00002ae0: 7265 6374 6f72 7920 2020 2020 2020 2020  rectory         
-00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00002b50: 2060 6f75 7470 7574 2f66 696c 655f 6e61   `output/file_na
-00002b60: 6d65 6020 2020 2020 2020 7c20 2043 6f6e  me`       |  Con
-00002b70: 6669 6720 207c 2020 2020 2020 2020 3a78  fig  |        :x
-00002b80: 3a20 2020 2020 2020 2020 7c20 2020 2020  :         |     
-00002b90: 2020 2020 2073 7472 696e 6720 2020 2020       string     
-00002ba0: 2020 2020 207c 2060 6d69 6d65 6f2d 6f75       | `mimeo-ou
-00002bb0: 7470 7574 6020 7c20 466f 7220 6066 696c  tput` | For `fil
-00002bc0: 6560 2064 6972 6563 7469 6f6e 202d 2064  e` direction - d
-00002bd0: 6566 696e 6573 2061 6e20 6f75 7470 7574  efines an output
-00002be0: 2066 696c 6520 6e61 6d65 2020 2020 2020   file name      
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c50: 7c0a 7c20 606f 7574 7075 742f 6d65 7468  |.| `output/meth
-00002c60: 6f64 6020 2020 2020 2020 2020 207c 2020  od`          |  
-00002c70: 436f 6e66 6967 2020 7c20 2020 2020 2020  Config  |       
-00002c80: 203a 783a 2020 2020 2020 2020 207c 2020   :x:         |  
-00002c90: 2020 2020 6050 4f53 5460 2c20 6050 5554      `POST`, `PUT
-00002ca0: 6020 2020 2020 2020 7c20 2020 2020 6050  `       |     `P
-00002cb0: 4f53 5460 2020 2020 207c 2046 6f72 2060  OST`     | For `
-00002cc0: 6874 7470 6020 6469 7265 6374 696f 6e20  http` direction 
-00002cd0: 2d20 6465 6669 6e65 7320 6120 7265 7175  - defines a requ
-00002ce0: 6573 7420 6d65 7468 6f64 2020 2020 2020  est method      
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d50: 2020 207c 0a7c 2060 6f75 7470 7574 2f70     |.| `output/p
-00002d60: 726f 746f 636f 6c60 2020 2020 2020 2020  rotocol`        
-00002d70: 7c20 2043 6f6e 6669 6720 207c 2020 2020  |  Config  |    
-00002d80: 2020 2020 3a78 3a20 2020 2020 2020 2020      :x:         
-00002d90: 7c20 2020 2020 6068 7474 7060 2c20 6068  |     `http`, `h
-00002da0: 7474 7073 6020 2020 2020 207c 2020 2020  ttps`      |    
-00002db0: 2060 6874 7470 6020 2020 2020 7c20 466f   `http`     | Fo
-00002dc0: 7220 6068 7474 7060 2064 6972 6563 7469  r `http` directi
-00002dd0: 6f6e 202d 2064 6566 696e 6573 2061 2075  on - defines a u
-00002de0: 726c 2070 726f 746f 636f 6c20 2020 2020  rl protocol     
-00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e50: 2020 2020 2020 7c0a 7c20 606f 7574 7075        |.| `outpu
-00002e60: 742f 686f 7374 6020 2020 2020 2020 2020  t/host`         
-00002e70: 2020 207c 2020 436f 6e66 6967 2020 7c20     |  Config  | 
-00002e80: 3a68 6561 7679 5f63 6865 636b 5f6d 6172  :heavy_check_mar
-00002e90: 6b3a 207c 2020 2020 2020 2020 2020 7374  k: |          st
-00002ea0: 7269 6e67 2020 2020 2020 2020 2020 7c20  ring          | 
-00002eb0: 2020 2020 202d 2d2d 2020 2020 2020 207c       ---       |
-00002ec0: 2046 6f72 2060 6874 7470 6020 6469 7265   For `http` dire
-00002ed0: 6374 696f 6e20 2d20 6465 6669 6e65 7320  ction - defines 
-00002ee0: 6120 7572 6c20 686f 7374 2020 2020 2020  a url host      
-00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2020 2020 2020 2020 207c 0a7c 2060 6f75           |.| `ou
-00002f60: 7470 7574 2f70 6f72 7460 2020 2020 2020  tput/port`      
-00002f70: 2020 2020 2020 7c20 2043 6f6e 6669 6720        |  Config 
-00002f80: 207c 2020 2020 2020 2020 3a78 3a20 2020   |        :x:   
-00002f90: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00002fa0: 696e 7465 6765 7220 2020 2020 2020 2020  integer         
-00002fb0: 207c 2020 2020 2060 6e75 6c6c 6020 2020   |     `null`   
-00002fc0: 2020 7c20 466f 7220 6068 7474 7060 2064    | For `http` d
-00002fd0: 6972 6563 7469 6f6e 202d 2064 6566 696e  irection - defin
-00002fe0: 6573 2061 2075 726c 2070 6f72 7420 2863  es a url port (c
-00002ff0: 616e 2062 6520 656d 7074 7929 2020 2020  an be empty)    
-00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00003060: 606f 7574 7075 742f 656e 6470 6f69 6e74  `output/endpoint
-00003070: 6020 2020 2020 2020 207c 2020 436f 6e66  `        |  Conf
-00003080: 6967 2020 7c20 3a68 6561 7679 5f63 6865  ig  | :heavy_che
-00003090: 636b 5f6d 6172 6b3a 207c 2020 2020 2020  ck_mark: |      
-000030a0: 2020 2020 7374 7269 6e67 2020 2020 2020      string      
-000030b0: 2020 2020 7c20 2020 2020 202d 2d2d 2020      |      ---  
-000030c0: 2020 2020 207c 2046 6f72 2060 6874 7470       | For `http
-000030d0: 6020 6469 7265 6374 696f 6e20 2d20 6465  ` direction - de
-000030e0: 6669 6e65 7320 6120 7572 6c20 656e 6470  fines a url endp
-000030f0: 6f69 6e74 2020 2020 2020 2020 2020 2020  oint            
-00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003150: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00003160: 0a7c 2060 6f75 7470 7574 2f75 7365 726e  .| `output/usern
-00003170: 616d 6560 2020 2020 2020 2020 7c20 2043  ame`        |  C
-00003180: 6f6e 6669 6720 207c 203a 6865 6176 795f  onfig  | :heavy_
-00003190: 6368 6563 6b5f 6d61 726b 3a20 7c20 2020  check_mark: |   
-000031a0: 2020 2020 2020 2073 7472 696e 6720 2020         string   
-000031b0: 2020 2020 2020 207c 2020 2020 2020 2d2d         |      --
-000031c0: 2d20 2020 2020 2020 7c20 466f 7220 6068  -       | For `h
-000031d0: 7474 7060 2064 6972 6563 7469 6f6e 202d  ttp` direction -
-000031e0: 2064 6566 696e 6573 2061 2075 7365 726e   defines a usern
-000031f0: 616d 6520 2020 2020 2020 2020 2020 2020  ame             
-00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003260: 2020 7c0a 7c20 606f 7574 7075 742f 7061    |.| `output/pa
-00003270: 7373 776f 7264 6020 2020 2020 2020 207c  ssword`        |
-00003280: 2020 436f 6e66 6967 2020 7c20 3a68 6561    Config  | :hea
-00003290: 7679 5f63 6865 636b 5f6d 6172 6b3a 207c  vy_check_mark: |
-000032a0: 2020 2020 2020 2020 2020 7374 7269 6e67            string
-000032b0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000032c0: 202d 2d2d 2020 2020 2020 207c 2046 6f72   ---       | For
-000032d0: 2060 6874 7470 6020 6469 7265 6374 696f   `http` directio
-000032e0: 6e20 2d20 6465 6669 6e65 7320 6120 7061  n - defines a pa
-000032f0: 7373 776f 7264 2020 2020 2020 2020 2020  ssword          
-00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003360: 2020 2020 207c 0a7c 2060 7661 7273 6020       |.| `vars` 
-00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003380: 2020 2020 2020 2020 2020 7c20 2043 6f6e            |  Con
-00003390: 6669 6720 207c 2020 2020 2020 2020 3a78  fig  |        :x
-000033a0: 3a20 2020 2020 2020 2020 7c20 2020 2020  :         |     
-000033b0: 2020 2020 206f 626a 6563 7420 2020 2020       object     
-000033c0: 2020 2020 207c 2020 2020 2020 2d2d 2d20       |      --- 
-000033d0: 2020 2020 2020 7c20 4465 6669 6e65 7320        | Defines 
-000033e0: 7661 7269 6162 6c65 7320 746f 2062 6520  variables to be 
-000033f0: 7573 6564 2069 6e20 6120 4d69 6d65 6f20  used in a Mimeo 
-00003400: 5465 6d70 6c61 7465 2028 7265 6164 206d  Template (read m
-00003410: 6f72 6520 696e 206e 6578 7420 7365 6374  ore in next sect
-00003420: 696f 6e29 2020 2020 2020 2020 2020 2020  ion)            
-00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 7c0a 7c20 605f 7465 6d70 6c61 7465 735f  |.| `_templates_
-00003480: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00003490: 2020 2020 207c 2020 436f 6e66 6967 2020       |  Config  
-000034a0: 7c20 3a68 6561 7679 5f63 6865 636b 5f6d  | :heavy_check_m
-000034b0: 6172 6b3a 207c 2020 2020 2020 2020 2020  ark: |          
-000034c0: 6172 7261 7920 2020 2020 2020 2020 2020  array           
-000034d0: 7c20 2020 2020 202d 2d2d 2020 2020 2020  |      ---      
-000034e0: 207c 2053 746f 7265 7320 7465 6d70 6c61   | Stores templa
-000034f0: 7465 7320 666f 7220 6461 7461 2067 656e  tes for data gen
-00003500: 6572 6174 696f 6e20 2020 2020 2020 2020  eration         
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
-00003580: 636f 756e 7460 2020 2020 2020 2020 2020  count`          
-00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035a0: 7c20 5465 6d70 6c61 7465 207c 203a 6865  | Template | :he
-000035b0: 6176 795f 6368 6563 6b5f 6d61 726b 3a20  avy_check_mark: 
-000035c0: 7c20 2020 2020 2020 2020 696e 7465 6765  |         intege
-000035d0: 7220 2020 2020 2020 2020 207c 2020 2020  r          |    
-000035e0: 2020 2d2d 2d20 2020 2020 2020 7c20 496e    ---       | In
-000035f0: 6469 6361 7465 7320 6e75 6d62 6572 206f  dicates number o
-00003600: 6620 636f 7069 6573 2020 2020 2020 2020  f copies        
-00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003680: 2020 2020 2020 7c0a 7c20 606d 6f64 656c        |.| `model
-00003690: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-000036a0: 2020 2020 2020 2020 2020 207c 2054 656d             | Tem
-000036b0: 706c 6174 6520 7c20 3a68 6561 7679 5f63  plate | :heavy_c
-000036c0: 6865 636b 5f6d 6172 6b3a 207c 2020 2020  heck_mark: |    
-000036d0: 2020 2020 2020 6f62 6a65 6374 2020 2020        object    
-000036e0: 2020 2020 2020 7c20 2020 2020 202d 2d2d        |      ---
-000036f0: 2020 2020 2020 207c 2044 6566 696e 6573         | Defines
-00003700: 2064 6174 6120 7465 6d70 6c61 7465 2074   data template t
-00003710: 6f20 6265 2063 6f70 6965 6420 2020 2020  o be copied     
-00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003790: 207c 0a7c 2060 636f 6e74 6578 7460 2020   |.| `context`  
-000037a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037b0: 2020 2020 2020 7c20 204d 6f64 656c 2020        |  Model  
-000037c0: 207c 2020 2020 2020 2020 3a78 3a20 2020   |        :x:   
-000037d0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000037e0: 206f 626a 6563 7420 2020 2020 2020 2020   object         
-000037f0: 207c 2020 2020 2020 2d2d 2d20 2020 2020   |      ---     
-00003800: 2020 7c20 4465 6669 6e65 7320 6120 636f    | Defines a co
-00003810: 6e74 6578 7420 6e61 6d65 2074 6861 7420  ntext name that 
-00003820: 6973 2069 6e74 6572 6e61 6c6c 7920 7573  is internally us
-00003830: 6564 2065 2e67 2e20 7573 696e 6720 6063  ed e.g. using `c
-00003840: 7572 725f 6974 6572 2829 6020 616e 6420  urr_iter()` and 
-00003850: 6067 6574 5f6b 6579 2829 6020 6d69 6d65  `get_key()` mime
-00003860: 6f20 7574 696c 7320 2862 7920 6465 6661  o utils (by defa
-00003870: 756c 7420 6d6f 6465 6c20 6e61 6d65 2069  ult model name i
-00003880: 7320 7573 6564 2061 7320 7468 6520 636f  s used as the co
-00003890: 6e74 6578 7420 6e61 6d65 2920 7c0a 0a23  ntext name) |..#
-000038a0: 2323 2320 4d69 6d65 6f20 456e 7669 726f  ### Mimeo Enviro
-000038b0: 6e6d 656e 740a 0a54 6f20 6d61 6b65 2060  nment..To make `
-000038c0: 6874 7470 6020 6f75 7470 7574 2064 6972  http` output dir
-000038d0: 6563 746f 7279 2065 6173 6965 7220 746f  ectory easier to
-000038e0: 2075 7365 2c20 6d69 6d65 6f20 616c 6c6f   use, mimeo allo
-000038f0: 7773 2079 6f75 2074 6f20 636f 6e66 6967  ws you to config
-00003900: 7572 6520 4d69 6d65 6f20 456e 7669 726f  ure Mimeo Enviro
-00003910: 6e6d 656e 7473 2e0a 5468 6579 2061 7265  nments..They are
-00003920: 2063 6f6e 6669 6775 7265 6420 696e 2061   configured in a
-00003930: 204a 534f 4e20 6669 6c65 2028 6279 2064   JSON file (by d
-00003940: 6566 6175 6c74 3a20 6d69 6d65 6f2e 656e  efault: mimeo.en
-00003950: 7673 2e6a 736f 6e29 2061 6e64 2073 7570  vs.json) and sup
-00003960: 706f 7274 2074 6865 2066 6f6c 6c6f 7769  port the followi
-00003970: 6e67 206f 7574 7075 7420 6465 7461 696c  ng output detail
-00003980: 733a 0a2d 2060 7072 6f74 6f63 6f6c 600a  s:.- `protocol`.
-00003990: 2d20 6068 6f73 7460 0a2d 2060 706f 7274  - `host`.- `port
-000039a0: 600a 2d20 6075 7365 726e 616d 6560 0a2d  `.- `username`.-
-000039b0: 2060 7061 7373 776f 7264 600a 0a45 7861   `password`..Exa
-000039c0: 6d70 6c65 0a60 6060 6a73 6f6e 0a7b 0a20  mple.```json.{. 
-000039d0: 2020 2022 6c6f 6361 6c22 3a20 7b0a 2020     "local": {.  
-000039e0: 2020 2020 2020 2268 6f73 7422 3a20 226c        "host": "l
-000039f0: 6f63 616c 686f 7374 222c 0a20 2020 2020  ocalhost",.     
-00003a00: 2020 2022 706f 7274 223a 2038 3030 302c     "port": 8000,
-00003a10: 0a20 2020 2020 2020 2022 7573 6572 6e61  .        "userna
-00003a20: 6d65 223a 2022 6164 6d69 6e22 2c0a 2020  me": "admin",.  
-00003a30: 2020 2020 2020 2270 6173 7377 6f72 6422        "password"
-00003a40: 3a20 2261 646d 696e 220a 2020 2020 7d2c  : "admin".    },
-00003a50: 0a20 2020 2022 6465 7622 3a20 7b0a 2020  .    "dev": {.  
-00003a60: 2020 2020 2020 2270 726f 746f 636f 6c22        "protocol"
-00003a70: 3a20 2268 7474 7073 222c 0a20 2020 2020  : "https",.     
-00003a80: 2020 2022 686f 7374 223a 2022 3131 2e31     "host": "11.1
-00003a90: 3131 2e31 312e 3131 3122 2c0a 2020 2020  11.11.111",.    
-00003aa0: 2020 2020 2270 6f72 7422 3a20 3830 3030      "port": 8000
-00003ab0: 2c0a 2020 2020 2020 2020 2275 7365 726e  ,.        "usern
-00003ac0: 616d 6522 3a20 2273 6f6d 652d 7573 6572  ame": "some-user
-00003ad0: 222c 0a20 2020 2020 2020 2022 7061 7373  ",.        "pass
-00003ae0: 776f 7264 223a 2022 736f 6d65 2d70 6173  word": "some-pas
-00003af0: 7377 6f72 6422 0a20 2020 207d 0a7d 0a60  sword".    }.}.`
-00003b00: 6060 0a0a 546f 2075 7365 2061 2073 7065  ``..To use a spe
-00003b10: 6369 6669 6320 4d69 6d65 6f20 456e 7669  cific Mimeo Envi
-00003b20: 726f 6e6d 656e 7420 796f 7520 6361 6e20  ronment you can 
-00003b30: 7573 6520 7468 6520 666f 6c6c 6f77 696e  use the followin
-00003b40: 6720 636f 6d6d 616e 6473 3a0a 6060 6073  g commands:.```s
-00003b50: 680a 6d69 6d65 6f20 536f 6d65 456e 7469  h.mimeo SomeEnti
-00003b60: 7479 2d63 6f6e 6669 672e 6a73 6f6e 202d  ty-config.json -
-00003b70: 6520 6465 760a 6d69 6d65 6f20 536f 6d65  e dev.mimeo Some
-00003b80: 456e 7469 7479 2d63 6f6e 6669 672e 6a73  Entity-config.js
-00003b90: 6f6e 202d 6520 6465 7620 2d2d 6874 7470  on -e dev --http
-00003ba0: 2d65 6e76 732d 6669 6c65 2065 6e76 6972  -envs-file envir
-00003bb0: 6f6e 6d65 6e74 732e 6a73 6f6e 0a60 6060  onments.json.```
-00003bc0: 0a0a 2323 2323 204d 696d 656f 2056 6172  ..#### Mimeo Var
-00003bd0: 730a 0a4d 696d 656f 2061 6c6c 6f77 7320  s..Mimeo allows 
-00003be0: 796f 7520 746f 2064 6566 696e 6520 6120  you to define a 
-00003bf0: 6c69 7374 206f 6620 7661 7269 6162 6c65  list of variable
-00003c00: 732e 0a59 6f75 2063 616e 2075 7365 2074  s..You can use t
-00003c10: 6865 6d20 696e 2079 6f75 7220 4d69 6d65  hem in your Mime
-00003c20: 6f20 436f 6e66 6967 2062 7920 7772 6170  o Config by wrap
-00003c30: 7069 6e67 2074 6865 6d20 696e 2063 7572  ping them in cur
-00003c40: 6c79 2062 7261 636b 6574 7320 5b60 7b56  ly brackets [`{V
-00003c50: 4152 4941 424c 457d 605d 2e0a 0a54 6865  ARIABLE}`]...The
-00003c60: 7265 2061 7265 206f 6e6c 7920 3220 7275  re are only 2 ru
-00003c70: 6c65 7320 666f 7220 7661 7269 6162 6c65  les for variable
-00003c80: 206e 616d 6573 3a0a 2d20 5661 7269 6162   names:.- Variab
-00003c90: 6c65 206e 616d 6520 6361 6e20 696e 636c  le name can incl
-00003ca0: 7564 6520 7570 7065 722d 6361 7365 6420  ude upper-cased 
-00003cb0: 6c65 7474 6572 7320 5c5b 6041 2d5a 605c  letters \[`A-Z`\
-00003cc0: 5d2c 2075 6e64 6572 7363 6f72 6520 5c5b  ], underscore \[
-00003cd0: 605f 605c 5d20 616e 6420 6469 6769 7473  `_`\] and digits
-00003ce0: 205c 7b60 302d 3960 5c7d 206f 6e6c 790a   \{`0-9`\} only.
-00003cf0: 2d20 5661 7269 6162 6c65 206e 616d 6520  - Variable name 
-00003d00: 6d75 7374 2073 7461 7274 2077 6974 6820  must start with 
-00003d10: 6120 6c65 7474 6572 0a0a 5661 7269 6162  a letter..Variab
-00003d20: 6c65 2063 616e 2062 6520 6465 6669 6e65  le can be define
-00003d30: 6420 7769 7468 3a0a 2d20 616e 7920 6174  d with:.- any at
-00003d40: 6f6d 6963 2076 616c 7565 0a2d 2061 6e79  omic value.- any
-00003d50: 206f 7468 6572 2076 6172 6961 626c 6520   other variable 
-00003d60: 6465 6669 6e65 640a 2d20 616e 7920 4d69  defined.- any Mi
-00003d70: 6d65 6f20 5574 696c 0a0a 596f 7520 6361  meo Util..You ca
-00003d80: 6e20 7573 6520 4d69 6d65 6f20 5661 7273  n use Mimeo Vars
-00003d90: 2061 7320 7061 7274 6961 6c20 7661 6c75   as partial valu
-00003da0: 6573 2028 756e 6c65 7373 2074 6865 7920  es (unless they 
-00003db0: 6172 6520 6465 6669 6e65 6420 6173 204d  are defined as M
-00003dc0: 696d 656f 2055 7469 6c73 292e 0a0a 4578  imeo Utils)...Ex
-00003dd0: 616d 706c 653a 0a60 6060 6a73 6f6e 0a7b  ample:.```json.{
-00003de0: 0a20 2022 7661 7273 223a 207b 0a20 2020  .  "vars": {.   
-00003df0: 2022 4355 5354 4f4d 5f56 4152 5f31 223a   "CUSTOM_VAR_1":
-00003e00: 2022 6375 7374 6f6d 2d76 616c 7565 2d31   "custom-value-1
-00003e10: 222c 0a20 2020 2022 4355 5354 4f4d 5f56  ",.    "CUSTOM_V
-00003e20: 4152 5f32 223a 2031 2c0a 2020 2020 2243  AR_2": 1,.    "C
-00003e30: 5553 544f 4d5f 5641 525f 3322 3a20 7472  USTOM_VAR_3": tr
-00003e40: 7565 2c0a 2020 2020 2243 5553 544f 4d5f  ue,.    "CUSTOM_
-00003e50: 5641 525f 3422 3a20 227b 4355 5354 4f4d  VAR_4": "{CUSTOM
-00003e60: 5f56 4152 5f32 7d22 2c0a 2020 2020 2243  _VAR_2}",.    "C
-00003e70: 5553 544f 4d5f 5641 525f 3522 3a20 227b  USTOM_VAR_5": "{
-00003e80: 6175 746f 5f69 6e63 7265 6d65 6e74 7d22  auto_increment}"
-00003e90: 2c0a 2020 2020 2243 5553 544f 4d5f 5641  ,.    "CUSTOM_VA
-00003ea0: 525f 3622 3a20 7b0a 2020 2020 2020 225f  R_6": {.      "_
-00003eb0: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
-00003ec0: 2020 2020 2020 2022 5f6e 616d 6522 3a20         "_name": 
-00003ed0: 2272 616e 646f 6d5f 696e 7422 2c0a 2020  "random_int",.  
-00003ee0: 2020 2020 2020 226c 696d 6974 223a 2039        "limit": 9
-00003ef0: 390a 2020 2020 2020 7d0a 2020 2020 7d0a  9.      }.    }.
-00003f00: 2020 7d2c 0a20 2022 5f74 656d 706c 6174    },.  "_templat
-00003f10: 6573 5f22 3a20 5b0a 2020 2020 7b0a 2020  es_": [.    {.  
-00003f20: 2020 2020 2263 6f75 6e74 223a 2035 2c0a      "count": 5,.
-00003f30: 2020 2020 2020 226d 6f64 656c 223a 207b        "model": {
-00003f40: 0a20 2020 2020 2020 2022 536f 6d65 456e  .        "SomeEn
-00003f50: 7469 7479 223a 207b 0a20 2020 2020 2020  tity": {.       
-00003f60: 2020 2022 4368 696c 644e 6f64 6531 223a     "ChildNode1":
-00003f70: 2022 7b43 5553 544f 4d5f 5641 525f 317d   "{CUSTOM_VAR_1}
-00003f80: 222c 0a20 2020 2020 2020 2020 2022 4368  ",.          "Ch
-00003f90: 696c 644e 6f64 6532 223a 2022 7b43 5553  ildNode2": "{CUS
-00003fa0: 544f 4d5f 5641 525f 327d 222c 0a20 2020  TOM_VAR_2}",.   
-00003fb0: 2020 2020 2020 2022 4368 696c 644e 6f64         "ChildNod
-00003fc0: 6533 223a 2022 7b43 5553 544f 4d5f 5641  e3": "{CUSTOM_VA
-00003fd0: 525f 337d 222c 0a20 2020 2020 2020 2020  R_3}",.         
-00003fe0: 2022 4368 696c 644e 6f64 6534 223a 2022   "ChildNode4": "
-00003ff0: 7b43 5553 544f 4d5f 5641 525f 347d 222c  {CUSTOM_VAR_4}",
-00004000: 0a20 2020 2020 2020 2020 2022 4368 696c  .          "Chil
-00004010: 644e 6f64 6535 223a 2022 7b43 5553 544f  dNode5": "{CUSTO
-00004020: 4d5f 5641 525f 357d 222c 0a20 2020 2020  M_VAR_5}",.     
-00004030: 2020 2020 2022 4368 696c 644e 6f64 6536       "ChildNode6
-00004040: 223a 2022 7b43 5553 544f 4d5f 5641 525f  ": "{CUSTOM_VAR_
-00004050: 367d 222c 0a20 2020 2020 2020 2020 2022  6}",.          "
-00004060: 4368 696c 644e 6f64 6537 223a 2022 7b43  ChildNode7": "{C
-00004070: 5553 544f 4d5f 5641 525f 317d 2d77 6974  USTOM_VAR_1}-wit
-00004080: 682d 7375 6666 6978 220a 2020 2020 2020  h-suffix".      
-00004090: 2020 7d0a 2020 2020 2020 7d0a 2020 2020    }.      }.    
-000040a0: 7d0a 2020 5d0a 7d0a 6060 600a 0a23 2323  }.  ].}.```..###
-000040b0: 2320 4d69 6d65 6f20 5370 6563 6961 6c20  # Mimeo Special 
-000040c0: 4669 656c 6473 0a0a 496e 204d 696d 656f  Fields..In Mimeo
-000040d0: 2054 656d 706c 6174 6520 796f 7520 6361   Template you ca
-000040e0: 6e20 7573 6520 736f 2d63 616c 6c65 6420  n use so-called 
-000040f0: 5f73 7065 6369 616c 2066 6965 6c64 735f  _special fields_
-00004100: 2e0a 4576 6572 7920 6669 656c 6420 696e  ..Every field in
-00004110: 2061 2074 656d 706c 6174 6520 6361 6e20   a template can 
-00004120: 6265 2073 746f 7265 6420 696e 206d 656d  be stored in mem
-00004130: 6f72 7920 285f 7072 6f76 6964 6564 5f29  ory (_provided_)
-00004140: 2061 6e64 2075 7365 6420 6c61 7465 7220   and used later 
-00004150: 6173 2061 2076 616c 7565 206f 6620 6f74  as a value of ot
-00004160: 6865 7220 6669 656c 6473 2028 5f69 6e6a  her fields (_inj
-00004170: 6563 7465 645f 292e 0a54 6f20 7072 6f76  ected_)..To prov
-00004180: 6964 6520 6120 7370 6563 6961 6c20 6669  ide a special fi
-00004190: 656c 642c 2077 7261 7020 6974 7320 6e61  eld, wrap its na
-000041a0: 6d65 2077 6974 6820 636f 6c6f 6e73 3a20  me with colons: 
-000041b0: 5b60 3a53 6f6d 6546 6965 6c64 3a60 5d2e  [`:SomeField:`].
-000041c0: 2054 6f20 696e 6a65 6374 2c20 7573 6520   To inject, use 
-000041d0: 6164 6469 7469 6f6e 616c 6c79 2063 7572  additionally cur
-000041e0: 6c79 2062 7261 6365 7320 746f 0a6c 6574  ly braces to.let
-000041f0: 2069 6e74 6572 7072 6574 6572 206b 6e6f   interpreter kno
-00004200: 7720 6974 2073 686f 756c 6420 6265 2072  w it should be r
-00004210: 656e 6465 7265 6420 5b60 7b3a 536f 6d65  endered [`{:Some
-00004220: 4669 656c 643a 7d60 5d2e 0a54 6865 7920  Field:}`]..They 
-00004230: 6361 6e20 6265 2069 6e6a 6563 7465 6420  can be injected 
-00004240: 6173 2070 6172 7469 616c 2076 616c 7565  as partial value
-00004250: 732c 2073 696d 696c 6172 6c79 2074 6f20  s, similarly to 
-00004260: 4d69 6d65 6f20 5661 7273 2e0a 0a45 7861  Mimeo Vars...Exa
-00004270: 6d70 6c65 0a60 6060 6a73 6f6e 0a7b 0a20  mple.```json.{. 
-00004280: 2022 5f74 656d 706c 6174 6573 5f22 3a20   "_templates_": 
-00004290: 5b0a 2020 2020 7b0a 2020 2020 2020 2263  [.    {.      "c
-000042a0: 6f75 6e74 223a 2035 2c0a 2020 2020 2020  ount": 5,.      
-000042b0: 226d 6f64 656c 223a 207b 0a20 2020 2020  "model": {.     
-000042c0: 2020 2022 536f 6d65 456e 7469 7479 223a     "SomeEntity":
-000042d0: 207b 0a20 2020 2020 2020 2020 2022 3a43   {.          ":C
-000042e0: 6869 6c64 4e6f 6465 313a 223a 2022 6375  hildNode1:": "cu
-000042f0: 7374 6f6d 2d76 616c 7565 222c 0a20 2020  stom-value",.   
-00004300: 2020 2020 2020 2022 4368 696c 644e 6f64         "ChildNod
-00004310: 6532 223a 2022 7b3a 4368 696c 644e 6f64  e2": "{:ChildNod
-00004320: 6531 3a7d 222c 0a20 2020 2020 2020 2020  e1:}",.         
-00004330: 2022 4368 696c 644e 6f64 6533 223a 2022   "ChildNode3": "
-00004340: 7b3a 4368 696c 644e 6f64 6531 3a7d 2d77  {:ChildNode1:}-w
-00004350: 6974 682d 7375 6666 6978 220a 2020 2020  ith-suffix".    
-00004360: 2020 2020 7d0a 2020 2020 2020 7d0a 2020      }.      }.  
-00004370: 2020 7d0a 2020 5d0a 7d0a 6060 600a 0a23    }.  ].}.```..#
-00004380: 2323 2320 4d69 6d65 6f20 5574 696c 730a  ### Mimeo Utils.
-00004390: 0a59 6f75 2063 616e 2075 7365 2073 6576  .You can use sev
-000043a0: 6572 616c 2070 7265 6465 6669 6e65 6420  eral predefined 
-000043b0: 6675 6e63 7469 6f6e 7320 746f 2067 656e  functions to gen
-000043c0: 6572 6174 6520 6461 7461 2e20 5468 6579  erate data. They
-000043d0: 2063 616e 2062 6520 7573 6564 2069 6e20   can be used in 
-000043e0: 6120 5f72 6177 5f20 666f 726d 6174 206f  a _raw_ format o
-000043f0: 7220 5f70 6172 616d 6574 7269 7a65 645f  r _parametrized_
-00004400: 2e0a 0a23 2323 2323 2052 616e 646f 6d20  ...##### Random 
-00004410: 5374 7269 6e67 0a0a 4765 6e65 7261 7465  String..Generate
-00004420: 7320 6120 7261 6e64 6f6d 2073 7472 696e  s a random strin
-00004430: 6720 7661 6c75 652e 0a0a 7c20 5061 7261  g value...| Para
-00004440: 6d65 7465 7220 7c20 5375 7070 6f72 7465  meter | Supporte
-00004450: 6420 7661 6c75 6573 207c 2044 6566 6175  d values | Defau
-00004460: 6c74 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d  lt |.|:---------
-00004470: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|:-------------
-00004480: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d3a 7c0a  ---:|:-------:|.
-00004490: 7c20 206c 656e 6774 6820 2020 7c20 2020  |  length   |   
-000044a0: 2020 2060 696e 7460 2020 2020 2020 207c     `int`       |
-000044b0: 2020 6032 3060 2020 207c 0a0a 2323 2323    `20`   |..####
-000044c0: 2323 2052 6177 0a0a 5573 6573 2074 6865  ## Raw..Uses the
-000044d0: 2064 6566 6175 6c74 206c 656e 6774 683a   default length:
-000044e0: 2032 3020 6368 6172 6163 7465 7273 2e0a   20 characters..
-000044f0: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7261  .```json.{.  "ra
-00004500: 6e64 6f6d 7374 7269 6e67 223a 2022 7b72  ndomstring": "{r
-00004510: 616e 646f 6d5f 7374 727d 220a 7d0a 6060  andom_str}".}.``
-00004520: 600a 0a23 2323 2323 2320 5061 7261 6d65  `..###### Parame
-00004530: 7472 697a 6564 0a0a 5573 6573 2074 6865  trized..Uses the
-00004540: 2063 7573 746f 6d69 7a65 6420 6c65 6e67   customized leng
-00004550: 7468 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20  th...```json.{. 
-00004560: 2022 7261 6e64 6f6d 7374 7269 6e67 223a   "randomstring":
-00004570: 207b 0a20 2020 2022 5f6d 696d 656f 5f75   {.    "_mimeo_u
-00004580: 7469 6c22 3a20 7b0a 2020 2020 2020 225f  til": {.      "_
-00004590: 6e61 6d65 223a 2022 7261 6e64 6f6d 5f73  name": "random_s
-000045a0: 7472 222c 0a20 2020 2020 2022 6c65 6e67  tr",.      "leng
-000045b0: 7468 223a 2035 0a20 2020 207d 0a20 207d  th": 5.    }.  }
-000045c0: 0a7d 0a60 6060 0a0a 2323 2323 2320 5261  .}.```..##### Ra
-000045d0: 6e64 6f6d 2049 6e74 6567 6572 0a0a 4765  ndom Integer..Ge
-000045e0: 6e65 7261 7465 7320 6120 7261 6e64 6f6d  nerates a random
-000045f0: 2069 6e74 6567 6572 2076 616c 7565 2062   integer value b
-00004600: 6574 7765 656e 2060 7374 6172 7460 2061  etween `start` a
-00004610: 6e64 2060 6c69 6d69 7460 2070 6172 616d  nd `limit` param
-00004620: 6574 6572 7320 2869 6e63 6c75 7369 7665  eters (inclusive
-00004630: 292e 0a0a 7c20 5061 7261 6d65 7465 7220  )...| Parameter 
-00004640: 7c20 5375 7070 6f72 7465 6420 7661 6c75  | Supported valu
-00004650: 6573 207c 2044 6566 6175 6c74 207c 0a7c  es | Default |.|
-00004660: 3a2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d  :---------:|:---
-00004670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a  -------------:|:
-00004680: 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2020 7374  -------:|.|   st
-00004690: 6172 7420 2020 7c20 2020 2020 2060 696e  art   |      `in
-000046a0: 7460 2020 2020 2020 207c 2020 2060 3160  t`       |   `1`
-000046b0: 2020 207c 0a7c 2020 206c 696d 6974 2020     |.|   limit  
-000046c0: 207c 2020 2020 2020 6069 6e74 6020 2020   |      `int`   
-000046d0: 2020 2020 7c20 2060 3130 3060 2020 7c0a      |  `100`  |.
-000046e0: 0a23 2323 2323 2320 5261 770a 0a55 7365  .###### Raw..Use
-000046f0: 7320 7468 6520 6465 6661 756c 7420 7374  s the default st
-00004700: 6172 7420 2831 2920 616e 6420 6c69 6d69  art (1) and limi
-00004710: 7420 2831 3030 2920 7661 6c75 6573 2e0a  t (100) values..
-00004720: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7261  .```json.{.  "ra
-00004730: 6e64 6f6d 696e 7465 6765 7222 3a20 227b  ndominteger": "{
-00004740: 7261 6e64 6f6d 5f69 6e74 7d22 0a7d 0a60  random_int}".}.`
-00004750: 6060 0a0a 2323 2323 2323 2050 6172 616d  ``..###### Param
-00004760: 6574 7269 7a65 640a 0a55 7365 7320 7468  etrized..Uses th
-00004770: 6520 6375 7374 6f6d 697a 6564 206c 696d  e customized lim
-00004780: 6974 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20  it...```json.{. 
-00004790: 2022 7261 6e64 6f6d 696e 7465 6765 7231   "randominteger1
-000047a0: 223a 207b 0a20 2020 2022 5f6d 696d 656f  ": {.    "_mimeo
-000047b0: 5f75 7469 6c22 3a20 7b0a 2020 2020 2020  _util": {.      
-000047c0: 225f 6e61 6d65 223a 2022 7261 6e64 6f6d  "_name": "random
-000047d0: 5f69 6e74 222c 0a20 2020 2020 2022 7374  _int",.      "st
-000047e0: 6172 7422 3a20 300a 2020 2020 7d0a 2020  art": 0.    }.  
-000047f0: 7d2c 0a20 2022 7261 6e64 6f6d 696e 7465  },.  "randominte
-00004800: 6765 7232 223a 207b 0a20 2020 2022 5f6d  ger2": {.    "_m
-00004810: 696d 656f 5f75 7469 6c22 3a20 7b0a 2020  imeo_util": {.  
-00004820: 2020 2020 225f 6e61 6d65 223a 2022 7261      "_name": "ra
-00004830: 6e64 6f6d 5f69 6e74 222c 0a20 2020 2020  ndom_int",.     
-00004840: 2022 6c69 6d69 7422 3a20 350a 2020 2020   "limit": 5.    
-00004850: 7d0a 2020 7d2c 0a20 2022 7261 6e64 6f6d  }.  },.  "random
-00004860: 696e 7465 6765 7233 223a 207b 0a20 2020  integer3": {.   
-00004870: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
-00004880: 7b0a 2020 2020 2020 225f 6e61 6d65 223a  {.      "_name":
-00004890: 2022 7261 6e64 6f6d 5f69 6e74 222c 0a20   "random_int",. 
-000048a0: 2020 2020 2022 7374 6172 7422 3a20 302c       "start": 0,
-000048b0: 0a20 2020 2020 2022 6c69 6d69 7422 3a20  .      "limit": 
-000048c0: 350a 2020 2020 7d0a 2020 7d0a 7d0a 6060  5.    }.  }.}.``
-000048d0: 600a 0a23 2323 2323 2052 616e 646f 6d20  `..##### Random 
-000048e0: 4974 656d 0a0a 4765 6e65 7261 7465 7320  Item..Generates 
-000048f0: 6120 7261 6e64 6f6d 2076 616c 7565 2066  a random value f
-00004900: 726f 6d20 6974 656d 7320 7072 6f76 6964  rom items provid
-00004910: 6564 2e20 200a 4e4f 5449 4345 3a20 5468  ed.  .NOTICE: Th
-00004920: 6520 7261 7720 666f 726d 206f 6620 7468  e raw form of th
-00004930: 6973 204d 696d 656f 2055 7469 6c20 7769  is Mimeo Util wi
-00004940: 6c6c 2067 656e 6572 6174 6520 6120 626c  ll generate a bl
-00004950: 616e 6b20 7374 7269 6e67 2076 616c 7565  ank string value
-00004960: 2028 6173 2073 616d 6520 6173 206e 6f20   (as same as no 
-00004970: 6974 656d 7320 7061 7261 6d65 7472 697a  items parametriz
-00004980: 6564 292e 0a0a 7c20 5061 7261 6d65 7465  ed)...| Paramete
-00004990: 7220 7c20 5375 7070 6f72 7465 6420 7661  r | Supported va
-000049a0: 6c75 6573 207c 2044 6566 6175 6c74 207c  lues | Default |
-000049b0: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  .|:---------:|:-
-000049c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
-000049d0: 7c3a 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2020  |:-------:|.|   
-000049e0: 6974 656d 7320 2020 7c20 2020 2020 2060  items   |      `
-000049f0: 6c69 7374 6020 2020 2020 207c 2060 5b22  list`      | `["
-00004a00: 225d 6020 207c 0a0a 2323 2323 2323 2050  "]`  |..###### P
-00004a10: 6172 616d 6574 7269 7a65 640a 0a60 6060  arametrized..```
-00004a20: 6a73 6f6e 0a7b 0a20 2022 7261 6e64 6f6d  json.{.  "random
-00004a30: 223a 207b 0a20 2020 2022 5f6d 696d 656f  ": {.    "_mimeo
-00004a40: 5f75 7469 6c22 3a20 7b0a 2020 2020 2020  _util": {.      
-00004a50: 225f 6e61 6d65 223a 2022 7261 6e64 6f6d  "_name": "random
-00004a60: 5f69 7465 6d22 2c0a 2020 2020 2020 2269  _item",.      "i
-00004a70: 7465 6d73 223a 205b 2276 616c 7565 222c  tems": ["value",
-00004a80: 2031 2c20 7472 7565 5d0a 2020 2020 7d0a   1, true].    }.
-00004a90: 2020 7d0a 7d0a 6060 600a 0a23 2323 2323    }.}.```..#####
-00004aa0: 2044 6174 650a 0a47 656e 6572 6174 6573   Date..Generates
-00004ab0: 2061 2064 6174 6520 7661 6c75 6520 696e   a date value in
-00004ac0: 2066 6f72 6d61 7420 6059 5959 592d 4d4d   format `YYYY-MM
-00004ad0: 2d44 4460 2e0a 0a7c 2050 6172 616d 6574  -DD`...| Paramet
-00004ae0: 6572 2020 7c20 5375 7070 6f72 7465 6420  er  | Supported 
-00004af0: 7661 6c75 6573 207c 2044 6566 6175 6c74  values | Default
-00004b00: 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d3a   |.|:----------:
-00004b10: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-00004b20: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 3a7c 0a7c  --:|:-------:|.|
-00004b30: 2064 6179 735f 6465 6c74 6120 7c20 2020   days_delta |   
-00004b40: 2020 2060 696e 7460 2020 2020 2020 207c     `int`       |
-00004b50: 2020 2060 3060 2020 207c 0a0a 2323 2323     `0`   |..####
-00004b60: 2323 2052 6177 0a0a 5573 6573 2074 6865  ## Raw..Uses the
-00004b70: 2074 6f64 6179 2773 2064 6174 652e 0a0a   today's date...
-00004b80: 6060 606a 736f 6e0a 7b0a 2020 2254 6f64  ```json.{.  "Tod
-00004b90: 6179 223a 2022 7b64 6174 657d 220a 7d0a  ay": "{date}".}.
-00004ba0: 6060 600a 0a23 2323 2323 2320 5061 7261  ```..###### Para
-00004bb0: 6d65 7472 697a 6564 0a0a 5573 6573 2074  metrized..Uses t
-00004bc0: 6865 2063 7573 746f 6d69 7a65 6420 6461  he customized da
-00004bd0: 7973 2064 656c 7461 2e0a 0a60 6060 6a73  ys delta...```js
-00004be0: 6f6e 0a7b 0a20 2022 5965 7374 6572 6461  on.{.  "Yesterda
-00004bf0: 7922 3a20 7b0a 2020 2020 225f 6d69 6d65  y": {.    "_mime
-00004c00: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
-00004c10: 2022 5f6e 616d 6522 3a20 2264 6174 6522   "_name": "date"
-00004c20: 2c0a 2020 2020 2020 2264 6179 735f 6465  ,.      "days_de
-00004c30: 6c74 6122 3a20 2d31 0a20 2020 207d 0a20  lta": -1.    }. 
-00004c40: 207d 2c0a 2020 2254 6f6d 6f72 726f 7722   },.  "Tomorrow"
-00004c50: 3a20 7b0a 2020 2020 225f 6d69 6d65 6f5f  : {.    "_mimeo_
-00004c60: 7574 696c 223a 207b 0a20 2020 2020 2022  util": {.      "
-00004c70: 5f6e 616d 6522 3a20 2264 6174 6522 2c0a  _name": "date",.
-00004c80: 2020 2020 2020 2264 6179 735f 6465 6c74        "days_delt
-00004c90: 6122 3a20 310a 2020 2020 7d0a 2020 7d0a  a": 1.    }.  }.
-00004ca0: 7d0a 6060 600a 0a23 2323 2323 2044 6174  }.```..##### Dat
-00004cb0: 6520 5469 6d65 0a0a 4765 6e65 7261 7465  e Time..Generate
-00004cc0: 7320 6120 6461 7465 2074 696d 6520 7661  s a date time va
-00004cd0: 6c75 6520 696e 2066 6f72 6d61 7420 6059  lue in format `Y
-00004ce0: 5959 592d 4d4d 2d44 4427 5427 4848 3a6d  YYY-MM-DD'T'HH:m
-00004cf0: 6d3a 5353 602e 0a0a 7c20 2020 5061 7261  m:SS`...|   Para
-00004d00: 6d65 7465 7220 2020 7c20 5375 7070 6f72  meter   | Suppor
-00004d10: 7465 6420 7661 6c75 6573 207c 2044 6566  ted values | Def
-00004d20: 6175 6c74 207c 0a7c 3a2d 2d2d 2d2d 2d2d  ault |.|:-------
-00004d30: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
-00004d40: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
-00004d50: 2d2d 2d3a 7c0a 7c20 2064 6179 735f 6465  ---:|.|  days_de
-00004d60: 6c74 6120 2020 7c20 2020 2020 2060 696e  lta   |      `in
-00004d70: 7460 2020 2020 2020 207c 2020 2060 3060  t`       |   `0`
-00004d80: 2020 207c 0a7c 2020 686f 7572 735f 6465     |.|  hours_de
-00004d90: 6c74 6120 207c 2020 2020 2020 6069 6e74  lta  |      `int
-00004da0: 6020 2020 2020 2020 7c20 2020 6030 6020  `       |   `0` 
-00004db0: 2020 7c0a 7c20 6d69 6e75 7465 735f 6465    |.| minutes_de
-00004dc0: 6c74 6120 7c20 2020 2020 2060 696e 7460  lta |      `int`
-00004dd0: 2020 2020 2020 207c 2020 2060 3060 2020         |   `0`  
-00004de0: 207c 0a7c 2073 6563 6f6e 6473 5f64 656c   |.| seconds_del
-00004df0: 7461 207c 2020 2020 2020 6069 6e74 6020  ta |      `int` 
-00004e00: 2020 2020 2020 7c20 2020 6030 6020 2020        |   `0`   
-00004e10: 7c0a 0a23 2323 2323 2320 5261 770a 0a55  |..###### Raw..U
-00004e20: 7365 7320 7468 6520 6375 7272 656e 7420  ses the current 
-00004e30: 7469 6d65 7374 616d 702e 0a0a 6060 606a  timestamp...```j
-00004e40: 736f 6e0a 7b0a 2020 224e 6f77 223a 2022  son.{.  "Now": "
-00004e50: 7b64 6174 655f 7469 6d65 7d22 0a7d 0a60  {date_time}".}.`
-00004e60: 6060 0a0a 2323 2323 2323 2050 6172 616d  ``..###### Param
-00004e70: 6574 7269 7a65 640a 0a55 7365 7320 7468  etrized..Uses th
-00004e80: 6520 6375 7374 6f6d 697a 6564 2064 656c  e customized del
-00004e90: 7461 732e 0a0a 6060 606a 736f 6e0a 7b0a  tas...```json.{.
-00004ea0: 2020 2254 6f6d 6f72 726f 7754 6872 6565    "TomorrowThree
-00004eb0: 486f 7572 734c 6174 6572 5477 656e 7479  HoursLaterTwenty
-00004ec0: 4d69 6e75 7465 7341 676f 5477 6f53 6563  MinutesAgoTwoSec
-00004ed0: 6f6e 6473 4c61 7465 7222 3a20 7b0a 2020  ondsLater": {.  
-00004ee0: 2020 225f 6d69 6d65 6f5f 7574 696c 223a    "_mimeo_util":
-00004ef0: 207b 0a20 2020 2020 2022 5f6e 616d 6522   {.      "_name"
-00004f00: 3a20 2264 6174 655f 7469 6d65 222c 0a20  : "date_time",. 
-00004f10: 2020 2020 2022 6461 7973 5f64 656c 7461       "days_delta
-00004f20: 223a 2031 2c0a 2020 2020 2020 2268 6f75  ": 1,.      "hou
-00004f30: 7273 5f64 656c 7461 223a 2033 2c0a 2020  rs_delta": 3,.  
-00004f40: 2020 2020 226d 696e 7574 6573 5f64 656c      "minutes_del
-00004f50: 7461 223a 202d 3230 2c0a 2020 2020 2020  ta": -20,.      
-00004f60: 2273 6563 6f6e 6473 5f64 656c 7461 223a  "seconds_delta":
-00004f70: 2032 0a20 2020 207d 0a20 207d 0a7d 0a60   2.    }.  }.}.`
-00004f80: 6060 0a0a 2323 2323 2320 4175 746f 2049  ``..##### Auto I
-00004f90: 6e63 7265 6d65 6e74 0a0a 4765 6e65 7261  ncrement..Genera
-00004fa0: 7465 7320 6120 6e65 7874 2069 6e74 6567  tes a next integ
-00004fb0: 6572 2069 6e20 636f 6e74 6578 7420 6f66  er in context of
-00004fc0: 2061 206d 6f64 656c 2028 696e 206e 6573   a model (in nes
-00004fd0: 7465 6420 7465 6d70 6c61 7465 7320 6974  ted templates it
-00004fe0: 2077 696c 6c20 7573 6520 6120 7365 7061   will use a sepa
-00004ff0: 7261 7465 6420 636f 6e74 6578 7429 2e0a  rated context)..
-00005000: 0a7c 2050 6172 616d 6574 6572 207c 2053  .| Parameter | S
-00005010: 7570 706f 7274 6564 2076 616c 7565 7320  upported values 
-00005020: 7c20 4465 6661 756c 7420 207c 0a7c 3a2d  | Default  |.|:-
-00005030: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
-00005040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
-00005050: 2d2d 2d2d 2d2d 3a7c 0a7c 2020 7061 7474  ------:|.|  patt
-00005060: 6572 6e20 207c 2020 2020 2020 6073 7472  ern  |      `str
-00005070: 6020 2020 2020 2020 7c20 607b 3a30 3564  `       | `{:05d
-00005080: 7d60 207c 0a0a 2323 2323 2323 2052 6177  }` |..###### Raw
-00005090: 0a0a 5573 6573 2061 2064 6566 6175 6c74  ..Uses a default
-000050a0: 2070 6174 7465 726e 3a20 2a2a 7b3a 3035   pattern: **{:05
-000050b0: 647d 2a2a 2028 616e 2069 6e74 6567 6572  d}** (an integer
-000050c0: 2077 6974 6820 3520 6c65 6164 696e 6720   with 5 leading 
-000050d0: 7a65 726f 7329 2e0a 0a60 6060 6a73 6f6e  zeros)...```json
-000050e0: 0a7b 0a20 2022 4944 223a 2022 7b61 7574  .{.  "ID": "{aut
-000050f0: 6f5f 696e 6372 656d 656e 747d 220a 7d0a  o_increment}".}.
-00005100: 6060 600a 0a23 2323 2323 2320 5061 7261  ```..###### Para
-00005110: 6d65 7472 697a 6564 0a0a 5573 6573 2074  metrized..Uses t
-00005120: 6865 2073 7472 696e 6720 7061 7474 6572  he string patter
-00005130: 6e20 7072 6f76 6964 6564 2e0a 0a60 6060  n provided...```
-00005140: 6a73 6f6e 0a7b 0a20 2022 4944 223a 207b  json.{.  "ID": {
-00005150: 0a20 2020 2022 5f6d 696d 656f 5f75 7469  .    "_mimeo_uti
-00005160: 6c22 3a20 7b0a 2020 2020 2020 225f 6e61  l": {.      "_na
-00005170: 6d65 223a 2022 6175 746f 5f69 6e63 7265  me": "auto_incre
-00005180: 6d65 6e74 222c 0a20 2020 2020 2022 7061  ment",.      "pa
-00005190: 7474 6572 6e22 3a20 224d 595f 4944 5f7b  ttern": "MY_ID_{
-000051a0: 3a30 3130 647d 220a 2020 2020 7d0a 2020  :010d}".    }.  
-000051b0: 7d0a 7d0a 6060 600a 0a23 2323 2323 2043  }.}.```..##### C
-000051c0: 7572 7265 6e74 2049 7465 7261 7469 6f6e  urrent Iteration
-000051d0: 0a0a 4765 6e65 7261 7465 7320 6120 7661  ..Generates a va
-000051e0: 6c75 6520 6f66 2074 6865 2063 7572 7265  lue of the curre
-000051f0: 6e74 2069 7465 7261 7469 6f6e 2069 6e20  nt iteration in 
-00005200: 6120 4d69 6d65 6f20 5465 6d70 6c61 7465  a Mimeo Template
-00005210: 2063 6f6e 7465 7874 2e0a 0a7c 2050 6172   context...| Par
-00005220: 616d 6574 6572 207c 2053 7570 706f 7274  ameter | Support
-00005230: 6564 2076 616c 7565 7320 7c20 2020 2020  ed values |     
-00005240: 2044 6566 6175 6c74 2020 2020 2020 7c0a   Default      |.
-00005250: 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  |:---------:|:--
-00005260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
-00005270: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-00005280: 2d2d 3a7c 0a7c 2020 636f 6e74 6578 7420  --:|.|  context 
-00005290: 207c 2020 2020 2020 6073 7472 6020 2020   |      `str`   
-000052a0: 2020 2020 7c20 6120 6375 7272 656e 7420      | a current 
-000052b0: 636f 6e74 6578 7420 7c0a 0a23 2323 2323  context |..#####
-000052c0: 2320 5261 770a 0a55 7365 7320 7468 6520  # Raw..Uses the 
-000052d0: 6375 7272 656e 7420 636f 6e74 6578 742e  current context.
-000052e0: 0a0a 6060 606a 736f 6e0a 7b0a 2020 2249  ..```json.{.  "I
-000052f0: 4422 3a20 227b 6375 7272 5f69 7465 727d  D": "{curr_iter}
-00005300: 220a 7d0a 6060 600a 0a23 2323 2323 2320  ".}.```..###### 
-00005310: 5061 7261 6d65 7472 697a 6564 0a0a 5573  Parametrized..Us
-00005320: 6573 2061 2073 7065 6369 6669 6320 4d69  es a specific Mi
-00005330: 6d65 6f20 4d6f 6465 6c20 636f 6e74 6578  meo Model contex
-00005340: 7420 286d 6f64 656c 206e 616d 6520 7768  t (model name wh
-00005350: 656e 2060 636f 6e74 6578 7460 2069 7320  en `context` is 
-00005360: 6e6f 7420 636f 6e66 6967 7572 6564 292e  not configured).
-00005370: 0a0a 6060 606a 736f 6e0a 7b0a 2020 2250  ..```json.{.  "P
-00005380: 6172 656e 7422 3a20 7b0a 2020 2020 225f  arent": {.    "_
-00005390: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
-000053a0: 2020 2020 2022 5f6e 616d 6522 3a20 2263       "_name": "c
-000053b0: 7572 725f 6974 6572 222c 0a20 2020 2020  urr_iter",.     
-000053c0: 2022 636f 6e74 6578 7422 3a20 2253 6f6d   "context": "Som
-000053d0: 6545 6e74 6974 7922 0a20 2020 207d 0a20  eEntity".    }. 
-000053e0: 207d 0a7d 0a60 6060 0a0a 2323 2323 2320   }.}.```..##### 
-000053f0: 4b65 790a 0a47 656e 6572 6174 6573 2061  Key..Generates a
-00005400: 206b 6579 2075 6e69 7175 6520 6163 726f   key unique acro
-00005410: 7373 2061 6c6c 204d 696d 656f 204d 6f64  ss all Mimeo Mod
-00005420: 656c 7320 616e 6420 6265 696e 6720 7468  els and being th
-00005430: 6520 7361 6d65 2077 6974 6869 6e20 6120  e same within a 
-00005440: 7369 6e67 6c65 204d 696d 656f 204d 6f64  single Mimeo Mod
-00005450: 656c 2063 6f6e 7465 7874 2e0a 0a7c 2050  el context...| P
-00005460: 6172 616d 6574 6572 207c 2053 7570 706f  arameter | Suppo
-00005470: 7274 6564 2076 616c 7565 7320 7c20 2020  rted values |   
-00005480: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00005490: 6c74 2020 2020 2020 2020 2020 2020 2020  lt              
-000054a0: 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 3a7c   |.|:---------:|
-000054b0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-000054c0: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
-000054d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000054e0: 2d2d 2d2d 2d2d 3a7c 0a7c 2020 636f 6e74  ------:|.|  cont
-000054f0: 6578 7420 207c 2020 2020 2020 6073 7472  ext  |      `str
-00005500: 6020 2020 2020 2020 7c20 2020 2020 2020  `       |       
-00005510: 2020 6120 6375 7272 656e 7420 636f 6e74    a current cont
-00005520: 6578 7420 2020 2020 2020 2020 207c 0a7c  ext          |.|
-00005530: 2069 7465 7261 7469 6f6e 207c 2020 2020   iteration |    
-00005540: 2020 6069 6e74 6020 2020 2020 2020 7c20    `int`       | 
-00005550: 6120 6375 7272 656e 7420 6974 6572 6174  a current iterat
-00005560: 696f 6e20 6f66 2074 6865 2063 6f6e 7465  ion of the conte
-00005570: 7874 207c 0a0a 2323 2323 2323 2052 6177  xt |..###### Raw
-00005580: 0a0a 5573 6573 2061 206b 6579 2066 726f  ..Uses a key fro
-00005590: 6d20 7468 6520 6375 7272 656e 7420 636f  m the current co
-000055a0: 6e74 6578 7420 616e 6420 6974 6572 6174  ntext and iterat
-000055b0: 696f 6e2e 0a0a 6060 606a 736f 6e0a 7b0a  ion...```json.{.
-000055c0: 2020 2249 4422 3a20 227b 6b65 797d 220a    "ID": "{key}".
-000055d0: 7d0a 6060 600a 0a23 2323 2323 2320 5061  }.```..###### Pa
-000055e0: 7261 6d65 7472 697a 6564 0a0a 5573 6573  rametrized..Uses
-000055f0: 2061 206b 6579 2066 726f 6d20 7468 6520   a key from the 
-00005600: 7370 6563 6966 6963 2063 6f6e 7465 7874  specific context
-00005610: 2061 6e64 2069 7465 7261 7469 6f6e 2e20   and iteration. 
-00005620: 200a 5768 656e 2063 6f6e 7465 7874 2069   .When context i
-00005630: 7320 696e 6469 6361 7465 6420 616e 6420  s indicated and 
-00005640: 6974 6572 6174 696f 6e20 6973 206e 6f74  iteration is not
-00005650: 2c20 7468 656e 2074 6865 2063 7572 7265  , then the curre
-00005660: 6e74 2069 7465 7261 7469 6f6e 202a 2a6f  nt iteration **o
-00005670: 6620 7468 6520 696e 6469 6361 7465 6420  f the indicated 
-00005680: 636f 6e74 6578 742a 2a20 6973 2062 6569  context** is bei
-00005690: 6e67 2075 7365 642e 0a0a 6060 606a 736f  ng used...```jso
-000056a0: 6e0a 7b0a 2020 2253 6f6d 6545 6e74 6974  n.{.  "SomeEntit
-000056b0: 7932 223a 207b 0a20 2020 2022 5f6d 696d  y2": {.    "_mim
-000056c0: 656f 5f75 7469 6c22 3a20 7b0a 2020 2020  eo_util": {.    
-000056d0: 2020 225f 6e61 6d65 223a 2022 6b65 7922    "_name": "key"
-000056e0: 2c0a 2020 2020 2020 2263 6f6e 7465 7874  ,.      "context
-000056f0: 223a 2022 536f 6d65 456e 7469 7479 222c  ": "SomeEntity",
-00005700: 0a20 2020 2020 2022 6974 6572 6174 696f  .      "iteratio
-00005710: 6e22 3a20 227b 6375 7272 5f69 7465 727d  n": "{curr_iter}
-00005720: 220a 2020 2020 7d0a 2020 7d0a 7d0a 6060  ".    }.  }.}.``
-00005730: 600a 0a23 2323 2323 2043 6974 790a 0a47  `..##### City..G
-00005740: 656e 6572 6174 6573 2061 2063 6974 7920  enerates a city 
-00005750: 6e61 6d65 2e0a 0a7c 2050 6172 616d 6574  name...| Paramet
-00005760: 6572 207c 2053 7570 706f 7274 6564 2076  er | Supported v
-00005770: 616c 7565 7320 7c20 4465 6661 756c 7420  alues | Default 
-00005780: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a  |.|:---------:|:
-00005790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000057a0: 3a7c 3a2d 2d2d 2d2d 2d2d 3a7c 0a7c 2020  :|:-------:|.|  
-000057b0: 756e 6971 7565 2020 207c 2020 2020 2020  unique   |      
-000057c0: 6062 6f6f 6c60 2020 2020 2020 7c20 6054  `bool`      | `T
-000057d0: 7275 6560 2020 7c0a 7c20 2063 6f75 6e74  rue`  |.|  count
-000057e0: 7279 2020 7c20 2020 2020 2060 7374 7260  ry  |      `str`
-000057f0: 2020 2020 2020 207c 2060 4e6f 6e65 6020         | `None` 
-00005800: 207c 0a0a 2323 2323 2323 2052 6177 0a0a   |..###### Raw..
-00005810: 4279 2064 6566 6175 6c74 2063 6974 7920  By default city 
-00005820: 6e61 6d65 7320 7769 6c6c 2062 6520 756e  names will be un
-00005830: 6971 7565 2061 6372 6f73 7320 6120 4d69  ique across a Mi
-00005840: 6d65 6f20 436f 6e74 6578 742e 0a0a 6060  meo Context...``
-00005850: 606a 736f 6e0a 7b0a 2020 2243 6974 7922  `json.{.  "City"
-00005860: 3a20 227b 6369 7479 7d22 0a7d 0a60 6060  : "{city}".}.```
-00005870: 0a0a 2323 2323 2323 2050 6172 616d 6574  ..###### Paramet
-00005880: 7269 7a65 640a 0a55 7365 7320 636f 756e  rized..Uses coun
-00005890: 7472 7920 286e 616d 652c 2069 736f 322c  try (name, iso2,
-000058a0: 2069 736f 3329 2061 6e64 2060 756e 6971   iso3) and `uniq
-000058b0: 7565 6020 666c 6167 2074 6f20 6765 6e65  ue` flag to gene
-000058c0: 7261 7465 2061 2063 6974 7920 6e61 6d65  rate a city name
-000058d0: 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  ...```json.{.  "
-000058e0: 4369 7479 5769 7468 4475 706c 6963 6174  CityWithDuplicat
-000058f0: 6573 223a 207b 0a20 2020 2022 5f6d 696d  es": {.    "_mim
-00005900: 656f 5f75 7469 6c22 3a20 7b0a 2020 2020  eo_util": {.    
-00005910: 2020 225f 6e61 6d65 223a 2022 6369 7479    "_name": "city
-00005920: 222c 0a20 2020 2020 2022 756e 6971 7565  ",.      "unique
-00005930: 223a 2066 616c 7365 0a20 2020 207d 0a20  ": false.    }. 
-00005940: 207d 2c0a 2020 2243 6974 794f 6643 6f75   },.  "CityOfCou
-00005950: 6e74 7279 4e61 6d65 223a 207b 0a20 2020  ntryName": {.   
-00005960: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
-00005970: 7b0a 2020 2020 2020 225f 6e61 6d65 223a  {.      "_name":
-00005980: 2022 6369 7479 222c 0a20 2020 2020 2022   "city",.      "
-00005990: 636f 756e 7472 7922 3a20 2255 6e69 7465  country": "Unite
-000059a0: 6420 4b69 6e67 646f 6d22 0a20 2020 207d  d Kingdom".    }
-000059b0: 0a20 207d 2c0a 2020 2243 6974 794f 6643  .  },.  "CityOfC
-000059c0: 6f75 6e74 7279 4953 4f32 223a 207b 0a20  ountryISO2": {. 
-000059d0: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
-000059e0: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
-000059f0: 223a 2022 6369 7479 222c 0a20 2020 2020  ": "city",.     
-00005a00: 2022 636f 756e 7472 7922 3a20 2247 4222   "country": "GB"
-00005a10: 0a20 2020 207d 0a20 207d 2c0a 2020 2243  .    }.  },.  "C
-00005a20: 6974 794f 6643 6f75 6e74 7279 4953 4f33  ityOfCountryISO3
-00005a30: 223a 207b 0a20 2020 2022 5f6d 696d 656f  ": {.    "_mimeo
-00005a40: 5f75 7469 6c22 3a20 7b0a 2020 2020 2020  _util": {.      
-00005a50: 225f 6e61 6d65 223a 2022 6369 7479 222c  "_name": "city",
-00005a60: 0a20 2020 2020 2022 636f 756e 7472 7922  .      "country"
-00005a70: 3a20 2247 4252 220a 2020 2020 7d0a 2020  : "GBR".    }.  
-00005a80: 7d2c 0a20 2022 4369 7479 4f66 436f 756e  },.  "CityOfCoun
-00005a90: 7472 7957 6974 6844 7570 6c69 6361 7465  tryWithDuplicate
-00005aa0: 7322 3a20 7b0a 2020 2020 225f 6d69 6d65  s": {.    "_mime
-00005ab0: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
-00005ac0: 2022 5f6e 616d 6522 3a20 2263 6974 7922   "_name": "city"
-00005ad0: 2c0a 2020 2020 2020 2263 6f75 6e74 7279  ,.      "country
-00005ae0: 223a 2022 556e 6974 6564 204b 696e 6764  ": "United Kingd
-00005af0: 6f6d 222c 0a20 2020 2020 2022 756e 6971  om",.      "uniq
-00005b00: 7565 223a 2066 616c 7365 0a20 2020 207d  ue": false.    }
-00005b10: 0a20 207d 0a7d 0a60 6060 0a0a 2323 2323  .  }.}.```..####
-00005b20: 2320 436f 756e 7472 790a 0a47 656e 6572  # Country..Gener
-00005b30: 6174 6573 2061 2063 6f75 6e74 7279 206e  ates a country n
-00005b40: 616d 6520 2862 7920 6465 6661 756c 7429  ame (by default)
-00005b50: 2c20 6973 6f32 206f 7220 6973 6f33 2e0a  , iso2 or iso3..
-00005b60: 0a7c 2050 6172 616d 6574 6572 207c 2020  .| Parameter |  
-00005b70: 2020 2020 2053 7570 706f 7274 6564 2076       Supported v
-00005b80: 616c 7565 7320 2020 2020 2020 7c20 4465  alues       | De
-00005b90: 6661 756c 7420 207c 0a7c 3a2d 2d2d 2d2d  fault  |.|:-----
-00005ba0: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00005bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005bc0: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 3a7c  ---:|:--------:|
-00005bd0: 0a7c 2020 756e 6971 7565 2020 207c 2020  .|  unique   |  
-00005be0: 2020 2020 2020 2020 2020 6062 6f6f 6c60            `bool`
-00005bf0: 2020 2020 2020 2020 2020 2020 7c20 2060              |  `
-00005c00: 5472 7565 6020 207c 0a7c 2020 2076 616c  True`  |.|   val
-00005c10: 7565 2020 207c 2060 226e 616d 6522 602c  ue   | `"name"`,
-00005c20: 2060 2269 736f 3322 602c 2060 2269 736f   `"iso3"`, `"iso
-00005c30: 3222 6020 7c20 6022 6e61 6d65 2260 207c  2"` | `"name"` |
-00005c40: 0a7c 2020 636f 756e 7472 7920 207c 2020  .|  country  |  
-00005c50: 2020 2020 2020 2020 2020 6073 7472 6020            `str` 
-00005c60: 2020 2020 2020 2020 2020 2020 7c20 2060              |  `
-00005c70: 4e6f 6e65 6020 207c 0a0a 2323 2323 2323  None`  |..######
-00005c80: 2052 6177 0a0a 4279 2064 6566 6175 6c74   Raw..By default
-00005c90: 2063 6f75 6e74 7279 206e 616d 6573 2077   country names w
-00005ca0: 696c 6c20 6265 2075 6e69 7175 6520 6163  ill be unique ac
-00005cb0: 726f 7373 2061 204d 696d 656f 2043 6f6e  ross a Mimeo Con
-00005cc0: 7465 7874 2e0a 0a60 6060 6a73 6f6e 0a7b  text...```json.{
-00005cd0: 0a20 2022 436f 756e 7472 7922 3a20 227b  .  "Country": "{
-00005ce0: 636f 756e 7472 797d 220a 7d0a 6060 600a  country}".}.```.
-00005cf0: 0a23 2323 2323 2320 5061 7261 6d65 7472  .###### Parametr
-00005d00: 697a 6564 0a0a 4974 2063 616e 2067 656e  ized..It can gen
-00005d10: 6572 6174 653a 0a2d 2063 6f75 6e74 7279  erate:.- country
-00005d20: 2069 736f 3320 6f72 2069 736f 2032 2069   iso3 or iso 2 i
-00005d30: 6e73 7465 6164 206f 6620 6e61 6d65 0a2d  nstead of name.-
-00005d40: 2063 6f75 6e74 7279 2077 6974 6820 6475   country with du
-00005d50: 706c 6963 6174 6573 0a2d 2063 6f75 6e74  plicates.- count
-00005d60: 7279 206e 616d 6520 666f 7220 6120 7072  ry name for a pr
-00005d70: 6f76 6964 6564 2069 736f 3320 6f72 2069  ovided iso3 or i
-00005d80: 736f 320a 2d20 636f 756e 7472 7920 6973  so2.- country is
-00005d90: 6f32 2066 6f72 2061 2070 726f 7669 6465  o2 for a provide
-00005da0: 6420 6e61 6d65 206f 7220 6973 6f33 0a2d  d name or iso3.-
-00005db0: 2063 6f75 6e74 7279 2069 736f 3320 666f   country iso3 fo
-00005dc0: 7220 6120 7072 6f76 6964 6564 206e 616d  r a provided nam
-00005dd0: 6520 6f72 2069 736f 320a 0a57 6865 6e20  e or iso2..When 
-00005de0: 7468 6520 6063 6f75 6e74 7279 6020 7061  the `country` pa
-00005df0: 7261 6d20 6973 2070 726f 7669 6465 6420  ram is provided 
-00005e00: 7468 656e 2074 6865 2060 756e 6971 7565  then the `unique
-00005e10: 6020 666c 6167 2069 7320 6967 6e6f 7265  ` flag is ignore
-00005e20: 642e 0a0a 6060 606a 736f 6e0a 7b0a 2020  d...```json.{.  
-00005e30: 2243 6f75 6e74 7279 4e61 6d65 5769 7468  "CountryNameWith
-00005e40: 4475 706c 6963 6174 6573 223a 207b 0a20  Duplicates": {. 
-00005e50: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
-00005e60: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
-00005e70: 223a 2022 636f 756e 7472 7922 2c0a 2020  ": "country",.  
-00005e80: 2020 2020 2275 6e69 7175 6522 3a20 6661      "unique": fa
-00005e90: 6c73 650a 2020 2020 7d0a 2020 7d2c 0a20  lse.    }.  },. 
-00005ea0: 2022 436f 756e 7472 7949 534f 3222 3a20   "CountryISO2": 
-00005eb0: 7b0a 2020 2020 225f 6d69 6d65 6f5f 7574  {.    "_mimeo_ut
-00005ec0: 696c 223a 207b 0a20 2020 2020 2022 5f6e  il": {.      "_n
-00005ed0: 616d 6522 3a20 2263 6f75 6e74 7279 222c  ame": "country",
-00005ee0: 0a20 2020 2020 2022 7661 6c75 6522 3a20  .      "value": 
-00005ef0: 2269 736f 3222 0a20 2020 207d 0a20 207d  "iso2".    }.  }
-00005f00: 2c0a 2020 2243 6f75 6e74 7279 4953 4f33  ,.  "CountryISO3
-00005f10: 223a 207b 0a20 2020 2022 5f6d 696d 656f  ": {.    "_mimeo
-00005f20: 5f75 7469 6c22 3a20 7b0a 2020 2020 2020  _util": {.      
-00005f30: 225f 6e61 6d65 223a 2022 636f 756e 7472  "_name": "countr
-00005f40: 7922 2c0a 2020 2020 2020 2276 616c 7565  y",.      "value
-00005f50: 223a 2022 6973 6f33 220a 2020 2020 7d0a  ": "iso3".    }.
-00005f60: 2020 7d2c 0a20 2022 436f 756e 7472 794e    },.  "CountryN
-00005f70: 616d 6546 6f72 4953 4f33 223a 207b 0a20  ameForISO3": {. 
-00005f80: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
-00005f90: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
-00005fa0: 223a 2022 636f 756e 7472 7922 2c0a 2020  ": "country",.  
-00005fb0: 2020 2020 2263 6f75 6e74 7279 223a 2022      "country": "
-00005fc0: 4742 5222 0a20 2020 207d 0a20 207d 2c0a  GBR".    }.  },.
-00005fd0: 2020 2243 6f75 6e74 7279 4953 4f32 466f    "CountryISO2Fo
-00005fe0: 724e 616d 6522 3a20 7b0a 2020 2020 225f  rName": {.    "_
-00005ff0: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
-00006000: 2020 2020 2022 5f6e 616d 6522 3a20 2263       "_name": "c
-00006010: 6f75 6e74 7279 222c 0a20 2020 2020 2022  ountry",.      "
-00006020: 7661 6c75 6522 3a20 2269 736f 3222 2c0a  value": "iso2",.
-00006030: 2020 2020 2020 2263 6f75 6e74 7279 223a        "country":
-00006040: 2022 556e 6974 6564 204b 696e 6764 6f6d   "United Kingdom
-00006050: 220a 2020 2020 7d0a 2020 7d0a 7d0a 6060  ".    }.  }.}.``
-00006060: 600a 0a23 2323 2323 2043 7572 7265 6e63  `..##### Currenc
-00006070: 790a 0a47 656e 6572 6174 6573 2061 2063  y..Generates a c
-00006080: 7572 7265 6e63 7920 636f 6465 2028 6279  urrency code (by
-00006090: 2064 6566 6175 6c74 2920 6f72 206e 616d   default) or nam
-000060a0: 652e 0a0a 7c20 5061 7261 6d65 7465 7220  e...| Parameter 
-000060b0: 7c20 2053 7570 706f 7274 6564 2076 616c  |  Supported val
-000060c0: 7565 7320 207c 2044 6566 6175 6c74 2020  ues  | Default  
-000060d0: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a  |.|:---------:|:
-000060e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000060f0: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d3a 7c0a  --:|:--------:|.
-00006100: 7c20 2075 6e69 7175 6520 2020 7c20 2020  |  unique   |   
-00006110: 2020 2020 6062 6f6f 6c60 2020 2020 2020      `bool`      
-00006120: 207c 2060 4661 6c73 6560 2020 7c0a 7c20   | `False`  |.| 
-00006130: 2020 7661 6c75 6520 2020 7c20 6022 636f    value   | `"co
-00006140: 6465 2260 2c20 6022 6e61 6d65 2260 207c  de"`, `"name"` |
-00006150: 2060 2263 6f64 6522 6020 7c0a 7c20 2063   `"code"` |.|  c
-00006160: 6f75 6e74 7279 2020 7c20 2020 2020 2020  ountry  |       
-00006170: 6073 7472 6020 2020 2020 2020 207c 2020  `str`        |  
-00006180: 604e 6f6e 6560 2020 7c0a 0a23 2323 2323  `None`  |..#####
-00006190: 2320 5261 770a 0a42 7920 6465 6661 756c  # Raw..By defaul
-000061a0: 7420 6369 7479 206e 616d 6573 2077 696c  t city names wil
-000061b0: 6c20 5f4e 4f54 5f20 6265 2075 6e69 7175  l _NOT_ be uniqu
-000061c0: 6520 6163 726f 7373 2061 204d 696d 656f  e across a Mimeo
-000061d0: 2043 6f6e 7465 7874 2e0a 0a60 6060 6a73   Context...```js
-000061e0: 6f6e 0a7b 0a20 2022 4375 7272 656e 6379  on.{.  "Currency
-000061f0: 223a 2022 7b63 7572 7265 6e63 797d 220a  ": "{currency}".
-00006200: 7d0a 6060 600a 0a23 2323 2323 2320 5061  }.```..###### Pa
-00006210: 7261 6d65 7472 697a 6564 0a0a 4974 2063  rametrized..It c
-00006220: 616e 2067 656e 6572 6174 653a 0a2d 2075  an generate:.- u
-00006230: 6e69 7175 6520 6375 7272 656e 6369 6573  nique currencies
-00006240: 0a2d 2063 7572 7265 6e63 7920 6e61 6d65  .- currency name
-00006250: 2069 6e73 7465 6164 206f 6620 636f 6465   instead of code
-00006260: 0a2d 2063 7572 7265 6e63 7920 636f 6465  .- currency code
-00006270: 206f 7220 6e61 6d65 206f 6620 6120 7370   or name of a sp
-00006280: 6563 6966 6963 2063 6f75 6e74 7279 2028  ecific country (
-00006290: 7573 696e 6720 6973 6f33 2c20 6973 6f32  using iso3, iso2
-000062a0: 206f 7220 6e61 6d65 290a 0a57 6865 6e20   or name)..When 
-000062b0: 7468 6520 6063 6f75 6e74 7279 6020 7061  the `country` pa
-000062c0: 7261 6d20 6973 2070 726f 7669 6465 6420  ram is provided 
-000062d0: 7468 656e 2074 6865 2060 756e 6971 7565  then the `unique
-000062e0: 6020 666c 6167 2069 7320 6967 6e6f 7265  ` flag is ignore
-000062f0: 642e 0a0a 6060 606a 736f 6e0a 7b0a 2020  d...```json.{.  
-00006300: 2255 6e69 7175 6543 7572 7265 6e63 7943  "UniqueCurrencyC
-00006310: 6f64 6522 3a20 7b0a 2020 2020 225f 6d69  ode": {.    "_mi
-00006320: 6d65 6f5f 7574 696c 223a 207b 0a20 2020  meo_util": {.   
-00006330: 2020 2022 5f6e 616d 6522 3a20 2263 7572     "_name": "cur
-00006340: 7265 6e63 7922 2c0a 2020 2020 2020 2275  rency",.      "u
-00006350: 6e69 7175 6522 3a20 7472 7565 0a20 2020  nique": true.   
-00006360: 207d 0a20 207d 2c0a 2020 2243 7572 7265   }.  },.  "Curre
-00006370: 6e63 794e 616d 6522 3a20 7b0a 2020 2020  ncyName": {.    
-00006380: 225f 6d69 6d65 6f5f 7574 696c 223a 207b  "_mimeo_util": {
-00006390: 0a20 2020 2020 2022 5f6e 616d 6522 3a20  .      "_name": 
-000063a0: 2263 7572 7265 6e63 7922 2c0a 2020 2020  "currency",.    
-000063b0: 2020 2276 616c 7565 223a 2022 6e61 6d65    "value": "name
-000063c0: 220a 2020 2020 7d0a 2020 7d2c 0a20 2022  ".    }.  },.  "
-000063d0: 4375 7272 656e 6379 436f 6465 466f 7243  CurrencyCodeForC
-000063e0: 6f75 6e74 7279 4953 4f33 223a 207b 0a20  ountryISO3": {. 
-000063f0: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
-00006400: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
-00006410: 223a 2022 6375 7272 656e 6379 222c 0a20  ": "currency",. 
-00006420: 2020 2020 2022 636f 756e 7472 7922 3a20       "country": 
-00006430: 2247 4252 220a 2020 2020 7d0a 2020 7d2c  "GBR".    }.  },
-00006440: 0a20 2022 4375 7272 656e 6379 4e61 6d65  .  "CurrencyName
-00006450: 466f 7243 6f75 6e74 7279 4953 4f32 223a  ForCountryISO2":
-00006460: 207b 0a20 2020 2022 5f6d 696d 656f 5f75   {.    "_mimeo_u
-00006470: 7469 6c22 3a20 7b0a 2020 2020 2020 225f  til": {.      "_
-00006480: 6e61 6d65 223a 2022 6375 7272 656e 6379  name": "currency
-00006490: 222c 0a20 2020 2020 2022 7661 6c75 6522  ",.      "value"
-000064a0: 3a20 226e 616d 6522 2c0a 2020 2020 2020  : "name",.      
-000064b0: 2263 6f75 6e74 7279 223a 2022 4742 220a  "country": "GB".
-000064c0: 2020 2020 7d0a 2020 7d2c 0a20 2022 4375      }.  },.  "Cu
-000064d0: 7272 656e 6379 4e61 6d65 466f 7243 6f75  rrencyNameForCou
-000064e0: 6e74 7279 4e61 6d65 223a 207b 0a20 2020  ntryName": {.   
-000064f0: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
-00006500: 7b0a 2020 2020 2020 225f 6e61 6d65 223a  {.      "_name":
-00006510: 2022 6375 7272 656e 6379 222c 0a20 2020   "currency",.   
-00006520: 2020 2022 7661 6c75 6522 3a20 226e 616d     "value": "nam
-00006530: 6522 2c0a 2020 2020 2020 2263 6f75 6e74  e",.      "count
-00006540: 7279 223a 2022 556e 6974 6564 204b 696e  ry": "United Kin
-00006550: 6764 6f6d 220a 2020 2020 7d0a 2020 7d0a  gdom".    }.  }.
-00006560: 7d0a 6060 600a 0a23 2323 2323 2046 6972  }.```..##### Fir
-00006570: 7374 204e 616d 650a 0a47 656e 6572 6174  st Name..Generat
-00006580: 6573 2061 2066 6972 7374 206e 616d 652e  es a first name.
-00006590: 0a0a 7c20 5061 7261 6d65 7465 7220 7c20  ..| Parameter | 
-000065a0: 2020 2020 2053 7570 706f 7274 6564 2076       Supported v
-000065b0: 616c 7565 7320 2020 2020 207c 2044 6566  alues      | Def
-000065c0: 6175 6c74 2020 7c0a 7c3a 2d2d 2d2d 2d2d  ault  |.|:------
-000065d0: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
-000065e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000065f0: 3a7c 3a2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20  :|:--------:|.| 
-00006600: 2075 6e69 7175 6520 2020 7c20 2020 2020   unique   |     
-00006610: 2020 2020 2020 6062 6f6f 6c60 2020 2020        `bool`    
-00006620: 2020 2020 2020 207c 2020 6054 7275 6560         |  `True`
-00006630: 2020 7c0a 7c20 2020 2073 6578 2020 2020    |.|    sex    
-00006640: 7c20 604d 602c 2060 4d61 6c65 602c 2060  | `M`, `Male`, `
-00006650: 4660 2c20 6046 656d 616c 6560 207c 2020  F`, `Female` |  
-00006660: 604e 6f6e 6560 2020 7c0a 0a23 2323 2323  `None`  |..#####
-00006670: 2320 5261 770a 0a42 7920 6465 6661 756c  # Raw..By defaul
-00006680: 7420 6669 7273 7420 6e61 6d65 7320 7769  t first names wi
-00006690: 6c6c 2062 6520 756e 6971 7565 2061 6372  ll be unique acr
-000066a0: 6f73 7320 6120 4d69 6d65 6f20 436f 6e74  oss a Mimeo Cont
-000066b0: 6578 742e 0a0a 6060 606a 736f 6e0a 7b0a  ext...```json.{.
-000066c0: 2020 2246 6972 7374 4e61 6d65 223a 2022    "FirstName": "
-000066d0: 7b66 6972 7374 5f6e 616d 657d 220a 7d0a  {first_name}".}.
-000066e0: 6060 600a 0a23 2323 2323 2320 5061 7261  ```..###### Para
-000066f0: 6d65 7472 697a 6564 0a0a 5573 6573 2073  metrized..Uses s
-00006700: 6578 2028 604d 6020 2f20 604d 616c 6560  ex (`M` / `Male`
-00006710: 202f 2060 4660 202f 2060 4665 6d61 6c65   / `F` / `Female
-00006720: 6029 2061 6e64 2060 756e 6971 7565 6020  `) and `unique` 
-00006730: 666c 6167 2074 6f20 6765 6e65 7261 7465  flag to generate
-00006740: 2061 2066 6972 7374 206e 616d 652e 0a0a   a first name...
-00006750: 6060 606a 736f 6e0a 7b0a 2020 2246 6972  ```json.{.  "Fir
-00006760: 7374 4e61 6d65 5769 7468 4475 706c 6963  stNameWithDuplic
-00006770: 6174 6573 223a 207b 0a20 2020 2022 5f6d  ates": {.    "_m
-00006780: 696d 656f 5f75 7469 6c22 3a20 7b0a 2020  imeo_util": {.  
-00006790: 2020 2020 225f 6e61 6d65 223a 2022 6669      "_name": "fi
-000067a0: 7273 745f 6e61 6d65 222c 0a20 2020 2020  rst_name",.     
-000067b0: 2022 756e 6971 7565 223a 2066 616c 7365   "unique": false
-000067c0: 0a20 2020 207d 0a20 207d 2c0a 2020 224d  .    }.  },.  "M
-000067d0: 616c 6546 6972 7374 4e61 6d65 223a 207b  aleFirstName": {
-000067e0: 0a20 2020 2022 5f6d 696d 656f 5f75 7469  .    "_mimeo_uti
-000067f0: 6c22 3a20 7b0a 2020 2020 2020 225f 6e61  l": {.      "_na
-00006800: 6d65 223a 2022 6669 7273 745f 6e61 6d65  me": "first_name
-00006810: 222c 0a20 2020 2020 2022 7365 7822 3a20  ",.      "sex": 
-00006820: 224d 220a 2020 2020 7d0a 2020 7d2c 0a20  "M".    }.  },. 
-00006830: 2022 4665 6d61 6c65 4669 7273 744e 616d   "FemaleFirstNam
-00006840: 6522 3a20 7b0a 2020 2020 225f 6d69 6d65  e": {.    "_mime
-00006850: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
-00006860: 2022 5f6e 616d 6522 3a20 2266 6972 7374   "_name": "first
-00006870: 5f6e 616d 6522 2c0a 2020 2020 2020 2273  _name",.      "s
-00006880: 6578 223a 2022 4622 0a20 2020 207d 0a20  ex": "F".    }. 
-00006890: 207d 2c0a 2020 224d 616c 6546 6972 7374   },.  "MaleFirst
-000068a0: 4e61 6d65 5769 7468 4475 706c 6963 6174  NameWithDuplicat
-000068b0: 6573 223a 207b 0a20 2020 2022 5f6d 696d  es": {.    "_mim
-000068c0: 656f 5f75 7469 6c22 3a20 7b0a 2020 2020  eo_util": {.    
-000068d0: 2020 225f 6e61 6d65 223a 2022 6669 7273    "_name": "firs
-000068e0: 745f 6e61 6d65 222c 0a20 2020 2020 2022  t_name",.      "
-000068f0: 7365 7822 3a20 224d 222c 0a20 2020 2020  sex": "M",.     
-00006900: 2022 756e 6971 7565 223a 2066 616c 7365   "unique": false
-00006910: 0a20 2020 207d 0a20 207d 0a7d 0a60 6060  .    }.  }.}.```
-00006920: 0a0a 2323 2323 2320 4c61 7374 204e 616d  ..##### Last Nam
-00006930: 650a 0a47 656e 6572 6174 6573 2061 206c  e..Generates a l
-00006940: 6173 7420 6e61 6d65 2e0a 0a7c 2050 6172  ast name...| Par
-00006950: 616d 6574 6572 207c 2053 7570 706f 7274  ameter | Support
-00006960: 6564 2076 616c 7565 7320 7c20 4465 6661  ed values | Defa
-00006970: 756c 7420 207c 0a7c 3a2d 2d2d 2d2d 2d2d  ult  |.|:-------
-00006980: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
-00006990: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-000069a0: 3a7c 0a7c 2020 756e 6971 7565 2020 207c  :|.|  unique   |
-000069b0: 2020 2020 2020 6062 6f6f 6c60 2020 2020        `bool`    
-000069c0: 2020 7c20 2060 5472 7565 6020 207c 0a0a    |  `True`  |..
-000069d0: 2323 2323 2323 2052 6177 0a0a 4279 2064  ###### Raw..By d
-000069e0: 6566 6175 6c74 206c 6173 7420 6e61 6d65  efault last name
-000069f0: 7320 7769 6c6c 2062 6520 756e 6971 7565  s will be unique
-00006a00: 2061 6372 6f73 7320 6120 4d69 6d65 6f20   across a Mimeo 
-00006a10: 436f 6e74 6578 742e 0a0a 6060 606a 736f  Context...```jso
-00006a20: 6e0a 7b0a 2020 224c 6173 744e 616d 6522  n.{.  "LastName"
-00006a30: 3a20 227b 6c61 7374 5f6e 616d 657d 220a  : "{last_name}".
-00006a40: 7d0a 6060 600a 0a23 2323 2323 2320 5061  }.```..###### Pa
-00006a50: 7261 6d65 7472 697a 6564 0a0a 5573 6573  rametrized..Uses
-00006a60: 2060 756e 6971 7565 6020 666c 6167 2074   `unique` flag t
-00006a70: 6f20 6765 6e65 7261 7465 2061 206c 6173  o generate a las
-00006a80: 7420 6e61 6d65 2e0a 0a60 6060 6a73 6f6e  t name...```json
-00006a90: 0a7b 0a20 2022 4c61 7374 4e61 6d65 5769  .{.  "LastNameWi
-00006aa0: 7468 4475 706c 6963 6174 6573 223a 207b  thDuplicates": {
-00006ab0: 0a20 2020 2022 5f6d 696d 656f 5f75 7469  .    "_mimeo_uti
-00006ac0: 6c22 3a20 7b0a 2020 2020 2020 225f 6e61  l": {.      "_na
-00006ad0: 6d65 223a 2022 6c61 7374 5f6e 616d 6522  me": "last_name"
-00006ae0: 2c0a 2020 2020 2020 2275 6e69 7175 6522  ,.      "unique"
-00006af0: 3a20 6661 6c73 650a 2020 2020 7d0a 2020  : false.    }.  
-00006b00: 7d0a 7d0a 6060 600a 0a0a 2323 204c 6963  }.}.```...## Lic
-00006b10: 656e 7365 0a0a 4d49 540a 0a0a 2323 2041  ense..MIT...## A
-00006b20: 7574 686f 7273 0a0a 2d20 5b40 546f 6d61  uthors..- [@Toma
-00006b30: 737a 416e 696f 6c6f 7773 6b69 5d28 6874  szAniolowski](ht
-00006b40: 7470 733a 2f2f 7777 772e 6769 7468 7562  tps://www.github
-00006b50: 2e63 6f6d 2f54 6f6d 6173 7a41 6e69 6f6c  .com/TomaszAniol
-00006b60: 6f77 736b 6929 0a0a 0a23 2320 4163 6b6e  owski)...## Ackn
-00006b70: 6f77 6c65 6467 656d 656e 7473 0a0a 202d  owledgements.. -
-00006b80: 205b 5369 6d70 6c65 4d61 7073 2e63 6f6d   [SimpleMaps.com
-00006b90: 5d28 6874 7470 733a 2f2f 7369 6d70 6c65  ](https://simple
-00006ba0: 6d61 7073 2e63 6f6d 2f64 6174 612f 776f  maps.com/data/wo
-00006bb0: 726c 642d 6369 7469 6573 2920 2843 6974  rld-cities) (Cit
-00006bc0: 6965 7320 2620 636f 756e 7472 6965 7320  ies & countries 
-00006bd0: 6461 7461 290a 202d 205b 4068 6164 6c65  data). - [@hadle
-00006be0: 792f 6461 7461 2d62 6162 792d 6e61 6d65  y/data-baby-name
-00006bf0: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00006c00: 622e 636f 6d2f 6861 646c 6579 2f64 6174  b.com/hadley/dat
-00006c10: 612d 6261 6279 2d6e 616d 6573 2f29 2028  a-baby-names/) (
-00006c20: 466f 7265 6e61 6d65 7320 6461 7461 290a  Forenames data).
-00006c30: 202d 205b 4066 6976 6574 6869 7274 7965   - [@fivethirtye
-00006c40: 6967 682f 6461 7461 2f6d 6f73 742d 636f  igh/data/most-co
-00006c50: 6d6d 6f6e 2d6e 616d 655d 2868 7474 7073  mmon-name](https
-00006c60: 3a2f 2f67 6974 6875 622e 636f 6d2f 6669  ://github.com/fi
-00006c70: 7665 7468 6972 7479 6569 6768 742f 6461  vethirtyeight/da
-00006c80: 7461 2f74 7265 652f 6d61 7374 6572 2f6d  ta/tree/master/m
-00006c90: 6f73 742d 636f 6d6d 6f6e 2d6e 616d 6529  ost-common-name)
-00006ca0: 2028 5375 726e 616d 6573 2064 6174 6129   (Surnames data)
-00006cb0: 0a0a                                     ..
+00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fb0: 2020 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d     |.|:---------
+00001fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001fd0: 7c3a 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d  |:--------:|:---
+00001fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+00001ff0: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
+00002000: 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d  ----------:|:---
+00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c2d 2d2d  -----------:|---
+00002020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000020a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000020b0: 2d2d 2d2d 2d2d 7c0a 7c20 606f 7574 7075  ------|.| `outpu
+000020c0: 7460 2020 2020 2020 2020 2020 2020 2020  t`              
+000020d0: 2020 207c 2020 436f 6e66 6967 2020 7c20     |  Config  | 
+000020e0: 2020 2020 2020 203a 783a 2020 2020 2020         :x:      
+000020f0: 2020 207c 2020 2020 2020 2020 2020 6f62     |          ob
+00002100: 6a65 6374 2020 2020 2020 2020 2020 7c20  ject          | 
+00002110: 2020 2020 202d 2d2d 2020 2020 2020 207c       ---       |
+00002120: 2044 6566 696e 6573 206f 7574 7075 7420   Defines output 
+00002130: 6465 7461 696c 7320 6f6e 2068 6f77 2069  details on how i
+00002140: 7420 7769 6c6c 2062 6520 636f 6e73 756d  t will be consum
+00002150: 6564 2020 2020 2020 2020 2020 2020 2020  ed              
+00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021b0: 2020 2020 2020 2020 207c 0a7c 2060 6f75           |.| `ou
+000021c0: 7470 7574 2f64 6972 6563 7469 6f6e 6020  tput/direction` 
+000021d0: 2020 2020 2020 7c20 2043 6f6e 6669 6720        |  Config 
+000021e0: 207c 2020 2020 2020 2020 3a78 3a20 2020   |        :x:   
+000021f0: 2020 2020 2020 7c20 6066 696c 6560 2c20        | `file`, 
+00002200: 6073 7464 6f75 7460 2c20 6068 7474 7060  `stdout`, `http`
+00002210: 207c 2020 2020 2060 6669 6c65 6020 2020   |     `file`   
+00002220: 2020 7c20 4465 6669 6e65 7320 686f 7720    | Defines how 
+00002230: 6f75 7470 7574 2077 696c 6c20 6265 2063  output will be c
+00002240: 6f6e 7375 6d65 6420 2020 2020 2020 2020  onsumed         
+00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022b0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000022c0: 606f 7574 7075 742f 666f 726d 6174 6020  `output/format` 
+000022d0: 2020 2020 2020 2020 207c 2020 436f 6e66           |  Conf
+000022e0: 6967 2020 7c20 2020 2020 2020 203a 783a  ig  |        :x:
+000022f0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00002300: 6078 6d6c 602c 2060 6a73 6f6e 6020 2020  `xml`, `json`   
+00002310: 2020 2020 7c20 2020 2020 6078 6d6c 6020      |     `xml` 
+00002320: 2020 2020 207c 2044 6566 696e 6573 206f       | Defines o
+00002330: 7574 7075 7420 6461 7461 2066 6f72 6d61  utput data forma
+00002340: 7420 2020 2020 2020 2020 2020 2020 2020  t               
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000023c0: 0a7c 2060 6f75 7470 7574 2f69 6e64 656e  .| `output/inden
+000023d0: 7460 2020 2020 2020 2020 2020 7c20 2043  t`          |  C
+000023e0: 6f6e 6669 6720 207c 2020 2020 2020 2020  onfig  |        
+000023f0: 3a78 3a20 2020 2020 2020 2020 7c20 2020  :x:         |   
+00002400: 2020 2020 2020 696e 7465 6765 7220 2020        integer   
+00002410: 2020 2020 2020 207c 2020 2020 2060 6e75         |     `nu
+00002420: 6c6c 6020 2020 2020 7c20 4465 6669 6e65  ll`     | Define
+00002430: 7320 696e 6465 6e74 2061 7070 6c69 6564  s indent applied
+00002440: 2069 6e20 6f75 7470 7574 2064 6174 6120   in output data 
+00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 7c0a 7c20 606f 7574 7075 742f 786d    |.| `output/xm
+000024d0: 6c5f 6465 636c 6172 6174 696f 6e60 207c  l_declaration` |
+000024e0: 2020 436f 6e66 6967 2020 7c20 2020 2020    Config  |     
+000024f0: 2020 203a 783a 2020 2020 2020 2020 207c     :x:         |
+00002500: 2020 2020 2020 2020 2062 6f6f 6c65 616e           boolean
+00002510: 2020 2020 2020 2020 2020 7c20 2020 2060            |    `
+00002520: 6661 6c73 6560 2020 2020 207c 2049 6e64  false`     | Ind
+00002530: 6963 6174 6573 2077 6865 7468 6572 2061  icates whether a
+00002540: 6e20 786d 6c20 6465 636c 6172 6174 696f  n xml declaratio
+00002550: 6e20 7368 6f75 6c64 2062 6520 6164 6465  n should be adde
+00002560: 6420 746f 206f 7574 7075 7420 6461 7461  d to output data
+00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025c0: 2020 2020 207c 0a7c 2060 6f75 7470 7574       |.| `output
+000025d0: 2f64 6972 6563 746f 7279 5f70 6174 6860  /directory_path`
+000025e0: 2020 7c20 2043 6f6e 6669 6720 207c 2020    |  Config  |  
+000025f0: 2020 2020 2020 3a78 3a20 2020 2020 2020        :x:       
+00002600: 2020 7c20 2020 2020 2020 2020 2073 7472    |          str
+00002610: 696e 6720 2020 2020 2020 2020 207c 2060  ing          | `
+00002620: 6d69 6d65 6f2d 6f75 7470 7574 6020 7c20  mimeo-output` | 
+00002630: 466f 7220 6066 696c 6560 2064 6972 6563  For `file` direc
+00002640: 7469 6f6e 202d 2064 6566 696e 6573 2061  tion - defines a
+00002650: 6e20 6f75 7470 7574 2064 6972 6563 746f  n output directo
+00002660: 7279 2020 2020 2020 2020 2020 2020 2020  ry              
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 2020 2020 2020 2020 7c0a 7c20 606f 7574          |.| `out
+000026d0: 7075 742f 6669 6c65 5f6e 616d 6560 2020  put/file_name`  
+000026e0: 2020 2020 207c 2020 436f 6e66 6967 2020       |  Config  
+000026f0: 7c20 2020 2020 2020 203a 783a 2020 2020  |        :x:    
+00002700: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00002710: 7374 7269 6e67 2020 2020 2020 2020 2020  string          
+00002720: 7c20 606d 696d 656f 2d6f 7574 7075 7460  | `mimeo-output`
+00002730: 207c 2046 6f72 2060 6669 6c65 6020 6469   | For `file` di
+00002740: 7265 6374 696f 6e20 2d20 6465 6669 6e65  rection - define
+00002750: 7320 616e 206f 7574 7075 7420 6669 6c65  s an output file
+00002760: 206e 616d 6520 2020 2020 2020 2020 2020   name           
+00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027c0: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
+000027d0: 6f75 7470 7574 2f6d 6574 686f 6460 2020  output/method`  
+000027e0: 2020 2020 2020 2020 7c20 2043 6f6e 6669          |  Confi
+000027f0: 6720 207c 2020 2020 2020 2020 3a78 3a20  g  |        :x: 
+00002800: 2020 2020 2020 2020 7c20 2020 2020 2060          |      `
+00002810: 504f 5354 602c 2060 5055 5460 2020 2020  POST`, `PUT`    
+00002820: 2020 207c 2020 2020 2060 504f 5354 6020     |     `POST` 
+00002830: 2020 2020 7c20 466f 7220 6068 7474 7060      | For `http`
+00002840: 2064 6972 6563 7469 6f6e 202d 2064 6566   direction - def
+00002850: 696e 6573 2061 2072 6571 7565 7374 206d  ines a request m
+00002860: 6574 686f 6420 2020 2020 2020 2020 2020  ethod           
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+000028d0: 7c20 606f 7574 7075 742f 7072 6f74 6f63  | `output/protoc
+000028e0: 6f6c 6020 2020 2020 2020 207c 2020 436f  ol`        |  Co
+000028f0: 6e66 6967 2020 7c20 2020 2020 2020 203a  nfig  |        :
+00002900: 783a 2020 2020 2020 2020 207c 2020 2020  x:         |    
+00002910: 2060 6874 7470 602c 2060 6874 7470 7360   `http`, `https`
+00002920: 2020 2020 2020 7c20 2020 2020 6068 7474        |     `htt
+00002930: 7060 2020 2020 207c 2046 6f72 2060 6874  p`     | For `ht
+00002940: 7470 6020 6469 7265 6374 696f 6e20 2d20  tp` direction - 
+00002950: 6465 6669 6e65 7320 6120 7572 6c20 7072  defines a url pr
+00002960: 6f74 6f63 6f6c 2020 2020 2020 2020 2020  otocol          
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029d0: 207c 0a7c 2060 6f75 7470 7574 2f68 6f73   |.| `output/hos
+000029e0: 7460 2020 2020 2020 2020 2020 2020 7c20  t`            | 
+000029f0: 2043 6f6e 6669 6720 207c 203a 6865 6176   Config  | :heav
+00002a00: 795f 6368 6563 6b5f 6d61 726b 3a20 7c20  y_check_mark: | 
+00002a10: 2020 2020 2020 2020 2073 7472 696e 6720           string 
+00002a20: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00002a30: 2d2d 2d20 2020 2020 2020 7c20 466f 7220  ---       | For 
+00002a40: 6068 7474 7060 2064 6972 6563 7469 6f6e  `http` direction
+00002a50: 202d 2064 6566 696e 6573 2061 2075 726c   - defines a url
+00002a60: 2068 6f73 7420 2020 2020 2020 2020 2020   host           
+00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2020 7c0a 7c20 606f 7574 7075 742f      |.| `output/
+00002ae0: 706f 7274 6020 2020 2020 2020 2020 2020  port`           
+00002af0: 207c 2020 436f 6e66 6967 2020 7c20 2020   |  Config  |   
+00002b00: 2020 2020 203a 783a 2020 2020 2020 2020       :x:        
+00002b10: 207c 2020 2020 2020 2020 2069 6e74 6567   |         integ
+00002b20: 6572 2020 2020 2020 2020 2020 7c20 2020  er          |   
+00002b30: 2020 606e 756c 6c60 2020 2020 207c 2046    `null`     | F
+00002b40: 6f72 2060 6874 7470 6020 6469 7265 6374  or `http` direct
+00002b50: 696f 6e20 2d20 6465 6669 6e65 7320 6120  ion - defines a 
+00002b60: 7572 6c20 706f 7274 2028 6361 6e20 6265  url port (can be
+00002b70: 2065 6d70 7479 2920 2020 2020 2020 2020   empty)         
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bd0: 2020 2020 2020 207c 0a7c 2060 6f75 7470         |.| `outp
+00002be0: 7574 2f65 6e64 706f 696e 7460 2020 2020  ut/endpoint`    
+00002bf0: 2020 2020 7c20 2043 6f6e 6669 6720 207c      |  Config  |
+00002c00: 203a 6865 6176 795f 6368 6563 6b5f 6d61   :heavy_check_ma
+00002c10: 726b 3a20 7c20 2020 2020 2020 2020 2073  rk: |          s
+00002c20: 7472 696e 6720 2020 2020 2020 2020 207c  tring          |
+00002c30: 2020 2020 2020 2d2d 2d20 2020 2020 2020        ---       
+00002c40: 7c20 466f 7220 6068 7474 7060 2064 6972  | For `http` dir
+00002c50: 6563 7469 6f6e 202d 2064 6566 696e 6573  ection - defines
+00002c60: 2061 2075 726c 2065 6e64 706f 696e 7420   a url endpoint 
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cd0: 2020 2020 2020 2020 2020 7c0a 7c20 606f            |.| `o
+00002ce0: 7574 7075 742f 7573 6572 6e61 6d65 6020  utput/username` 
+00002cf0: 2020 2020 2020 207c 2020 436f 6e66 6967         |  Config
+00002d00: 2020 7c20 3a68 6561 7679 5f63 6865 636b    | :heavy_check
+00002d10: 5f6d 6172 6b3a 207c 2020 2020 2020 2020  _mark: |        
+00002d20: 2020 7374 7269 6e67 2020 2020 2020 2020    string        
+00002d30: 2020 7c20 2020 2020 202d 2d2d 2020 2020    |      ---    
+00002d40: 2020 207c 2046 6f72 2060 6874 7470 6020     | For `http` 
+00002d50: 6469 7265 6374 696f 6e20 2d20 6465 6669  direction - defi
+00002d60: 6e65 7320 6120 7573 6572 6e61 6d65 2020  nes a username  
+00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dd0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00002de0: 2060 6f75 7470 7574 2f70 6173 7377 6f72   `output/passwor
+00002df0: 6460 2020 2020 2020 2020 7c20 2043 6f6e  d`        |  Con
+00002e00: 6669 6720 207c 203a 6865 6176 795f 6368  fig  | :heavy_ch
+00002e10: 6563 6b5f 6d61 726b 3a20 7c20 2020 2020  eck_mark: |     
+00002e20: 2020 2020 2073 7472 696e 6720 2020 2020       string     
+00002e30: 2020 2020 207c 2020 2020 2020 2d2d 2d20       |      --- 
+00002e40: 2020 2020 2020 7c20 466f 7220 6068 7474        | For `htt
+00002e50: 7060 2064 6972 6563 7469 6f6e 202d 2064  p` direction - d
+00002e60: 6566 696e 6573 2061 2070 6173 7377 6f72  efines a passwor
+00002e70: 6420 2020 2020 2020 2020 2020 2020 2020  d               
+00002e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ee0: 7c0a 7c20 6076 6172 7360 2020 2020 2020  |.| `vars`      
+00002ef0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00002f00: 436f 6e66 6967 2020 7c20 2020 2020 2020  Config  |       
+00002f10: 203a 783a 2020 2020 2020 2020 207c 2020   :x:         |  
+00002f20: 2020 2020 2020 2020 6f62 6a65 6374 2020          object  
+00002f30: 2020 2020 2020 2020 7c20 2020 2020 202d          |      -
+00002f40: 2d2d 2020 2020 2020 207c 2044 6566 696e  --       | Defin
+00002f50: 6573 2076 6172 6961 626c 6573 2074 6f20  es variables to 
+00002f60: 6265 2075 7365 6420 696e 2061 204d 696d  be used in a Mim
+00002f70: 656f 2054 656d 706c 6174 6520 2872 6561  eo Template (rea
+00002f80: 6420 6d6f 7265 2069 6e20 6e65 7874 2073  d more in next s
+00002f90: 6563 7469 6f6e 2920 2020 2020 2020 2020  ection)         
+00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fe0: 2020 207c 0a7c 2060 5f74 656d 706c 6174     |.| `_templat
+00002ff0: 6573 5f60 2020 2020 2020 2020 2020 2020  es_`            
+00003000: 7c20 2043 6f6e 6669 6720 207c 203a 6865  |  Config  | :he
+00003010: 6176 795f 6368 6563 6b5f 6d61 726b 3a20  avy_check_mark: 
+00003020: 7c20 2020 2020 2020 2020 2061 7272 6179  |          array
+00003030: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00003040: 2020 2d2d 2d20 2020 2020 2020 7c20 5374    ---       | St
+00003050: 6f72 6573 2074 656d 706c 6174 6573 2066  ores templates f
+00003060: 6f72 2064 6174 6120 6765 6e65 7261 7469  or data generati
+00003070: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030e0: 2020 2020 2020 7c0a 7c20 6063 6f75 6e74        |.| `count
+000030f0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00003100: 2020 207c 2054 656d 706c 6174 6520 7c20     | Template | 
+00003110: 3a68 6561 7679 5f63 6865 636b 5f6d 6172  :heavy_check_mar
+00003120: 6b3a 207c 2020 2020 2020 2020 2069 6e74  k: |         int
+00003130: 6567 6572 2020 2020 2020 2020 2020 7c20  eger          | 
+00003140: 2020 2020 202d 2d2d 2020 2020 2020 207c       ---       |
+00003150: 2049 6e64 6963 6174 6573 206e 756d 6265   Indicates numbe
+00003160: 7220 6f66 2063 6f70 6965 7320 2020 2020  r of copies     
+00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031e0: 2020 2020 2020 2020 207c 0a7c 2060 6d6f           |.| `mo
+000031f0: 6465 6c60 2020 2020 2020 2020 2020 2020  del`            
+00003200: 2020 2020 2020 7c20 5465 6d70 6c61 7465        | Template
+00003210: 207c 203a 6865 6176 795f 6368 6563 6b5f   | :heavy_check_
+00003220: 6d61 726b 3a20 7c20 2020 2020 2020 2020  mark: |         
+00003230: 206f 626a 6563 7420 2020 2020 2020 2020   object         
+00003240: 207c 2020 2020 2020 2d2d 2d20 2020 2020   |      ---     
+00003250: 2020 7c20 4465 6669 6e65 7320 6461 7461    | Defines data
+00003260: 2074 656d 706c 6174 6520 746f 2062 6520   template to be 
+00003270: 636f 7069 6564 2020 2020 2020 2020 2020  copied          
+00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032e0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000032f0: 6063 6f6e 7465 7874 6020 2020 2020 2020  `context`       
+00003300: 2020 2020 2020 2020 207c 2020 4d6f 6465           |  Mode
+00003310: 6c20 2020 7c20 2020 2020 2020 203a 783a  l   |        :x:
+00003320: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00003330: 2020 2020 6f62 6a65 6374 2020 2020 2020      object      
+00003340: 2020 2020 7c20 2020 2020 202d 2d2d 2020      |      ---  
+00003350: 2020 2020 207c 2044 6566 696e 6573 2061       | Defines a
+00003360: 2063 6f6e 7465 7874 206e 616d 6520 7468   context name th
+00003370: 6174 2069 7320 696e 7465 726e 616c 6c79  at is internally
+00003380: 2075 7365 6420 652e 672e 2075 7369 6e67   used e.g. using
+00003390: 2060 6375 7272 5f69 7465 7228 2960 2061   `curr_iter()` a
+000033a0: 6e64 2060 6765 745f 6b65 7928 2960 206d  nd `get_key()` m
+000033b0: 696d 656f 2075 7469 6c73 2028 6279 2064  imeo utils (by d
+000033c0: 6566 6175 6c74 206d 6f64 656c 206e 616d  efault model nam
+000033d0: 6520 6973 2075 7365 6420 6173 2074 6865  e is used as the
+000033e0: 2063 6f6e 7465 7874 206e 616d 6529 207c   context name) |
+000033f0: 0a0a 2323 2323 204d 696d 656f 2045 6e76  ..#### Mimeo Env
+00003400: 6972 6f6e 6d65 6e74 0a0a 546f 206d 616b  ironment..To mak
+00003410: 6520 6068 7474 7060 206f 7574 7075 7420  e `http` output 
+00003420: 6469 7265 6374 6f72 7920 6561 7369 6572  directory easier
+00003430: 2074 6f20 7573 652c 206d 696d 656f 2061   to use, mimeo a
+00003440: 6c6c 6f77 7320 796f 7520 746f 2063 6f6e  llows you to con
+00003450: 6669 6775 7265 204d 696d 656f 2045 6e76  figure Mimeo Env
+00003460: 6972 6f6e 6d65 6e74 732e 0a54 6865 7920  ironments..They 
+00003470: 6172 6520 636f 6e66 6967 7572 6564 2069  are configured i
+00003480: 6e20 6120 4a53 4f4e 2066 696c 6520 2862  n a JSON file (b
+00003490: 7920 6465 6661 756c 743a 206d 696d 656f  y default: mimeo
+000034a0: 2e65 6e76 732e 6a73 6f6e 2920 616e 6420  .envs.json) and 
+000034b0: 7375 7070 6f72 7420 7468 6520 666f 6c6c  support the foll
+000034c0: 6f77 696e 6720 6f75 7470 7574 2064 6574  owing output det
+000034d0: 6169 6c73 3a0a 2d20 6070 726f 746f 636f  ails:.- `protoco
+000034e0: 6c60 0a2d 2060 686f 7374 600a 2d20 6070  l`.- `host`.- `p
+000034f0: 6f72 7460 0a2d 2060 7573 6572 6e61 6d65  ort`.- `username
+00003500: 600a 2d20 6070 6173 7377 6f72 6460 0a0a  `.- `password`..
+00003510: 4578 616d 706c 650a 6060 606a 736f 6e0a  Example.```json.
+00003520: 7b0a 2020 2020 226c 6f63 616c 223a 207b  {.    "local": {
+00003530: 0a20 2020 2020 2020 2022 686f 7374 223a  .        "host":
+00003540: 2022 6c6f 6361 6c68 6f73 7422 2c0a 2020   "localhost",.  
+00003550: 2020 2020 2020 2270 6f72 7422 3a20 3830        "port": 80
+00003560: 3030 2c0a 2020 2020 2020 2020 2275 7365  00,.        "use
+00003570: 726e 616d 6522 3a20 2261 646d 696e 222c  rname": "admin",
+00003580: 0a20 2020 2020 2020 2022 7061 7373 776f  .        "passwo
+00003590: 7264 223a 2022 6164 6d69 6e22 0a20 2020  rd": "admin".   
+000035a0: 207d 2c0a 2020 2020 2264 6576 223a 207b   },.    "dev": {
+000035b0: 0a20 2020 2020 2020 2022 7072 6f74 6f63  .        "protoc
+000035c0: 6f6c 223a 2022 6874 7470 7322 2c0a 2020  ol": "https",.  
+000035d0: 2020 2020 2020 2268 6f73 7422 3a20 2231        "host": "1
+000035e0: 312e 3131 312e 3131 2e31 3131 222c 0a20  1.111.11.111",. 
+000035f0: 2020 2020 2020 2022 706f 7274 223a 2038         "port": 8
+00003600: 3030 302c 0a20 2020 2020 2020 2022 7573  000,.        "us
+00003610: 6572 6e61 6d65 223a 2022 736f 6d65 2d75  ername": "some-u
+00003620: 7365 7222 2c0a 2020 2020 2020 2020 2270  ser",.        "p
+00003630: 6173 7377 6f72 6422 3a20 2273 6f6d 652d  assword": "some-
+00003640: 7061 7373 776f 7264 220a 2020 2020 7d0a  password".    }.
+00003650: 7d0a 6060 600a 0a54 6f20 7573 6520 6120  }.```..To use a 
+00003660: 7370 6563 6966 6963 204d 696d 656f 2045  specific Mimeo E
+00003670: 6e76 6972 6f6e 6d65 6e74 2079 6f75 2063  nvironment you c
+00003680: 616e 2075 7365 2074 6865 2066 6f6c 6c6f  an use the follo
+00003690: 7769 6e67 2063 6f6d 6d61 6e64 733a 0a60  wing commands:.`
+000036a0: 6060 7368 0a6d 696d 656f 2053 6f6d 6545  ``sh.mimeo SomeE
+000036b0: 6e74 6974 792d 636f 6e66 6967 2e6a 736f  ntity-config.jso
+000036c0: 6e20 2d65 2064 6576 0a6d 696d 656f 2053  n -e dev.mimeo S
+000036d0: 6f6d 6545 6e74 6974 792d 636f 6e66 6967  omeEntity-config
+000036e0: 2e6a 736f 6e20 2d65 2064 6576 202d 2d68  .json -e dev --h
+000036f0: 7474 702d 656e 7673 2d66 696c 6520 656e  ttp-envs-file en
+00003700: 7669 726f 6e6d 656e 7473 2e6a 736f 6e0a  vironments.json.
+00003710: 6060 600a 0a23 2323 2320 4d69 6d65 6f20  ```..#### Mimeo 
+00003720: 5661 7273 0a0a 4d69 6d65 6f20 616c 6c6f  Vars..Mimeo allo
+00003730: 7773 2079 6f75 2074 6f20 6465 6669 6e65  ws you to define
+00003740: 2061 206c 6973 7420 6f66 2076 6172 6961   a list of varia
+00003750: 626c 6573 2e0a 596f 7520 6361 6e20 7573  bles..You can us
+00003760: 6520 7468 656d 2069 6e20 796f 7572 204d  e them in your M
+00003770: 696d 656f 2043 6f6e 6669 6720 6279 2077  imeo Config by w
+00003780: 7261 7070 696e 6720 7468 656d 2069 6e20  rapping them in 
+00003790: 6375 726c 7920 6272 6163 6b65 7473 205b  curly brackets [
+000037a0: 607b 5641 5249 4142 4c45 7d60 5d2e 0a0a  `{VARIABLE}`]...
+000037b0: 5468 6572 6520 6172 6520 6f6e 6c79 2032  There are only 2
+000037c0: 2072 756c 6573 2066 6f72 2076 6172 6961   rules for varia
+000037d0: 626c 6520 6e61 6d65 733a 0a2d 2056 6172  ble names:.- Var
+000037e0: 6961 626c 6520 6e61 6d65 2063 616e 2069  iable name can i
+000037f0: 6e63 6c75 6465 2075 7070 6572 2d63 6173  nclude upper-cas
+00003800: 6564 206c 6574 7465 7273 205c 5b60 412d  ed letters \[`A-
+00003810: 5a60 5c5d 2c20 756e 6465 7273 636f 7265  Z`\], underscore
+00003820: 205c 5b60 5f60 5c5d 2061 6e64 2064 6967   \[`_`\] and dig
+00003830: 6974 7320 5c7b 6030 2d39 605c 7d20 6f6e  its \{`0-9`\} on
+00003840: 6c79 0a2d 2056 6172 6961 626c 6520 6e61  ly.- Variable na
+00003850: 6d65 206d 7573 7420 7374 6172 7420 7769  me must start wi
+00003860: 7468 2061 206c 6574 7465 720a 0a56 6172  th a letter..Var
+00003870: 6961 626c 6520 6361 6e20 6265 2064 6566  iable can be def
+00003880: 696e 6564 2077 6974 683a 0a2d 2061 6e79  ined with:.- any
+00003890: 2061 746f 6d69 6320 7661 6c75 650a 2d20   atomic value.- 
+000038a0: 616e 7920 6f74 6865 7220 7661 7269 6162  any other variab
+000038b0: 6c65 2064 6566 696e 6564 0a2d 2061 6e79  le defined.- any
+000038c0: 204d 696d 656f 2055 7469 6c0a 0a59 6f75   Mimeo Util..You
+000038d0: 2063 616e 2075 7365 204d 696d 656f 2056   can use Mimeo V
+000038e0: 6172 7320 6173 2070 6172 7469 616c 2076  ars as partial v
+000038f0: 616c 7565 7320 2875 6e6c 6573 7320 7468  alues (unless th
+00003900: 6579 2061 7265 2064 6566 696e 6564 2061  ey are defined a
+00003910: 7320 4d69 6d65 6f20 5574 696c 7329 2e0a  s Mimeo Utils)..
+00003920: 0a45 7861 6d70 6c65 3a0a 6060 606a 736f  .Example:.```jso
+00003930: 6e0a 7b0a 2020 2276 6172 7322 3a20 7b0a  n.{.  "vars": {.
+00003940: 2020 2020 2243 5553 544f 4d5f 5641 525f      "CUSTOM_VAR_
+00003950: 3122 3a20 2263 7573 746f 6d2d 7661 6c75  1": "custom-valu
+00003960: 652d 3122 2c0a 2020 2020 2243 5553 544f  e-1",.    "CUSTO
+00003970: 4d5f 5641 525f 3222 3a20 312c 0a20 2020  M_VAR_2": 1,.   
+00003980: 2022 4355 5354 4f4d 5f56 4152 5f33 223a   "CUSTOM_VAR_3":
+00003990: 2074 7275 652c 0a20 2020 2022 4355 5354   true,.    "CUST
+000039a0: 4f4d 5f56 4152 5f34 223a 2022 7b43 5553  OM_VAR_4": "{CUS
+000039b0: 544f 4d5f 5641 525f 327d 222c 0a20 2020  TOM_VAR_2}",.   
+000039c0: 2022 4355 5354 4f4d 5f56 4152 5f35 223a   "CUSTOM_VAR_5":
+000039d0: 2022 7b61 7574 6f5f 696e 6372 656d 656e   "{auto_incremen
+000039e0: 747d 222c 0a20 2020 2022 4355 5354 4f4d  t}",.    "CUSTOM
+000039f0: 5f56 4152 5f36 223a 207b 0a20 2020 2020  _VAR_6": {.     
+00003a00: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
+00003a10: 7b0a 2020 2020 2020 2020 225f 6e61 6d65  {.        "_name
+00003a20: 223a 2022 7261 6e64 6f6d 5f69 6e74 222c  ": "random_int",
+00003a30: 0a20 2020 2020 2020 2022 6c69 6d69 7422  .        "limit"
+00003a40: 3a20 3939 0a20 2020 2020 207d 0a20 2020  : 99.      }.   
+00003a50: 207d 0a20 207d 2c0a 2020 225f 7465 6d70   }.  },.  "_temp
+00003a60: 6c61 7465 735f 223a 205b 0a20 2020 207b  lates_": [.    {
+00003a70: 0a20 2020 2020 2022 636f 756e 7422 3a20  .      "count": 
+00003a80: 352c 0a20 2020 2020 2022 6d6f 6465 6c22  5,.      "model"
+00003a90: 3a20 7b0a 2020 2020 2020 2020 2253 6f6d  : {.        "Som
+00003aa0: 6545 6e74 6974 7922 3a20 7b0a 2020 2020  eEntity": {.    
+00003ab0: 2020 2020 2020 2243 6869 6c64 4e6f 6465        "ChildNode
+00003ac0: 3122 3a20 227b 4355 5354 4f4d 5f56 4152  1": "{CUSTOM_VAR
+00003ad0: 5f31 7d22 2c0a 2020 2020 2020 2020 2020  _1}",.          
+00003ae0: 2243 6869 6c64 4e6f 6465 3222 3a20 227b  "ChildNode2": "{
+00003af0: 4355 5354 4f4d 5f56 4152 5f32 7d22 2c0a  CUSTOM_VAR_2}",.
+00003b00: 2020 2020 2020 2020 2020 2243 6869 6c64            "Child
+00003b10: 4e6f 6465 3322 3a20 227b 4355 5354 4f4d  Node3": "{CUSTOM
+00003b20: 5f56 4152 5f33 7d22 2c0a 2020 2020 2020  _VAR_3}",.      
+00003b30: 2020 2020 2243 6869 6c64 4e6f 6465 3422      "ChildNode4"
+00003b40: 3a20 227b 4355 5354 4f4d 5f56 4152 5f34  : "{CUSTOM_VAR_4
+00003b50: 7d22 2c0a 2020 2020 2020 2020 2020 2243  }",.          "C
+00003b60: 6869 6c64 4e6f 6465 3522 3a20 227b 4355  hildNode5": "{CU
+00003b70: 5354 4f4d 5f56 4152 5f35 7d22 2c0a 2020  STOM_VAR_5}",.  
+00003b80: 2020 2020 2020 2020 2243 6869 6c64 4e6f          "ChildNo
+00003b90: 6465 3622 3a20 227b 4355 5354 4f4d 5f56  de6": "{CUSTOM_V
+00003ba0: 4152 5f36 7d22 2c0a 2020 2020 2020 2020  AR_6}",.        
+00003bb0: 2020 2243 6869 6c64 4e6f 6465 3722 3a20    "ChildNode7": 
+00003bc0: 227b 4355 5354 4f4d 5f56 4152 5f31 7d2d  "{CUSTOM_VAR_1}-
+00003bd0: 7769 7468 2d73 7566 6669 7822 0a20 2020  with-suffix".   
+00003be0: 2020 2020 207d 0a20 2020 2020 207d 0a20       }.      }. 
+00003bf0: 2020 207d 0a20 205d 0a7d 0a60 6060 0a0a     }.  ].}.```..
+00003c00: 2323 2323 204d 696d 656f 2053 7065 6369  #### Mimeo Speci
+00003c10: 616c 2046 6965 6c64 730a 0a49 6e20 4d69  al Fields..In Mi
+00003c20: 6d65 6f20 5465 6d70 6c61 7465 2079 6f75  meo Template you
+00003c30: 2063 616e 2075 7365 2073 6f2d 6361 6c6c   can use so-call
+00003c40: 6564 205f 7370 6563 6961 6c20 6669 656c  ed _special fiel
+00003c50: 6473 5f2e 0a45 7665 7279 2066 6965 6c64  ds_..Every field
+00003c60: 2069 6e20 6120 7465 6d70 6c61 7465 2063   in a template c
+00003c70: 616e 2062 6520 7374 6f72 6564 2069 6e20  an be stored in 
+00003c80: 6d65 6d6f 7279 2028 5f70 726f 7669 6465  memory (_provide
+00003c90: 645f 2920 616e 6420 7573 6564 206c 6174  d_) and used lat
+00003ca0: 6572 2061 7320 6120 7661 6c75 6520 6f66  er as a value of
+00003cb0: 206f 7468 6572 2066 6965 6c64 7320 285f   other fields (_
+00003cc0: 696e 6a65 6374 6564 5f29 2e0a 546f 2070  injected_)..To p
+00003cd0: 726f 7669 6465 2061 2073 7065 6369 616c  rovide a special
+00003ce0: 2066 6965 6c64 2c20 7772 6170 2069 7473   field, wrap its
+00003cf0: 206e 616d 6520 7769 7468 2063 6f6c 6f6e   name with colon
+00003d00: 733a 205b 603a 536f 6d65 4669 656c 643a  s: [`:SomeField:
+00003d10: 605d 2e20 546f 2069 6e6a 6563 742c 2075  `]. To inject, u
+00003d20: 7365 2061 6464 6974 696f 6e61 6c6c 7920  se additionally 
+00003d30: 6375 726c 7920 6272 6163 6573 2074 6f0a  curly braces to.
+00003d40: 6c65 7420 696e 7465 7270 7265 7465 7220  let interpreter 
+00003d50: 6b6e 6f77 2069 7420 7368 6f75 6c64 2062  know it should b
+00003d60: 6520 7265 6e64 6572 6564 205b 607b 3a53  e rendered [`{:S
+00003d70: 6f6d 6546 6965 6c64 3a7d 605d 2e0a 5468  omeField:}`]..Th
+00003d80: 6579 2063 616e 2062 6520 696e 6a65 6374  ey can be inject
+00003d90: 6564 2061 7320 7061 7274 6961 6c20 7661  ed as partial va
+00003da0: 6c75 6573 2c20 7369 6d69 6c61 726c 7920  lues, similarly 
+00003db0: 746f 204d 696d 656f 2056 6172 732e 0a0a  to Mimeo Vars...
+00003dc0: 4578 616d 706c 650a 6060 606a 736f 6e0a  Example.```json.
+00003dd0: 7b0a 2020 225f 7465 6d70 6c61 7465 735f  {.  "_templates_
+00003de0: 223a 205b 0a20 2020 207b 0a20 2020 2020  ": [.    {.     
+00003df0: 2022 636f 756e 7422 3a20 352c 0a20 2020   "count": 5,.   
+00003e00: 2020 2022 6d6f 6465 6c22 3a20 7b0a 2020     "model": {.  
+00003e10: 2020 2020 2020 2253 6f6d 6545 6e74 6974        "SomeEntit
+00003e20: 7922 3a20 7b0a 2020 2020 2020 2020 2020  y": {.          
+00003e30: 223a 4368 696c 644e 6f64 6531 3a22 3a20  ":ChildNode1:": 
+00003e40: 2263 7573 746f 6d2d 7661 6c75 6522 2c0a  "custom-value",.
+00003e50: 2020 2020 2020 2020 2020 2243 6869 6c64            "Child
+00003e60: 4e6f 6465 3222 3a20 227b 3a43 6869 6c64  Node2": "{:Child
+00003e70: 4e6f 6465 313a 7d22 2c0a 2020 2020 2020  Node1:}",.      
+00003e80: 2020 2020 2243 6869 6c64 4e6f 6465 3322      "ChildNode3"
+00003e90: 3a20 227b 3a43 6869 6c64 4e6f 6465 313a  : "{:ChildNode1:
+00003ea0: 7d2d 7769 7468 2d73 7566 6669 7822 0a20  }-with-suffix". 
+00003eb0: 2020 2020 2020 207d 0a20 2020 2020 207d         }.      }
+00003ec0: 0a20 2020 207d 0a20 205d 0a7d 0a60 6060  .    }.  ].}.```
+00003ed0: 0a0a 2323 2323 204d 696d 656f 2055 7469  ..#### Mimeo Uti
+00003ee0: 6c73 0a0a 596f 7520 6361 6e20 7573 6520  ls..You can use 
+00003ef0: 7365 7665 7261 6c20 7072 6564 6566 696e  several predefin
+00003f00: 6564 2066 756e 6374 696f 6e73 2074 6f20  ed functions to 
+00003f10: 6765 6e65 7261 7465 2064 6174 612e 2054  generate data. T
+00003f20: 6865 7920 6361 6e20 6265 2075 7365 6420  hey can be used 
+00003f30: 696e 2061 205f 7261 775f 2066 6f72 6d61  in a _raw_ forma
+00003f40: 7420 6f72 205f 7061 7261 6d65 7472 697a  t or _parametriz
+00003f50: 6564 5f2e 0a0a 2323 2323 2320 5261 6e64  ed_...##### Rand
+00003f60: 6f6d 2053 7472 696e 670a 0a47 656e 6572  om String..Gener
+00003f70: 6174 6573 2061 2072 616e 646f 6d20 7374  ates a random st
+00003f80: 7269 6e67 2076 616c 7565 2e0a 0a7c 2050  ring value...| P
+00003f90: 6172 616d 6574 6572 207c 2053 7570 706f  arameter | Suppo
+00003fa0: 7274 6564 2076 616c 7565 7320 7c20 4465  rted values | De
+00003fb0: 6661 756c 7420 7c0a 7c3a 2d2d 2d2d 2d2d  fault |.|:------
+00003fc0: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00003fd0: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
+00003fe0: 3a7c 0a7c 2020 6c65 6e67 7468 2020 207c  :|.|  length   |
+00003ff0: 2020 2020 2020 6069 6e74 6020 2020 2020        `int`     
+00004000: 2020 7c20 2060 3230 6020 2020 7c0a 0a23    |  `20`   |..#
+00004010: 2323 2323 2320 5261 770a 0a55 7365 7320  ##### Raw..Uses 
+00004020: 7468 6520 6465 6661 756c 7420 6c65 6e67  the default leng
+00004030: 7468 3a20 3230 2063 6861 7261 6374 6572  th: 20 character
+00004040: 732e 0a0a 6060 606a 736f 6e0a 7b0a 2020  s...```json.{.  
+00004050: 2272 616e 646f 6d73 7472 696e 6722 3a20  "randomstring": 
+00004060: 227b 7261 6e64 6f6d 5f73 7472 7d22 0a7d  "{random_str}".}
+00004070: 0a60 6060 0a0a 2323 2323 2323 2050 6172  .```..###### Par
+00004080: 616d 6574 7269 7a65 640a 0a55 7365 7320  ametrized..Uses 
+00004090: 7468 6520 6375 7374 6f6d 697a 6564 206c  the customized l
+000040a0: 656e 6774 682e 0a0a 6060 606a 736f 6e0a  ength...```json.
+000040b0: 7b0a 2020 2272 616e 646f 6d73 7472 696e  {.  "randomstrin
+000040c0: 6722 3a20 7b0a 2020 2020 225f 6d69 6d65  g": {.    "_mime
+000040d0: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
+000040e0: 2022 5f6e 616d 6522 3a20 2272 616e 646f   "_name": "rando
+000040f0: 6d5f 7374 7222 2c0a 2020 2020 2020 226c  m_str",.      "l
+00004100: 656e 6774 6822 3a20 350a 2020 2020 7d0a  ength": 5.    }.
+00004110: 2020 7d0a 7d0a 6060 600a 0a23 2323 2323    }.}.```..#####
+00004120: 2052 616e 646f 6d20 496e 7465 6765 720a   Random Integer.
+00004130: 0a47 656e 6572 6174 6573 2061 2072 616e  .Generates a ran
+00004140: 646f 6d20 696e 7465 6765 7220 7661 6c75  dom integer valu
+00004150: 6520 6265 7477 6565 6e20 6073 7461 7274  e between `start
+00004160: 6020 616e 6420 606c 696d 6974 6020 7061  ` and `limit` pa
+00004170: 7261 6d65 7465 7273 2028 696e 636c 7573  rameters (inclus
+00004180: 6976 6529 2e0a 0a7c 2050 6172 616d 6574  ive)...| Paramet
+00004190: 6572 207c 2053 7570 706f 7274 6564 2076  er | Supported v
+000041a0: 616c 7565 7320 7c20 4465 6661 756c 7420  alues | Default 
+000041b0: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a  |.|:---------:|:
+000041c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000041d0: 3a7c 3a2d 2d2d 2d2d 2d2d 3a7c 0a7c 2020  :|:-------:|.|  
+000041e0: 2073 7461 7274 2020 207c 2020 2020 2020   start   |      
+000041f0: 6069 6e74 6020 2020 2020 2020 7c20 2020  `int`       |   
+00004200: 6031 6020 2020 7c0a 7c20 2020 6c69 6d69  `1`   |.|   limi
+00004210: 7420 2020 7c20 2020 2020 2060 696e 7460  t   |      `int`
+00004220: 2020 2020 2020 207c 2020 6031 3030 6020         |  `100` 
+00004230: 207c 0a0a 2323 2323 2323 2052 6177 0a0a   |..###### Raw..
+00004240: 5573 6573 2074 6865 2064 6566 6175 6c74  Uses the default
+00004250: 2073 7461 7274 2028 3129 2061 6e64 206c   start (1) and l
+00004260: 696d 6974 2028 3130 3029 2076 616c 7565  imit (100) value
+00004270: 732e 0a0a 6060 606a 736f 6e0a 7b0a 2020  s...```json.{.  
+00004280: 2272 616e 646f 6d69 6e74 6567 6572 223a  "randominteger":
+00004290: 2022 7b72 616e 646f 6d5f 696e 747d 220a   "{random_int}".
+000042a0: 7d0a 6060 600a 0a23 2323 2323 2320 5061  }.```..###### Pa
+000042b0: 7261 6d65 7472 697a 6564 0a0a 5573 6573  rametrized..Uses
+000042c0: 2074 6865 2063 7573 746f 6d69 7a65 6420   the customized 
+000042d0: 6c69 6d69 742e 0a0a 6060 606a 736f 6e0a  limit...```json.
+000042e0: 7b0a 2020 2272 616e 646f 6d69 6e74 6567  {.  "randominteg
+000042f0: 6572 3122 3a20 7b0a 2020 2020 225f 6d69  er1": {.    "_mi
+00004300: 6d65 6f5f 7574 696c 223a 207b 0a20 2020  meo_util": {.   
+00004310: 2020 2022 5f6e 616d 6522 3a20 2272 616e     "_name": "ran
+00004320: 646f 6d5f 696e 7422 2c0a 2020 2020 2020  dom_int",.      
+00004330: 2273 7461 7274 223a 2030 0a20 2020 207d  "start": 0.    }
+00004340: 0a20 207d 2c0a 2020 2272 616e 646f 6d69  .  },.  "randomi
+00004350: 6e74 6567 6572 3222 3a20 7b0a 2020 2020  nteger2": {.    
+00004360: 225f 6d69 6d65 6f5f 7574 696c 223a 207b  "_mimeo_util": {
+00004370: 0a20 2020 2020 2022 5f6e 616d 6522 3a20  .      "_name": 
+00004380: 2272 616e 646f 6d5f 696e 7422 2c0a 2020  "random_int",.  
+00004390: 2020 2020 226c 696d 6974 223a 2035 0a20      "limit": 5. 
+000043a0: 2020 207d 0a20 207d 2c0a 2020 2272 616e     }.  },.  "ran
+000043b0: 646f 6d69 6e74 6567 6572 3322 3a20 7b0a  dominteger3": {.
+000043c0: 2020 2020 225f 6d69 6d65 6f5f 7574 696c      "_mimeo_util
+000043d0: 223a 207b 0a20 2020 2020 2022 5f6e 616d  ": {.      "_nam
+000043e0: 6522 3a20 2272 616e 646f 6d5f 696e 7422  e": "random_int"
+000043f0: 2c0a 2020 2020 2020 2273 7461 7274 223a  ,.      "start":
+00004400: 2030 2c0a 2020 2020 2020 226c 696d 6974   0,.      "limit
+00004410: 223a 2035 0a20 2020 207d 0a20 207d 0a7d  ": 5.    }.  }.}
+00004420: 0a60 6060 0a0a 2323 2323 2320 5261 6e64  .```..##### Rand
+00004430: 6f6d 2049 7465 6d0a 0a47 656e 6572 6174  om Item..Generat
+00004440: 6573 2061 2072 616e 646f 6d20 7661 6c75  es a random valu
+00004450: 6520 6672 6f6d 2069 7465 6d73 2070 726f  e from items pro
+00004460: 7669 6465 642e 2020 0a4e 4f54 4943 453a  vided.  .NOTICE:
+00004470: 2054 6865 2072 6177 2066 6f72 6d20 6f66   The raw form of
+00004480: 2074 6869 7320 4d69 6d65 6f20 5574 696c   this Mimeo Util
+00004490: 2077 696c 6c20 6765 6e65 7261 7465 2061   will generate a
+000044a0: 2062 6c61 6e6b 2073 7472 696e 6720 7661   blank string va
+000044b0: 6c75 6520 2861 7320 7361 6d65 2061 7320  lue (as same as 
+000044c0: 6e6f 2069 7465 6d73 2070 6172 616d 6574  no items paramet
+000044d0: 7269 7a65 6429 2e0a 0a7c 2050 6172 616d  rized)...| Param
+000044e0: 6574 6572 207c 2053 7570 706f 7274 6564  eter | Supported
+000044f0: 2076 616c 7565 7320 7c20 4465 6661 756c   values | Defaul
+00004500: 7420 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a  t |.|:---------:
+00004510: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
+00004520: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 3a7c 0a7c  --:|:-------:|.|
+00004530: 2020 2069 7465 6d73 2020 207c 2020 2020     items   |    
+00004540: 2020 606c 6973 7460 2020 2020 2020 7c20    `list`      | 
+00004550: 605b 2222 5d60 2020 7c0a 0a23 2323 2323  `[""]`  |..#####
+00004560: 2320 5061 7261 6d65 7472 697a 6564 0a0a  # Parametrized..
+00004570: 6060 606a 736f 6e0a 7b0a 2020 2272 616e  ```json.{.  "ran
+00004580: 646f 6d22 3a20 7b0a 2020 2020 225f 6d69  dom": {.    "_mi
+00004590: 6d65 6f5f 7574 696c 223a 207b 0a20 2020  meo_util": {.   
+000045a0: 2020 2022 5f6e 616d 6522 3a20 2272 616e     "_name": "ran
+000045b0: 646f 6d5f 6974 656d 222c 0a20 2020 2020  dom_item",.     
+000045c0: 2022 6974 656d 7322 3a20 5b22 7661 6c75   "items": ["valu
+000045d0: 6522 2c20 312c 2074 7275 655d 0a20 2020  e", 1, true].   
+000045e0: 207d 0a20 207d 0a7d 0a60 6060 0a0a 2323   }.  }.}.```..##
+000045f0: 2323 2320 4461 7465 0a0a 4765 6e65 7261  ### Date..Genera
+00004600: 7465 7320 6120 6461 7465 2076 616c 7565  tes a date value
+00004610: 2069 6e20 666f 726d 6174 2060 5959 5959   in format `YYYY
+00004620: 2d4d 4d2d 4444 602e 0a0a 7c20 5061 7261  -MM-DD`...| Para
+00004630: 6d65 7465 7220 207c 2053 7570 706f 7274  meter  | Support
+00004640: 6564 2076 616c 7565 7320 7c20 4465 6661  ed values | Defa
+00004650: 756c 7420 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d  ult |.|:--------
+00004660: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
+00004670: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d3a  -----:|:-------:
+00004680: 7c0a 7c20 6461 7973 5f64 656c 7461 207c  |.| days_delta |
+00004690: 2020 2020 2020 6069 6e74 6020 2020 2020        `int`     
+000046a0: 2020 7c20 2020 6030 6020 2020 7c0a 0a23    |   `0`   |..#
+000046b0: 2323 2323 2320 5261 770a 0a55 7365 7320  ##### Raw..Uses 
+000046c0: 7468 6520 746f 6461 7927 7320 6461 7465  the today's date
+000046d0: 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  ...```json.{.  "
+000046e0: 546f 6461 7922 3a20 227b 6461 7465 7d22  Today": "{date}"
+000046f0: 0a7d 0a60 6060 0a0a 2323 2323 2323 2050  .}.```..###### P
+00004700: 6172 616d 6574 7269 7a65 640a 0a55 7365  arametrized..Use
+00004710: 7320 7468 6520 6375 7374 6f6d 697a 6564  s the customized
+00004720: 2064 6179 7320 6465 6c74 612e 0a0a 6060   days delta...``
+00004730: 606a 736f 6e0a 7b0a 2020 2259 6573 7465  `json.{.  "Yeste
+00004740: 7264 6179 223a 207b 0a20 2020 2022 5f6d  rday": {.    "_m
+00004750: 696d 656f 5f75 7469 6c22 3a20 7b0a 2020  imeo_util": {.  
+00004760: 2020 2020 225f 6e61 6d65 223a 2022 6461      "_name": "da
+00004770: 7465 222c 0a20 2020 2020 2022 6461 7973  te",.      "days
+00004780: 5f64 656c 7461 223a 202d 310a 2020 2020  _delta": -1.    
+00004790: 7d0a 2020 7d2c 0a20 2022 546f 6d6f 7272  }.  },.  "Tomorr
+000047a0: 6f77 223a 207b 0a20 2020 2022 5f6d 696d  ow": {.    "_mim
+000047b0: 656f 5f75 7469 6c22 3a20 7b0a 2020 2020  eo_util": {.    
+000047c0: 2020 225f 6e61 6d65 223a 2022 6461 7465    "_name": "date
+000047d0: 222c 0a20 2020 2020 2022 6461 7973 5f64  ",.      "days_d
+000047e0: 656c 7461 223a 2031 0a20 2020 207d 0a20  elta": 1.    }. 
+000047f0: 207d 0a7d 0a60 6060 0a0a 2323 2323 2320   }.}.```..##### 
+00004800: 4461 7465 2054 696d 650a 0a47 656e 6572  Date Time..Gener
+00004810: 6174 6573 2061 2064 6174 6520 7469 6d65  ates a date time
+00004820: 2076 616c 7565 2069 6e20 666f 726d 6174   value in format
+00004830: 2060 5959 5959 2d4d 4d2d 4444 2754 2748   `YYYY-MM-DD'T'H
+00004840: 483a 6d6d 3a53 5360 2e0a 0a7c 2020 2050  H:mm:SS`...|   P
+00004850: 6172 616d 6574 6572 2020 207c 2053 7570  arameter   | Sup
+00004860: 706f 7274 6564 2076 616c 7565 7320 7c20  ported values | 
+00004870: 4465 6661 756c 7420 7c0a 7c3a 2d2d 2d2d  Default |.|:----
+00004880: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
+00004890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  ------------:|:-
+000048a0: 2d2d 2d2d 2d2d 3a7c 0a7c 2020 6461 7973  ------:|.|  days
+000048b0: 5f64 656c 7461 2020 207c 2020 2020 2020  _delta   |      
+000048c0: 6069 6e74 6020 2020 2020 2020 7c20 2020  `int`       |   
+000048d0: 6030 6020 2020 7c0a 7c20 2068 6f75 7273  `0`   |.|  hours
+000048e0: 5f64 656c 7461 2020 7c20 2020 2020 2060  _delta  |      `
+000048f0: 696e 7460 2020 2020 2020 207c 2020 2060  int`       |   `
+00004900: 3060 2020 207c 0a7c 206d 696e 7574 6573  0`   |.| minutes
+00004910: 5f64 656c 7461 207c 2020 2020 2020 6069  _delta |      `i
+00004920: 6e74 6020 2020 2020 2020 7c20 2020 6030  nt`       |   `0
+00004930: 6020 2020 7c0a 7c20 7365 636f 6e64 735f  `   |.| seconds_
+00004940: 6465 6c74 6120 7c20 2020 2020 2060 696e  delta |      `in
+00004950: 7460 2020 2020 2020 207c 2020 2060 3060  t`       |   `0`
+00004960: 2020 207c 0a0a 2323 2323 2323 2052 6177     |..###### Raw
+00004970: 0a0a 5573 6573 2074 6865 2063 7572 7265  ..Uses the curre
+00004980: 6e74 2074 696d 6573 7461 6d70 2e0a 0a60  nt timestamp...`
+00004990: 6060 6a73 6f6e 0a7b 0a20 2022 4e6f 7722  ``json.{.  "Now"
+000049a0: 3a20 227b 6461 7465 5f74 696d 657d 220a  : "{date_time}".
+000049b0: 7d0a 6060 600a 0a23 2323 2323 2320 5061  }.```..###### Pa
+000049c0: 7261 6d65 7472 697a 6564 0a0a 5573 6573  rametrized..Uses
+000049d0: 2074 6865 2063 7573 746f 6d69 7a65 6420   the customized 
+000049e0: 6465 6c74 6173 2e0a 0a60 6060 6a73 6f6e  deltas...```json
+000049f0: 0a7b 0a20 2022 546f 6d6f 7272 6f77 5468  .{.  "TomorrowTh
+00004a00: 7265 6548 6f75 7273 4c61 7465 7254 7765  reeHoursLaterTwe
+00004a10: 6e74 794d 696e 7574 6573 4167 6f54 776f  ntyMinutesAgoTwo
+00004a20: 5365 636f 6e64 734c 6174 6572 223a 207b  SecondsLater": {
+00004a30: 0a20 2020 2022 5f6d 696d 656f 5f75 7469  .    "_mimeo_uti
+00004a40: 6c22 3a20 7b0a 2020 2020 2020 225f 6e61  l": {.      "_na
+00004a50: 6d65 223a 2022 6461 7465 5f74 696d 6522  me": "date_time"
+00004a60: 2c0a 2020 2020 2020 2264 6179 735f 6465  ,.      "days_de
+00004a70: 6c74 6122 3a20 312c 0a20 2020 2020 2022  lta": 1,.      "
+00004a80: 686f 7572 735f 6465 6c74 6122 3a20 332c  hours_delta": 3,
+00004a90: 0a20 2020 2020 2022 6d69 6e75 7465 735f  .      "minutes_
+00004aa0: 6465 6c74 6122 3a20 2d32 302c 0a20 2020  delta": -20,.   
+00004ab0: 2020 2022 7365 636f 6e64 735f 6465 6c74     "seconds_delt
+00004ac0: 6122 3a20 320a 2020 2020 7d0a 2020 7d0a  a": 2.    }.  }.
+00004ad0: 7d0a 6060 600a 0a23 2323 2323 2041 7574  }.```..##### Aut
+00004ae0: 6f20 496e 6372 656d 656e 740a 0a47 656e  o Increment..Gen
+00004af0: 6572 6174 6573 2061 206e 6578 7420 696e  erates a next in
+00004b00: 7465 6765 7220 696e 2063 6f6e 7465 7874  teger in context
+00004b10: 206f 6620 6120 6d6f 6465 6c20 2869 6e20   of a model (in 
+00004b20: 6e65 7374 6564 2074 656d 706c 6174 6573  nested templates
+00004b30: 2069 7420 7769 6c6c 2075 7365 2061 2073   it will use a s
+00004b40: 6570 6172 6174 6564 2063 6f6e 7465 7874  eparated context
+00004b50: 292e 0a0a 7c20 5061 7261 6d65 7465 7220  )...| Parameter 
+00004b60: 7c20 5375 7070 6f72 7465 6420 7661 6c75  | Supported valu
+00004b70: 6573 207c 2044 6566 6175 6c74 2020 7c0a  es | Default  |.
+00004b80: 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  |:---------:|:--
+00004b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
+00004ba0: 3a2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2070  :--------:|.|  p
+00004bb0: 6174 7465 726e 2020 7c20 2020 2020 2060  attern  |      `
+00004bc0: 7374 7260 2020 2020 2020 207c 2060 7b3a  str`       | `{:
+00004bd0: 3035 647d 6020 7c0a 0a23 2323 2323 2320  05d}` |..###### 
+00004be0: 5261 770a 0a55 7365 7320 6120 6465 6661  Raw..Uses a defa
+00004bf0: 756c 7420 7061 7474 6572 6e3a 202a 2a7b  ult pattern: **{
+00004c00: 3a30 3564 7d2a 2a20 2861 6e20 696e 7465  :05d}** (an inte
+00004c10: 6765 7220 7769 7468 2035 206c 6561 6469  ger with 5 leadi
+00004c20: 6e67 207a 6572 6f73 292e 0a0a 6060 606a  ng zeros)...```j
+00004c30: 736f 6e0a 7b0a 2020 2249 4422 3a20 227b  son.{.  "ID": "{
+00004c40: 6175 746f 5f69 6e63 7265 6d65 6e74 7d22  auto_increment}"
+00004c50: 0a7d 0a60 6060 0a0a 2323 2323 2323 2050  .}.```..###### P
+00004c60: 6172 616d 6574 7269 7a65 640a 0a55 7365  arametrized..Use
+00004c70: 7320 7468 6520 7374 7269 6e67 2070 6174  s the string pat
+00004c80: 7465 726e 2070 726f 7669 6465 642e 0a0a  tern provided...
+00004c90: 6060 606a 736f 6e0a 7b0a 2020 2249 4422  ```json.{.  "ID"
+00004ca0: 3a20 7b0a 2020 2020 225f 6d69 6d65 6f5f  : {.    "_mimeo_
+00004cb0: 7574 696c 223a 207b 0a20 2020 2020 2022  util": {.      "
+00004cc0: 5f6e 616d 6522 3a20 2261 7574 6f5f 696e  _name": "auto_in
+00004cd0: 6372 656d 656e 7422 2c0a 2020 2020 2020  crement",.      
+00004ce0: 2270 6174 7465 726e 223a 2022 4d59 5f49  "pattern": "MY_I
+00004cf0: 445f 7b3a 3031 3064 7d22 0a20 2020 207d  D_{:010d}".    }
+00004d00: 0a20 207d 0a7d 0a60 6060 0a0a 2323 2323  .  }.}.```..####
+00004d10: 2320 4375 7272 656e 7420 4974 6572 6174  # Current Iterat
+00004d20: 696f 6e0a 0a47 656e 6572 6174 6573 2061  ion..Generates a
+00004d30: 2076 616c 7565 206f 6620 7468 6520 6375   value of the cu
+00004d40: 7272 656e 7420 6974 6572 6174 696f 6e20  rrent iteration 
+00004d50: 696e 2061 204d 696d 656f 2054 656d 706c  in a Mimeo Templ
+00004d60: 6174 6520 636f 6e74 6578 742e 0a0a 7c20  ate context...| 
+00004d70: 5061 7261 6d65 7465 7220 7c20 5375 7070  Parameter | Supp
+00004d80: 6f72 7465 6420 7661 6c75 6573 207c 2020  orted values |  
+00004d90: 2020 2020 4465 6661 756c 7420 2020 2020      Default     
+00004da0: 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 3a7c   |.|:---------:|
+00004db0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+00004dc0: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
+00004dd0: 2d2d 2d2d 2d3a 7c0a 7c20 2063 6f6e 7465  -----:|.|  conte
+00004de0: 7874 2020 7c20 2020 2020 2060 7374 7260  xt  |      `str`
+00004df0: 2020 2020 2020 207c 2061 2063 7572 7265         | a curre
+00004e00: 6e74 2063 6f6e 7465 7874 207c 0a0a 2323  nt context |..##
+00004e10: 2323 2323 2052 6177 0a0a 5573 6573 2074  #### Raw..Uses t
+00004e20: 6865 2063 7572 7265 6e74 2063 6f6e 7465  he current conte
+00004e30: 7874 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20  xt...```json.{. 
+00004e40: 2022 4944 223a 2022 7b63 7572 725f 6974   "ID": "{curr_it
+00004e50: 6572 7d22 0a7d 0a60 6060 0a0a 2323 2323  er}".}.```..####
+00004e60: 2323 2050 6172 616d 6574 7269 7a65 640a  ## Parametrized.
+00004e70: 0a55 7365 7320 6120 7370 6563 6966 6963  .Uses a specific
+00004e80: 204d 696d 656f 204d 6f64 656c 2063 6f6e   Mimeo Model con
+00004e90: 7465 7874 2028 6d6f 6465 6c20 6e61 6d65  text (model name
+00004ea0: 2077 6865 6e20 6063 6f6e 7465 7874 6020   when `context` 
+00004eb0: 6973 206e 6f74 2063 6f6e 6669 6775 7265  is not configure
+00004ec0: 6429 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20  d)...```json.{. 
+00004ed0: 2022 5061 7265 6e74 223a 207b 0a20 2020   "Parent": {.   
+00004ee0: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
+00004ef0: 7b0a 2020 2020 2020 225f 6e61 6d65 223a  {.      "_name":
+00004f00: 2022 6375 7272 5f69 7465 7222 2c0a 2020   "curr_iter",.  
+00004f10: 2020 2020 2263 6f6e 7465 7874 223a 2022      "context": "
+00004f20: 536f 6d65 456e 7469 7479 220a 2020 2020  SomeEntity".    
+00004f30: 7d0a 2020 7d0a 7d0a 6060 600a 0a23 2323  }.  }.}.```..###
+00004f40: 2323 204b 6579 0a0a 4765 6e65 7261 7465  ## Key..Generate
+00004f50: 7320 6120 6b65 7920 756e 6971 7565 2061  s a key unique a
+00004f60: 6372 6f73 7320 616c 6c20 4d69 6d65 6f20  cross all Mimeo 
+00004f70: 4d6f 6465 6c73 2061 6e64 2062 6569 6e67  Models and being
+00004f80: 2074 6865 2073 616d 6520 7769 7468 696e   the same within
+00004f90: 2061 2073 696e 676c 6520 4d69 6d65 6f20   a single Mimeo 
+00004fa0: 4d6f 6465 6c20 636f 6e74 6578 742e 0a0a  Model context...
+00004fb0: 7c20 5061 7261 6d65 7465 7220 7c20 5375  | Parameter | Su
+00004fc0: 7070 6f72 7465 6420 7661 6c75 6573 207c  pported values |
+00004fd0: 2020 2020 2020 2020 2020 2020 2020 4465                De
+00004fe0: 6661 756c 7420 2020 2020 2020 2020 2020  fault           
+00004ff0: 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d      |.|:--------
+00005000: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
+00005010: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
+00005020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005030: 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2063  ---------:|.|  c
+00005040: 6f6e 7465 7874 2020 7c20 2020 2020 2060  ontext  |      `
+00005050: 7374 7260 2020 2020 2020 207c 2020 2020  str`       |    
+00005060: 2020 2020 2061 2063 7572 7265 6e74 2063       a current c
+00005070: 6f6e 7465 7874 2020 2020 2020 2020 2020  ontext          
+00005080: 7c0a 7c20 6974 6572 6174 696f 6e20 7c20  |.| iteration | 
+00005090: 2020 2020 2060 696e 7460 2020 2020 2020       `int`      
+000050a0: 207c 2061 2063 7572 7265 6e74 2069 7465   | a current ite
+000050b0: 7261 7469 6f6e 206f 6620 7468 6520 636f  ration of the co
+000050c0: 6e74 6578 7420 7c0a 0a23 2323 2323 2320  ntext |..###### 
+000050d0: 5261 770a 0a55 7365 7320 6120 6b65 7920  Raw..Uses a key 
+000050e0: 6672 6f6d 2074 6865 2063 7572 7265 6e74  from the current
+000050f0: 2063 6f6e 7465 7874 2061 6e64 2069 7465   context and ite
+00005100: 7261 7469 6f6e 2e0a 0a60 6060 6a73 6f6e  ration...```json
+00005110: 0a7b 0a20 2022 4944 223a 2022 7b6b 6579  .{.  "ID": "{key
+00005120: 7d22 0a7d 0a60 6060 0a0a 2323 2323 2323  }".}.```..######
+00005130: 2050 6172 616d 6574 7269 7a65 640a 0a55   Parametrized..U
+00005140: 7365 7320 6120 6b65 7920 6672 6f6d 2074  ses a key from t
+00005150: 6865 2073 7065 6369 6669 6320 636f 6e74  he specific cont
+00005160: 6578 7420 616e 6420 6974 6572 6174 696f  ext and iteratio
+00005170: 6e2e 2020 0a57 6865 6e20 636f 6e74 6578  n.  .When contex
+00005180: 7420 6973 2069 6e64 6963 6174 6564 2061  t is indicated a
+00005190: 6e64 2069 7465 7261 7469 6f6e 2069 7320  nd iteration is 
+000051a0: 6e6f 742c 2074 6865 6e20 7468 6520 6375  not, then the cu
+000051b0: 7272 656e 7420 6974 6572 6174 696f 6e20  rrent iteration 
+000051c0: 2a2a 6f66 2074 6865 2069 6e64 6963 6174  **of the indicat
+000051d0: 6564 2063 6f6e 7465 7874 2a2a 2069 7320  ed context** is 
+000051e0: 6265 696e 6720 7573 6564 2e0a 0a60 6060  being used...```
+000051f0: 6a73 6f6e 0a7b 0a20 2022 536f 6d65 456e  json.{.  "SomeEn
+00005200: 7469 7479 3222 3a20 7b0a 2020 2020 225f  tity2": {.    "_
+00005210: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
+00005220: 2020 2020 2022 5f6e 616d 6522 3a20 226b       "_name": "k
+00005230: 6579 222c 0a20 2020 2020 2022 636f 6e74  ey",.      "cont
+00005240: 6578 7422 3a20 2253 6f6d 6545 6e74 6974  ext": "SomeEntit
+00005250: 7922 2c0a 2020 2020 2020 2269 7465 7261  y",.      "itera
+00005260: 7469 6f6e 223a 2022 7b63 7572 725f 6974  tion": "{curr_it
+00005270: 6572 7d22 0a20 2020 207d 0a20 207d 0a7d  er}".    }.  }.}
+00005280: 0a60 6060 0a0a 2323 2323 2320 4369 7479  .```..##### City
+00005290: 0a0a 4765 6e65 7261 7465 7320 6120 6369  ..Generates a ci
+000052a0: 7479 206e 616d 652e 0a0a 7c20 5061 7261  ty name...| Para
+000052b0: 6d65 7465 7220 7c20 5375 7070 6f72 7465  meter | Supporte
+000052c0: 6420 7661 6c75 6573 207c 2044 6566 6175  d values | Defau
+000052d0: 6c74 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d  lt |.|:---------
+000052e0: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|:-------------
+000052f0: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d3a 7c0a  ---:|:-------:|.
+00005300: 7c20 2075 6e69 7175 6520 2020 7c20 2020  |  unique   |   
+00005310: 2020 2060 626f 6f6c 6020 2020 2020 207c     `bool`      |
+00005320: 2060 5472 7565 6020 207c 0a7c 2020 636f   `True`  |.|  co
+00005330: 756e 7472 7920 207c 2020 2020 2020 6073  untry  |      `s
+00005340: 7472 6020 2020 2020 2020 7c20 604e 6f6e  tr`       | `Non
+00005350: 6560 2020 7c0a 0a23 2323 2323 2320 5261  e`  |..###### Ra
+00005360: 770a 0a42 7920 6465 6661 756c 7420 6369  w..By default ci
+00005370: 7479 206e 616d 6573 2077 696c 6c20 6265  ty names will be
+00005380: 2075 6e69 7175 6520 6163 726f 7373 2061   unique across a
+00005390: 204d 696d 656f 2043 6f6e 7465 7874 2e0a   Mimeo Context..
+000053a0: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 4369  .```json.{.  "Ci
+000053b0: 7479 223a 2022 7b63 6974 797d 220a 7d0a  ty": "{city}".}.
+000053c0: 6060 600a 0a23 2323 2323 2320 5061 7261  ```..###### Para
+000053d0: 6d65 7472 697a 6564 0a0a 5573 6573 2063  metrized..Uses c
+000053e0: 6f75 6e74 7279 2028 6e61 6d65 2c20 6973  ountry (name, is
+000053f0: 6f32 2c20 6973 6f33 2920 616e 6420 6075  o2, iso3) and `u
+00005400: 6e69 7175 6560 2066 6c61 6720 746f 2067  nique` flag to g
+00005410: 656e 6572 6174 6520 6120 6369 7479 206e  enerate a city n
+00005420: 616d 652e 0a0a 6060 606a 736f 6e0a 7b0a  ame...```json.{.
+00005430: 2020 2243 6974 7957 6974 6844 7570 6c69    "CityWithDupli
+00005440: 6361 7465 7322 3a20 7b0a 2020 2020 225f  cates": {.    "_
+00005450: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
+00005460: 2020 2020 2022 5f6e 616d 6522 3a20 2263       "_name": "c
+00005470: 6974 7922 2c0a 2020 2020 2020 2275 6e69  ity",.      "uni
+00005480: 7175 6522 3a20 6661 6c73 650a 2020 2020  que": false.    
+00005490: 7d0a 2020 7d2c 0a20 2022 4369 7479 4f66  }.  },.  "CityOf
+000054a0: 436f 756e 7472 794e 616d 6522 3a20 7b0a  CountryName": {.
+000054b0: 2020 2020 225f 6d69 6d65 6f5f 7574 696c      "_mimeo_util
+000054c0: 223a 207b 0a20 2020 2020 2022 5f6e 616d  ": {.      "_nam
+000054d0: 6522 3a20 2263 6974 7922 2c0a 2020 2020  e": "city",.    
+000054e0: 2020 2263 6f75 6e74 7279 223a 2022 556e    "country": "Un
+000054f0: 6974 6564 204b 696e 6764 6f6d 220a 2020  ited Kingdom".  
+00005500: 2020 7d0a 2020 7d2c 0a20 2022 4369 7479    }.  },.  "City
+00005510: 4f66 436f 756e 7472 7949 534f 3222 3a20  OfCountryISO2": 
+00005520: 7b0a 2020 2020 225f 6d69 6d65 6f5f 7574  {.    "_mimeo_ut
+00005530: 696c 223a 207b 0a20 2020 2020 2022 5f6e  il": {.      "_n
+00005540: 616d 6522 3a20 2263 6974 7922 2c0a 2020  ame": "city",.  
+00005550: 2020 2020 2263 6f75 6e74 7279 223a 2022      "country": "
+00005560: 4742 220a 2020 2020 7d0a 2020 7d2c 0a20  GB".    }.  },. 
+00005570: 2022 4369 7479 4f66 436f 756e 7472 7949   "CityOfCountryI
+00005580: 534f 3322 3a20 7b0a 2020 2020 225f 6d69  SO3": {.    "_mi
+00005590: 6d65 6f5f 7574 696c 223a 207b 0a20 2020  meo_util": {.   
+000055a0: 2020 2022 5f6e 616d 6522 3a20 2263 6974     "_name": "cit
+000055b0: 7922 2c0a 2020 2020 2020 2263 6f75 6e74  y",.      "count
+000055c0: 7279 223a 2022 4742 5222 0a20 2020 207d  ry": "GBR".    }
+000055d0: 0a20 207d 2c0a 2020 2243 6974 794f 6643  .  },.  "CityOfC
+000055e0: 6f75 6e74 7279 5769 7468 4475 706c 6963  ountryWithDuplic
+000055f0: 6174 6573 223a 207b 0a20 2020 2022 5f6d  ates": {.    "_m
+00005600: 696d 656f 5f75 7469 6c22 3a20 7b0a 2020  imeo_util": {.  
+00005610: 2020 2020 225f 6e61 6d65 223a 2022 6369      "_name": "ci
+00005620: 7479 222c 0a20 2020 2020 2022 636f 756e  ty",.      "coun
+00005630: 7472 7922 3a20 2255 6e69 7465 6420 4b69  try": "United Ki
+00005640: 6e67 646f 6d22 2c0a 2020 2020 2020 2275  ngdom",.      "u
+00005650: 6e69 7175 6522 3a20 6661 6c73 650a 2020  nique": false.  
+00005660: 2020 7d0a 2020 7d0a 7d0a 6060 600a 0a23    }.  }.}.```..#
+00005670: 2323 2323 2043 6f75 6e74 7279 0a0a 4765  #### Country..Ge
+00005680: 6e65 7261 7465 7320 6120 636f 756e 7472  nerates a countr
+00005690: 7920 6e61 6d65 2028 6279 2064 6566 6175  y name (by defau
+000056a0: 6c74 292c 2069 736f 3220 6f72 2069 736f  lt), iso2 or iso
+000056b0: 332e 0a0a 7c20 5061 7261 6d65 7465 7220  3...| Parameter 
+000056c0: 7c20 2020 2020 2020 5375 7070 6f72 7465  |       Supporte
+000056d0: 6420 7661 6c75 6573 2020 2020 2020 207c  d values       |
+000056e0: 2044 6566 6175 6c74 2020 7c0a 7c3a 2d2d   Default  |.|:--
+000056f0: 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d  -------:|:------
+00005700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005710: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
+00005720: 2d3a 7c0a 7c20 2075 6e69 7175 6520 2020  -:|.|  unique   
+00005730: 7c20 2020 2020 2020 2020 2020 2060 626f  |            `bo
+00005740: 6f6c 6020 2020 2020 2020 2020 2020 207c  ol`            |
+00005750: 2020 6054 7275 6560 2020 7c0a 7c20 2020    `True`  |.|   
+00005760: 7661 6c75 6520 2020 7c20 6022 6e61 6d65  value   | `"name
+00005770: 2260 2c20 6022 6973 6f33 2260 2c20 6022  "`, `"iso3"`, `"
+00005780: 6973 6f32 2260 207c 2060 226e 616d 6522  iso2"` | `"name"
+00005790: 6020 7c0a 7c20 2063 6f75 6e74 7279 2020  ` |.|  country  
+000057a0: 7c20 2020 2020 2020 2020 2020 2060 7374  |            `st
+000057b0: 7260 2020 2020 2020 2020 2020 2020 207c  r`             |
+000057c0: 2020 604e 6f6e 6560 2020 7c0a 0a23 2323    `None`  |..###
+000057d0: 2323 2320 5261 770a 0a42 7920 6465 6661  ### Raw..By defa
+000057e0: 756c 7420 636f 756e 7472 7920 6e61 6d65  ult country name
+000057f0: 7320 7769 6c6c 2062 6520 756e 6971 7565  s will be unique
+00005800: 2061 6372 6f73 7320 6120 4d69 6d65 6f20   across a Mimeo 
+00005810: 436f 6e74 6578 742e 0a0a 6060 606a 736f  Context...```jso
+00005820: 6e0a 7b0a 2020 2243 6f75 6e74 7279 223a  n.{.  "Country":
+00005830: 2022 7b63 6f75 6e74 7279 7d22 0a7d 0a60   "{country}".}.`
+00005840: 6060 0a0a 2323 2323 2323 2050 6172 616d  ``..###### Param
+00005850: 6574 7269 7a65 640a 0a49 7420 6361 6e20  etrized..It can 
+00005860: 6765 6e65 7261 7465 3a0a 2d20 636f 756e  generate:.- coun
+00005870: 7472 7920 6973 6f33 206f 7220 6973 6f20  try iso3 or iso 
+00005880: 3220 696e 7374 6561 6420 6f66 206e 616d  2 instead of nam
+00005890: 650a 2d20 636f 756e 7472 7920 7769 7468  e.- country with
+000058a0: 2064 7570 6c69 6361 7465 730a 2d20 636f   duplicates.- co
+000058b0: 756e 7472 7920 6e61 6d65 2066 6f72 2061  untry name for a
+000058c0: 2070 726f 7669 6465 6420 6973 6f33 206f   provided iso3 o
+000058d0: 7220 6973 6f32 0a2d 2063 6f75 6e74 7279  r iso2.- country
+000058e0: 2069 736f 3220 666f 7220 6120 7072 6f76   iso2 for a prov
+000058f0: 6964 6564 206e 616d 6520 6f72 2069 736f  ided name or iso
+00005900: 330a 2d20 636f 756e 7472 7920 6973 6f33  3.- country iso3
+00005910: 2066 6f72 2061 2070 726f 7669 6465 6420   for a provided 
+00005920: 6e61 6d65 206f 7220 6973 6f32 0a0a 5768  name or iso2..Wh
+00005930: 656e 2074 6865 2060 636f 756e 7472 7960  en the `country`
+00005940: 2070 6172 616d 2069 7320 7072 6f76 6964   param is provid
+00005950: 6564 2074 6865 6e20 7468 6520 6075 6e69  ed then the `uni
+00005960: 7175 6560 2066 6c61 6720 6973 2069 676e  que` flag is ign
+00005970: 6f72 6564 2e0a 0a60 6060 6a73 6f6e 0a7b  ored...```json.{
+00005980: 0a20 2022 436f 756e 7472 794e 616d 6557  .  "CountryNameW
+00005990: 6974 6844 7570 6c69 6361 7465 7322 3a20  ithDuplicates": 
+000059a0: 7b0a 2020 2020 225f 6d69 6d65 6f5f 7574  {.    "_mimeo_ut
+000059b0: 696c 223a 207b 0a20 2020 2020 2022 5f6e  il": {.      "_n
+000059c0: 616d 6522 3a20 2263 6f75 6e74 7279 222c  ame": "country",
+000059d0: 0a20 2020 2020 2022 756e 6971 7565 223a  .      "unique":
+000059e0: 2066 616c 7365 0a20 2020 207d 0a20 207d   false.    }.  }
+000059f0: 2c0a 2020 2243 6f75 6e74 7279 4953 4f32  ,.  "CountryISO2
+00005a00: 223a 207b 0a20 2020 2022 5f6d 696d 656f  ": {.    "_mimeo
+00005a10: 5f75 7469 6c22 3a20 7b0a 2020 2020 2020  _util": {.      
+00005a20: 225f 6e61 6d65 223a 2022 636f 756e 7472  "_name": "countr
+00005a30: 7922 2c0a 2020 2020 2020 2276 616c 7565  y",.      "value
+00005a40: 223a 2022 6973 6f32 220a 2020 2020 7d0a  ": "iso2".    }.
+00005a50: 2020 7d2c 0a20 2022 436f 756e 7472 7949    },.  "CountryI
+00005a60: 534f 3322 3a20 7b0a 2020 2020 225f 6d69  SO3": {.    "_mi
+00005a70: 6d65 6f5f 7574 696c 223a 207b 0a20 2020  meo_util": {.   
+00005a80: 2020 2022 5f6e 616d 6522 3a20 2263 6f75     "_name": "cou
+00005a90: 6e74 7279 222c 0a20 2020 2020 2022 7661  ntry",.      "va
+00005aa0: 6c75 6522 3a20 2269 736f 3322 0a20 2020  lue": "iso3".   
+00005ab0: 207d 0a20 207d 2c0a 2020 2243 6f75 6e74   }.  },.  "Count
+00005ac0: 7279 4e61 6d65 466f 7249 534f 3322 3a20  ryNameForISO3": 
+00005ad0: 7b0a 2020 2020 225f 6d69 6d65 6f5f 7574  {.    "_mimeo_ut
+00005ae0: 696c 223a 207b 0a20 2020 2020 2022 5f6e  il": {.      "_n
+00005af0: 616d 6522 3a20 2263 6f75 6e74 7279 222c  ame": "country",
+00005b00: 0a20 2020 2020 2022 636f 756e 7472 7922  .      "country"
+00005b10: 3a20 2247 4252 220a 2020 2020 7d0a 2020  : "GBR".    }.  
+00005b20: 7d2c 0a20 2022 436f 756e 7472 7949 534f  },.  "CountryISO
+00005b30: 3246 6f72 4e61 6d65 223a 207b 0a20 2020  2ForName": {.   
+00005b40: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
+00005b50: 7b0a 2020 2020 2020 225f 6e61 6d65 223a  {.      "_name":
+00005b60: 2022 636f 756e 7472 7922 2c0a 2020 2020   "country",.    
+00005b70: 2020 2276 616c 7565 223a 2022 6973 6f32    "value": "iso2
+00005b80: 222c 0a20 2020 2020 2022 636f 756e 7472  ",.      "countr
+00005b90: 7922 3a20 2255 6e69 7465 6420 4b69 6e67  y": "United King
+00005ba0: 646f 6d22 0a20 2020 207d 0a20 207d 0a7d  dom".    }.  }.}
+00005bb0: 0a60 6060 0a0a 2323 2323 2320 4375 7272  .```..##### Curr
+00005bc0: 656e 6379 0a0a 4765 6e65 7261 7465 7320  ency..Generates 
+00005bd0: 6120 6375 7272 656e 6379 2063 6f64 6520  a currency code 
+00005be0: 2862 7920 6465 6661 756c 7429 206f 7220  (by default) or 
+00005bf0: 6e61 6d65 2e0a 0a7c 2050 6172 616d 6574  name...| Paramet
+00005c00: 6572 207c 2020 5375 7070 6f72 7465 6420  er |  Supported 
+00005c10: 7661 6c75 6573 2020 7c20 4465 6661 756c  values  | Defaul
+00005c20: 7420 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d  t  |.|:---------
+00005c30: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|:-------------
+00005c40: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
+00005c50: 3a7c 0a7c 2020 756e 6971 7565 2020 207c  :|.|  unique   |
+00005c60: 2020 2020 2020 2060 626f 6f6c 6020 2020         `bool`   
+00005c70: 2020 2020 7c20 6046 616c 7365 6020 207c      | `False`  |
+00005c80: 0a7c 2020 2076 616c 7565 2020 207c 2060  .|   value   | `
+00005c90: 2263 6f64 6522 602c 2060 226e 616d 6522  "code"`, `"name"
+00005ca0: 6020 7c20 6022 636f 6465 2260 207c 0a7c  ` | `"code"` |.|
+00005cb0: 2020 636f 756e 7472 7920 207c 2020 2020    country  |    
+00005cc0: 2020 2060 7374 7260 2020 2020 2020 2020     `str`        
+00005cd0: 7c20 2060 4e6f 6e65 6020 207c 0a0a 2323  |  `None`  |..##
+00005ce0: 2323 2323 2052 6177 0a0a 4279 2064 6566  #### Raw..By def
+00005cf0: 6175 6c74 2063 6974 7920 6e61 6d65 7320  ault city names 
+00005d00: 7769 6c6c 205f 4e4f 545f 2062 6520 756e  will _NOT_ be un
+00005d10: 6971 7565 2061 6372 6f73 7320 6120 4d69  ique across a Mi
+00005d20: 6d65 6f20 436f 6e74 6578 742e 0a0a 6060  meo Context...``
+00005d30: 606a 736f 6e0a 7b0a 2020 2243 7572 7265  `json.{.  "Curre
+00005d40: 6e63 7922 3a20 227b 6375 7272 656e 6379  ncy": "{currency
+00005d50: 7d22 0a7d 0a60 6060 0a0a 2323 2323 2323  }".}.```..######
+00005d60: 2050 6172 616d 6574 7269 7a65 640a 0a49   Parametrized..I
+00005d70: 7420 6361 6e20 6765 6e65 7261 7465 3a0a  t can generate:.
+00005d80: 2d20 756e 6971 7565 2063 7572 7265 6e63  - unique currenc
+00005d90: 6965 730a 2d20 6375 7272 656e 6379 206e  ies.- currency n
+00005da0: 616d 6520 696e 7374 6561 6420 6f66 2063  ame instead of c
+00005db0: 6f64 650a 2d20 6375 7272 656e 6379 2063  ode.- currency c
+00005dc0: 6f64 6520 6f72 206e 616d 6520 6f66 2061  ode or name of a
+00005dd0: 2073 7065 6369 6669 6320 636f 756e 7472   specific countr
+00005de0: 7920 2875 7369 6e67 2069 736f 332c 2069  y (using iso3, i
+00005df0: 736f 3220 6f72 206e 616d 6529 0a0a 5768  so2 or name)..Wh
+00005e00: 656e 2074 6865 2060 636f 756e 7472 7960  en the `country`
+00005e10: 2070 6172 616d 2069 7320 7072 6f76 6964   param is provid
+00005e20: 6564 2074 6865 6e20 7468 6520 6075 6e69  ed then the `uni
+00005e30: 7175 6560 2066 6c61 6720 6973 2069 676e  que` flag is ign
+00005e40: 6f72 6564 2e0a 0a60 6060 6a73 6f6e 0a7b  ored...```json.{
+00005e50: 0a20 2022 556e 6971 7565 4375 7272 656e  .  "UniqueCurren
+00005e60: 6379 436f 6465 223a 207b 0a20 2020 2022  cyCode": {.    "
+00005e70: 5f6d 696d 656f 5f75 7469 6c22 3a20 7b0a  _mimeo_util": {.
+00005e80: 2020 2020 2020 225f 6e61 6d65 223a 2022        "_name": "
+00005e90: 6375 7272 656e 6379 222c 0a20 2020 2020  currency",.     
+00005ea0: 2022 756e 6971 7565 223a 2074 7275 650a   "unique": true.
+00005eb0: 2020 2020 7d0a 2020 7d2c 0a20 2022 4375      }.  },.  "Cu
+00005ec0: 7272 656e 6379 4e61 6d65 223a 207b 0a20  rrencyName": {. 
+00005ed0: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
+00005ee0: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
+00005ef0: 223a 2022 6375 7272 656e 6379 222c 0a20  ": "currency",. 
+00005f00: 2020 2020 2022 7661 6c75 6522 3a20 226e       "value": "n
+00005f10: 616d 6522 0a20 2020 207d 0a20 207d 2c0a  ame".    }.  },.
+00005f20: 2020 2243 7572 7265 6e63 7943 6f64 6546    "CurrencyCodeF
+00005f30: 6f72 436f 756e 7472 7949 534f 3322 3a20  orCountryISO3": 
+00005f40: 7b0a 2020 2020 225f 6d69 6d65 6f5f 7574  {.    "_mimeo_ut
+00005f50: 696c 223a 207b 0a20 2020 2020 2022 5f6e  il": {.      "_n
+00005f60: 616d 6522 3a20 2263 7572 7265 6e63 7922  ame": "currency"
+00005f70: 2c0a 2020 2020 2020 2263 6f75 6e74 7279  ,.      "country
+00005f80: 223a 2022 4742 5222 0a20 2020 207d 0a20  ": "GBR".    }. 
+00005f90: 207d 2c0a 2020 2243 7572 7265 6e63 794e   },.  "CurrencyN
+00005fa0: 616d 6546 6f72 436f 756e 7472 7949 534f  ameForCountryISO
+00005fb0: 3222 3a20 7b0a 2020 2020 225f 6d69 6d65  2": {.    "_mime
+00005fc0: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
+00005fd0: 2022 5f6e 616d 6522 3a20 2263 7572 7265   "_name": "curre
+00005fe0: 6e63 7922 2c0a 2020 2020 2020 2276 616c  ncy",.      "val
+00005ff0: 7565 223a 2022 6e61 6d65 222c 0a20 2020  ue": "name",.   
+00006000: 2020 2022 636f 756e 7472 7922 3a20 2247     "country": "G
+00006010: 4222 0a20 2020 207d 0a20 207d 2c0a 2020  B".    }.  },.  
+00006020: 2243 7572 7265 6e63 794e 616d 6546 6f72  "CurrencyNameFor
+00006030: 436f 756e 7472 794e 616d 6522 3a20 7b0a  CountryName": {.
+00006040: 2020 2020 225f 6d69 6d65 6f5f 7574 696c      "_mimeo_util
+00006050: 223a 207b 0a20 2020 2020 2022 5f6e 616d  ": {.      "_nam
+00006060: 6522 3a20 2263 7572 7265 6e63 7922 2c0a  e": "currency",.
+00006070: 2020 2020 2020 2276 616c 7565 223a 2022        "value": "
+00006080: 6e61 6d65 222c 0a20 2020 2020 2022 636f  name",.      "co
+00006090: 756e 7472 7922 3a20 2255 6e69 7465 6420  untry": "United 
+000060a0: 4b69 6e67 646f 6d22 0a20 2020 207d 0a20  Kingdom".    }. 
+000060b0: 207d 0a7d 0a60 6060 0a0a 2323 2323 2320   }.}.```..##### 
+000060c0: 4669 7273 7420 4e61 6d65 0a0a 4765 6e65  First Name..Gene
+000060d0: 7261 7465 7320 6120 6669 7273 7420 6e61  rates a first na
+000060e0: 6d65 2e0a 0a7c 2050 6172 616d 6574 6572  me...| Parameter
+000060f0: 207c 2020 2020 2020 5375 7070 6f72 7465   |      Supporte
+00006100: 6420 7661 6c75 6573 2020 2020 2020 7c20  d values      | 
+00006110: 4465 6661 756c 7420 207c 0a7c 3a2d 2d2d  Default  |.|:---
+00006120: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
+00006130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006140: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 3a7c  ---:|:--------:|
+00006150: 0a7c 2020 756e 6971 7565 2020 207c 2020  .|  unique   |  
+00006160: 2020 2020 2020 2020 2060 626f 6f6c 6020           `bool` 
+00006170: 2020 2020 2020 2020 2020 7c20 2060 5472            |  `Tr
+00006180: 7565 6020 207c 0a7c 2020 2020 7365 7820  ue`  |.|    sex 
+00006190: 2020 207c 2060 4d60 2c20 604d 616c 6560     | `M`, `Male`
+000061a0: 2c20 6046 602c 2060 4665 6d61 6c65 6020  , `F`, `Female` 
+000061b0: 7c20 2060 4e6f 6e65 6020 207c 0a0a 2323  |  `None`  |..##
+000061c0: 2323 2323 2052 6177 0a0a 4279 2064 6566  #### Raw..By def
+000061d0: 6175 6c74 2066 6972 7374 206e 616d 6573  ault first names
+000061e0: 2077 696c 6c20 6265 2075 6e69 7175 6520   will be unique 
+000061f0: 6163 726f 7373 2061 204d 696d 656f 2043  across a Mimeo C
+00006200: 6f6e 7465 7874 2e0a 0a60 6060 6a73 6f6e  ontext...```json
+00006210: 0a7b 0a20 2022 4669 7273 744e 616d 6522  .{.  "FirstName"
+00006220: 3a20 227b 6669 7273 745f 6e61 6d65 7d22  : "{first_name}"
+00006230: 0a7d 0a60 6060 0a0a 2323 2323 2323 2050  .}.```..###### P
+00006240: 6172 616d 6574 7269 7a65 640a 0a55 7365  arametrized..Use
+00006250: 7320 7365 7820 2860 4d60 202f 2060 4d61  s sex (`M` / `Ma
+00006260: 6c65 6020 2f20 6046 6020 2f20 6046 656d  le` / `F` / `Fem
+00006270: 616c 6560 2920 616e 6420 6075 6e69 7175  ale`) and `uniqu
+00006280: 6560 2066 6c61 6720 746f 2067 656e 6572  e` flag to gener
+00006290: 6174 6520 6120 6669 7273 7420 6e61 6d65  ate a first name
+000062a0: 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  ...```json.{.  "
+000062b0: 4669 7273 744e 616d 6557 6974 6844 7570  FirstNameWithDup
+000062c0: 6c69 6361 7465 7322 3a20 7b0a 2020 2020  licates": {.    
+000062d0: 225f 6d69 6d65 6f5f 7574 696c 223a 207b  "_mimeo_util": {
+000062e0: 0a20 2020 2020 2022 5f6e 616d 6522 3a20  .      "_name": 
+000062f0: 2266 6972 7374 5f6e 616d 6522 2c0a 2020  "first_name",.  
+00006300: 2020 2020 2275 6e69 7175 6522 3a20 6661      "unique": fa
+00006310: 6c73 650a 2020 2020 7d0a 2020 7d2c 0a20  lse.    }.  },. 
+00006320: 2022 4d61 6c65 4669 7273 744e 616d 6522   "MaleFirstName"
+00006330: 3a20 7b0a 2020 2020 225f 6d69 6d65 6f5f  : {.    "_mimeo_
+00006340: 7574 696c 223a 207b 0a20 2020 2020 2022  util": {.      "
+00006350: 5f6e 616d 6522 3a20 2266 6972 7374 5f6e  _name": "first_n
+00006360: 616d 6522 2c0a 2020 2020 2020 2273 6578  ame",.      "sex
+00006370: 223a 2022 4d22 0a20 2020 207d 0a20 207d  ": "M".    }.  }
+00006380: 2c0a 2020 2246 656d 616c 6546 6972 7374  ,.  "FemaleFirst
+00006390: 4e61 6d65 223a 207b 0a20 2020 2022 5f6d  Name": {.    "_m
+000063a0: 696d 656f 5f75 7469 6c22 3a20 7b0a 2020  imeo_util": {.  
+000063b0: 2020 2020 225f 6e61 6d65 223a 2022 6669      "_name": "fi
+000063c0: 7273 745f 6e61 6d65 222c 0a20 2020 2020  rst_name",.     
+000063d0: 2022 7365 7822 3a20 2246 220a 2020 2020   "sex": "F".    
+000063e0: 7d0a 2020 7d2c 0a20 2022 4d61 6c65 4669  }.  },.  "MaleFi
+000063f0: 7273 744e 616d 6557 6974 6844 7570 6c69  rstNameWithDupli
+00006400: 6361 7465 7322 3a20 7b0a 2020 2020 225f  cates": {.    "_
+00006410: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
+00006420: 2020 2020 2022 5f6e 616d 6522 3a20 2266       "_name": "f
+00006430: 6972 7374 5f6e 616d 6522 2c0a 2020 2020  irst_name",.    
+00006440: 2020 2273 6578 223a 2022 4d22 2c0a 2020    "sex": "M",.  
+00006450: 2020 2020 2275 6e69 7175 6522 3a20 6661      "unique": fa
+00006460: 6c73 650a 2020 2020 7d0a 2020 7d0a 7d0a  lse.    }.  }.}.
+00006470: 6060 600a 0a23 2323 2323 204c 6173 7420  ```..##### Last 
+00006480: 4e61 6d65 0a0a 4765 6e65 7261 7465 7320  Name..Generates 
+00006490: 6120 6c61 7374 206e 616d 652e 0a0a 7c20  a last name...| 
+000064a0: 5061 7261 6d65 7465 7220 7c20 5375 7070  Parameter | Supp
+000064b0: 6f72 7465 6420 7661 6c75 6573 207c 2044  orted values | D
+000064c0: 6566 6175 6c74 2020 7c0a 7c3a 2d2d 2d2d  efault  |.|:----
+000064d0: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
+000064e0: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
+000064f0: 2d2d 2d3a 7c0a 7c20 2075 6e69 7175 6520  ---:|.|  unique 
+00006500: 2020 7c20 2020 2020 2060 626f 6f6c 6020    |      `bool` 
+00006510: 2020 2020 207c 2020 6054 7275 6560 2020       |  `True`  
+00006520: 7c0a 0a23 2323 2323 2320 5261 770a 0a42  |..###### Raw..B
+00006530: 7920 6465 6661 756c 7420 6c61 7374 206e  y default last n
+00006540: 616d 6573 2077 696c 6c20 6265 2075 6e69  ames will be uni
+00006550: 7175 6520 6163 726f 7373 2061 204d 696d  que across a Mim
+00006560: 656f 2043 6f6e 7465 7874 2e0a 0a60 6060  eo Context...```
+00006570: 6a73 6f6e 0a7b 0a20 2022 4c61 7374 4e61  json.{.  "LastNa
+00006580: 6d65 223a 2022 7b6c 6173 745f 6e61 6d65  me": "{last_name
+00006590: 7d22 0a7d 0a60 6060 0a0a 2323 2323 2323  }".}.```..######
+000065a0: 2050 6172 616d 6574 7269 7a65 640a 0a55   Parametrized..U
+000065b0: 7365 7320 6075 6e69 7175 6560 2066 6c61  ses `unique` fla
+000065c0: 6720 746f 2067 656e 6572 6174 6520 6120  g to generate a 
+000065d0: 6c61 7374 206e 616d 652e 0a0a 6060 606a  last name...```j
+000065e0: 736f 6e0a 7b0a 2020 224c 6173 744e 616d  son.{.  "LastNam
+000065f0: 6557 6974 6844 7570 6c69 6361 7465 7322  eWithDuplicates"
+00006600: 3a20 7b0a 2020 2020 225f 6d69 6d65 6f5f  : {.    "_mimeo_
+00006610: 7574 696c 223a 207b 0a20 2020 2020 2022  util": {.      "
+00006620: 5f6e 616d 6522 3a20 226c 6173 745f 6e61  _name": "last_na
+00006630: 6d65 222c 0a20 2020 2020 2022 756e 6971  me",.      "uniq
+00006640: 7565 223a 2066 616c 7365 0a20 2020 207d  ue": false.    }
+00006650: 0a20 207d 0a7d 0a60 6060 0a0a 2323 2320  .  }.}.```..### 
+00006660: 5079 7468 6f6e 204c 6962 0a0a 546f 2067  Python Lib..To g
+00006670: 656e 6572 6174 6520 6461 7461 2075 7369  enerate data usi
+00006680: 6e67 204d 696d 656f 2061 7320 6120 7079  ng Mimeo as a py
+00006690: 7468 6f6e 206c 6962 7261 7279 2079 6f75  thon library you
+000066a0: 206e 6565 6420 3320 636c 6173 7365 733a   need 3 classes:
+000066b0: 0a2a 2060 4d69 6d65 6f43 6f6e 6669 6760  .* `MimeoConfig`
+000066c0: 2028 4120 7079 7468 6f6e 2072 6570 7265   (A python repre
+000066d0: 7365 6e74 6174 696f 6e20 6f66 2061 204d  sentation of a M
+000066e0: 696d 656f 2043 6f6e 6669 6775 7261 7469  imeo Configurati
+000066f0: 6f6e 290a 2a20 604d 696d 656f 436f 6e66  on).* `MimeoConf
+00006700: 6967 4661 6374 6f72 7960 2028 4120 6661  igFactory` (A fa
+00006710: 6374 6f72 7920 7061 7273 696e 6720 6120  ctory parsing a 
+00006720: 4d69 6d65 6f20 436f 6e66 6967 7572 6174  Mimeo Configurat
+00006730: 696f 6e29 0a2a 2060 4d69 6d65 6f67 7261  ion).* `Mimeogra
+00006740: 7068 6020 2861 2063 6c61 7373 2067 656e  ph` (a class gen
+00006750: 6572 6174 696e 6720 616e 6420 636f 6e73  erating and cons
+00006760: 756d 696e 6720 6461 7461 2066 726f 6d20  uming data from 
+00006770: 6120 4d69 6d65 6f20 436f 6e66 6967 7572  a Mimeo Configur
+00006780: 6174 696f 6e29 0a0a 2323 2323 2050 6172  ation)..#### Par
+00006790: 7369 6e67 204d 696d 656f 2043 6f6e 6669  sing Mimeo Confi
+000067a0: 6775 7261 7469 6f6e 0a0a 2323 2323 2320  guration..##### 
+000067b0: 604d 696d 656f 436f 6e66 6967 600a 0a54  `MimeoConfig`..T
+000067c0: 6865 2060 4d69 6d65 6f43 6f6e 6669 6760  he `MimeoConfig`
+000067d0: 2063 6c61 7373 2074 616b 6573 2061 2064   class takes a d
+000067e0: 6963 7469 6f6e 6172 7920 6173 2061 2070  ictionary as a p
+000067f0: 6172 616d 6574 6572 2061 6e64 2069 6e69  arameter and ini
+00006800: 7469 616c 697a 6573 2061 6c6c 2073 6574  tializes all set
+00006810: 7469 6e67 732e 0a0a 6060 6070 7974 686f  tings...```pytho
+00006820: 6e0a 6672 6f6d 206d 696d 656f 2069 6d70  n.from mimeo imp
+00006830: 6f72 7420 4d69 6d65 6f43 6f6e 6669 670a  ort MimeoConfig.
+00006840: 0a63 6f6e 6669 6720 3d20 7b0a 2020 225f  .config = {.  "_
+00006850: 7465 6d70 6c61 7465 735f 223a 205b 0a20  templates_": [. 
+00006860: 2020 207b 0a20 2020 2020 2022 636f 756e     {.      "coun
+00006870: 7422 3a20 3330 2c0a 2020 2020 2020 226d  t": 30,.      "m
+00006880: 6f64 656c 223a 207b 0a20 2020 2020 2020  odel": {.       
+00006890: 2022 536f 6d65 456e 7469 7479 223a 207b   "SomeEntity": {
+000068a0: 0a20 2020 2020 2020 2020 2022 4078 6d6c  .          "@xml
+000068b0: 6e73 223a 2022 6874 7470 3a2f 2f6d 696d  ns": "http://mim
+000068c0: 656f 2e61 7263 682e 636f 6d2f 6465 6661  eo.arch.com/defa
+000068d0: 756c 742d 6e61 6d65 7370 6163 6522 2c0a  ult-namespace",.
+000068e0: 2020 2020 2020 2020 2020 2240 786d 6c6e            "@xmln
+000068f0: 733a 706e 223a 2022 6874 7470 3a2f 2f6d  s:pn": "http://m
+00006900: 696d 656f 2e61 7263 682e 636f 6d2f 7072  imeo.arch.com/pr
+00006910: 6566 6978 6564 2d6e 616d 6573 7061 6365  efixed-namespace
+00006920: 222c 0a20 2020 2020 2020 2020 2022 4368  ",.          "Ch
+00006930: 696c 644e 6f64 6531 223a 2031 2c0a 2020  ildNode1": 1,.  
+00006940: 2020 2020 2020 2020 2243 6869 6c64 4e6f          "ChildNo
+00006950: 6465 3222 3a20 2276 616c 7565 2d32 222c  de2": "value-2",
+00006960: 0a20 2020 2020 2020 2020 2022 4368 696c  .          "Chil
+00006970: 644e 6f64 6533 223a 2054 7275 650a 2020  dNode3": True.  
+00006980: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
+00006990: 2020 2020 7d0a 2020 5d0a 7d0a 6d69 6d65      }.  ].}.mime
+000069a0: 6f5f 636f 6e66 6967 203d 204d 696d 656f  o_config = Mimeo
+000069b0: 436f 6e66 6967 2863 6f6e 6669 6729 0a60  Config(config).`
+000069c0: 6060 0a0a 2323 2323 2320 604d 696d 656f  ``..##### `Mimeo
+000069d0: 436f 6e66 6967 4661 6374 6f72 7960 0a0a  ConfigFactory`..
+000069e0: 546f 2065 6173 696c 7920 7061 7273 6520  To easily parse 
+000069f0: 4d69 6d65 6f20 436f 6e66 6967 7572 6174  Mimeo Configurat
+00006a00: 696f 6e20 796f 7520 6361 6e20 7573 6520  ion you can use 
+00006a10: 7468 6520 604d 696d 656f 436f 6e66 6967  the `MimeoConfig
+00006a20: 4661 6374 6f72 7960 2e0a 4974 2061 6c6c  Factory`..It all
+00006a30: 6f77 7320 796f 7520 746f 2070 726f 7669  ows you to provi
+00006a40: 6465 2061 2072 6177 2063 6f6e 6669 6720  de a raw config 
+00006a50: 6173 3a0a 2a20 6120 6469 6374 696f 6e61  as:.* a dictiona
+00006a60: 7279 0a2a 2061 2073 7472 696e 6769 6669  ry.* a stringifi
+00006a70: 6564 2058 4d4c 206e 6f64 650a 2a20 6120  ed XML node.* a 
+00006a80: 6669 6c65 2070 6174 680a 0a3c 7461 626c  file path..<tabl
+00006a90: 653e 0a20 2020 203c 7472 3e0a 2020 2020  e>.    <tr>.    
+00006aa0: 2020 2020 3c74 683e 3c2f 7468 3e0a 2020      <th></th>.  
+00006ab0: 2020 2020 2020 3c74 683e 4a53 4f4e 3c2f        <th>JSON</
+00006ac0: 7468 3e0a 2020 2020 2020 2020 3c74 683e  th>.        <th>
+00006ad0: 584d 4c3c 2f74 683e 0a20 2020 203c 2f74  XML</th>.    </t
+00006ae0: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+00006af0: 2020 2020 3c74 643e 3c62 3e52 6177 2064      <td><b>Raw d
+00006b00: 6174 613c 2f62 3e3c 2f74 643e 0a20 2020  ata</b></td>.   
+00006b10: 2020 2020 203c 7464 2076 616c 6967 6e3d       <td valign=
+00006b20: 2274 6f70 223e 0a0a 6060 6070 7974 686f  "top">..```pytho
+00006b30: 6e0a 6672 6f6d 206d 696d 656f 2069 6d70  n.from mimeo imp
+00006b40: 6f72 7420 4d69 6d65 6f43 6f6e 6669 6746  ort MimeoConfigF
+00006b50: 6163 746f 7279 0a0a 636f 6e66 6967 203d  actory..config =
+00006b60: 207b 0a20 2022 5f74 656d 706c 6174 6573   {.  "_templates
+00006b70: 5f22 3a20 5b0a 2020 2020 7b0a 2020 2020  _": [.    {.    
+00006b80: 2020 2263 6f75 6e74 223a 2033 302c 0a20    "count": 30,. 
+00006b90: 2020 2020 2022 6d6f 6465 6c22 3a20 7b0a       "model": {.
+00006ba0: 2020 2020 2020 2020 2253 6f6d 6545 6e74          "SomeEnt
+00006bb0: 6974 7922 3a20 7b0a 2020 2020 2020 2020  ity": {.        
+00006bc0: 2020 2240 786d 6c6e 7322 3a20 2268 7474    "@xmlns": "htt
+00006bd0: 703a 2f2f 6d69 6d65 6f2e 6172 6368 2e63  p://mimeo.arch.c
+00006be0: 6f6d 2f64 6566 6175 6c74 2d6e 616d 6573  om/default-names
+00006bf0: 7061 6365 222c 0a20 2020 2020 2020 2020  pace",.         
+00006c00: 2022 4078 6d6c 6e73 3a70 6e22 3a20 2268   "@xmlns:pn": "h
+00006c10: 7474 703a 2f2f 6d69 6d65 6f2e 6172 6368  ttp://mimeo.arch
+00006c20: 2e63 6f6d 2f70 7265 6669 7865 642d 6e61  .com/prefixed-na
+00006c30: 6d65 7370 6163 6522 2c0a 2020 2020 2020  mespace",.      
+00006c40: 2020 2020 2243 6869 6c64 4e6f 6465 3122      "ChildNode1"
+00006c50: 3a20 312c 0a20 2020 2020 2020 2020 2022  : 1,.          "
+00006c60: 4368 696c 644e 6f64 6532 223a 2022 7661  ChildNode2": "va
+00006c70: 6c75 652d 3222 2c0a 2020 2020 2020 2020  lue-2",.        
+00006c80: 2020 2243 6869 6c64 4e6f 6465 3322 3a20    "ChildNode3": 
+00006c90: 5472 7565 0a20 2020 2020 2020 207d 0a20  True.        }. 
+00006ca0: 2020 2020 207d 0a20 2020 207d 0a20 205d       }.    }.  ]
+00006cb0: 0a7d 0a6d 696d 656f 5f63 6f6e 6669 6720  .}.mimeo_config 
+00006cc0: 3d20 4d69 6d65 6f43 6f6e 6669 6746 6163  = MimeoConfigFac
+00006cd0: 746f 7279 2e70 6172 7365 2863 6f6e 6669  tory.parse(confi
+00006ce0: 6729 0a60 6060 0a3c 2f74 643e 0a20 2020  g).```.</td>.   
+00006cf0: 203c 7464 2076 616c 6967 6e3d 2274 6f70   <td valign="top
+00006d00: 223e 0a0a 6060 6070 7974 686f 6e0a 6672  ">..```python.fr
+00006d10: 6f6d 206d 696d 656f 2069 6d70 6f72 7420  om mimeo import 
+00006d20: 4d69 6d65 6f43 6f6e 6669 6746 6163 746f  MimeoConfigFacto
+00006d30: 7279 0a0a 636f 6e66 6967 203d 2028 0a20  ry..config = (. 
+00006d40: 2020 2027 3c6d 696d 656f 5f63 6f6e 6669     '<mimeo_confi
+00006d50: 6775 7261 7469 6f6e 3e27 0a20 2020 2027  guration>'.    '
+00006d60: 2020 2020 3c5f 7465 6d70 6c61 7465 735f      <_templates_
+00006d70: 3e27 0a20 2020 2027 2020 2020 2020 2020  >'.    '        
+00006d80: 3c5f 7465 6d70 6c61 7465 5f3e 270a 2020  <_template_>'.  
+00006d90: 2020 2720 2020 2020 2020 2020 2020 203c    '            <
+00006da0: 636f 756e 743e 3330 3c2f 636f 756e 743e  count>30</count>
+00006db0: 270a 2020 2020 2720 2020 2020 2020 2020  '.    '         
+00006dc0: 2020 203c 6d6f 6465 6c3e 270a 2020 2020     <model>'.    
+00006dd0: 2727 0a20 2020 2027 2020 2020 2020 2020  ''.    '        
+00006de0: 2020 2020 2020 2020 3c53 6f6d 6545 6e74          <SomeEnt
+00006df0: 6974 7927 0a20 2020 2027 2020 2020 2020  ity'.    '      
+00006e00: 2020 2020 2020 2020 2020 2020 2020 786d                xm
+00006e10: 6c6e 733d 2268 7474 703a 2f2f 6d69 6d65  lns="http://mime
+00006e20: 6f2e 6172 6368 2e63 6f6d 2f64 6566 6175  o.arch.com/defau
+00006e30: 6c74 2d6e 616d 6573 7061 6365 2227 0a20  lt-namespace"'. 
+00006e40: 2020 2027 2020 2020 2020 2020 2020 2020     '            
+00006e50: 2020 2020 2020 2020 786d 6c6e 733a 706e          xmlns:pn
+00006e60: 3d22 6874 7470 3a2f 2f6d 696d 656f 2e61  ="http://mimeo.a
+00006e70: 7263 682e 636f 6d2f 7072 6566 6978 6564  rch.com/prefixed
+00006e80: 2d6e 616d 6573 7061 6365 223e 270a 2020  -namespace">'.  
+00006e90: 2020 2720 2020 2020 2020 2020 2020 2020    '             
+00006ea0: 2020 2020 2020 203c 4368 696c 644e 6f64         <ChildNod
+00006eb0: 6531 3e31 3c2f 4368 696c 644e 6f64 6531  e1>1</ChildNode1
+00006ec0: 3e27 0a20 2020 2027 2020 2020 2020 2020  >'.    '        
+00006ed0: 2020 2020 2020 2020 2020 2020 3c70 6e3a              <pn:
+00006ee0: 4368 696c 644e 6f64 6532 3e76 616c 7565  ChildNode2>value
+00006ef0: 2d32 3c2f 706e 3a43 6869 6c64 4e6f 6465  -2</pn:ChildNode
+00006f00: 323e 270a 2020 2020 2720 2020 2020 2020  2>'.    '       
+00006f10: 2020 2020 2020 2020 2020 2020 203c 4368               <Ch
+00006f20: 696c 644e 6f64 6533 3e74 7275 653c 2f43  ildNode3>true</C
+00006f30: 6869 6c64 4e6f 6465 333e 270a 2020 2020  hildNode3>'.    
+00006f40: 2720 2020 2020 2020 2020 2020 2020 2020  '               
+00006f50: 203c 2f53 6f6d 6545 6e74 6974 793e 270a   </SomeEntity>'.
+00006f60: 2020 2020 2727 0a20 2020 2027 2020 2020      ''.    '    
+00006f70: 2020 2020 2020 2020 3c2f 6d6f 6465 6c3e          </model>
+00006f80: 270a 2020 2020 2720 2020 2020 2020 203c  '.    '        <
+00006f90: 2f5f 7465 6d70 6c61 7465 5f3e 270a 2020  /_template_>'.  
+00006fa0: 2020 2720 2020 203c 2f5f 7465 6d70 6c61    '    </_templa
+00006fb0: 7465 735f 3e27 0a20 2020 2027 3c2f 6d69  tes_>'.    '</mi
+00006fc0: 6d65 6f5f 636f 6e66 6967 7572 6174 696f  meo_configuratio
+00006fd0: 6e3e 2729 0a6d 696d 656f 5f63 6f6e 6669  n>').mimeo_confi
+00006fe0: 6720 3d20 4d69 6d65 6f43 6f6e 6669 6746  g = MimeoConfigF
+00006ff0: 6163 746f 7279 2e70 6172 7365 2863 6f6e  actory.parse(con
+00007000: 6669 6729 0a60 6060 0a3c 2f74 643e 0a20  fig).```.</td>. 
+00007010: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+00007020: 2020 2020 2020 2020 3c74 643e 3c62 3e46          <td><b>F
+00007030: 696c 6520 7061 7468 3c2f 623e 3c2f 7464  ile path</b></td
+00007040: 3e0a 2020 2020 2020 2020 3c74 6420 7661  >.        <td va
+00007050: 6c69 676e 3d22 746f 7022 3e0a 0a60 6060  lign="top">..```
+00007060: 7079 7468 6f6e 0a66 726f 6d20 6d69 6d65  python.from mime
+00007070: 6f20 696d 706f 7274 204d 696d 656f 436f  o import MimeoCo
+00007080: 6e66 6967 4661 6374 6f72 790a 0a63 6f6e  nfigFactory..con
+00007090: 6669 6720 3d20 2253 6f6d 6545 6e74 6974  fig = "SomeEntit
+000070a0: 792d 636f 6e66 6967 2e6a 736f 6e22 0a6d  y-config.json".m
+000070b0: 696d 656f 5f63 6f6e 6669 6720 3d20 4d69  imeo_config = Mi
+000070c0: 6d65 6f43 6f6e 6669 6746 6163 746f 7279  meoConfigFactory
+000070d0: 2e70 6172 7365 2863 6f6e 6669 6729 0a60  .parse(config).`
+000070e0: 6060 0a3c 2f74 643e 0a20 2020 203c 7464  ``.</td>.    <td
+000070f0: 2076 616c 6967 6e3d 2274 6f70 223e 0a0a   valign="top">..
+00007100: 6060 6070 7974 686f 6e0a 6672 6f6d 206d  ```python.from m
+00007110: 696d 656f 2069 6d70 6f72 7420 4d69 6d65  imeo import Mime
+00007120: 6f43 6f6e 6669 6746 6163 746f 7279 0a0a  oConfigFactory..
+00007130: 636f 6e66 6967 203d 2022 536f 6d65 456e  config = "SomeEn
+00007140: 7469 7479 2d63 6f6e 6669 672e 786d 6c22  tity-config.xml"
+00007150: 0a6d 696d 656f 5f63 6f6e 6669 6720 3d20  .mimeo_config = 
+00007160: 4d69 6d65 6f43 6f6e 6669 6746 6163 746f  MimeoConfigFacto
+00007170: 7279 2e70 6172 7365 2863 6f6e 6669 6729  ry.parse(config)
+00007180: 0a60 6060 0a3c 2f74 643e 0a20 203c 2f74  .```.</td>.  </t
+00007190: 723e 0a3c 2f74 6162 6c65 3e0a 0a23 2323  r>.</table>..###
+000071a0: 2320 5072 6f63 6573 7369 6e67 204d 696d  # Processing Mim
+000071b0: 656f 2043 6f6e 6669 6775 7261 7469 6f6e  eo Configuration
+000071c0: 0a0a 5573 696e 6720 7468 6520 4d69 6d65  ..Using the Mime
+000071d0: 6f20 6173 2061 2070 7974 686f 6e20 6c69  o as a python li
+000071e0: 6272 6172 7920 796f 7520 6361 6e20 7573  brary you can us
+000071f0: 6520 3220 7072 6f63 6573 7369 6e67 2061  e 2 processing a
+00007200: 7070 726f 6163 6865 733a 0a2a 2073 6571  pproaches:.* seq
+00007210: 7565 6e74 6961 6c20 7072 6f63 6573 7369  uential processi
+00007220: 6e67 0a2a 2070 726f 6365 7373 696e 6720  ng.* processing 
+00007230: 696e 2070 6172 616c 6c65 6c20 2875 7365  in parallel (use
+00007240: 6420 6279 2064 6566 6175 6c74 2069 6e20  d by default in 
+00007250: 4d69 6d65 6f20 434c 4929 0a0a 426f 7468  Mimeo CLI)..Both
+00007260: 206e 6565 6420 7468 6520 604d 696d 656f   need the `Mimeo
+00007270: 6772 6170 6860 2063 6c61 7373 2e0a 0a0a  graph` class....
+00007280: 2323 2323 2320 5365 7175 656e 7469 616c  ##### Sequential
+00007290: 2070 726f 6365 7373 696e 670a 0a53 6571   processing..Seq
+000072a0: 7565 6e74 6961 6c20 7072 6f63 6573 7369  uential processi
+000072b0: 6e67 2069 7320 7072 6574 7479 2073 7472  ng is pretty str
+000072c0: 6169 6768 7466 6f72 7761 7264 2061 6e64  aightforward and
+000072d0: 2063 616e 2062 6520 646f 6e65 2077 6974   can be done wit
+000072e0: 686f 7574 2060 4d69 6d65 6f67 7261 7068  hout `Mimeograph
+000072f0: 6020 696e 7374 616e 7469 6174 696f 6e2e  ` instantiation.
+00007300: 0a0a 2323 2323 2323 2050 726f 6365 7373  ..###### Process
+00007310: 696e 670a 0a54 6f20 7369 6d70 6c79 2070  ing..To simply p
+00007320: 726f 6365 7373 2064 6174 6120 6672 6f6d  rocess data from
+00007330: 2061 204d 696d 656f 2043 6f6e 6669 6775   a Mimeo Configu
+00007340: 7261 7469 6f6e 2079 6f75 2063 616e 2075  ration you can u
+00007350: 7365 2074 6865 2060 4d69 6d65 6f67 7261  se the `Mimeogra
+00007360: 7068 2e70 726f 6365 7373 2829 6020 6d65  ph.process()` me
+00007370: 7468 6f64 3a0a 6060 6070 7974 686f 6e0a  thod:.```python.
+00007380: 6672 6f6d 206d 696d 656f 2069 6d70 6f72  from mimeo impor
+00007390: 7420 4d69 6d65 6f43 6f6e 6669 6746 6163  t MimeoConfigFac
+000073a0: 746f 7279 2c20 4d69 6d65 6f67 7261 7068  tory, Mimeograph
+000073b0: 0a0a 636f 6e66 6967 5f70 6174 6820 3d20  ..config_path = 
+000073c0: 2265 7861 6d70 6c65 732f 312d 696e 7472  "examples/1-intr
+000073d0: 6f64 7563 7469 6f6e 2f30 312d 6261 7369  oduction/01-basi
+000073e0: 632e 6a73 6f6e 220a 6d69 6d65 6f5f 636f  c.json".mimeo_co
+000073f0: 6e66 6967 203d 204d 696d 656f 436f 6e66  nfig = MimeoConf
+00007400: 6967 4661 6374 6f72 792e 7061 7273 6528  igFactory.parse(
+00007410: 636f 6e66 6967 5f70 6174 6829 0a4d 696d  config_path).Mim
+00007420: 656f 6772 6170 682e 7072 6f63 6573 7328  eograph.process(
+00007430: 6d69 6d65 6f5f 636f 6e66 6967 290a 6060  mimeo_config).``
+00007440: 600a 0a49 7420 7769 6c6c 2067 656e 6572  `..It will gener
+00007450: 6174 6520 6461 7461 2061 6e64 2063 6f6e  ate data and con
+00007460: 7375 6d65 2069 7420 696d 6d65 6469 6174  sume it immediat
+00007470: 656c 792e 0a0a 2323 2323 2323 2047 656e  ely...###### Gen
+00007480: 6572 6174 696e 6720 6f6e 6c79 0a0a 4966  erating only..If
+00007490: 2079 6f75 2772 6520 676f 696e 6720 746f   you're going to
+000074a0: 2067 656e 6572 6174 6520 6461 7461 2061   generate data a
+000074b0: 6e64 2075 7365 2069 7420 6173 2061 2070  nd use it as a p
+000074c0: 7974 686f 6e20 7265 7072 6573 656e 7461  ython representa
+000074d0: 7469 6f6e 0a28 6064 6963 7460 2c20 6078  tion.(`dict`, `x
+000074e0: 6d6c 2e65 7472 6565 2e45 6c65 6d65 6e74  ml.etree.Element
+000074f0: 5472 6565 2e45 6c65 6d65 6e74 6029 202d  Tree.Element`) -
+00007500: 2075 7365 2060 4d69 6d65 6f67 7261 7068   use `Mimeograph
+00007510: 2e67 656e 6572 6174 6528 2960 206d 6574  .generate()` met
+00007520: 686f 643a 0a60 6060 7079 7468 6f6e 0a66  hod:.```python.f
+00007530: 726f 6d20 6d69 6d65 6f20 696d 706f 7274  rom mimeo import
+00007540: 204d 696d 656f 436f 6e66 6967 4661 6374   MimeoConfigFact
+00007550: 6f72 792c 204d 696d 656f 6772 6170 680a  ory, Mimeograph.
+00007560: 0a63 6f6e 6669 675f 7061 7468 203d 2022  .config_path = "
+00007570: 6578 616d 706c 6573 2f31 2d69 6e74 726f  examples/1-intro
+00007580: 6475 6374 696f 6e2f 3031 2d62 6173 6963  duction/01-basic
+00007590: 2e6a 736f 6e22 0a6d 696d 656f 5f63 6f6e  .json".mimeo_con
+000075a0: 6669 6720 3d20 4d69 6d65 6f43 6f6e 6669  fig = MimeoConfi
+000075b0: 6746 6163 746f 7279 2e70 6172 7365 2863  gFactory.parse(c
+000075c0: 6f6e 6669 675f 7061 7468 290a 6461 7461  onfig_path).data
+000075d0: 203d 204d 696d 656f 6772 6170 682e 6765   = Mimeograph.ge
+000075e0: 6e65 7261 7465 286d 696d 656f 5f63 6f6e  nerate(mimeo_con
+000075f0: 6669 6729 0a60 6060 0a0a 2323 2323 2323  fig).```..######
+00007600: 2047 656e 6572 6174 696e 6720 616e 6420   Generating and 
+00007610: 636f 6e73 756d 696e 6720 696e 2032 2073  consuming in 2 s
+00007620: 7461 6765 730a 0a49 6e20 6361 7365 2079  tages..In case y
+00007630: 6f75 2077 6f75 6c64 206c 696b 6520 746f  ou would like to
+00007640: 2073 6f6d 6568 6f77 206d 6f64 6966 7920   somehow modify 
+00007650: 6765 6e65 7261 7465 6420 6461 7461 2062  generated data b
+00007660: 6566 6f72 6520 6974 2077 696c 6c20 6265  efore it will be
+00007670: 2063 6f6e 7375 6d65 642c 0a75 7365 2060   consumed,.use `
+00007680: 4d69 6d65 6f67 7261 7068 2e67 656e 6572  Mimeograph.gener
+00007690: 6174 6528 2960 2061 6e64 2060 4d69 6d65  ate()` and `Mime
+000076a0: 6f67 7261 7068 2e63 6f6e 7375 6d65 2829  ograph.consume()
+000076b0: 6020 6d65 7468 6f64 732e 0a60 6060 7079  ` methods..```py
+000076c0: 7468 6f6e 0a66 726f 6d20 6d69 6d65 6f20  thon.from mimeo 
+000076d0: 696d 706f 7274 204d 696d 656f 436f 6e66  import MimeoConf
+000076e0: 6967 4661 6374 6f72 792c 204d 696d 656f  igFactory, Mimeo
+000076f0: 6772 6170 680a 0a63 6f6e 6669 675f 7061  graph..config_pa
+00007700: 7468 203d 2022 6578 616d 706c 6573 2f31  th = "examples/1
+00007710: 2d69 6e74 726f 6475 6374 696f 6e2f 3031  -introduction/01
+00007720: 2d62 6173 6963 2e6a 736f 6e22 0a6d 696d  -basic.json".mim
+00007730: 656f 5f63 6f6e 6669 6720 3d20 4d69 6d65  eo_config = Mime
+00007740: 6f43 6f6e 6669 6746 6163 746f 7279 2e70  oConfigFactory.p
+00007750: 6172 7365 2863 6f6e 6669 675f 7061 7468  arse(config_path
+00007760: 290a 6461 7461 203d 204d 696d 656f 6772  ).data = Mimeogr
+00007770: 6170 682e 6765 6e65 7261 7465 286d 696d  aph.generate(mim
+00007780: 656f 5f63 6f6e 6669 6729 0a23 202e 2e2e  eo_config).# ...
+00007790: 2079 6f75 7220 6d6f 6469 6669 6361 7469   your modificati
+000077a0: 6f6e 7320 2e2e 2e0a 4d69 6d65 6f67 7261  ons ....Mimeogra
+000077b0: 7068 2e63 6f6e 7375 6d65 286d 696d 656f  ph.consume(mimeo
+000077c0: 5f63 6f6e 6669 672c 2064 6174 6129 0a60  _config, data).`
+000077d0: 6060 0a0a 2323 2323 2320 5072 6f63 6573  ``..##### Proces
+000077e0: 7369 6e67 2069 6e20 7061 7261 6c6c 656c  sing in parallel
+000077f0: 0a0a 5768 656e 2079 6f75 2772 6520 676f  ..When you're go
+00007800: 696e 6720 746f 2070 726f 6365 7373 2064  ing to process d
+00007810: 6174 6120 2867 656e 6572 6174 6520 616e  ata (generate an
+00007820: 6420 636f 6e73 756d 6529 2066 726f 6d20  d consume) from 
+00007830: 7365 7665 7261 6c20 4d69 6d65 6f20 436f  several Mimeo Co
+00007840: 6e66 6967 7572 6174 696f 6e73 0a70 726f  nfigurations.pro
+00007850: 6365 7373 696e 6720 696e 2070 6172 616c  cessing in paral
+00007860: 6c65 6c20 6973 206d 6f72 6520 7065 7266  lel is more perf
+00007870: 6f72 6d61 6e74 2077 6179 2e20 546f 2064  ormant way. To d
+00007880: 6f20 7468 6174 2c20 796f 7520 6e65 6564  o that, you need
+00007890: 2075 7365 2074 6865 2060 4d69 6d65 6f67   use the `Mimeog
+000078a0: 7261 7068 6020 6173 2061 2043 6f6e 7465  raph` as a Conte
+000078b0: 7874 204d 616e 6167 6572 0a61 6e64 2073  xt Manager.and s
+000078c0: 7562 6d69 7420 636f 6e66 6967 7320 746f  ubmit configs to
+000078d0: 6765 7468 6572 2077 6974 6820 736f 6d65  gether with some
+000078e0: 206b 696e 6420 6f66 2069 6465 6e74 6966   kind of identif
+000078f0: 6965 7220 2865 2e67 2e20 636f 6e66 6967  ier (e.g. config
+00007900: 2070 6174 6829 2e20 5468 616e 6b73 2074   path). Thanks t
+00007910: 6f20 7468 6174 2079 6f75 2077 696c 6c20  o that you will 
+00007920: 6b6e 6f77 0a77 6869 6368 2063 6f6e 6669  know.which confi
+00007930: 6720 6861 7320 6661 696c 6564 2028 6966  g has failed (if
+00007940: 2073 6f29 2e0a 0a60 6060 7079 7468 6f6e   so)...```python
+00007950: 0a66 726f 6d20 6d69 6d65 6f20 696d 706f  .from mimeo impo
+00007960: 7274 204d 696d 656f 436f 6e66 6967 4661  rt MimeoConfigFa
+00007970: 6374 6f72 792c 204d 696d 656f 6772 6170  ctory, Mimeograp
+00007980: 680a 0a63 6f6e 6669 675f 7061 7468 7320  h..config_paths 
+00007990: 3d20 5b0a 2020 2020 2265 7861 6d70 6c65  = [.    "example
+000079a0: 732f 312d 696e 7472 6f64 7563 7469 6f6e  s/1-introduction
+000079b0: 2f30 312d 6261 7369 632e 6a73 6f6e 222c  /01-basic.json",
+000079c0: 0a20 2020 2022 6578 616d 706c 6573 2f31  .    "examples/1
+000079d0: 2d69 6e74 726f 6475 6374 696f 6e2f 3032  -introduction/02
+000079e0: 2d63 6f6d 706c 6578 2e6a 736f 6e22 2c0a  -complex.json",.
+000079f0: 2020 2020 2265 7861 6d70 6c65 732f 312d      "examples/1-
+00007a00: 696e 7472 6f64 7563 7469 6f6e 2f30 332d  introduction/03-
+00007a10: 6f75 7470 7574 2d66 6f72 6d61 742d 786d  output-format-xm
+00007a20: 6c2e 6a73 6f6e 222c 0a20 2020 2022 6578  l.json",.    "ex
+00007a30: 616d 706c 6573 2f31 2d69 6e74 726f 6475  amples/1-introdu
+00007a40: 6374 696f 6e2f 3034 2d6f 7574 7075 742d  ction/04-output-
+00007a50: 666f 726d 6174 2d6a 736f 6e2e 6a73 6f6e  format-json.json
+00007a60: 222c 0a5d 0a77 6974 6820 4d69 6d65 6f67  ",.].with Mimeog
+00007a70: 7261 7068 2829 2061 7320 6d69 6d65 6f3a  raph() as mimeo:
+00007a80: 0a20 2020 2066 6f72 2063 6f6e 6669 675f  .    for config_
+00007a90: 7061 7468 2069 6e20 636f 6e66 6967 5f70  path in config_p
+00007aa0: 6174 6873 3a0a 2020 2020 2020 2020 6d69  aths:.        mi
+00007ab0: 6d65 6f5f 636f 6e66 6967 203d 204d 696d  meo_config = Mim
+00007ac0: 656f 436f 6e66 6967 4661 6374 6f72 792e  eoConfigFactory.
+00007ad0: 7061 7273 6528 636f 6e66 6967 5f70 6174  parse(config_pat
+00007ae0: 6829 0a20 2020 2020 2020 206d 696d 656f  h).        mimeo
+00007af0: 5f63 6f6e 6669 672e 6f75 7470 7574 2e64  _config.output.d
+00007b00: 6972 6563 7469 6f6e 203d 2022 7374 646f  irection = "stdo
+00007b10: 7574 220a 2020 2020 2020 2020 6d69 6d65  ut".        mime
+00007b20: 6f2e 7375 626d 6974 2828 636f 6e66 6967  o.submit((config
+00007b30: 5f70 6174 682c 206d 696d 656f 5f63 6f6e  _path, mimeo_con
+00007b40: 6669 6729 290a 6060 600a 0a23 2320 4c69  fig)).```..## Li
+00007b50: 6365 6e73 650a 0a4d 4954 0a0a 0a23 2320  cense..MIT...## 
+00007b60: 4175 7468 6f72 730a 0a2d 205b 4054 6f6d  Authors..- [@Tom
+00007b70: 6173 7a41 6e69 6f6c 6f77 736b 695d 2868  aszAniolowski](h
+00007b80: 7474 7073 3a2f 2f77 7777 2e67 6974 6875  ttps://www.githu
+00007b90: 622e 636f 6d2f 546f 6d61 737a 416e 696f  b.com/TomaszAnio
+00007ba0: 6c6f 7773 6b69 290a 0a0a 2323 2041 636b  lowski)...## Ack
+00007bb0: 6e6f 776c 6564 6765 6d65 6e74 730a 0a20  nowledgements.. 
+00007bc0: 2d20 5b53 696d 706c 654d 6170 732e 636f  - [SimpleMaps.co
+00007bd0: 6d5d 2868 7474 7073 3a2f 2f73 696d 706c  m](https://simpl
+00007be0: 656d 6170 732e 636f 6d2f 6461 7461 2f77  emaps.com/data/w
+00007bf0: 6f72 6c64 2d63 6974 6965 7329 2028 4369  orld-cities) (Ci
+00007c00: 7469 6573 2026 2063 6f75 6e74 7269 6573  ties & countries
+00007c10: 2064 6174 6129 0a20 2d20 5b40 6861 646c   data). - [@hadl
+00007c20: 6579 2f64 6174 612d 6261 6279 2d6e 616d  ey/data-baby-nam
+00007c30: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00007c40: 7562 2e63 6f6d 2f68 6164 6c65 792f 6461  ub.com/hadley/da
+00007c50: 7461 2d62 6162 792d 6e61 6d65 732f 2920  ta-baby-names/) 
+00007c60: 2846 6f72 656e 616d 6573 2064 6174 6129  (Forenames data)
+00007c70: 0a20 2d20 5b40 6669 7665 7468 6972 7479  . - [@fivethirty
+00007c80: 6569 6768 2f64 6174 612f 6d6f 7374 2d63  eigh/data/most-c
+00007c90: 6f6d 6d6f 6e2d 6e61 6d65 5d28 6874 7470  ommon-name](http
+00007ca0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
+00007cb0: 6976 6574 6869 7274 7965 6967 6874 2f64  ivethirtyeight/d
+00007cc0: 6174 612f 7472 6565 2f6d 6173 7465 722f  ata/tree/master/
+00007cd0: 6d6f 7374 2d63 6f6d 6d6f 6e2d 6e61 6d65  most-common-name
+00007ce0: 2920 2853 7572 6e61 6d65 7320 6461 7461  ) (Surnames data
+00007cf0: 290a 202d 205b 4064 6174 6173 6574 732f  ). - [@datasets/
+00007d00: 6375 7272 656e 6379 2d63 6f64 6573 5d28  currency-codes](
+00007d10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00007d20: 6f6d 2f64 6174 6173 6574 732f 6375 7272  om/datasets/curr
+00007d30: 656e 6379 2d63 6f64 6573 2f29 2028 4375  ency-codes/) (Cu
+00007d40: 7272 656e 6369 6573 2064 6174 6129 0a    rrencies data).
```

### Comparing `mimeograph-0.7.0/pyproject.toml` & `mimeograph-1.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "0.7.0"
-description = "Generate data based on a simple template"
+version = "1.0.3"
+description = "Generate NoSQL data based on a simple template"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Database",
     "Topic :: Software Development",
     "Topic :: Software Development :: Testing",
     "Topic :: Utilities",
 ]
-keywords = ["mimeograph", "mimeo", "generate", "generator", "data", "xml"]
+keywords = ["mimeograph", "mimeo", "generate", "generator", "data", "xml", "json", "nosql"]
 dependencies = [
     "xmltodict",
     "aiohttp",
     "aiofiles",
     "pandas",
     "pyyaml",
     "haggis"
@@ -61,15 +61,15 @@
     "pytest-asyncio"
 ]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "0.7.0"
+current_version = "1.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
@@ -98,15 +98,16 @@
     "src/mimeo/context/__init__.py",
     "src/mimeo/generators/__init__.py"
 ]
 
 [tool.ruff]
 select = [
     "F", "E", "W", "C90", "N", "D", "UP", "B", "A", "COM", "C4", "EM", "EXE", "ISC", "G", "PIE", "T20",
-    "PT", "Q", "RSE", "RET", "SLF", "SIM", "ARG", "PTH", "ERA", "PD", "PGH", "PL", "TRY", "RUF", "FLY"
+    "PT", "Q", "RSE", "RET", "SLF", "SIM", "ARG", "PTH", "ERA", "PD", "PGH", "PL", "TRY", "RUF", "FLY",
+    "ASYNC", "FA", "FIX"
 ]
 ignore = []
 exclude = [
     ".git",
     ".github",
     ".idea",
     ".pytest_cache",
@@ -131,15 +132,16 @@
 "scripts/*" = [
     "T20" # allow for print in scripts
 ]
 "tests/*" = [
     "D", # disable pydocstyle for tests
     "EM101", # allow string literals in exceptions' tests
     "PLC1901", # allow comparison to blank string in tests
-    "PLR2004" # allow magic values in tests
+    "PLR2004", # allow magic values in tests
+    "SLF001" # allow private members access in tests
 ]
 "src/mimeo/consumers/raw_consumer.py" = [
     "T20" # allow for print in raw consumer
 ]
 "src/mimeo/logging/filters.py" = [
     "A003" # an external superclass
 ]
```

### Comparing `mimeograph-0.7.0/src/mimeo/__init__.py` & `mimeograph-1.0.3/src/mimeo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,18 +37,20 @@
     The Mimeo Utils package
 
 The same apply to the following modules included by the Mimeo package:
 * mimeo
     The Mimeo module
 * tools
     The Mimeo Tools module
+* exc
+    The Mimeograph Exceptions module.
 
 To use this package, simply import the desired classes:
     from mimeo import MimeoConfig, Mimeograph
 """
 from __future__ import annotations
 
 from .config import MimeoConfig, MimeoConfigFactory
 from .mimeo import Mimeograph
 
-__version__ = "0.7.0"
+__version__ = "1.0.3"
 __all__ = ["MimeoConfig", "MimeoConfigFactory", "Mimeograph"]
```

### Comparing `mimeograph-0.7.0/src/mimeo/cli/__init__.py` & `mimeograph-1.0.3/src/mimeo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/cli/exc.py` & `mimeograph-1.0.3/src/mimeo/cli/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/cli/job.py` & `mimeograph-1.0.3/src/mimeo/cli/job.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 It exports a single class:
     * MimeoJob
         A class representing a single Mimeo processing job.
 """
 from __future__ import annotations
 
-import asyncio
 import logging
 from argparse import Namespace
 from os import walk
 from pathlib import Path
 
 from mimeo import MimeoConfig, Mimeograph
 from mimeo.cli import MimeoArgumentParser, MimeoConfigParser
@@ -34,63 +33,75 @@
         Executes a Mimeo Job based on the CLI arguments.
     """
 
     def __init__(
             self,
     ):
         """Initialize MimeoJob class."""
-        self._args = MimeoArgumentParser().parse_args()
+        self._args: Namespace = MimeoArgumentParser().parse_args()
 
     def run(
             self,
     ):
         """Execute a Mimeo Job based on the CLI arguments.
 
-        First it customizes a log level. After that all Mimeo Configs
-        paths are collected. Each of them is used in the next steps,
-        which are: (1) parsing the configuration and (2) processing
-        it.
+        First it customizes a log level. After that all Mimeo Configs paths are
+        collected. Each of them is used in the next steps, which are: (1) parsing
+        the configuration and (2) processing it. Depending on arguments provided,
+        it processes configs sequentially or in parallel.
         """
         self._customize_log_level(self._args)
         logger.info("Starting a Mimeo job")
-        for config_path in self._get_config_paths(self._args.paths):
-            mimeo_config = self._get_mimeo_config(config_path, self._args)
-            asyncio.run(
-                Mimeograph(mimeo_config).process(),
-            )
+        if self._args.sequentially:
+            self._process_sequentially()
+        else:
+            self._process_in_parallel()
 
     @staticmethod
     def _customize_log_level(
             args,
     ):
         """Customize the log level based on command line arguments."""
         if args.silent:
             logging.getLogger("mimeo").setLevel(logging.WARNING)
         elif args.debug:
             logging.getLogger("mimeo").setLevel(logging.DEBUG)
         elif args.fine and hasattr(logging, "FINE"):
             logging.getLogger("mimeo").setLevel(logging.FINE)
 
+    def _process_sequentially(self):
+        config_paths = self._get_config_paths(self._args.paths)
+        for config_path in config_paths:
+            mimeo_config = self._get_mimeo_config(config_path, self._args)
+            Mimeograph.process(mimeo_config)
+
+    def _process_in_parallel(self):
+        config_paths = self._get_config_paths(self._args.paths)
+        with Mimeograph() as mimeo:
+            for config_path in config_paths:
+                mimeo_config = self._get_mimeo_config(config_path, self._args)
+                mimeo.submit((config_path, mimeo_config))
+
     @staticmethod
     def _get_config_paths(
-            paths: list,
-    ) -> list:
+            paths: list[str],
+    ) -> list[str]:
         """Collect Mimeo Configuration paths.
 
         This method traverses directory paths and collects all files
         within.
 
         Parameters
         ----------
-        paths : list
+        paths : list[str]
             A list of paths provided in command line
 
         Returns
         -------
-        file_paths : list
+        file_paths : list[str]
             A list of file paths
         """
         file_paths = []
         for file_path in paths:
             if Path(file_path).is_dir():
                 for dir_path, _, file_names in walk(file_path):
                     for file_name in file_names:
```

### Comparing `mimeograph-0.7.0/src/mimeo/cli/parsers.py` & `mimeograph-1.0.3/src/mimeo/cli/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 """
 from __future__ import annotations
 
 import json
 import logging
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
+from typing import ClassVar
 
 from mimeo import MimeoConfig
 from mimeo.cli.exc import (EnvironmentNotFoundError,
                            EnvironmentsFileNotFoundError)
 from mimeo.config import MimeoConfigFactory
 from mimeo.config import constants as cc
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_ENVS_PATH = "mimeo.envs.json"
+DEFAULT_ENVS_PATH: str = "mimeo.envs.json"
 
 
 class MimeoArgumentParser(ArgumentParser):
     """A custom ArgumentParser for the Mimeo CLI."""
 
     def __init__(
             self,
@@ -45,14 +46,16 @@
           paths                 take paths to Mimeo Configuration files
 
         optional arguments:
           -h, --help            show this help message and exit
           -v, --version         show program's version number and exit
 
         Mimeo Configuration arguments:
+          -F {xml,json}, --format {xml,json}
+                                overwrite the output/format property
           -o {file,stdout,http}, --output {file,stdout,http}
                                 overwrite the output/direction property
           -x {true,false}, --xml-declaration {true,false}
                                 overwrite the output/xml_declaration property
           -i INDENT, --indent INDENT
                                 overwrite the output/indent property
           -d DIRECTORY_PATH, --directory DIRECTORY_PATH
@@ -75,49 +78,62 @@
                                 overwrite the output/protocol property
           -e ENVIRONMENT, --http-env ENVIRONMENT
                                 overwrite the output http properties using a mimeo
                                 env configuration
           --http-envs-file PATH
                                 use a custom environments file
                                 (by default: mimeo.envs.json)
+          --raw
+                                same as -o stdout
+                                overwrite the output/direction property to stdout
 
         Logging arguments:
           --silent              disable INFO logs
           --debug               enable DEBUG mode
           --fine                enable FINE mode
+
+        Other arguments:
+          --sequentially        process Mimeo Configurations in a single thread
         """
         super().__init__(
             prog="mimeo",
             description="Generate data based on a template",
             usage="%(prog)s [OPTIONS] paths")
         self._add_positional_arguments()
         self._add_mimeo_configuration_arguments()
         self._add_logging_arguments()
+        self._add_other_arguments()
 
     def _add_positional_arguments(
             self,
     ):
         """Add positional arguments."""
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v0.7.0")
+            version="%(prog)s v1.0.3")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configuration files")
 
     def _add_mimeo_configuration_arguments(
             self,
     ):
         """Add arguments overwriting Mimeo Configuration."""
         mimeo_config_args = self.add_argument_group("Mimeo Configuration arguments")
         mimeo_config_args.add_argument(
+            "-F",
+            "--format",
+            type=str,
+            choices=["xml", "json"],
+            help="overwrite the output/format property")
+        mimeo_config_args.add_argument(
             "-o",
             "--output",
             type=str,
             choices=["file", "stdout", "http"],
             help="overwrite the output/direction property")
         mimeo_config_args.add_argument(
             "-x",
@@ -189,14 +205,19 @@
             metavar="ENVIRONMENT",
             help="overwrite the output http properties using a mimeo env configuration")
         mimeo_config_args.add_argument(
             "--http-envs-file",
             type=str,
             metavar="PATH",
             help=f"use a custom environments file (by default: {DEFAULT_ENVS_PATH})")
+        mimeo_config_args.add_argument(
+            "--raw",
+            action="store_true",
+            help="same as -o stdout - "
+                 "overwrite the output/direction property to stdout")
 
     def _add_logging_arguments(
             self,
     ):
         """Add arguments customizing logs producing."""
         logging_args = self.add_argument_group("Logging arguments")
         logging_args_excl = logging_args.add_mutually_exclusive_group()
@@ -209,33 +230,47 @@
             action="store_true",
             help="enable DEBUG mode")
         logging_args_excl.add_argument(
             "--fine",
             action="store_true",
             help="enable FINE mode")
 
+    def _add_other_arguments(
+            self,
+    ):
+        """Add other arguments."""
+        other_args = self.add_argument_group("Other arguments")
+        other_args.add_argument(
+            "--sequentially",
+            action="store_true",
+            help="process Mimeo Configurations in a single thread")
+
 
 class MimeoConfigParser:
     """A class parsing source Mimeo Configuration with Mimeo arguments.
 
     Methods
     -------
     parse_config() -> MimeoConfig
         Parse a Mimeo Configuration using Mimeo arguments.
     """
 
-    _ENVIRONMENT_PROPS = [cc.OUTPUT_PROTOCOL_KEY,
-                          cc.OUTPUT_HOST_KEY,
-                          cc.OUTPUT_PORT_KEY,
-                          cc.OUTPUT_USERNAME_KEY,
-                          cc.OUTPUT_PASSWORD_KEY]
-
-    _ENTRY_PATH_KEY = "entry_path"
-    _GET_VALUE_KEY = "get_value"
-    _ARGS_MAPPING = {
+    _ENVIRONMENT_PROPS: ClassVar[list] = [
+        cc.OUTPUT_PROTOCOL_KEY,
+        cc.OUTPUT_HOST_KEY,
+        cc.OUTPUT_PORT_KEY,
+        cc.OUTPUT_USERNAME_KEY,
+        cc.OUTPUT_PASSWORD_KEY]
+
+    _ENTRY_PATH_KEY: str = "entry_path"
+    _GET_VALUE_KEY: str = "get_value"
+    _ARGS_MAPPING: ClassVar[dict] = {
+        "format": {
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_FORMAT_KEY],
+        },
         "output": {
             "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_DIRECTION_KEY],
         },
         "xml_declaration": {
             "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_XML_DECLARATION_KEY],
             "get_value": lambda arg: arg.lower() == "true",
         },
@@ -281,16 +316,16 @@
         Parameters
         ----------
         config_path: str
             A source config path
         args: Namespace
             Arguments parsed by MimeoArgumentParser
         """
-        self._raw_config = MimeoConfigFactory.parse_source(config_path)
-        self._args = args
+        self._raw_config: dict = MimeoConfigFactory.parse_source(config_path)
+        self._args: Namespace = args
 
     def parse_config(
             self,
     ) -> MimeoConfig:
         """Parse a Mimeo Configuration using Mimeo arguments.
 
         The parsing is made according to the following rule:
@@ -374,14 +409,16 @@
         Returns
         -------
         config : dict
             An overwritten Mimeo Configuration dictionary when
             some configuration arguments have been provided. Otherwise,
             the source one, without any modification.
         """
+        if self._args.raw:
+            self._args.output = "stdout"
         for arg_name, mapping in self._ARGS_MAPPING.items():
             arg = getattr(self._args, arg_name, None)
             if arg is not None:
                 entry_path = mapping.get(self._ENTRY_PATH_KEY, arg_name)
                 get_value = mapping.get(self._GET_VALUE_KEY, lambda a: a)
                 value = get_value(arg)
                 config = self._overwrite_config_entry(config, entry_path, value)
```

### Comparing `mimeograph-0.7.0/src/mimeo/config/__init__.py` & `mimeograph-1.0.3/src/mimeo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/config/constants.py` & `mimeograph-1.0.3/src/mimeo/config/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,105 +5,111 @@
 
 from mimeo import tools
 
 with tools.get_resource("constants.yaml") as config_file:
     constants = yaml.safe_load(config_file.read())
     _cc = constants["mimeo-config"]
 
-CONFIG_XML_ROOT_NAME = _cc["key"]
+CONFIG_XML_ROOT_NAME: str = _cc["key"]
 
 ########################################################################################
 #                                    OUTPUT DETAILS                                    #
 ########################################################################################
 _output_constants = _cc["output"]
-OUTPUT_KEY = _output_constants["key"]
-OUTPUT_FORMAT_KEY = _output_constants["format"]["key"]
-OUTPUT_DIRECTION_KEY = _output_constants["direction"]["key"]
+OUTPUT_KEY: str = _output_constants["key"]
+OUTPUT_FORMAT_KEY: str = _output_constants["format"]["key"]
+OUTPUT_DIRECTION_KEY: str = _output_constants["direction"]["key"]
 
 ########################################################################################
 # --------------------------------- format specific ---------------------------------- #
-_format_details = _output_constants["format"]["values"]
-SUPPORTED_OUTPUT_FORMATS = tuple(format_["key"] for format_ in _format_details.values())
-OUTPUT_FORMAT_XML = _format_details["xml"]["key"]
+_format_details = _output_constants["format"]["details"]
+OUTPUT_INDENT_KEY: str = _format_details["indent"]["key"]
+
+_format_values = _output_constants["format"]["values"]
+SUPPORTED_OUTPUT_FORMATS: tuple = tuple(
+    format_["key"]
+    for format_ in _format_values.values())
+OUTPUT_FORMAT_XML: str = _format_values["xml"]["key"]
+OUTPUT_FORMAT_JSON: str = _format_values["json"]["key"]
 
 # -------------------------------- xml format specific ------------------------------- #
-_xml_format_details = _format_details["xml"]["details"]
-OUTPUT_XML_DECLARATION_KEY = _xml_format_details["xml-declaration"]["key"]
-OUTPUT_INDENT_KEY = _xml_format_details["indent"]["key"]
+_xml_format_details = _format_values["xml"]["details"]
+OUTPUT_XML_DECLARATION_KEY: str = _xml_format_details["xml-declaration"]["key"]
 
 ########################################################################################
 # -------------------------------- direction specific -------------------------------- #
 _direction_details = _output_constants["direction"]["values"]
-SUPPORTED_OUTPUT_DIRECTIONS = tuple(
+SUPPORTED_OUTPUT_DIRECTIONS: tuple = tuple(
     direction["key"]
     for direction in _direction_details.values())
-OUTPUT_DIRECTION_FILE = _direction_details["file"]["key"]
-OUTPUT_DIRECTION_STD_OUT = _direction_details["std-out"]["key"]
-OUTPUT_DIRECTION_HTTP = _direction_details["http"]["key"]
+OUTPUT_DIRECTION_FILE: str = _direction_details["file"]["key"]
+OUTPUT_DIRECTION_STD_OUT: str = _direction_details["std-out"]["key"]
+OUTPUT_DIRECTION_HTTP: str = _direction_details["http"]["key"]
 
 # ----------------------------- file direction specific ------------------------------ #
 _file_direction_details = _direction_details["file"]["details"]
-OUTPUT_DIRECTORY_PATH_KEY = _file_direction_details["directory-path"]["key"]
-OUTPUT_FILE_NAME_KEY = _file_direction_details["file-name"]["key"]
+OUTPUT_DIRECTORY_PATH_KEY: str = _file_direction_details["directory-path"]["key"]
+OUTPUT_FILE_NAME_KEY: str = _file_direction_details["file-name"]["key"]
 
 # ----------------------------- http direction specific ------------------------------ #
 _http_direction_details = _direction_details["http"]["details"]
-REQUIRED_HTTP_DETAILS = tuple(
+REQUIRED_HTTP_DETAILS: tuple = tuple(
     prop["key"] for prop in _http_direction_details.values()
     if prop.get("required", False) is True)
 
-OUTPUT_METHOD_KEY = _http_direction_details["method"]["key"]
-OUTPUT_PROTOCOL_KEY = _http_direction_details["protocol"]["key"]
-OUTPUT_HOST_KEY = _http_direction_details["host"]["key"]
-OUTPUT_PORT_KEY = _http_direction_details["port"]["key"]
-OUTPUT_ENDPOINT_KEY = _http_direction_details["endpoint"]["key"]
-OUTPUT_USERNAME_KEY = _http_direction_details["username"]["key"]
-OUTPUT_PASSWORD_KEY = _http_direction_details["password"]["key"]
+OUTPUT_METHOD_KEY: str = _http_direction_details["method"]["key"]
+OUTPUT_PROTOCOL_KEY: str = _http_direction_details["protocol"]["key"]
+OUTPUT_HOST_KEY: str = _http_direction_details["host"]["key"]
+OUTPUT_PORT_KEY: str = _http_direction_details["port"]["key"]
+OUTPUT_ENDPOINT_KEY: str = _http_direction_details["endpoint"]["key"]
+OUTPUT_USERNAME_KEY: str = _http_direction_details["username"]["key"]
+OUTPUT_PASSWORD_KEY: str = _http_direction_details["password"]["key"]
 
 _req_method_details = _http_direction_details["method"]["values"]
-SUPPORTED_REQUEST_METHODS = _req_method_details.values()
-OUTPUT_HTTP_REQUEST_POST = _req_method_details["post"]
-OUTPUT_HTTP_REQUEST_PUT = _req_method_details["put"]
+SUPPORTED_REQUEST_METHODS: str = _req_method_details.values()
+OUTPUT_HTTP_REQUEST_POST: str = _req_method_details["post"]
+OUTPUT_HTTP_REQUEST_PUT: str = _req_method_details["put"]
 
 _req_protocol_details = _http_direction_details["protocol"]["values"]
-SUPPORTED_REQUEST_PROTOCOLS = _req_protocol_details.values()
-OUTPUT_PROTOCOL_HTTP = _req_protocol_details["http"]
-OUTPUT_PROTOCOL_HTTPS = _req_protocol_details["https"]
+SUPPORTED_REQUEST_PROTOCOLS: str = _req_protocol_details.values()
+OUTPUT_PROTOCOL_HTTP: str = _req_protocol_details["http"]
+OUTPUT_PROTOCOL_HTTPS: str = _req_protocol_details["https"]
 
 ########################################################################################
 #                                      MIMEO VARS                                      #
 ########################################################################################
 _vars_constants = _cc["vars"]
-VARS_KEY = _vars_constants["key"]
+VARS_KEY: str = _vars_constants["key"]
 
 ########################################################################################
 #                                   MIMEO TEMPLATES                                    #
 ########################################################################################
 _templates_constants = _cc["templates"]
-TEMPLATES_KEY = _templates_constants["key"]
-TEMPLATES_XML_TEMPLATE_TAG = _templates_constants["xml-template-tag"]["key"]
-TEMPLATES_COUNT_KEY = _templates_constants["count"]["key"]
-TEMPLATES_MODEL_KEY = _templates_constants["model"]["key"]
+TEMPLATES_KEY: str = _templates_constants["key"]
+TEMPLATES_XML_TEMPLATE_TAG: str = _templates_constants["xml-template-tag"]["key"]
+TEMPLATES_COUNT_KEY: str = _templates_constants["count"]["key"]
+TEMPLATES_MODEL_KEY: str = _templates_constants["model"]["key"]
 
 ########################################################################################
 # -------------------------------- Mimeo Model level --------------------------------- #
 _model_constants = _templates_constants["model"]
-MODEL_CONTEXT_KEY = _model_constants["context"]["key"]
-MODEL_ATTRIBUTES_KEY = _model_constants["attributes"]["key"]
-MODEL_TEXT_VALUE_KEY = _model_constants["text-node-value"]["key"]
-MODEL_MIMEO_UTIL_KEY = _model_constants["mimeo-util"]["key"]
-MODEL_MIMEO_UTIL_NAME_KEY = _model_constants["mimeo-util"]["name"]["key"]
+MODEL_CONTEXT_KEY: str = _model_constants["context"]["key"]
+MODEL_ATTRIBUTES_KEY: str = _model_constants["attributes"]["key"]
+MODEL_TEXT_VALUE_KEY: str = _model_constants["text-node-value"]["key"]
+MODEL_MIMEO_UTIL_KEY: str = _model_constants["mimeo-util"]["key"]
+MODEL_MIMEO_UTIL_NAME_KEY: str = _model_constants["mimeo-util"]["name"]["key"]
 
 __all__ = [
     "CONFIG_XML_ROOT_NAME",
     "OUTPUT_KEY",
     "OUTPUT_FORMAT_KEY",
     "OUTPUT_DIRECTION_KEY",
     "SUPPORTED_OUTPUT_FORMATS",
     "OUTPUT_FORMAT_XML",
+    "OUTPUT_FORMAT_JSON",
     "OUTPUT_XML_DECLARATION_KEY",
     "OUTPUT_INDENT_KEY",
     "SUPPORTED_OUTPUT_DIRECTIONS",
     "OUTPUT_DIRECTION_FILE",
     "OUTPUT_DIRECTION_STD_OUT",
     "OUTPUT_DIRECTION_HTTP",
     "OUTPUT_DIRECTORY_PATH_KEY",
```

### Comparing `mimeograph-0.7.0/src/mimeo/config/exc.py` & `mimeograph-1.0.3/src/mimeo/config/exc.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,17 +126,17 @@
             An error code for vars not being a dictionary
         ERR_2: str
             An error code for vars with non-atomic values
         ERR_2: str
             An error code for vars with not allowed characters
         """
 
-        ERR_1 = "NOT_A_DICT"
-        ERR_2 = "COMPLEX_VALUE"
-        ERR_3 = "INVALID_NAME"
+        ERR_1: str = "NOT_A_DICT"
+        ERR_2: str = "COMPLEX_VALUE"
+        ERR_3: str = "INVALID_NAME"
 
     def __init__(
             self,
             code: InvalidVarsError.Code,
             **kwargs,
     ):
         """Initialize InvalidVarsError exception with details.
@@ -208,17 +208,17 @@
             An error code for missing root in the Mimeo Model
         ERR_2: str
             An error code for multiple roots in the Mimeo Model
         ERR_2: str
             An error code for invalid context name in Mimeo Model
         """
 
-        ERR_1 = "MISSING_ROOT"
-        ERR_2 = "MULTIPLE_ROOTS"
-        ERR_3 = "INVALID_CONTEXT_NAME"
+        ERR_1: str = "MISSING_ROOT"
+        ERR_2: str = "MULTIPLE_ROOTS"
+        ERR_3: str = "INVALID_CONTEXT_NAME"
 
     def __init__(
             self,
             code: InvalidMimeoModelError.Code,
             **kwargs,
     ):
         """Initialize InvalidMimeoModelError exception with details.
@@ -312,16 +312,16 @@
         ----------
         ERR_1: str
             An error code for missing templates in the Mimeo Configuration
         ERR_2: str
             An error code for invalid templates in the Mimeo Configuration
         """
 
-        ERR_1 = "MISSING_TEMPLATES"
-        ERR_2 = "NOT_AN_ARRAY"
+        ERR_1: str = "MISSING_TEMPLATES"
+        ERR_2: str = "NOT_AN_ARRAY"
 
     def __init__(
             self,
             code: InvalidMimeoConfigError.Code,
             **kwargs,
     ):
         """Initialize InvalidMimeoConfigError exception with details.
```

### Comparing `mimeograph-0.7.0/src/mimeo/config/mimeo_config.py` & `mimeograph-1.0.3/src/mimeo/config/mimeo_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,15 +447,15 @@
         """Initialize MimeoDTO class.
 
         Parameters
         ----------
         source : dict
             The source dictionary for a Mimeo DTO
         """
-        self._source = source
+        self._source: dict = source
 
     def __str__(
             self,
     ) -> str:
         """Return the stringified source dictionary of a DTO."""
         return str(self._source)
 
@@ -483,17 +483,17 @@
 
         Parameters
         ----------
         config : dict
             A source config dictionary
         """
         super().__init__(config)
-        self.output = MimeoOutput(config.get(cc.OUTPUT_KEY, {}))
-        self.vars = self._get_vars(config)
-        self.templates = self._get_templates(config)
+        self.output: MimeoOutput = MimeoOutput(config.get(cc.OUTPUT_KEY, {}))
+        self.vars: dict = self._get_vars(config)
+        self.templates: list[MimeoTemplate] = self._get_templates(config)
 
     @classmethod
     def _get_vars(
             cls,
             config: dict,
     ) -> dict:
         """Extract variables from the source dictionary.
@@ -526,25 +526,25 @@
                 raise InvalidVarsError(InvalidVarsError.Code.ERR_3, var=var)
         return variables
 
     @classmethod
     def _get_templates(
             cls,
             config: dict,
-    ) -> list:
+    ) -> list[MimeoTemplate]:
         """Extract Mimeo Templates from the source dictionary.
 
         Parameters
         ----------
         config : dict
             A source config dictionary
 
         Returns
         -------
-        list
+        list[MimeoTemplate]
             A Mimeo Templates list
 
         Raises
         ------
         InvalidMimeoConfigError
             If (1) the source dictionary does not include the _templates_ key or
             (2) the _templates_ key does not point to a list
@@ -589,15 +589,15 @@
 
     Attributes
     ----------
     direction : str, default 'file'
         The configured output direction
     format : str, default 'xml'
         A Mimeo Configuration output format setting
-    xml_declaration : bool, default False
+    xml_declaration : bool, default None
         A Mimeo Configuration xml declaration setting
     indent : int, default 0
         A Mimeo Configuration indent setting
     directory_path : str, default 'mimeo-output'
         The configured file output directory
     file_name : str, default 'mimeo-output-{}.{output_format}'
         The configured file output file name template
@@ -627,28 +627,28 @@
 
         Parameters
         ----------
         output : dict
             A source config output details dictionary
         """
         super().__init__(output)
-        self.direction = self._get_direction(output)
+        self.direction: str = self._get_direction(output)
         self._validate_output(self.direction, output)
-        self.format = self._get_format(output)
-        self.xml_declaration = output.get(cc.OUTPUT_XML_DECLARATION_KEY, False)
-        self.indent = self._get_indent(output)
-        self.directory_path = self._get_directory_path(self.direction, output)
-        self.file_name = self._get_file_name(self.direction, output, self.format)
-        self.method = self._get_method(self.direction, output)
-        self.protocol = self._get_protocol(self.direction, output)
-        self.host = self._get_host(self.direction, output)
-        self.port = self._get_port(self.direction, output)
-        self.endpoint = self._get_endpoint(self.direction, output)
-        self.username = self._get_username(self.direction, output)
-        self.password = self._get_password(self.direction, output)
+        self.format: str = self._get_format(output)
+        self.xml_declaration: bool = self._get_xml_declaration(output, self.format)
+        self.indent: int = self._get_indent(output)
+        self.directory_path: str = self._get_directory_path(self.direction, output)
+        self.file_name: str = self._get_file_name(self.direction, output, self.format)
+        self.method: str = self._get_method(self.direction, output)
+        self.protocol: str = self._get_protocol(self.direction, output)
+        self.host: str = self._get_host(self.direction, output)
+        self.port: int = self._get_port(self.direction, output)
+        self.endpoint: str = self._get_endpoint(self.direction, output)
+        self.username: str = self._get_username(self.direction, output)
+        self.password: str = self._get_password(self.direction, output)
 
     @staticmethod
     def _get_direction(
             output: dict,
     ) -> str:
         """Extract output direction from the source dictionary.
 
@@ -701,14 +701,39 @@
             raise UnsupportedPropertyValueError(
                 cc.OUTPUT_FORMAT_KEY,
                 output_format,
                 cc.SUPPORTED_OUTPUT_FORMATS)
         return output_format
 
     @staticmethod
+    def _get_xml_declaration(
+            config: dict,
+            output_format: str,
+    ) -> bool | None:
+        """Extract an XML declaration setting from the source dictionary.
+
+        Parameters
+        ----------
+        config : dict
+            A source config dictionary
+        output_format : str
+            The configured output format
+
+        Returns
+        -------
+        bool | None
+            The configured XML declaration setting when the output format is 'xml'.
+            Otherwise, None. If the 'xml_declaration' setting is missing returns
+            False by default.
+        """
+        if output_format == cc.OUTPUT_FORMAT_XML:
+            return config.get(cc.OUTPUT_XML_DECLARATION_KEY, False)
+        return None
+
+    @staticmethod
     def _get_indent(
             config: dict,
     ) -> int:
         """Extract an indent value from the source dictionary.
 
         Parameters
         ----------
@@ -769,14 +794,16 @@
 
         Parameters
         ----------
         direction : str
             The configured output direction
         output : dict
             A source config output details dictionary
+        output_format : str
+            The configured output format
 
         Returns
         -------
         str | None
             The configured output file name template when the output direction is
             'file'. Otherwise, None. If the 'file_name' setting is missing returns
             'mimeo-output-{}.{output_format}' by default.
@@ -888,29 +915,29 @@
             return output.get(cc.OUTPUT_HOST_KEY)
         return None
 
     @staticmethod
     def _get_port(
             direction: str,
             output: dict,
-    ) -> str | None:
+    ) -> int | None:
         """Extract an HTTP port from the source dictionary.
 
         It is extracted only when the output direction is 'http'.
 
         Parameters
         ----------
         direction : str
             The configured output direction
         output : dict
             A source config output details dictionary
 
         Returns
         -------
-        str | None
+        int | None
             The configured HTTP port when the output direction is 'http'.
             Otherwise, None.
         """
         if direction == cc.OUTPUT_DIRECTION_HTTP:
             return output.get(cc.OUTPUT_PORT_KEY)
         return None
 
@@ -1048,16 +1075,16 @@
         Parameters
         ----------
         template : dict
             A source config template dictionary
         """
         super().__init__(template)
         self._validate_template(template)
-        self.count = template.get(cc.TEMPLATES_COUNT_KEY)
-        self.model = MimeoModel(template.get(cc.TEMPLATES_MODEL_KEY))
+        self.count: int = template.get(cc.TEMPLATES_COUNT_KEY)
+        self.model: MimeoModel = MimeoModel(template.get(cc.TEMPLATES_MODEL_KEY))
 
     @staticmethod
     def _validate_template(
             template: dict,
     ) -> None:
         """Validate template in the source dictionary.
 
@@ -1104,17 +1131,17 @@
 
         Parameters
         ----------
         model : dict
             A source config model dictionary
         """
         super().__init__(model)
-        self.root_name = MimeoModel._get_root_name(model)
-        self.root_data = model.get(self.root_name)
-        self.context_name = MimeoModel._get_context_name(model, self.root_name)
+        self.root_name: str = MimeoModel._get_root_name(model)
+        self.root_data: dict = model.get(self.root_name)
+        self.context_name: str = MimeoModel._get_context_name(model, self.root_name)
 
     @staticmethod
     def _get_root_name(
             model: dict,
     ) -> str:
         """Extract a root name from the source dictionary.
```

### Comparing `mimeograph-0.7.0/src/mimeo/consumers/__init__.py` & `mimeograph-1.0.3/src/mimeo/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/consumers/consumer.py` & `mimeograph-1.0.3/src/mimeo/consumers/consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/consumers/consumer_factory.py` & `mimeograph-1.0.3/src/mimeo/consumers/consumer_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
     Methods
     -------
     get_consumer(mimeo_config: MimeoConfig) -> Consumer
         Initialize a Consumer based on the Mimeo Output Direction.
     """
 
-    FILE_DIRECTION = cc.OUTPUT_DIRECTION_FILE
-    STD_OUT_DIRECTION = cc.OUTPUT_DIRECTION_STD_OUT
-    HTTP_DIRECTION = cc.OUTPUT_DIRECTION_HTTP
+    FILE_DIRECTION: str = cc.OUTPUT_DIRECTION_FILE
+    STD_OUT_DIRECTION: str = cc.OUTPUT_DIRECTION_STD_OUT
+    HTTP_DIRECTION: str = cc.OUTPUT_DIRECTION_HTTP
 
     @staticmethod
     def get_consumer(
             mimeo_config: MimeoConfig,
     ) -> Consumer:
         """Initialize a Consumer based on the Mimeo Output Direction.
```

### Comparing `mimeograph-0.7.0/src/mimeo/consumers/file_consumer.py` & `mimeograph-1.0.3/src/mimeo/consumers/file_consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         """Initialize FileConsumer class.
 
         Parameters
         ----------
         output : MimeoOutput
             Configured Mimeo Output Details
         """
-        self.directory = output.directory_path
-        self.output_path_tmplt = f"{self.directory}/{output.file_name}"
+        self.directory: str = output.directory_path
+        self.output_path_tmplt: str = f"{self.directory}/{output.file_name}"
 
     async def consume(
             self,
             data: Collection | Generator,
     ) -> None:
         """Save data generated by Mimeo into a file.
```

### Comparing `mimeograph-0.7.0/src/mimeo/consumers/http_consumer.py` & `mimeograph-1.0.3/src/mimeo/consumers/http_consumer.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import uuid
 from typing import Collection, Generator
 
-import aiohttp
-from aiohttp import ClientSession
+from aiohttp import BasicAuth, ClientSession
 
 from mimeo.config.mimeo_config import MimeoOutput
 from mimeo.consumers import Consumer
 
 logger = logging.getLogger(__name__)
 
 
@@ -47,17 +46,18 @@
         """Initialize HTTPConsumer class.
 
         Parameters
         ----------
         output : MimeoOutput
             Configured Mimeo Output Details
         """
-        self.method = output.method
-        self.url = HttpConsumer.__build_url(output)
-        self.__auth = aiohttp.BasicAuth(output.username, output.password, "utf-8")
+        self.method: str = output.method
+        self.url: str = HttpConsumer.__build_url(output)
+        self.__auth: BasicAuth = BasicAuth(output.username, output.password, "utf-8")
+        self.__content_type: str = f"application/{output.format}"
 
     async def consume(
             self,
             data: Collection | Generator,
     ):
         """Send data generated by Mimeo in an HTTP request.
 
@@ -72,15 +72,15 @@
             req_id = str(uuid.uuid4())
             logger.info("Sending request %s %s [%s]", self.method, self.url, req_id)
             resp = await sess.request(
                 self.method,
                 self.url,
                 auth=self.__auth,
                 data=data_unit,
-                headers={"Content-Type": "application/xml"})
+                headers={"Content-Type": self.__content_type})
             logger.info("[%s] Status: %s", req_id, resp.status)
 
         async with ClientSession() as s:
             await asyncio.gather(*[send_request(s, d) for d in data])
 
     @staticmethod
     def __build_url(
```

### Comparing `mimeograph-0.7.0/src/mimeo/consumers/raw_consumer.py` & `mimeograph-1.0.3/src/mimeo/consumers/raw_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/context/__init__.py` & `mimeograph-1.0.3/src/mimeo/context/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/context/decorators.py` & `mimeograph-1.0.3/src/mimeo/context/decorators.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/context/exc.py` & `mimeograph-1.0.3/src/mimeo/context/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/context/mimeo_context.py` & `mimeograph-1.0.3/src/mimeo/context/mimeo_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,37 +55,37 @@
         Provide next unique currency index.
     next_first_name_index(sex: str = None) -> int
         Provide next unique first name index.
     next_last_name_index() -> int
         Provide next unique last name index.
     """
 
-    _ALL = "_ALL_"
-    _INITIAL_COUNT = "init-count"
-    _INDEXES = "indexes"
+    _ALL: str = "_ALL_"
+    _INITIAL_COUNT: str = "init-count"
+    _INDEXES: str = "indexes"
 
     def __init__(
             self,
             name: str,
     ):
         """Initialize MimeoContext class.
 
         Parameters
         ----------
         name : str
             A context name
         """
-        self.name = name
-        self._id = 0
-        self._iterations = []
-        self._countries_indexes = None
-        self._cities_indexes = {}
-        self._currencies_indexes = None
-        self._first_names_indexes = {}
-        self._last_names_indexes = None
+        self.name: str = name
+        self._id: int = 0
+        self._iterations: list[MimeoIteration] = []
+        self._countries_indexes: list[int] | None = None
+        self._cities_indexes: dict = {}
+        self._currencies_indexes: list[int] | None = None
+        self._first_names_indexes: dict = {}
+        self._last_names_indexes: list[int] | None = None
 
     def next_id(
             self,
     ) -> int:
         """Increment an identifier and return the current (incremented) one.
 
         Identifier is used by Auto Increment Mimeo Util.
@@ -160,15 +160,15 @@
     def curr_iteration(
             self,
     ) -> MimeoIteration:
         """Return the current iteration within the context.
 
         Returns
         -------
-        int
+        MimeoIteration
             The current iteration within the context
 
         Raises
         ------
         UninitializedContextIterationError
             If no iteration has been initialized yet for the context
         """
@@ -235,15 +235,15 @@
         self._initialize_countries_indexes()
         self._validate_countries()
 
         return self._countries_indexes.pop()
 
     def next_city_index(
             self,
-            country: str = None,
+            country: str | None = None,
     ) -> int:
         """Provide next unique city index.
 
         When used for the first time in the specific context
         it populates internal cities' indexes map. Each `country` key
         has its own list initialized as same as country-agnostic one.
         This approach ensures city uniqueness without time-consuming
@@ -303,15 +303,15 @@
         self._initialize_currencies_indexes()
         self._validate_currencies()
 
         return self._currencies_indexes.pop()
 
     def next_first_name_index(
             self,
-            sex: str = None,
+            sex: str | None = None,
     ) -> int:
         """Provide next unique first name index.
 
         When used for the first time in the specific context
         it populates internal first names' indexes map. Each `sex` key
         has its own list initialized as same as sex-agnostic one.
         This approach ensures forename uniqueness without
```

### Comparing `mimeograph-0.7.0/src/mimeo/context/mimeo_context_manager.py` & `mimeograph-1.0.3/src/mimeo/context/mimeo_context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,28 @@
         Set the current Mimeo Context.
     get_var(self, variable_name: str)
         Return a specific Mimeo Var value.
     """
 
     def __init__(
             self,
-            mimeo_config: MimeoConfig = None,
+            mimeo_config: MimeoConfig | None = None,
     ):
         """Initialize MimeoContextManager class.
 
         Parameters
         ----------
         mimeo_config : MimeoConfig
             The Mimeo Configuration
         """
         super().__init__()
-        self._mimeo_config = mimeo_config
-        self._vars = {}
-        self._contexts = {}
-        self._current_context = None
+        self._mimeo_config: MimeoConfig = mimeo_config
+        self._vars: dict = {}
+        self._contexts: dict = {}
+        self._current_context: MimeoContext | None = None
 
     def __enter__(
             self,
     ) -> MimeoContextManager:
         """Enter the MimeoContextManager instance.
 
         Extends Alive __enter__ function and initializes vars.
```

### Comparing `mimeograph-0.7.0/src/mimeo/context/mimeo_iteration.py` & `mimeograph-1.0.3/src/mimeo/context/mimeo_iteration.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         """Initialize MimeoIteration class.
 
         Parameters
         ----------
         identifier : int
             An ordinal number in a Mimeo Context
         """
-        self.id = identifier
-        self.key = str(uuid.uuid4())
-        self._special_fields = {}
+        self.id: identifier = identifier
+        self.key: str = str(uuid.uuid4())
+        self._special_fields: dict = {}
 
     def add_special_field(
             self,
             field_name: str,
             field_value: str | int | bool,
     ):
         """Put a special field entry to memory.
```

### Comparing `mimeograph-0.7.0/src/mimeo/database/__init__.py` & `mimeograph-1.0.3/src/mimeo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/database/cities.py` & `mimeograph-1.0.3/src/mimeo/database/cities.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,18 @@
     * City
         DTO class representing a single row in cities CSV data.
     * CitiesDB
         Class exposing READ operations on cities CSV data.
 """
 from __future__ import annotations
 
+from typing import ClassVar
+
 import pandas
+from pandas import DataFrame
 
 from mimeo import tools
 from mimeo.database.exc import InvalidIndexError
 
 
 class City:
     """DTO class representing a single row in cities CSV data.
@@ -45,18 +48,18 @@
         name : str
             A city name
         name_ascii : str
             A city name in ASCII encoding
         country : str
             A country of a city
         """
-        self.id = int(identifier)
-        self.name = name
-        self.name_ascii = name_ascii
-        self.country = country
+        self.id: int = int(identifier)
+        self.name: str = name
+        self.name_ascii: str = name_ascii
+        self.country: str = country
 
     def __str__(
             self,
     ) -> str:
         """Stringify the City instance.
 
         Returns
@@ -102,19 +105,19 @@
         Get all cities.
     get_cities_of(country_iso3: str) -> list[City]
         Get cities of a specific country.
     get_city_at(index: int) -> City
         Get a city at `index` position.
     """
 
-    NUM_OF_RECORDS = 42905
-    _CITIES_DB = "cities.csv"
-    _CITIES_DF = None
-    _CITIES = None
-    _COUNTRY_CITIES = {}
+    NUM_OF_RECORDS: int = 42905
+    _CITIES_DB: str = "cities.csv"
+    _CITIES_DF: DataFrame = None
+    _CITIES: ClassVar[list] = None
+    _COUNTRY_CITIES: ClassVar[dict] = {}
 
     def get_city_at(
             self,
             index: int,
     ) -> City:
         """Get a city at `index` position.
```

### Comparing `mimeograph-0.7.0/src/mimeo/database/countries.py` & `mimeograph-1.0.3/src/mimeo/database/countries.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,18 @@
         DTO class representing a single row in countries CSV
         data.
     * CountriesDB
         Class exposing READ operations on countries CSV data.
 """
 from __future__ import annotations
 
+from typing import ClassVar
+
 import pandas
+from pandas import DataFrame
 
 from mimeo import tools
 from mimeo.database.exc import InvalidIndexError
 
 
 class Country:
     """DTO class representing a single row in cities CSV data.
@@ -41,17 +44,17 @@
         iso_3 : str
             A country ISO3 code
         iso_2 : str
             A country ISO2 code
         name : str
             A country name
         """
-        self.iso_3 = iso_3
-        self.iso_2 = iso_2
-        self.name = name
+        self.iso_3: str = iso_3
+        self.iso_2: str = iso_2
+        self.name: str = name
 
     def __str__(
             self,
     ) -> str:
         """Stringify the Country instance.
 
         Returns
@@ -99,18 +102,18 @@
         Get a country having a specific ISO3 code.
     get_country_by_iso_3(iso_2: str) -> Country
         Get a country having a specific ISO2 code.
     get_country_by_name(name: str) -> Country
         Get a country having a specific name.
     """
 
-    NUM_OF_RECORDS = 239
-    _COUNTRIES_DB = "countries.csv"
-    _COUNTRIES_DF = None
-    _COUNTRIES = None
+    NUM_OF_RECORDS: int = 239
+    _COUNTRIES_DB: str = "countries.csv"
+    _COUNTRIES_DF: DataFrame = None
+    _COUNTRIES: ClassVar[list] = None
 
     def get_country_at(
             self,
             index: int,
     ) -> Country:
         """Get a country at `index` position.
```

### Comparing `mimeograph-0.7.0/src/mimeo/database/currencies.py` & `mimeograph-1.0.3/src/mimeo/database/currencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,53 +4,56 @@
     * Currency
         DTO class representing a single row in currencies CSV data.
     * CurrenciesDB
         Class exposing READ operations on currencies CSV data.
 """
 from __future__ import annotations
 
+from typing import ClassVar
+
 import pandas
+from pandas import DataFrame
 
 from mimeo import tools
 from mimeo.database.exc import InvalidIndexError
 
 
 class Currency:
     """DTO class representing a single row in currencies CSV data.
 
     Attributes
     ----------
     code : str
         A currency code
     name : str
         A currency name
-    countries : list
+    countries : list[str]
         A countries using the currency
     """
 
     def __init__(
             self,
             code: str,
             name: str,
-            countries: list,
+            countries: list[str],
     ):
         """Initialize Currency class.
 
         Parameters
         ----------
         code : str
             A currency code
         name : str
             A currency name
         countries : list
             A countries using the currency
         """
-        self.code = code
-        self.name = name
-        self.countries = countries
+        self.code: str = code
+        self.name: str = name
+        self.countries: list[str] = countries
 
     def __str__(
             self,
     ) -> str:
         """Stringify the Currency instance.
 
         Returns
@@ -94,19 +97,19 @@
         Get all currencies.
     get_currency_of(country_name: str) -> Currency | None
         Get currency of a specific country.
     get_currency_at(index: int) -> Currency
         Get a currency at `index` position.
     """
 
-    NUM_OF_RECORDS = 169
-    _CURRENCIES_DB = "currencies.csv"
-    _CURRENCIES_DF = None
-    _CURRENCIES = None
-    _COUNTRY_CURRENCIES = {}
+    NUM_OF_RECORDS: int = 169
+    _CURRENCIES_DB: str = "currencies.csv"
+    _CURRENCIES_DF: DataFrame = None
+    _CURRENCIES: ClassVar[list] = None
+    _COUNTRY_CURRENCIES: ClassVar[dict] = {}
 
     def get_currency_at(
             self,
             index: int,
     ) -> Currency:
         """Get a currency at `index` position.
```

### Comparing `mimeograph-0.7.0/src/mimeo/database/exc.py` & `mimeograph-1.0.3/src/mimeo/database/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/database/first_names.py` & `mimeograph-1.0.3/src/mimeo/database/first_names.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,18 @@
     * FirstName
         DTO class representing a single row in forenames CSV data.
     * FirstNamesDB
         Class exposing READ operations on forenames CSV data.
 """
 from __future__ import annotations
 
+from typing import ClassVar
+
 import pandas
+from pandas import DataFrame
 
 from mimeo import tools
 from mimeo.database.exc import InvalidIndexError, InvalidSexError
 
 
 class FirstName:
     """DTO class representing a single row in forenames CSV data.
@@ -35,16 +38,16 @@
         Parameters
         ----------
         name : str
             A first name
         sex : str
             A sex value
         """
-        self.name = name
-        self.sex = sex
+        self.name: str = name
+        self.sex: str = sex
 
     def __str__(
             self,
     ) -> str:
         """Stringify the FirstName instance.
 
         Returns
@@ -86,20 +89,20 @@
         Get all first names.
     get_first_names_by_sex(sex: str) -> list[FirstName]
         Get first names for a specific sex.
     get_first_name_at(index: int) -> FirstName
         Get a first name at `index` position.
     """
 
-    NUM_OF_RECORDS = 7455
-    __SUPPORTED_SEX = ("M", "F")
-    __FIRST_NAMES_DB = "forenames.csv"
-    __FIRST_NAMES_DF = None
-    __FIRST_NAMES = None
-    __NAMES_FOR_SEX = {}
+    NUM_OF_RECORDS: int = 7455
+    __SUPPORTED_SEX: tuple = ("M", "F")
+    __FIRST_NAMES_DB: str = "forenames.csv"
+    __FIRST_NAMES_DF: DataFrame = None
+    __FIRST_NAMES: ClassVar[list] = None
+    __NAMES_FOR_SEX: ClassVar[dict] = {}
 
     def get_first_name_at(
             self,
             index: int,
     ) -> FirstName:
         """Get a first name at `index` position.
```

### Comparing `mimeograph-0.7.0/src/mimeo/database/last_names.py` & `mimeograph-1.0.3/src/mimeo/database/last_names.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 It exports a class related to surnames CSV data:
     * LastNamesDB
         Class exposing READ operations on surnames CSV data.
 """
 from __future__ import annotations
 
+from typing import ClassVar
+
 from mimeo import tools
 from mimeo.database.exc import InvalidIndexError
 
 
 class LastNamesDB:
     """Class exposing READ operations on surnames CSV data.
 
@@ -22,17 +24,17 @@
     -------
     get_last_names() -> list[str]
         Get all last names.
     get_last_name_at(index: int) -> str
         Get a last name at `index` position.
     """
 
-    NUM_OF_RECORDS = 151670
-    _LAST_NAMES_DB = "surnames.txt"
-    _LAST_NAMES = None
+    NUM_OF_RECORDS: int = 151670
+    _LAST_NAMES_DB: str = "surnames.txt"
+    _LAST_NAMES: ClassVar[list] = None
 
     def get_last_name_at(
             self,
             index: int,
     ) -> str:
         """Get a last name at `index` position.
```

### Comparing `mimeograph-0.7.0/src/mimeo/database/mimeo_db.py` & `mimeograph-1.0.3/src/mimeo/database/mimeo_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,19 +66,19 @@
         Get a first name at `index` position.
     get_last_names() -> list[str]
         Get all last names.
     get_last_name_at(index: int) -> str
         Get a last name at `index` position.
     """
 
-    NUM_OF_CITIES = CitiesDB.NUM_OF_RECORDS
-    NUM_OF_COUNTRIES = CountriesDB.NUM_OF_RECORDS
-    NUM_OF_CURRENCIES = CurrenciesDB.NUM_OF_RECORDS
-    NUM_OF_FIRST_NAMES = FirstNamesDB.NUM_OF_RECORDS
-    NUM_OF_LAST_NAMES = LastNamesDB.NUM_OF_RECORDS
+    NUM_OF_CITIES: int = CitiesDB.NUM_OF_RECORDS
+    NUM_OF_COUNTRIES: int = CountriesDB.NUM_OF_RECORDS
+    NUM_OF_CURRENCIES: int = CurrenciesDB.NUM_OF_RECORDS
+    NUM_OF_FIRST_NAMES: int = FirstNamesDB.NUM_OF_RECORDS
+    NUM_OF_LAST_NAMES: int = LastNamesDB.NUM_OF_RECORDS
 
     def __init__(
             self,
     ):
         self._cities_db = CitiesDB()
         self._countries_db = CountriesDB()
         self._currencies_db = CurrenciesDB()
```

### Comparing `mimeograph-0.7.0/src/mimeo/generators/__init__.py` & `mimeograph-1.0.3/src/mimeo/generators/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 """The Mimeo Generators package.
 
 It contains modules supporting the Mimeo Config output formats:
 * generator
     The Mimeo Generator module.
 * generator_factory
     The Mimeo Generator Factory module.
+* json_generator
+    The Mimeo JSON Generator module.
 * xml_generator
     The Mimeo XML Generator module.
 * exc
     The Mimeo Generators Exceptions module.
 
 This package exports the following classes:
 * Generator:
     An abstract class for data generators in Mimeo.
 * GeneratorFactory:
     A Factory class instantiating a Generator based on Mimeo Config.
+* JSONGenerator:
+    A Generator implementation producing data in the JSON format.
+    Corresponds to the 'json' output format
 * XMLGenerator:
     A Generator implementation producing data in the XML format.
     Corresponds to the 'xml' output format
 
 To use this package, simply import the desired class:
     from mimeo.generators import GeneratorFactory
     from mimeo.generators.exc import UnsupportedStructureError
 """
 from .generator import Generator
+from .json_generator import JSONGenerator
 from .xml_generator import XMLGenerator
 from .generator_factory import GeneratorFactory
 
-__all__ = ["Generator", "XMLGenerator", "GeneratorFactory"]
+__all__ = ["Generator", "JSONGenerator", "XMLGenerator", "GeneratorFactory"]
```

### Comparing `mimeograph-0.7.0/src/mimeo/generators/exc.py` & `mimeograph-1.0.3/src/mimeo/generators/exc.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from __future__ import annotations
 
 
 class UnsupportedStructureError(Exception):
     """A custom Exception class for an unsupported structure.
 
-    Raised while attempting to generate data from a Mimeo Model having a list
+    Raised while attempting to generate XML data from a Mimeo Model having a list
     of non-only atomic / non-only dict items.
     """
 
     def __init__(
             self,
             field_name: str,
             structure: list,
@@ -29,9 +29,9 @@
         ----------
         field_name : str
             A field name
         structure : list
             An unsupported structure
         """
         super().__init__("An array can include only atomic types (including Mimeo "
-                         "Utils) or only JSON objects! Unsupported structure found in "
-                         f"{field_name}: {structure}")
+                         "Utils) or only JSON objects (when output format is XML)! "
+                         f"Unsupported structure found in {field_name}: {structure}")
```

### Comparing `mimeograph-0.7.0/src/mimeo/generators/generator_factory.py` & `mimeograph-1.0.3/src/mimeo/generators/generator_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,35 +5,38 @@
         A Factory class instantiating a Generator based on Mimeo Config.
 """
 from __future__ import annotations
 
 from mimeo.config import constants as cc
 from mimeo.config.exc import UnsupportedPropertyValueError
 from mimeo.config.mimeo_config import MimeoConfig
-from mimeo.generators import Generator, XMLGenerator
+from mimeo.generators import Generator, JSONGenerator, XMLGenerator
 
 
 class GeneratorFactory:
     """A Factory class instantiating a Generator based on Mimeo Config.
 
     Implementation of the Generator class depends on the output format
     configured.
 
     Attributes
     ----------
     XML
         The 'xml' output format
+    JSON
+        The 'json' output format
 
     Methods
     -------
     get_generator(mimeo_config: MimeoConfig) -> Generator
         Initialize a Generator based on the Mimeo Output Format.
     """
 
-    XML = cc.OUTPUT_FORMAT_XML
+    XML: str = cc.OUTPUT_FORMAT_XML
+    JSON: str = cc.OUTPUT_FORMAT_JSON
 
     @staticmethod
     def get_generator(
             mimeo_config: MimeoConfig,
     ) -> Generator:
         """Initialize a Generator based on the Mimeo Output Format.
 
@@ -51,11 +54,13 @@
         ------
         UnsupportedPropertyValueError
             If the output format is not supported
         """
         output_format = mimeo_config.output.format
         if output_format == GeneratorFactory.XML:
             return XMLGenerator(mimeo_config)
+        if output_format == GeneratorFactory.JSON:
+            return JSONGenerator(mimeo_config)
         raise UnsupportedPropertyValueError(
             cc.OUTPUT_FORMAT_KEY,
             output_format,
             cc.SUPPORTED_OUTPUT_FORMATS)
```

### Comparing `mimeograph-0.7.0/src/mimeo/generators/xml_generator.py` & `mimeograph-1.0.3/src/mimeo/utils/renderers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,653 +1,697 @@
-"""The Mimeo XML Generator module.
+"""The Mimeo Renderers module.
 
-It exports only one class:
-    * XMLGenerator
-        A Generator implementation producing data in the XML format.
+This module contains classes useful in value rendering. It exports
+the following renderers:
+    * MimeoRenderer
+        A Facade class rendering Mimeo Utils, Vars and Special Fields.
+    * UtilsRenderer
+        A class rendering Mimeo Utils.
+    * VarsRenderer
+        A class rendering Mimeo Vars.
+    * SpecialFieldsRenderer
+        A class rendering Mimeo Special Fields.
 """
 from __future__ import annotations
 
 import logging
-import xml.etree.ElementTree as ElemTree
-from typing import Iterator
-from xml.dom import minidom
+import re
+from typing import Any, ClassVar, Pattern
 
 from mimeo.config import constants as cc
-from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
-from mimeo.context import MimeoContext
-from mimeo.context.decorators import (mimeo_clear_iterations, mimeo_context,
-                                      mimeo_context_switch,
-                                      mimeo_next_iteration)
-from mimeo.generators import Generator
-from mimeo.generators.exc import UnsupportedStructureError
-from mimeo.utils import MimeoRenderer
+from mimeo.context import MimeoContext, MimeoContextManager
+from mimeo.context.decorators import mimeo_context
+from mimeo.utils import (AutoIncrementUtil, CityUtil, CountryUtil,
+                         CurrencyUtil, CurrentIterationUtil, DateTimeUtil,
+                         DateUtil, FirstNameUtil, KeyUtil, LastNameUtil,
+                         MimeoUtil, RandomIntegerUtil, RandomItemUtil,
+                         RandomStringUtil)
+from mimeo.utils.exc import InvalidMimeoUtilError, NotASpecialFieldError
 
 logger = logging.getLogger(__name__)
 
 
-class XMLGenerator(Generator):
-    """A Generator implementation producing data in the XML format.
+class UtilsRenderer:
+    """A class rendering Mimeo Utils.
 
-    This Generator is instantiated for the 'xml' output format
-    and produces data using Mimeo Configuration.
+    It contains only class methods.
 
     Methods
     -------
-    generate(
-        templates: list | Iterator[MimeoTemplate],
-        parent: ElemTree.Element = None
-    ) -> Iterator[ElemTree.Element]
-        Generate XML data based on the Mimeo Configuration.
-    stringify(
-        data: Any,
-        mimeo_config: MimeoConfig
-    ) -> str
-        Stringify data generated by the generate() method.
+    render_raw(mimeo_util_key: str) -> Any
+        Render a Mimeo Util in a raw form.
+    render_parametrized(mimeo_util_config: dict) -> Any
+        Render a Mimeo Util in a parametrized form.
     """
 
-    def __init__(
-            self,
-            mimeo_config: MimeoConfig,
-    ):
-        """Initialize XMLGenerator class.
+    MIMEO_UTILS: ClassVar[dict] = {
+        RandomStringUtil.KEY: RandomStringUtil,
+        RandomIntegerUtil.KEY: RandomIntegerUtil,
+        RandomItemUtil.KEY: RandomItemUtil,
+        DateUtil.KEY: DateUtil,
+        DateTimeUtil.KEY: DateTimeUtil,
+        AutoIncrementUtil.KEY: AutoIncrementUtil,
+        CurrentIterationUtil.KEY: CurrentIterationUtil,
+        KeyUtil.KEY: KeyUtil,
+        CityUtil.KEY: CityUtil,
+        CountryUtil.KEY: CountryUtil,
+        CurrencyUtil.KEY: CurrencyUtil,
+        FirstNameUtil.KEY: FirstNameUtil,
+        LastNameUtil.KEY: LastNameUtil,
+    }
+    _INSTANCES: ClassVar[dict] = {}
+
+    @classmethod
+    def render_raw(
+            cls,
+            mimeo_util_key: str,
+    ) -> Any:
+        """Render a Mimeo Util in a raw form.
 
         Parameters
         ----------
-        mimeo_config : MimeoConfig
-            A Mimeo Configuration
+        mimeo_util_key : str
+            A Mimeo Util key (name)
+
+        Returns
+        -------
+        Any
+            Rendered Mimeo Util value.
+
+        Raises
+        ------
+        InvalidMimeoUtilError
+            If the Mimeo Util name does not match any existing Mimeo
+            Util.
         """
-        self.__indent = mimeo_config.output.indent
-        self.__xml_declaration = mimeo_config.output.xml_declaration
+        return cls.render_parametrized({cc.MODEL_MIMEO_UTIL_NAME_KEY: mimeo_util_key})
 
     @classmethod
-    def generate(
+    def render_parametrized(
             cls,
-            templates: list | Iterator[MimeoTemplate],
-            parent: ElemTree.Element = None,
-    ) -> Iterator[ElemTree.Element]:
-        """Generate XML data based on the Mimeo Configuration.
+            mimeo_util_config: dict,
+    ) -> Any:
+        """Render a Mimeo Util in a parametrized form.
 
-        This function is used recursively when a Mimeo Configuration
-        contains nested templates.
-        It iterates through all templates configured and yields data
-        units.
+        Parameters
+        ----------
+        mimeo_util_config : dict
+            A Mimeo Util configuration
+
+        Returns
+        -------
+        Any
+            Rendered Mimeo Util value.
+
+        Raises
+        ------
+        InvalidMimeoUtilError
+            If the Mimeo Util configuration does not include Mimeo
+            Util name, or the parametrized name does not match any
+            existing Mimeo Util.
+        InvalidValueError
+            If a Mimeo Util is incorrectly parametrized.
+        InvalidSexError
+            If the First Name Mimeo Util has not supported `sex`
+            parameter value assigned.
+        """
+        logger.fine("Rendering a mimeo util [%s]", mimeo_util_config)
+        mimeo_util = cls._get_mimeo_util(mimeo_util_config)
+        return mimeo_util.render()
+
+    @classmethod
+    def _get_mimeo_util(
+            cls,
+            config: dict,
+    ) -> MimeoUtil:
+        """Get a Mimeo Util instance based on the configuration.
+
+        All instances are cached to not re-create a Util with the same
+        parameters. This method instantiate a Mimeo Util for the first
+        time and use the one in the future.
 
         Parameters
         ----------
-        templates : list | Iterator[MimeoTemplate]
-            A collection of Mimeo Templates to process
-        parent : ElemTree.Element, default None
-            A parent XML node for the currently processed template.
-            It is passed only when a Mimeo Config contain nested
-            templates.
+        config : dict
+            A Mimeo Util configuration
 
         Returns
         -------
-        Iterator[ElemTree.Element]
-            Iterator for generated nodes
-        """
-        for template in templates:
-            for data_unit in cls._process_single_template(template, parent):
-                yield data_unit
+        MimeoUtil
+            A Mimeo Util instance
 
-    def stringify(
-            self,
-            data_unit: ElemTree.Element,
+        Raises
+        ------
+        InvalidMimeoUtilError
+            If the Mimeo Util configuration does not include Mimeo
+            Util name, or the parametrized name does not match any
+            existing Mimeo Util.
+        """
+        cache_key = cls._generate_cache_key(config)
+        if cache_key not in cls._INSTANCES:
+            return cls._instantiate_mimeo_util(cache_key, config)
+        return cls._INSTANCES.get(cache_key)
+
+    @staticmethod
+    def _generate_cache_key(
+            config: dict,
     ) -> str:
-        """Stringify XML data generated by the generate() method.
+        """Generate an internal Mimeo Util key from its parameters.
+
+        This method ensures that Mimeo Util instances are cached
+        properly for the same parameters.
 
         Parameters
         ----------
-        data_unit: ElemTree.Element
-            A single data unit generated by the generate() method
+        config : dict
+            A Mimeo Util configuration
 
         Returns
         -------
         str
-            Stringified data unit
+            An internal Mimeo Util cache key
         """
-        if self.__indent is None or self.__indent == 0:
-            node_str = ElemTree.tostring(
-                data_unit,
-                encoding="utf-8",
-                method="xml",
-                xml_declaration=self.__xml_declaration)
-        else:
-            xml_string = ElemTree.tostring(data_unit)
-            xml_minidom = minidom.parseString(xml_string)
-            if self.__xml_declaration is False:
-                xml_minidom = xml_minidom.childNodes[0]
-            node_str = xml_minidom.toprettyxml(
-                indent=" " * self.__indent,
-                encoding="utf-8")
-        return node_str.decode("ascii")
+        return "-".join(":".join([key, str(val)]) for key, val in config.items())
 
     @classmethod
-    @mimeo_context_switch
-    @mimeo_clear_iterations
-    def _process_single_template(
+    def _instantiate_mimeo_util(
             cls,
-            template: MimeoTemplate,
-            parent: ElemTree.Element = None,
-    ) -> list[ElemTree.Element]:
-        """Process a single Mimeo Template.
+            cache_key: str,
+            config: dict,
+    ) -> MimeoUtil:
+        """Instantiate a Mimeo Util based on the configuration.
 
-        This function is used recursively when a Mimeo Configuration
-        contains nested templates.
-        It repeats same processing operation so many times as it is
-        configured in the `count` property of a Mimeo Configuration.
-        Before the template execution it switches context managed by
-        MimeoContextManager and also clears iterations as nested
-        templates would collect iterations from previous parent's
-        iterations.
+        After instantiation the Mimeo Util is cached for the future.
 
         Parameters
         ----------
-        template : MimeoTemplate
-            A single Mimeo Template to process
-        parent : ElemTree.Element, default None
-            A parent node for processing nested templates
+        cache_key : str
+            An internal Mimeo Util cache key
+        config : dict
+            A Mimeo Util configuration
 
         Returns
         -------
-        list[ElemTree.Element]
-            A list of generated data units
-        """
-        logger.debug("Reading template [%s]", template)
-        return [cls._process_single_data_unit(template, parent)
-                for _ in iter(range(template.count))]
+        MimeoUtil
+            A Mimeo Util instance
+
+        Raises
+        ------
+        InvalidMimeoUtilError
+            If the Mimeo Util configuration does not include Mimeo
+            Util name, or the parametrized name does not match any
+            existing Mimeo Util.
+        """
+        mimeo_util_name = cls.get_mimeo_util_name(config)
+        mimeo_util = cls.MIMEO_UTILS.get(mimeo_util_name)(**config)
+        cls._INSTANCES[cache_key] = mimeo_util
+        return mimeo_util
 
     @classmethod
-    @mimeo_next_iteration
-    def _process_single_data_unit(
+    def get_mimeo_util_name(
             cls,
-            template: MimeoTemplate,
-            parent: ElemTree.Element = None,
-    ) -> ElemTree.Element:
-        """Process a single data unit from the template.
+            config: dict,
+    ) -> str:
+        """Return a verified Mimeo Util name.
 
-        This function is used recursively when a Mimeo Configuration
-        contains nested templates.
-        It processes a single data unit. The reason why it is separated
-        from the _process_node() function is the @mimeo_next_iteration
-        decorator. The _process_node() function is recursively called
-        by itself, and it produces data for a single iteration.
-        The purpose of this function is to increment iteration before
-        processing node.
+        Parameters
+        ----------
+        config : dict
+            A Mimeo Util configuration
+
+        Returns
+        -------
+        str
+            A Mimeo Util name
+
+        Raises
+        ------
+        InvalidMimeoUtilError
+            If the Mimeo Util configuration does not include Mimeo
+            Util name, or the parametrized name does not match any
+            existing Mimeo Util.
+        """
+        mimeo_util_name = config.get(cc.MODEL_MIMEO_UTIL_NAME_KEY)
+        if mimeo_util_name is None:
+            code = InvalidMimeoUtilError.Code.ERR_1
+            raise InvalidMimeoUtilError(code, config=config)
+        if mimeo_util_name not in cls.MIMEO_UTILS:
+            code = InvalidMimeoUtilError.Code.ERR_2
+            raise InvalidMimeoUtilError(code, name=mimeo_util_name)
+        return mimeo_util_name
+
+
+class VarsRenderer:
+    """A class rendering Mimeo Vars.
+
+    It contains only a class method.
+
+    Methods
+    -------
+    render(var: str) -> Any
+        Render a Mimeo Var.
+    """
+
+    @classmethod
+    def render(
+            cls,
+            var: str,
+    ) -> str | int | bool | dict:
+        """Render a Mimeo Var.
 
         Parameters
         ----------
-        template : MimeoTemplate
-            A single Mimeo Template to process
-        parent : ElemTree.Element, default None
-            A parent node for processing nested templates
+        var : str
+            A variable name
 
         Returns
         -------
-        ElemTree.Element
-            A single data unit generated within a single template
-            iteration. If the `parent` is not None it will not return
-            any value.
+        Any
+            A variable value
+
+        Raises
+        ------
+        InstanceNotAliveError
+            If the MimeoContextManager instance is not alive
+        VarNotFoundError
+            If the Mimeo Var with the `var` provided does not exist
         """
-        element_meta = cls._element_meta(
-            template.model.root_name,
-            template.model.root_data)
-        return cls._process_node(parent, element_meta)
+        logger.fine("Rendering a variable [%s]", var)
+        return MimeoContextManager().get_var(var)
+
+
+class SpecialFieldsRenderer:
+    """A class rendering Mimeo Special Fields.
+
+    It contains only a class method.
+
+    Methods
+    -------
+    render(field_name: str, context: MimeoContext = None) -> Any
+        Render a Mimeo Special Field.
+    """
 
     @classmethod
     @mimeo_context
-    def _process_node(
+    def render(
             cls,
-            parent: ElemTree.Element | None,
-            element_meta: dict,
-            context: MimeoContext = None,
-    ) -> ElemTree.Element:
-        """Process a single template's node.
-
-        This is a recursive function that traverses Mimeo Template and generates XML
-        nodes based on element's metadata. First, element is pre-processed, in meaning
-        of metadata being adjusted. Then, element is processed accordingly to its value
-        type.
+            field: str,
+            context: MimeoContext | None = None,
+    ) -> str | int | bool:
+        """Render a Mimeo Special Field.
 
         Parameters
         ----------
-        parent : ElemTree.Element | None
-            A parent node
-        element_meta : dict
-            Element's metadata
+        field : str
+            A special field name
         context : MimeoContext, default None
-            The current Mimeo Context (injected by MimeoContextManager)
+            A current Mimeo Context injected by a decorator
 
         Returns
         -------
-        ElemTree.Element
-            A single data unit generated within a single template iteration.
+        str | int | bool
 
         Raises
         ------
-        UnsupportedStructureError
-            If a list value elements are not atomic-only or dict-only.
-        InvalidSpecialFieldValueError
-            If a special field value is dict or list
+        UninitializedContextIterationError
+            If no iteration has been initialized yet for the context
         SpecialFieldNotFoundError
-            If a special field does not exist.
+            If the special field does not exist.
         """
-        logger.fine("Rendering element - parent [%s], element_meta [%s]",
-                    parent if parent is None else parent.tag, element_meta)
-        element_meta = cls._pre_process_node(element_meta)
+        logger.fine("Rendering a special field [%s]", field)
+        return context.curr_iteration().get_special_field(field)
+
 
-        if cls._is_complex(element_meta):
-            return cls._process_complex_value(parent, element_meta)
-        return cls._process_atomic_value(parent, element_meta, context)
+class MimeoRenderer:
+    """A Facade class rendering Mimeo Utils, Vars and Special Fields.
+
+    It contains only class methods.
+
+    Methods
+    -------
+    render(value: Any) -> Any
+        Render a value.
+    get_special_field_name(wrapped_field_name: str) -> str
+        Extract a special field name.
+    is_special_field(special_field: str) -> bool
+        Verify if the field is special (of form {:FIELD_NAME:}).
+    is_raw_mimeo_util(value: str) -> bool
+        Verify if the value is a raw Mimeo Util.
+    is_parametrized_mimeo_util(value: dict)
+        Verify if the value is a parametrized Mimeo Util.
+    """
+
+    _UTILS_PATTERN: Pattern = re.compile("^{(.+)}$")
+    _VARS_PATTERN: Pattern = re.compile(".*({[A-Z_0-9]+})")
+    _SPECIAL_FIELDS_PATTERN: Pattern = re.compile(".*({:([a-zA-Z]+:)?[-_a-zA-Z0-9]+:})")
 
     @classmethod
-    def _pre_process_node(
+    def get_special_field_name(
             cls,
-            element_meta: dict,
-    ) -> dict:
-        """Pre-process element's metadata.
-
-        This function adjusts existing element's metadata and completes it with custom
-        properties:
-        * the tag property is changed only for special fields
-          - field name is extracted
-        * the value property is being modified for dicts including attributes
-          - properties starting with '@' are being removed from the dict
-        * the attrs property
-          - is being populated by all properties starting with '@'
-          - takes the default value (an empty dict) when there's no such properties
-        * the mimeo_util property is being initialized
-          - True if element's value is a parametrized mimeo_util. Otherwise, False.
-        * the special property is being initialized
-          - True, when a field is special. Otherwise, False.
+            wrapped_field_name: str,
+    ) -> str:
+        """Extract a special field name.
 
         Parameters
         ----------
-        element_meta : dict
-            Initial element's metadata
+        wrapped_field_name : str
+            A field name wrapped with curly braces and colons,
+            e.g. :Field:
 
         Returns
         -------
-        dict
-            Complete element's metadata
+        str
+            A special field name
+
+        Raises
+        ------
+        NotASpecialFieldError
+            If the `wrapped_field_name` is not of form :FIELD_NAME:
         """
-        tag = element_meta["tag"]
-        value = element_meta["value"]
-        attrs = {}
-        is_mimeo_util = MimeoRenderer.is_parametrized_mimeo_util(value)
-        is_special_field = MimeoRenderer.is_special_field(tag)
-        if is_special_field:
-            tag = MimeoRenderer.get_special_field_name(tag)
-        if isinstance(value, dict):
-            value_copy = dict(value)
-            for prop in value:
-                if prop.startswith(cc.MODEL_ATTRIBUTES_KEY):
-                    attrs[prop[1:]] = value_copy.pop(prop)
-            value = value.get(cc.MODEL_TEXT_VALUE_KEY, value_copy)
-
-        return cls._element_meta(
-            tag,
-            value,
-            attrs,
-            is_mimeo_util,
-            is_special_field)
+        if not cls.is_special_field(wrapped_field_name):
+            raise NotASpecialFieldError(wrapped_field_name)
 
-    @staticmethod
-    def _is_complex(
-            element_meta: dict,
+        return wrapped_field_name[1:][:-1]
+
+    @classmethod
+    def is_special_field(
+            cls,
+            special_field: str,
     ) -> bool:
-        """Verify if an element is complex.
+        """Verify if the field is special (of form :FIELD_NAME:).
 
         Parameters
         ----------
-        element_meta : dict
-            Element's metadata
+        special_field : str
+            A special field
 
         Returns
         -------
         bool
-            True if element's value is a list or a dict not being a parametrized
-            Mimeo Util. Otherwise, False.
+            True if the field is of form :FIELD_NAME:. Otherwise,
+            False.
         """
-        return (isinstance(element_meta["value"], (list, dict)) and
-                not element_meta["mimeo_util"])
+        return bool(re.match(r"^:([a-zA-Z]+:)?[-_a-zA-Z0-9]+:$", special_field))
 
     @classmethod
-    def _process_complex_value(
+    def is_raw_mimeo_util(
             cls,
-            parent: ElemTree.Element | None,
-            element_meta: dict,
-    ) -> ElemTree.Element | None:
-        """Process a node with a complex value.
-
-        The node is processed accordingly to its value type.
-        When the type is list and tag is _templates_, node is processed
-        in a special way.
+            value: str,
+    ) -> bool:
+        """Verify if the value is a raw Mimeo Util.
 
         Parameters
         ----------
-        parent : ElemTree.Element | None
-            A parent node
-        element_meta : dict
-            Element's metadata
+        value : str
+            A string value
 
         Returns
         -------
-        ElemTree.Element
-            A processed node
+        bool
+            True if the value is a raw Mimeo Util, e.g. {random_str}.
+            Otherwise, False.
+        """
+        raw_mimeo_utils = UtilsRenderer.MIMEO_UTILS.keys()
+        raw_mimeo_utils_re = "^{(" + "|".join(raw_mimeo_utils) + ")}$"
+        return bool(re.match(raw_mimeo_utils_re, value))
 
-        Raises
-        ------
-        UnsupportedStructureError
-            If a list value elements are not atomic-only or dict-only.
-        InvalidSpecialFieldValueError
-            If a special field value is dict or list
-        SpecialFieldNotFoundError
-            If a special field does not exist.
+    @classmethod
+    def is_parametrized_mimeo_util(
+            cls,
+            value: dict,
+    ):
+        """Verify if the value is a parametrized Mimeo Util.
+
+        Parameters
+        ----------
+        value : dict
+            A dict value
+
+        Returns
+        -------
+        bool
+            True if the value is a dictionary having only one key,
+            "_mimeo_util". Otherwise, False.
         """
-        if isinstance(element_meta["value"], dict):
-            func = cls._process_dict_value
-        elif (isinstance(element_meta["value"], list) and
-              element_meta["tag"] != cc.TEMPLATES_KEY):
-            func = cls._process_list_value
-        else:
-            func = cls._process_templates_value
-        return func(parent, element_meta)
+        return (isinstance(value, dict) and
+                len(value) == 1 and
+                cc.MODEL_MIMEO_UTIL_KEY in value)
 
     @classmethod
-    def _process_dict_value(
+    def render(
             cls,
-            parent: ElemTree.Element | None,
-            element_meta: dict,
-    ) -> ElemTree.Element:
-        """Process a node with a dictionary value.
+            value: Any,
+    ) -> Any:
+        """Render a value.
 
-        It iterates through the dictionary items and processes each of them.
+        This method renders a value accordingly to its type and form.
+        If the value takes a form of Mimeo Util it is rendered as
+        Mimeo Util (raw or parametrized); if it takes a form of
+        a special field this renderer will try to reach it from
+        the current context; when the value takes a form of a Mimeo Var,
+        then it uses Mimeo Vars defined in Mimeo Config.
+        Otherwise, the raw value is returned.
+        It is recursively called to return a final value.
 
         Parameters
         ----------
-        parent : ElemTree.Element | None
-            A parent node
-        element_meta : dict
-            Element's metadata
+        value : Any
+            A value to be rendered
 
         Returns
         -------
-        ElemTree.Element
-            A processed node
+        Any
+            A rendered value
 
         Raises
         ------
-        UnsupportedStructureError
-            If a list value elements are not atomic-only or dict-only.
-        InvalidSpecialFieldValueError
-            If a special field value is dict or list
-        SpecialFieldNotFoundError
-            If a special field does not exist.
+        InstanceNotAliveError
+            If the MimeoContextManager instance is not alive
+        UninitializedContextIterationError
+            If no iteration has been initialized yet for the context
+        VarNotFoundError
+            If the Mimeo Var does not exist
+        InvalidMimeoUtilError
+            If the Mimeo Util node has missing _name property, or it
+            does not match any Mimeo Util.
+        InvalidValueError
+            If Mimeo Util node is incorrectly parametrized
+        OutOfStockError
+            If all unique values have been consumed already
+        DataNotFoundError
+            If database does not contain the expected value
+        InvalidSexError
+            If the First Name Mimeo Util has not supported `sex`
+            parameter value assigned.
+        """
+        logger.fine("Rendering a value [%s]", value)
+        try:
+            if isinstance(value, str):
+                value = cls._render_string_value(value)
+            if cls.is_parametrized_mimeo_util(value):
+                value = cls._render_parametrized_mimeo_util(value)
+        except Exception:
+            logger.exception("An error occurred for [%s].", value)
+            raise
+        return value
+
+    @classmethod
+    def _render_string_value(
+            cls,
+            value: str,
+    ) -> Any:
+        """Render a string value.
+
+        Depending on value form it can render it as a raw value,
+        a special field, a Mimeo Var or a raw Mimeo Util.
+
+        Parameters
+        ----------
+        value : str
+            A string value
 
-        Examples
-        --------
-        parent = ElemTree.Element("Root")
-        element_meta = cls._element_meta(
-            tag="SomeField",
-            value={"SomeChild1": 1, "SomeChild2": 2},
-        )
-        cls._process_dict_value(parent, element_meta)
-        ->
-        <SomeField>
-            <SomeChild1>1</SomeChild1>
-            <SomeChild2>2</SomeChild2>
-        </SomeField>
+        Returns
+        -------
+        Any
+            A rendered value
         """
-        element = cls._create_xml_element(parent, element_meta)
-        for child_tag, child_value in element_meta["value"].items():
-            cls._process_node(element, cls._element_meta(child_tag, child_value))
-        return element
+        if cls._SPECIAL_FIELDS_PATTERN.match(value):
+            return cls._render_special_field(value)
+        if cls._VARS_PATTERN.match(value):
+            return cls._render_var(value)
+        if cls.is_raw_mimeo_util(value):
+            return cls._render_raw_mimeo_util(value)
+        return value
 
     @classmethod
-    def _process_list_value(
+    def _render_special_field(
             cls,
-            parent: ElemTree.Element,
-            element_meta: dict,
-    ) -> ElemTree.Element:
-        """Process a node with a list value.
+            value: str,
+    ) -> Any:
+        """Render a value containing a Mimeo Special Field.
 
-        It iterates through the list items and processes each of them: generates
-        a child element for each value as direct children of the parent.
+        This method finds first special field and replaces all
+        occurrences. Then the result is passed to the render() method
+        again, to return a final value.
 
         Parameters
         ----------
-        parent : ElemTree.Element | None
-            A parent node
-        element_meta : dict
-            Element's metadata
+        value : str
+            A value containing a Mimeo Special Field
 
         Returns
         -------
-        ElemTree.Element
-            A processed node
+        Any
+            A rendered value
 
         Raises
         ------
-        UnsupportedStructureError
-            If any of the list value element is a list.
-        InvalidSpecialFieldValueError
-            If the special field value is dict or list
+        UninitializedContextIterationError
+            If no iteration has been initialized yet for the context
         SpecialFieldNotFoundError
             If the special field does not exist.
+        """
+        match = next(cls._SPECIAL_FIELDS_PATTERN.finditer(value))
+        wrapped_special_field = match.group(1)
+        r_val = SpecialFieldsRenderer.render(wrapped_special_field[2:][:-2])
+        logger.fine("Rendered special field value [%s]", r_val)
+        if len(wrapped_special_field) != len(value):
+            r_val = str(r_val).lower() if isinstance(r_val, bool) else str(r_val)
+            r_val = value.replace(wrapped_special_field, str(r_val))
+        return cls.render(r_val)
 
-        Examples
-        --------
-        parent = ElemTree.Element("Root")
-        element_meta = cls._element_meta(
-            tag="SomeField",
-            value=[
-                'value-1',
-                {'SomeChild1': True, 'SomeChild2': False},
-                {'_mimeo_util': {'_name': 'auto_increment', 'pattern': '{}'}}
-            ],
-        )
-        cls._process_list_value_with_atomic_children(parent, element_meta)
-        ->
-        <Root>
-            <SomeField>value-1</SomeField>
-            <SomeField>
-                <SomeChild1>true</SomeChild1>
-                <SomeChild2>false</SomeChild2>
-            </SomeField>
-            <SomeField>1</SomeField>
-        </Root>
-        """
-        for child in element_meta["value"]:
-            if isinstance(child, list):
-                raise UnsupportedStructureError(
-                    element_meta["tag"],
-                    element_meta["value"])
-            element_meta = cls._element_meta(element_meta["tag"], child)
-            cls._process_node(parent, element_meta)
-        return parent
-
-    @classmethod
-    def _process_templates_value(
-            cls,
-            parent: ElemTree.Element,
-            element_meta: dict,
-    ) -> ElemTree.Element:
-        """Process a node with a dictionary value storing templates.
-
-        It iterates through the templates and generates data based on them.
+    @classmethod
+    def _render_var(
+            cls,
+            value: str,
+    ) -> Any:
+        """Render a value containing a Mimeo Var.
+
+        This method finds first variable and replaces all occurrences.
+        Then the result is passed to the render() method again, to
+        return a final value.
 
         Parameters
         ----------
-        parent : ElemTree.Element | None
-            A parent node
-        element_meta : dict
-            Element's metadata
+        value : str
+            A value containing a Mimeo Var
 
         Returns
         -------
-        ElemTree.Element
-            A processed node
+        Any
+            A rendered value
 
         Raises
         ------
-        UnsupportedStructureError
-            If a list value elements are not atomic-only or dict-only.
-        InvalidSpecialFieldValueError
-            If a special field value is dict or list
-        SpecialFieldNotFoundError
-            If a special field does not exist.
+        InstanceNotAliveError
+            If the MimeoContextManager instance is not alive
+        VarNotFoundError
+            If the Mimeo Var with the `var` provided does not exist
+        """
+        match = next(cls._VARS_PATTERN.finditer(value))
+        wrapped_var = match.group(1)
+        r_val = VarsRenderer.render(wrapped_var[1:][:-1])
+        logger.fine("Rendered variable value [%s]", r_val)
+        if cls.is_parametrized_mimeo_util(r_val):
+            r_val = cls._render_parametrized_mimeo_util(r_val)
+        if len(wrapped_var) != len(value):
+            r_val = str(r_val).lower() if isinstance(r_val, bool) else str(r_val)
+            r_val = value.replace(wrapped_var, str(r_val))
+        return cls.render(r_val)
 
-        Examples
-        --------
-        parent = ElemTree.Element("Root")
-        element_meta = cls._element_meta(
-            tag="SomeField",
-            value={"_templates_": [
-                {
-                  "count": 10,
-                  "model": {
-                    "SomeChild": {
-                      "Node1": 1,
-                      "Node2": "value-2",
-                      "Node3": true
-                    }
-                  }
-                }
-            ]},
-        )
-        cls._process_templates_value(parent, element_meta)
-        ->
-        <Root>
-            <SomeField>
-                <SomeChild><Node1>1</Node1><Node2>value-2</Node2><Node3>true</Node3></SomeChild>
-                <SomeChild><Node1>1</Node1><Node2>value-2</Node2><Node3>true</Node3></SomeChild>
-                ... x10
-            </SomeField>
-        </Root>
-        """
-        templates = (MimeoTemplate(template) for template in element_meta["value"])
-        for _ in cls.generate(templates, parent):
-            pass
-        return parent
-
-    @classmethod
-    def _process_atomic_value(
-            cls,
-            parent: ElemTree.Element,
-            element_meta: dict,
-            context: MimeoContext,
-    ) -> ElemTree.Element:
-        """Process a node with an atomic value.
-
-        A parametrized Mimeo Util is considered as an atomic value as representing one.
-        It renders a value for the node.
+    @classmethod
+    def _render_raw_mimeo_util(
+            cls,
+            value: str,
+    ) -> Any:
+        """Render a raw Mimeo Util.
 
         Parameters
         ----------
-        parent : ElemTree.Element | None
-            A parent node
-        element_meta : dict
-            Element's metadata
-        context : MimeoContext, default None
-            The current Mimeo Context (injected by MimeoContextManager)
+        value : str
+            A raw Mimeo Util
 
         Returns
         -------
-        ElemTree.Element
-            A processed node
+        Any
+            A rendered value
 
         Raises
         ------
-        UnsupportedStructureError
-            If a list value elements are not atomic-only or dict-only.
-        InvalidSpecialFieldValueError
-            If a special field value is dict or list
-        SpecialFieldNotFoundError
-            If a special field does not exist.
+        OutOfStockError
+            If all unique values have been consumed already
+        DataNotFoundError
+            If database does not contain the expected value
+        """
+        rendered_value = UtilsRenderer.render_raw(value[1:][:-1])
+        return cls.render(rendered_value)
 
-        Examples
-        --------
-        context = MimeoContextManager().get_current_context()
-        parent = ElemTree.Element("Root")
-        element_meta = cls._element_meta(
-            tag="SomeField",
-            value="value-1",
-        )
-        cls._process_atomic_value(parent, element_meta, context)
-        ->
-        <SomeField>value-1</SomeField>
-        """
-        element = cls._create_xml_element(parent, element_meta)
-        value = MimeoRenderer.render(element_meta["value"])
-        if element_meta["special"]:
-            context.curr_iteration().add_special_field(element_meta["tag"], value)
-        val_str = str(value) if value is not None else ""
-        element.text = val_str.lower() if isinstance(value, bool) else val_str
-        logger.fine("Rendered value [%s]", element.text)
-        return element
+    @classmethod
+    def _render_parametrized_mimeo_util(
+            cls,
+            value: dict,
+    ) -> Any:
+        """Render a parametrized Mimeo Util.
 
-    @staticmethod
-    def _element_meta(
-            tag: str,
-            value: dict | list | str | int | float | bool,
-            attrs: dict | None = None,
-            is_mimeo_util: bool | None = None,
-            is_special_field: bool | None = None,
-    ) -> dict:
-        """Build element's metadata.
+        Before the Mimeo Util itself will be rendered, first all its
+        parameters (except name) are rendered.
 
         Parameters
         ----------
-        tag : str
-            An element's tag
-        value : dict | list | str | int | float | bool
-            An element's value
-        attrs : dict | None, default None
-            An element's attributes
-        is_mimeo_util : bool | None, default None
-            A is-mimeo-util flag
-        is_special_field : bool | None, default None
-            A is-special-field flag
+        value : str
+            A parametrized Mimeo Util
 
         Returns
         -------
-        dict
-            Element's metadata
-        """
-        return {
-            "tag": tag,
-            "value": value,
-            "attrs": attrs,
-            "mimeo_util": is_mimeo_util,
-            "special": is_special_field,
-        }
+        Any
+            A rendered value
 
-    @staticmethod
-    def _create_xml_element(
-            parent: ElemTree.Element,
-            element_meta: dict,
-    ) -> ElemTree.Element | ElemTree.SubElement:
-        """Create an XML element based on the `parent` existence.
+        Raises
+        ------
+        InvalidValueError
+            If a Mimeo Util is incorrectly parametrized.
+        OutOfStockError
+            If all unique values have been consumed already
+        DataNotFoundError
+            If database does not contain the expected value
+        InvalidSexError
+            If the First Name Mimeo Util has not supported `sex`
+            parameter value assigned.
+        """
+        mimeo_util = value[cc.MODEL_MIMEO_UTIL_KEY]
+        mimeo_util = cls._render_mimeo_util_parameters(mimeo_util)
+        logger.fine("Pre-rendered mimeo util [%s]", mimeo_util)
+        r_val = UtilsRenderer.render_parametrized(mimeo_util)
+        return cls.render(r_val)
+
+    @classmethod
+    def _render_mimeo_util_parameters(
+            cls,
+            mimeo_util_config: dict,
+    ) -> dict:
+        """Render Mimeo Util's parameters.
 
         Parameters
         ----------
-        parent : ElemTree.Element
-            A parent node
-        element_meta : dict
-            Element's metadata
+        mimeo_util_config : dict
+            A parametrized Mimeo Util
 
         Returns
         -------
-        ElemTree.Element | ElemTree.SubElement
-            If the `parent` is None, returns ElemTree.Element.
-            Otherwise, returns ElemTree.SubElement
-        """
-        if parent is None:
-            return ElemTree.Element(
-                element_meta["tag"],
-                attrib=element_meta["attrs"])
-        return ElemTree.SubElement(
-            parent,
-            element_meta["tag"],
-            attrib=element_meta["attrs"],
-        )
+        dict
+            A Mimeo Util with pre-rendered parameters
+
+        Raises
+        ------
+        InvalidValueError
+            If a Mimeo Util is incorrectly parametrized.
+        OutOfStockError
+            If all unique values have been consumed already
+        DataNotFoundError
+            If database does not contain the expected value
+        InvalidSexError
+            If the First Name Mimeo Util has not supported `sex`
+            parameter value assigned.
+        """
+        logger.fine("Rendering mimeo util parameters")
+        return {key: cls.render(value) if key != "_name" else value
+                for key, value in mimeo_util_config.items()}
```

### Comparing `mimeograph-0.7.0/src/mimeo/logging/__init__.py` & `mimeograph-1.0.3/src/mimeo/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/logging/filters.py` & `mimeograph-1.0.3/src/mimeo/logging/filters.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/meta/__init__.py` & `mimeograph-1.0.3/src/mimeo/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/meta/alive.py` & `mimeograph-1.0.3/src/mimeo/meta/alive.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,28 +34,29 @@
 
     print('Alive 1:', x_1)  # 1
     print('Alive 2:', x_2)  # 1
 """
 from __future__ import annotations
 
 from types import TracebackType
+from typing import ClassVar
 
 from mimeo.meta.exc import InstanceNotAliveError
 
 
 class OnlyOneAlive(type):
     """A type ensuring there's only one instance qualified to be used.
 
     The OnlyOneAlive type caches all instances being created for each
     Alive subclass. If there is any instance being alive, it is
     returned by a constructor. Otherwise, an Alive subclass is
     instantiated and returned.
     """
 
-    _INSTANCES = {}
+    _INSTANCES: ClassVar[dict] = {}
 
     def __call__(
             cls,
             *args,
             **kwargs,
     ):
         """Ensure there's only one instance qualified to be used."""
@@ -85,15 +86,15 @@
     assert_alive()
         Assert the instance is alive.
     """
 
     def __init__(
             self,
     ):
-        self._alive = False
+        self._alive: bool = False
 
     def __enter__(
             self,
     ) -> Alive:
         """Enter the Alive instance.
 
         It sets the internal `alive` attribute to True.
```

### Comparing `mimeograph-0.7.0/src/mimeo/meta/exc.py` & `mimeograph-1.0.3/src/mimeo/meta/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/resources/cities.csv` & `mimeograph-1.0.3/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/resources/constants.yaml` & `mimeograph-1.0.3/src/mimeo/resources/constants.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -43,22 +43,25 @@
               required: Yes
             password:
               key: password
               required: Yes
 
     format:
       key: format
+      details:
+        indent:
+          key: indent
       values:
         xml:
           key: xml
           details:
             xml-declaration:
               key: xml_declaration
-            indent:
-              key: indent
+        json:
+          key: json
 
 
   vars:
     key: vars
 
 
   templates:
```

### Comparing `mimeograph-0.7.0/src/mimeo/resources/countries.csv` & `mimeograph-1.0.3/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/resources/currencies.csv` & `mimeograph-1.0.3/src/mimeo/resources/currencies.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/resources/exc.py` & `mimeograph-1.0.3/src/mimeo/resources/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/resources/forenames.csv` & `mimeograph-1.0.3/src/mimeo/resources/forenames.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/resources/logging.yaml` & `mimeograph-1.0.3/src/mimeo/resources/logging.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 version: 1
 
 formatters:
   regular:
     format: '[mimeo] %(levelname)s - %(message)s'
   detailed:
-    format: '[mimeo] [%(filename)s:%(lineno)d] %(levelname)-5s - %(message)s'
+    format: '[mimeo] [%(threadName)s] [%(filename)s:%(lineno)d] %(levelname)-5s - %(message)s'
 
 filters:
   regularFilter:
     (): mimeo.logging.RegularFilter
   detailedFilter:
     (): mimeo.logging.DetailedFilter
```

### Comparing `mimeograph-0.7.0/src/mimeo/resources/surnames.txt` & `mimeograph-1.0.3/src/mimeo/resources/surnames.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/tools.py` & `mimeograph-1.0.3/src/mimeo/tools.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/utils/__init__.py` & `mimeograph-1.0.3/src/mimeo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.7.0/src/mimeo/utils/exc.py` & `mimeograph-1.0.3/src/mimeo/utils/exc.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         ----------
         ERR_1: str
             An error code for a missing Mimeo Util name in configuration
         ERR_2: str
             An error code for an unsupported Mimeo Util
         """
 
-        ERR_1 = "MISSING_NAME"
-        ERR_2 = "UNSUPPORTED_MIMEO_UTIL"
+        ERR_1: str = "MISSING_NAME"
+        ERR_2: str = "UNSUPPORTED_MIMEO_UTIL"
 
     def __init__(
             self,
             code: InvalidMimeoUtilError.Code,
             **kwargs,
     ):
         """Initialize InvalidMimeoUtilError exception with details.
@@ -111,18 +111,18 @@
             An error code for a limit param lower than start
         ERR_3: str
             An error code for an invalid param type
         ERR_3: str
             An error code for an unsupported value
         """
 
-        ERR_1 = "NEGATIVE_LENGTH"
-        ERR_2 = "LIMIT_LOWER_THAN_START"
-        ERR_3 = "INVALID_TYPE"
-        ERR_4 = "UNSUPPORTED_VALUE"
+        ERR_1: str = "NEGATIVE_LENGTH"
+        ERR_2: str = "LIMIT_LOWER_THAN_START"
+        ERR_3: str = "INVALID_TYPE"
+        ERR_4: str = "UNSUPPORTED_VALUE"
 
     def __init__(
             self,
             code: InvalidValueError.Code,
             **kwargs,
     ):
         """Initialize InvalidValueError exception with details.
```

### Comparing `mimeograph-0.7.0/src/mimeo/utils/mimeo_utils.py` & `mimeograph-1.0.3/src/mimeo/utils/mimeo_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "random_str"
+    KEY: str = "random_str"
 
     def __init__(
             self,
             length: int = 20,
             **kwargs,
     ):
         """Initialize RandomStringUtil class.
@@ -116,15 +116,15 @@
         Parameters
         ----------
         length : int, default 20
             A length of a string to render
         kwargs : dict
             Arbitrary keyword arguments (ignored).
         """
-        self._length = length
+        self._length: int = length
 
     def render(
             self,
     ) -> str:
         """Render a random string value.
 
         Returns
@@ -154,15 +154,15 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "random_int"
+    KEY: str = "random_int"
 
     def __init__(
             self,
             start: int = 1,
             limit: int = 100,
             **kwargs,
     ):
@@ -173,16 +173,16 @@
         start : int, default 1
             A lower bound for integers (inclusive)
         limit : int, default 100
             An upper bound for integers (inclusive)
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._start = start
-        self._limit = limit
+        self._start: int = start
+        self._limit: int = limit
 
     def render(
             self,
     ) -> int:
         """Render a random integer value.
 
         Returns
@@ -213,31 +213,31 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "random_item"
+    KEY: str = "random_item"
 
     def __init__(
             self,
-            items: list = None,
+            items: list | None = None,
             **kwargs,
     ):
         """Initialize RandomItemUtil class.
 
         Parameters
         ----------
         items : int, default ['']
             A list of items from which a value will be picked up
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._items = items if items is not None and len(items) != 0 else [""]
+        self._items: list = items if items is not None and len(items) != 0 else [""]
 
     def render(
             self,
     ) -> Any:
         """Render a random item.
 
         Returns
@@ -259,15 +259,15 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "date"
+    KEY: str = "date"
 
     def __init__(
             self,
             days_delta: int = 0,
             **kwargs,
     ):
         """Initialize DateUtil class.
@@ -275,15 +275,15 @@
         Parameters
         ----------
         days_delta : int, default 0
             An integer value of days to add or subtract from today
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._days_delta = days_delta
+        self._days_delta: int = days_delta
 
     def render(
             self,
     ) -> str:
         """Render a stringified date value.
 
         Returns
@@ -308,15 +308,15 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "date_time"
+    KEY: str = "date_time"
 
     def __init__(self,
                  days_delta: int = 0,
                  hours_delta: int = 0,
                  minutes_delta: int = 0,
                  seconds_delta: int = 0,
                  **kwargs):
@@ -331,18 +331,18 @@
         minutes_delta : int, default 0
             An integer value of minutes to add or subtract from now
         seconds_delta : int, default 0
             An integer value of seconds to add or subtract from now
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._days_delta = days_delta
-        self._hours_delta = hours_delta
-        self._minutes_delta = minutes_delta
-        self._seconds_delta = seconds_delta
+        self._days_delta: int = days_delta
+        self._hours_delta: int = hours_delta
+        self._minutes_delta: int = minutes_delta
+        self._seconds_delta: int = seconds_delta
 
     def render(
             self,
     ) -> str:
         """Render a stringified date time value.
 
         Returns
@@ -370,15 +370,15 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "auto_increment"
+    KEY: str = "auto_increment"
 
     def __init__(
             self,
             pattern: str = "{:05d}",
             **kwargs,
     ):
         """Initialize AutoIncrementUtil class.
@@ -386,20 +386,20 @@
         Parameters
         ----------
         pattern : str, default '{:05d}'
             A pattern to inject incremented ID
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._pattern = pattern
+        self._pattern: str = pattern
 
     @mimeo_context
     def render(
             self,
-            context: MimeoContext = None,
+            context: MimeoContext | None = None,
     ) -> str:
         """Render an auto incremented identifier.
 
         Parameters
         ----------
         context : MimeoContext, default None
             A current Mimeo Context injected by a decorator
@@ -439,36 +439,36 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "curr_iter"
+    KEY: str = "curr_iter"
 
     def __init__(
             self,
-            context: str = None,
+            context: str | None = None,
             **kwargs,
     ):
         """Initialize CurrentIterationUtil class.
 
         Parameters
         ----------
         context : str, default None
             A context name to reach the current iteration
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._context_name = context
+        self._context_name: str = context
 
     @mimeo_context
     def render(
             self,
-            context: MimeoContext = None,
+            context: MimeoContext | None = None,
     ) -> int:
         """Render a current iteration ID.
 
         Parameters
         ----------
         context : MimeoContext, default None
             A current Mimeo Context injected by a decorator
@@ -497,40 +497,40 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "key"
+    KEY: str = "key"
 
     def __init__(
             self,
-            context: str = None,
-            iteration: int = None,
+            context: str | None = None,
+            iteration: int | None = None,
             **kwargs,
     ):
         """Initialize KeyUtil class.
 
         Parameters
         ----------
         context : str, default None
             A context name to reach already generated identifier
         iteration : int, default None
             A iteration id to reach already generated identifier
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._context_name = context
-        self._iteration = iteration
+        self._context_name: str = context
+        self._iteration: int = iteration
 
     @mimeo_context
     def render(
             self,
-            context: MimeoContext = None,
+            context: MimeoContext | None = None,
     ) -> str:
         """Render a unique identifier.
 
         By default, Key Mimeo Util renders identifier from the current
         iteration of the current Mimeo Context.
         If the context name is parametrized and iteration is not, then
         identifier is pulled from the current iteration of THIS
@@ -570,42 +570,42 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "city"
-    _MIMEO_DB = MimeoDB()
+    KEY: str = "city"
+    _MIMEO_DB: MimeoDB = MimeoDB()
 
     def __init__(
             self,
             unique: bool = True,
-            country: str = None,
+            country: str | None = None,
             **kwargs,
     ):
         """Initialize CityUtil class.
 
         Parameters
         ----------
         unique : bool, default True
             Indicates if rendered city names will be unique across
             a Mimeo Context
         country : str, default None
             A country limiting city names that can be rendered
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._unique = unique
-        self._country = country
+        self._unique: bool = unique
+        self._country: str = country
 
     @mimeo_context
     def render(
             self,
-            context: MimeoContext = None,
+            context: MimeoContext | None = None,
     ) -> str:
         """Render a city name.
 
         By default, City Mimeo Util generates a unique city name across
         a Mimeo Context without `country` limitation. If `country` is
         parametrized, then this Mimeo Util will render only those
         city names that lie in the specific country.
@@ -665,27 +665,27 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "country"
+    KEY: str = "country"
 
-    _VALUE_NAME = "name"
-    _VALUE_ISO3 = "iso3"
-    _VALUE_ISO2 = "iso2"
-    _SUPPORTED_VALUES = (_VALUE_NAME, _VALUE_ISO3, _VALUE_ISO2)
-    _MIMEO_DB = MimeoDB()
+    _VALUE_NAME: str = "name"
+    _VALUE_ISO3: str = "iso3"
+    _VALUE_ISO2: str = "iso2"
+    _SUPPORTED_VALUES: tuple = (_VALUE_NAME, _VALUE_ISO3, _VALUE_ISO2)
+    _MIMEO_DB: MimeoDB = MimeoDB()
 
     def __init__(
             self,
-            value: str = None,
+            value: str | None = None,
             unique: bool = True,
-            country: str = None,
+            country: str | None = None,
             **kwargs,
     ):
         """Initialize CountryUtil class.
 
         Parameters
         ----------
         value : str, default 'name'
@@ -695,22 +695,22 @@
             Indicates if rendered country names will be unique across
             a Mimeo Context
         country : str, default None
             A one country detail to get its other detail
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._value = value if value is not None else self._VALUE_NAME
-        self._unique = unique
-        self._country = country
+        self._value: str = value if value is not None else self._VALUE_NAME
+        self._unique: bool = unique
+        self._country: str = country
 
     @mimeo_context
     def render(
             self,
-            context: MimeoContext = None,
+            context: MimeoContext | None = None,
     ) -> str:
         """Render a country name.
 
         By default, Country Mimeo Util generates a unique country name
         across a Mimeo Context. If `value` is parametrized, then it
         will render a specific country detail (name, ISO3 code or ISO2
         code). This Mimeo Util allows you to provide a `country` detail
@@ -785,26 +785,26 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "currency"
+    KEY: str = "currency"
 
-    _VALUE_CODE = "code"
-    _VALUE_NAME = "name"
-    _SUPPORTED_VALUES = (_VALUE_CODE, _VALUE_NAME)
-    _MIMEO_DB = MimeoDB()
+    _VALUE_CODE: str = "code"
+    _VALUE_NAME: str = "name"
+    _SUPPORTED_VALUES: tuple = (_VALUE_CODE, _VALUE_NAME)
+    _MIMEO_DB: MimeoDB = MimeoDB()
 
     def __init__(
             self,
-            value: str = None,
+            value: str | None = None,
             unique: bool = False,
-            country: str = None,
+            country: str | None = None,
             **kwargs,
     ):
         """Initialize CurrencyUtil class.
 
         Parameters
         ----------
         value : str, default 'code'
@@ -814,22 +814,22 @@
             Indicates if rendered currency codes will be unique across
             a Mimeo Context
         country : str, default None
             A country of which the currency should be rendered
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._value = value if value is not None else self._VALUE_CODE
-        self._unique = unique
-        self._country = country
+        self._value: str = value if value is not None else self._VALUE_CODE
+        self._unique: bool = unique
+        self._country: str = country
 
     @mimeo_context
     def render(
             self,
-            context: MimeoContext = None,
+            context: MimeoContext | None = None,
     ) -> str:
         """Render a currency code.
 
         By default, Currency Mimeo Util generates a non-unique currency code across
         a Mimeo Context. If `value` is parametrized, then it will render a specific
         currency detail (code or name). This Mimeo Util allows you to provide
         a `country` to get a currency being used there. When `country` is parametrized,
@@ -896,42 +896,42 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "first_name"
-    __MIMEO_DB = MimeoDB()
+    KEY: str = "first_name"
+    __MIMEO_DB: MimeoDB = MimeoDB()
 
     def __init__(
             self,
             unique: bool = True,
-            sex: str = None,
+            sex: str | None = None,
             **kwargs,
     ):
         """Initialize FirstNameUtil class.
 
         Parameters
         ----------
         unique : bool, default True
             Indicates if rendered forenames will be unique across
             a Mimeo Context
         sex : str, default None
             A sex to limit forenames
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._unique = unique
-        self._sex = self._standardize_sex(sex)
+        self._unique: bool = unique
+        self._sex: str = self._standardize_sex(sex)
 
     @mimeo_context
     def render(
             self,
-            context: MimeoContext = None,
+            context: MimeoContext | None = None,
     ) -> str:
         """Render a first name.
 
         By default, First Name Mimeo Util generates a unique forename
         across a Mimeo Context without sex limitation. If `sex` is
         parametrized, then this Mimeo Util will render only those
         first names that are assigned to the specific sex.
@@ -998,16 +998,16 @@
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
-    KEY = "last_name"
-    __MIMEO_DB = MimeoDB()
+    KEY: str = "last_name"
+    __MIMEO_DB: MimeoDB = MimeoDB()
 
     def __init__(
             self,
             unique: bool = True,
             **kwargs,
     ):
         """Initialize LastNameUtil class.
@@ -1016,20 +1016,20 @@
         ----------
         unique : bool, default True
             Indicates if rendered forenames will be unique across
             a Mimeo Context
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._unique = unique
+        self._unique: bool = unique
 
     @mimeo_context
     def render(
             self,
-            context: MimeoContext = None,
+            context: MimeoContext | None = None,
     ) -> str:
         """Render a last name.
 
         By default, First Name Mimeo Util generates a unique surname
         across a Mimeo Context.
 
         Parameters
```

### Comparing `mimeograph-0.7.0/src/mimeo/utils/renderers.py` & `mimeograph-1.0.3/src/mimeo/generators/json_generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,697 +1,623 @@
-"""The Mimeo Renderers module.
+"""The Mimeo JSON Generator module.
 
-This module contains classes useful in value rendering. It exports
-the following renderers:
-    * MimeoRenderer
-        A Facade class rendering Mimeo Utils, Vars and Special Fields.
-    * UtilsRenderer
-        A class rendering Mimeo Utils.
-    * VarsRenderer
-        A class rendering Mimeo Vars.
-    * SpecialFieldsRenderer
-        A class rendering Mimeo Special Fields.
+It exports only one class:
+    * JSONGenerator
+        A Generator implementation producing data in the JSON format.
 """
 from __future__ import annotations
 
+import json
 import logging
-import re
-from typing import Any
+from typing import Iterator
 
 from mimeo.config import constants as cc
-from mimeo.context import MimeoContext, MimeoContextManager
+from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
+from mimeo.context import MimeoContext
 from mimeo.context.decorators import mimeo_context
-from mimeo.utils import (AutoIncrementUtil, CityUtil, CountryUtil,
-                         CurrencyUtil, CurrentIterationUtil, DateTimeUtil,
-                         DateUtil, FirstNameUtil, KeyUtil, LastNameUtil,
-                         MimeoUtil, RandomIntegerUtil, RandomItemUtil,
-                         RandomStringUtil)
-from mimeo.utils.exc import InvalidMimeoUtilError, NotASpecialFieldError
+from mimeo.generators import Generator
+from mimeo.utils import MimeoRenderer
 
 logger = logging.getLogger(__name__)
 
 
-class UtilsRenderer:
-    """A class rendering Mimeo Utils.
+class JSONGenerator(Generator):
+    """A Generator implementation producing data in the JSON format.
 
-    It contains only class methods.
+    This Generator is instantiated for the 'json' output format
+    and produces data using Mimeo Configuration.
 
     Methods
     -------
-    render_raw(mimeo_util_key: str) -> Any
-        Render a Mimeo Util in a raw form.
-    render_parametrized(mimeo_util_config: dict) -> Any
-        Render a Mimeo Util in a parametrized form.
+    generate(
+        templates: list | Iterator[MimeoTemplate],
+        parent: dict = None
+    ) -> Iterator[dict]
+        Generate JSON data based on the Mimeo Configuration.
+    stringify(
+        data: json
+    ) -> str
+        Stringify data generated by the generate() method.
     """
 
-    MIMEO_UTILS = {
-        RandomStringUtil.KEY: RandomStringUtil,
-        RandomIntegerUtil.KEY: RandomIntegerUtil,
-        RandomItemUtil.KEY: RandomItemUtil,
-        DateUtil.KEY: DateUtil,
-        DateTimeUtil.KEY: DateTimeUtil,
-        AutoIncrementUtil.KEY: AutoIncrementUtil,
-        CurrentIterationUtil.KEY: CurrentIterationUtil,
-        KeyUtil.KEY: KeyUtil,
-        CityUtil.KEY: CityUtil,
-        CountryUtil.KEY: CountryUtil,
-        CurrencyUtil.KEY: CurrencyUtil,
-        FirstNameUtil.KEY: FirstNameUtil,
-        LastNameUtil.KEY: LastNameUtil,
-    }
-    _INSTANCES = {}
-
-    @classmethod
-    def render_raw(
-            cls,
-            mimeo_util_key: str,
-    ) -> Any:
-        """Render a Mimeo Util in a raw form.
+    def __init__(
+            self,
+            mimeo_config: MimeoConfig,
+    ):
+        """Initialize JSONGenerator class.
 
         Parameters
         ----------
-        mimeo_util_key : str
-            A Mimeo Util key (name)
-
-        Returns
-        -------
-        Any
-            Rendered Mimeo Util value.
-
-        Raises
-        ------
-        InvalidMimeoUtilError
-            If the Mimeo Util name does not match any existing Mimeo
-            Util.
+        mimeo_config : MimeoConfig
+            A Mimeo Configuration
         """
-        return cls.render_parametrized({cc.MODEL_MIMEO_UTIL_NAME_KEY: mimeo_util_key})
-
-    @classmethod
-    def render_parametrized(
-            cls,
-            mimeo_util_config: dict,
-    ) -> Any:
-        """Render a Mimeo Util in a parametrized form.
-
-        Parameters
-        ----------
-        mimeo_util_config : dict
-            A Mimeo Util configuration
-
-        Returns
-        -------
-        Any
-            Rendered Mimeo Util value.
-
-        Raises
-        ------
-        InvalidMimeoUtilError
-            If the Mimeo Util configuration does not include Mimeo
-            Util name, or the parametrized name does not match any
-            existing Mimeo Util.
-        InvalidValueError
-            If a Mimeo Util is incorrectly parametrized.
-        InvalidSexError
-            If the First Name Mimeo Util has not supported `sex`
-            parameter value assigned.
-        """
-        logger.fine("Rendering a mimeo util [%s]", mimeo_util_config)
-        mimeo_util = cls._get_mimeo_util(mimeo_util_config)
-        return mimeo_util.render()
+        self._indent: int = mimeo_config.output.indent
 
     @classmethod
-    def _get_mimeo_util(
+    def generate(
             cls,
-            config: dict,
-    ) -> MimeoUtil:
-        """Get a Mimeo Util instance based on the configuration.
+            templates: list | Iterator[MimeoTemplate],
+            parent: dict | list | None = None,
+    ) -> Iterator[dict]:
+        """Generate JSON data based on the Mimeo Configuration.
 
-        All instances are cached to not re-create a Util with the same
-        parameters. This method instantiate a Mimeo Util for the first
-        time and use the one in the future.
+        This function is used recursively when a Mimeo Configuration
+        contains nested templates.
+        It iterates through all templates configured and yields data
+        units.
 
         Parameters
         ----------
-        config : dict
-            A Mimeo Util configuration
+        templates : list | Iterator[MimeoTemplate]
+            A collection of Mimeo Templates to process
+        parent : dict | list | None, default None
+            A parent node for the currently processed template.
+            It is passed only when a Mimeo Config contain nested
+            templates.
 
         Returns
         -------
-        MimeoUtil
-            A Mimeo Util instance
-
-        Raises
-        ------
-        InvalidMimeoUtilError
-            If the Mimeo Util configuration does not include Mimeo
-            Util name, or the parametrized name does not match any
-            existing Mimeo Util.
-        """
-        cache_key = cls._generate_cache_key(config)
-        if cache_key not in cls._INSTANCES:
-            return cls._instantiate_mimeo_util(cache_key, config)
-        return cls._INSTANCES.get(cache_key)
-
-    @staticmethod
-    def _generate_cache_key(
-            config: dict,
-    ) -> str:
-        """Generate an internal Mimeo Util key from its parameters.
-
-        This method ensures that Mimeo Util instances are cached
-        properly for the same parameters.
-
-        Parameters
-        ----------
-        config : dict
-            A Mimeo Util configuration
-
-        Returns
-        -------
-        str
-            An internal Mimeo Util cache key
+        Iterator[ElemTree.Element]
+            Iterator for generated nodes
         """
-        return "-".join(":".join([key, str(val)]) for key, val in config.items())
-
-    @classmethod
-    def _instantiate_mimeo_util(
-            cls,
-            cache_key: str,
-            config: dict,
-    ) -> MimeoUtil:
-        """Instantiate a Mimeo Util based on the configuration.
-
-        After instantiation the Mimeo Util is cached for the future.
-
-        Parameters
-        ----------
-        cache_key : str
-            An internal Mimeo Util cache key
-        config : dict
-            A Mimeo Util configuration
+        for template in templates:
+            for data_unit in cls._process_single_template(template, parent):
+                yield data_unit
 
-        Returns
-        -------
-        MimeoUtil
-            A Mimeo Util instance
-
-        Raises
-        ------
-        InvalidMimeoUtilError
-            If the Mimeo Util configuration does not include Mimeo
-            Util name, or the parametrized name does not match any
-            existing Mimeo Util.
-        """
-        mimeo_util_name = cls.get_mimeo_util_name(config)
-        mimeo_util = cls.MIMEO_UTILS.get(mimeo_util_name)(**config)
-        cls._INSTANCES[cache_key] = mimeo_util
-        return mimeo_util
-
-    @classmethod
-    def get_mimeo_util_name(
-            cls,
-            config: dict,
+    def stringify(
+            self,
+            data_unit: dict,
     ) -> str:
-        """Return a verified Mimeo Util name.
+        """Stringify JSON data generated by the generate() method.
 
         Parameters
         ----------
-        config : dict
-            A Mimeo Util configuration
+        data_unit: dict
+            A single data unit generated by the generate() method
 
         Returns
         -------
         str
-            A Mimeo Util name
-
-        Raises
-        ------
-        InvalidMimeoUtilError
-            If the Mimeo Util configuration does not include Mimeo
-            Util name, or the parametrized name does not match any
-            existing Mimeo Util.
-        """
-        mimeo_util_name = config.get(cc.MODEL_MIMEO_UTIL_NAME_KEY)
-        if mimeo_util_name is None:
-            code = InvalidMimeoUtilError.Code.ERR_1
-            raise InvalidMimeoUtilError(code, config=config)
-        if mimeo_util_name not in cls.MIMEO_UTILS:
-            code = InvalidMimeoUtilError.Code.ERR_2
-            raise InvalidMimeoUtilError(code, name=mimeo_util_name)
-        return mimeo_util_name
-
-
-class VarsRenderer:
-    """A class rendering Mimeo Vars.
-
-    It contains only a class method.
-
-    Methods
-    -------
-    render(var: str) -> Any
-        Render a Mimeo Var.
-    """
-
-    @classmethod
-    def render(
-            cls,
-            var: str,
-    ) -> str | int | bool | dict:
-        """Render a Mimeo Var.
-
-        Parameters
-        ----------
-        var : str
-            A variable name
-
-        Returns
-        -------
-        Any
-            A variable value
-
-        Raises
-        ------
-        InstanceNotAliveError
-            If the MimeoContextManager instance is not alive
-        VarNotFoundError
-            If the Mimeo Var with the `var` provided does not exist
+            Stringified data unit
         """
-        logger.fine("Rendering a variable [%s]", var)
-        return MimeoContextManager().get_var(var)
-
+        if self._indent is not None and self._indent != 0:
+            return json.dumps(data_unit, indent=self._indent)
 
-class SpecialFieldsRenderer:
-    """A class rendering Mimeo Special Fields.
-
-    It contains only a class method.
-
-    Methods
-    -------
-    render(field_name: str, context: MimeoContext = None) -> Any
-        Render a Mimeo Special Field.
-    """
+        return json.dumps(data_unit)
 
     @classmethod
     @mimeo_context
-    def render(
+    def _process_node(
             cls,
-            field: str,
-            context: MimeoContext = None,
-    ) -> str | int | bool:
-        """Render a Mimeo Special Field.
+            parent: dict | list | None,
+            node_meta: dict,
+            context: MimeoContext | None = None,
+    ) -> dict | list:
+        """Process a single template's node.
+
+        Extends Generator's implementation by setting a parent node when it is None.
+        It is required for JSON format to initialize an object.
 
         Parameters
         ----------
-        field : str
-            A special field name
+        parent : dict | list | None
+            A parent node
+        node_meta : dict
+            Node's metadata
         context : MimeoContext, default None
-            A current Mimeo Context injected by a decorator
+            The current Mimeo Context (injected by MimeoContextManager)
 
         Returns
         -------
-        str | int | bool
+        dict | list
+            A single data unit generated within a single template iteration.
 
         Raises
         ------
-        UninitializedContextIterationError
-            If no iteration has been initialized yet for the context
+        InvalidSpecialFieldValueError
+            If a special field value is dict or list
         SpecialFieldNotFoundError
-            If the special field does not exist.
+            If a special field does not exist.
         """
-        logger.fine("Rendering a special field [%s]", field)
-        return context.curr_iteration().get_special_field(field)
-
-
-class MimeoRenderer:
-    """A Facade class rendering Mimeo Utils, Vars and Special Fields.
-
-    It contains only class methods.
-
-    Methods
-    -------
-    render(value: Any) -> Any
-        Render a value.
-    get_special_field_name(wrapped_field_name: str) -> str
-        Extract a special field name.
-    is_special_field(special_field: str) -> bool
-        Verify if the field is special (of form {:FIELD_NAME:}).
-    is_raw_mimeo_util(value: str) -> bool
-        Verify if the value is a raw Mimeo Util.
-    is_parametrized_mimeo_util(value: dict)
-        Verify if the value is a parametrized Mimeo Util.
-    """
-
-    _UTILS_PATTERN = re.compile("^{(.+)}$")
-    _VARS_PATTERN = re.compile(".*({[A-Z_0-9]+})")
-    _SPECIAL_FIELDS_PATTERN = re.compile(".*({:([a-zA-Z]+:)?[-_a-zA-Z0-9]+:})")
+        parent = parent if parent is not None else {}
+        return super()._process_node(parent, node_meta, context)
 
     @classmethod
-    def get_special_field_name(
+    def _pre_process_node(
             cls,
-            wrapped_field_name: str,
-    ) -> str:
-        """Extract a special field name.
-
-        Parameters
-        ----------
-        wrapped_field_name : str
-            A field name wrapped with curly braces and colons,
-            e.g. :Field:
-
-        Returns
-        -------
-        str
-            A special field name
-
-        Raises
-        ------
-        NotASpecialFieldError
-            If the `wrapped_field_name` is not of form :FIELD_NAME:
-        """
-        if not cls.is_special_field(wrapped_field_name):
-            raise NotASpecialFieldError(wrapped_field_name)
+            node_meta: dict,
+    ) -> dict:
+        """Pre-process node's metadata.
 
-        return wrapped_field_name[1:][:-1]
-
-    @classmethod
-    def is_special_field(
-            cls,
-            special_field: str,
-    ) -> bool:
-        """Verify if the field is special (of form :FIELD_NAME:).
+        This function adjusts existing node's metadata and completes it with custom
+        properties:
+        * the name property is changed only for special fields
+          - field name is extracted
+        * the mimeo_util property is being initialized
+          - True if element's value is a parametrized mimeo_util. Otherwise, False.
+        * the special property is being initialized
+          - True, when a field is special. Otherwise, False.
 
         Parameters
         ----------
-        special_field : str
-            A special field
+        node_meta : dict
+            Initial node's metadata
 
         Returns
         -------
-        bool
-            True if the field is of form :FIELD_NAME:. Otherwise,
-            False.
+        dict
+            Complete node's metadata
         """
-        return bool(re.match(r"^:([a-zA-Z]+:)?[-_a-zA-Z0-9]+:$", special_field))
+        name = node_meta["name"]
+        value = node_meta["value"]
+        is_mimeo_util = MimeoRenderer.is_parametrized_mimeo_util(value)
+        is_special_field = name is not None and MimeoRenderer.is_special_field(name)
+        if is_special_field:
+            name = MimeoRenderer.get_special_field_name(name)
 
-    @classmethod
-    def is_raw_mimeo_util(
-            cls,
-            value: str,
-    ) -> bool:
-        """Verify if the value is a raw Mimeo Util.
-
-        Parameters
-        ----------
-        value : str
-            A string value
-
-        Returns
-        -------
-        bool
-            True if the value is a raw Mimeo Util, e.g. {random_str}.
-            Otherwise, False.
-        """
-        raw_mimeo_utils = UtilsRenderer.MIMEO_UTILS.keys()
-        raw_mimeo_utils_re = "^{(" + "|".join(raw_mimeo_utils) + ")}$"
-        return bool(re.match(raw_mimeo_utils_re, value))
+        return cls._node_meta(
+            name=name,
+            value=value,
+            is_mimeo_util=is_mimeo_util,
+            is_special_field=is_special_field)
 
     @classmethod
-    def is_parametrized_mimeo_util(
+    def _process_complex_value(
             cls,
-            value: dict,
-    ):
-        """Verify if the value is a parametrized Mimeo Util.
+            parent: dict | list,
+            node_meta: dict,
+    ) -> dict | list:
+        """Process a node with a complex value.
 
-        Parameters
-        ----------
-        value : dict
-            A dict value
-
-        Returns
-        -------
-        bool
-            True if the value is a dictionary having only one key,
-            "_mimeo_util". Otherwise, False.
-        """
-        return (isinstance(value, dict) and
-                len(value) == 1 and
-                cc.MODEL_MIMEO_UTIL_KEY in value)
-
-    @classmethod
-    def render(
-            cls,
-            value: Any,
-    ) -> Any:
-        """Render a value.
-
-        This method renders a value accordingly to its type and form.
-        If the value takes a form of Mimeo Util it is rendered as
-        Mimeo Util (raw or parametrized); if it takes a form of
-        a special field this renderer will try to reach it from
-        the current context; when the value takes a form of a Mimeo Var,
-        then it uses Mimeo Vars defined in Mimeo Config.
-        Otherwise, the raw value is returned.
-        It is recursively called to return a final value.
+        The node is processed accordingly to its value type.
+        When the type is dict, and it includes the _templates_ property, node
+        is processed in a special way.
 
         Parameters
         ----------
-        value : Any
-            A value to be rendered
+        parent : dict | list
+            A parent node
+        node_meta : dict
+            Node's metadata
 
         Returns
         -------
-        Any
-            A rendered value
+        dict | list
+            A processed node
 
         Raises
         ------
-        InstanceNotAliveError
-            If the MimeoContextManager instance is not alive
-        UninitializedContextIterationError
-            If no iteration has been initialized yet for the context
-        VarNotFoundError
-            If the Mimeo Var does not exist
-        InvalidMimeoUtilError
-            If the Mimeo Util node has missing _name property, or it
-            does not match any Mimeo Util.
-        InvalidValueError
-            If Mimeo Util node is incorrectly parametrized
-        OutOfStockError
-            If all unique values have been consumed already
-        DataNotFoundError
-            If database does not contain the expected value
-        InvalidSexError
-            If the First Name Mimeo Util has not supported `sex`
-            parameter value assigned.
-        """
-        logger.fine("Rendering a value [%s]", value)
-        try:
-            if isinstance(value, str):
-                value = cls._render_string_value(value)
-            if cls.is_parametrized_mimeo_util(value):
-                value = cls._render_parametrized_mimeo_util(value)
-        except Exception:
-            logger.exception("An error occurred for [%s].", value)
-            raise
-        return value
-
-    @classmethod
-    def _render_string_value(
-            cls,
-            value: str,
-    ) -> Any:
-        """Render a string value.
-
-        Depending on value form it can render it as a raw value,
-        a special field, a Mimeo Var or a raw Mimeo Util.
-
-        Parameters
-        ----------
-        value : str
-            A string value
-
-        Returns
-        -------
-        Any
-            A rendered value
+        InvalidSpecialFieldValueError
+            If a special field value is dict or list
+        SpecialFieldNotFoundError
+            If a special field does not exist.
         """
-        if cls._SPECIAL_FIELDS_PATTERN.match(value):
-            return cls._render_special_field(value)
-        if cls._VARS_PATTERN.match(value):
-            return cls._render_var(value)
-        if cls.is_raw_mimeo_util(value):
-            return cls._render_raw_mimeo_util(value)
-        return value
+        if (isinstance(node_meta["value"], dict) and
+                cc.TEMPLATES_KEY not in node_meta["value"]):
+            func = cls._process_dict_value
+        elif isinstance(node_meta["value"], list):
+            func = cls._process_list_value
+        else:
+            func = cls._process_templates_value
+        return func(parent, node_meta)
 
     @classmethod
-    def _render_special_field(
+    def _process_dict_value(
             cls,
-            value: str,
-    ) -> Any:
-        """Render a value containing a Mimeo Special Field.
+            parent: dict | list,
+            node_meta: dict,
+    ) -> dict | list:
+        """Process a node with a dictionary value.
 
-        This method finds first special field and replaces all
-        occurrences. Then the result is passed to the render() method
-        again, to return a final value.
+        It iterates through the dictionary items and processes each of them.
 
         Parameters
         ----------
-        value : str
-            A value containing a Mimeo Special Field
+        parent : dict | list
+            A parent node
+        node_meta : dict
+            Node's metadata
 
         Returns
         -------
-        Any
-            A rendered value
+        dict | list
+            A processed node
 
         Raises
         ------
-        UninitializedContextIterationError
-            If no iteration has been initialized yet for the context
+        InvalidSpecialFieldValueError
+            If a special field value is dict or list
         SpecialFieldNotFoundError
-            If the special field does not exist.
-        """
-        match = next(cls._SPECIAL_FIELDS_PATTERN.finditer(value))
-        wrapped_special_field = match.group(1)
-        r_val = SpecialFieldsRenderer.render(wrapped_special_field[2:][:-2])
-        logger.fine("Rendered special field value [%s]", r_val)
-        if len(wrapped_special_field) != len(value):
-            r_val = str(r_val).lower() if isinstance(r_val, bool) else str(r_val)
-            r_val = value.replace(wrapped_special_field, str(r_val))
-        return cls.render(r_val)
+            If a special field does not exist.
 
-    @classmethod
-    def _render_var(
-            cls,
-            value: str,
-    ) -> Any:
-        """Render a value containing a Mimeo Var.
-
-        This method finds first variable and replaces all occurrences.
-        Then the result is passed to the render() method again, to
-        return a final value.
-
-        Parameters
-        ----------
-        value : str
-            A value containing a Mimeo Var
+        Examples
+        --------
+        parent = {}
+        node_meta = cls._node_meta(
+            name="SomeField",
+            value={"SomeChild1": 1, "SomeChild2": 2},
+        )
+        cls._process_dict_value(parent, node_meta)
+        ->
+        {
+          "SomeField": {
+            "SomeChild1": 1,
+            "SomeChild2": 2,
+          },
+        }
+
+        parent = []
+        node_meta = cls._node_meta(
+            name=None,
+            value={"SomeChild1": 1, "SomeChild2": 2},
+        )
+        cls._process_dict_value(parent, node_meta)
+        ->
+        [
+          {
+            "SomeChild1": 1,
+            "SomeChild2": 2,
+          },
+        ]
+        """
+        element = cls._create_node(parent, node_meta)
+        for child_tag, child_value in node_meta["value"].items():
+            cls._process_node(element, cls._node_meta(child_tag, child_value))
+        return parent
+
+    @classmethod
+    def _process_list_value(
+            cls,
+            parent: dict | list,
+            node_meta: dict,
+    ) -> dict | list:
+        """Process a node with a list value.
+
+        It iterates through the list items and processes each of them: generates
+        a child element for each value as direct children of the parent.
+
+        Parameters
+        ----------
+        parent : dict | list
+            A parent node
+        node_meta : dict
+            Node's metadata
 
         Returns
         -------
-        Any
-            A rendered value
+        dict | list
+            A processed node
 
         Raises
         ------
-        InstanceNotAliveError
-            If the MimeoContextManager instance is not alive
-        VarNotFoundError
-            If the Mimeo Var with the `var` provided does not exist
-        """
-        match = next(cls._VARS_PATTERN.finditer(value))
-        wrapped_var = match.group(1)
-        r_val = VarsRenderer.render(wrapped_var[1:][:-1])
-        logger.fine("Rendered variable value [%s]", r_val)
-        if cls.is_parametrized_mimeo_util(r_val):
-            r_val = cls._render_parametrized_mimeo_util(r_val)
-        if len(wrapped_var) != len(value):
-            r_val = str(r_val).lower() if isinstance(r_val, bool) else str(r_val)
-            r_val = value.replace(wrapped_var, str(r_val))
-        return cls.render(r_val)
-
-    @classmethod
-    def _render_raw_mimeo_util(
-            cls,
-            value: str,
-    ) -> Any:
-        """Render a raw Mimeo Util.
+        InvalidSpecialFieldValueError
+            If the special field value is dict or list
+        SpecialFieldNotFoundError
+            If the special field does not exist.
 
-        Parameters
-        ----------
-        value : str
-            A raw Mimeo Util
+        Examples
+        --------
+        parent = {}
+        node_meta = cls._node_meta(
+            name="SomeField",
+            value=[
+                'value-1',
+                {'SomeChild1': True, 'SomeChild2': False},
+                {'_mimeo_util': {'_name': 'auto_increment', 'pattern': '{}'}}
+            ],
+        )
+        cls._process_list_value_with_atomic_children(parent, node_meta)
+        ->
+        {
+          "SomeField": [
+            "value-1",
+            {
+                "SomeChild1": True,
+                "SomeChild2": False,
+            },
+            1,
+          ],
+        }
+
+        parent = []
+        node_meta = cls._node_meta(
+            name=None,
+            value=[
+                'value-1',
+                {'SomeChild1': True, 'SomeChild2': False},
+                {'_mimeo_util': {'_name': 'auto_increment', 'pattern': '{}'}}
+            ],
+        )
+        cls._process_list_value_with_atomic_children(parent, node_meta)
+        ->
+        [
+          [
+            "value-1",
+            {
+                "SomeChild1": True,
+                "SomeChild2": False,
+            },
+            1,
+          ],
+        ]
+        """
+        element = cls._create_node(parent, node_meta)
+        for child in node_meta["value"]:
+            node_meta = cls._node_meta(None, child)
+            cls._process_node(element, node_meta)
+        return parent
+
+    @classmethod
+    def _process_templates_value(
+            cls,
+            parent: dict | list,
+            node_meta: dict,
+    ) -> dict | list:
+        """Process a node with a dictionary value storing templates.
+
+        It iterates through the templates and generates data based on them.
+        If parent is a dict, the property name will take a value of an array.
+        All properties at the same level as _templates_ will be ignored.
+
+        Parameters
+        ----------
+        parent : dict | None
+            A parent node
+        node_meta : dict
+            Node's metadata
 
         Returns
         -------
-        Any
-            A rendered value
+        dict | list
+            A processed node
 
         Raises
         ------
-        OutOfStockError
-            If all unique values have been consumed already
-        DataNotFoundError
-            If database does not contain the expected value
-        """
-        rendered_value = UtilsRenderer.render_raw(value[1:][:-1])
-        return cls.render(rendered_value)
-
-    @classmethod
-    def _render_parametrized_mimeo_util(
-            cls,
-            value: dict,
-    ) -> Any:
-        """Render a parametrized Mimeo Util.
-
-        Before the Mimeo Util itself will be rendered, first all its
-        parameters (except name) are rendered.
+        InvalidSpecialFieldValueError
+            If a special field value is dict or list
+        SpecialFieldNotFoundError
+            If a special field does not exist.
 
-        Parameters
-        ----------
-        value : str
-            A parametrized Mimeo Util
+        Examples
+        --------
+        parent = []
+        node_meta = cls._node_meta(
+            name=None,
+            value={"_templates_": [
+                {
+                  "count": 10,
+                  "model": {
+                    "SomeChild": {
+                      "Node1": 1,
+                      "Node2": "value-2",
+                      "Node3": true
+                    }
+                  }
+                }
+            ]},
+        )
+        cls._process_templates_value(parent, node_meta)
+        ->
+        [
+          {
+            "SomeChild": {
+              "Node1": 1,
+              "Node2": "value-2",
+              "Node3": true,
+            },
+          },
+          {
+            "SomeChild": {
+              "Node1": 1,
+              "Node2": "value-2",
+              "Node3": true,
+            },
+          },
+          ... x10
+        ]
+
+        parent = {}
+        node_meta = cls._node_meta(
+            name="SomeField",
+            value={"_templates_": [
+                {
+                  "count": 10,
+                  "model": {
+                    "SomeChild": {
+                      "Node1": 1,
+                      "Node2": "value-2",
+                      "Node3": true
+                    }
+                  }
+                }
+            ]},
+        )
+        cls._process_templates_value(parent, node_meta)
+        ->
+        {
+          "SomeField": [
+            {
+              "SomeChild": {
+                "Node1": 1,
+                "Node2": "value-2",
+                "Node3": true,
+              },
+            },
+            {
+              "SomeChild": {
+                "Node1": 1,
+                "Node2": "value-2",
+                "Node3": true,
+              },
+            },
+            ... x10
+          ],
+        }
+        """
+        templates = (MimeoTemplate(template)
+                     for template in node_meta["value"][cc.TEMPLATES_KEY])
+        target = parent
+        if isinstance(parent, dict):
+            parent[node_meta["name"]] = []
+            target = parent[node_meta["name"]]
+
+        for child in cls.generate(templates):
+            target.append(child)
+        return parent
+
+    @classmethod
+    def _process_atomic_value(
+            cls,
+            parent: dict | list,
+            node_meta: dict,
+            context: MimeoContext,
+    ) -> dict | list:
+        """Process a node with an atomic value.
+
+        A parametrized Mimeo Util is considered as an atomic value as representing one.
+        It renders a value for the node.
+
+        Parameters
+        ----------
+        parent : dict | list
+            A parent node
+        node_meta : dict
+            Node's metadata
+        context : MimeoContext, default None
+            The current Mimeo Context (injected by MimeoContextManager)
 
         Returns
         -------
-        Any
-            A rendered value
+        dict | list
+            A processed node
 
         Raises
         ------
-        InvalidValueError
-            If a Mimeo Util is incorrectly parametrized.
-        OutOfStockError
-            If all unique values have been consumed already
-        DataNotFoundError
-            If database does not contain the expected value
-        InvalidSexError
-            If the First Name Mimeo Util has not supported `sex`
-            parameter value assigned.
-        """
-        mimeo_util = value[cc.MODEL_MIMEO_UTIL_KEY]
-        mimeo_util = cls._render_mimeo_util_parameters(mimeo_util)
-        logger.fine("Pre-rendered mimeo util [%s]", mimeo_util)
-        r_val = UtilsRenderer.render_parametrized(mimeo_util)
-        return cls.render(r_val)
-
-    @classmethod
-    def _render_mimeo_util_parameters(
-            cls,
-            mimeo_util_config: dict,
-    ) -> dict:
-        """Render Mimeo Util's parameters.
+        InvalidSpecialFieldValueError
+            If a special field value is dict or list
+        SpecialFieldNotFoundError
+            If a special field does not exist.
 
-        Parameters
-        ----------
-        mimeo_util_config : dict
-            A parametrized Mimeo Util
+        Examples
+        --------
+        context = MimeoContextManager().get_current_context()
+        parent = {}
+        node_meta = cls._node_meta(
+            name="SomeField",
+            value="value-1",
+        )
+        cls._process_atomic_value(parent, node_meta, context)
+        ->
+        {
+          "SomeField": "value-1"
+        }
+
+        context = MimeoContextManager().get_current_context()
+        parent = []
+        node_meta = cls._node_meta(
+            name=None,
+            value="value-1",
+        )
+        cls._process_atomic_value(parent, node_meta, context)
+        ->
+        [
+          "value-1"
+        ]
+        """
+        value = MimeoRenderer.render(node_meta["value"])
+        if node_meta["special"]:
+            context.curr_iteration().add_special_field(node_meta["name"], value)
+        if isinstance(parent, dict):
+            parent[node_meta["name"]] = value
+        elif isinstance(parent, list):
+            parent.append(value)
+        logger.fine("Rendered value [%s]", value)
+        return parent
 
-        Returns
-        -------
-        dict
-            A Mimeo Util with pre-rendered parameters
+    @staticmethod
+    def _create_node(
+            parent: dict | list,
+            node_meta: dict,
+    ) -> dict | list:
+        """Create an JSON element based on the `parent` and entry value types.
+
+        Parameters
+        ----------
+        parent : dict | list
+            A parent node
+        node_meta : dict
+            Node's metadata
+
+        Returns
+        -------
+        dict | list
+            If the new node's value is dict, returns dict. Otherwise, a list.
+
+        Examples
+        --------
+        parent = {}
+        node_meta = cls._node_meta(
+            name="SomeEntity",
+            value={"SomeField": "value-1"},
+        )
+        node = cls._create_node(parent, node_meta)
+        ->
+        parent: {"SomeEntity": {}}
+        node: {}
+
+        parent = []
+        node_meta = cls._node_meta(
+            name=None,
+            value={"SomeField": "value-1"},
+        )
+        node = cls._create_node(parent, node_meta)
+        ->
+        parent: [{}]
+        node: {}
+
+        parent = []
+        node_meta = cls._node_meta(
+            name=None,
+            value=["value-1"],
+        )
+        node = cls._create_node(parent, node_meta)
+        ->
+        parent: [[]]
+        node: []
+
+        parent = {}
+        node_meta = cls._node_meta(
+            name="SomeEntity",
+            value=["value-1"],
+        )
+        node = cls._create_node(parent, node_meta)
+        ->
+        parent: {"SomeEntity": []}
+        node: []
+        """
+        new_node = {} if isinstance(node_meta["value"], dict) else []
+        if isinstance(parent, list):
+            parent.append(new_node)
+            return parent[-1]
 
-        Raises
-        ------
-        InvalidValueError
-            If a Mimeo Util is incorrectly parametrized.
-        OutOfStockError
-            If all unique values have been consumed already
-        DataNotFoundError
-            If database does not contain the expected value
-        InvalidSexError
-            If the First Name Mimeo Util has not supported `sex`
-            parameter value assigned.
-        """
-        logger.fine("Rendering mimeo util parameters")
-        return {key: cls.render(value) if key != "_name" else value
-                for key, value in mimeo_util_config.items()}
+        parent[node_meta["name"]] = new_node
+        return parent[node_meta["name"]]
```

### Comparing `mimeograph-0.7.0/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,1740 +1,2155 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d69 6d65  : 2.1.Name: mime
 00000020: 6f67 7261 7068 0a56 6572 7369 6f6e 3a20  ograph.Version: 
-00000030: 302e 372e 300a 5375 6d6d 6172 793a 2047  0.7.0.Summary: G
-00000040: 656e 6572 6174 6520 6461 7461 2062 6173  enerate data bas
-00000050: 6564 206f 6e20 6120 7369 6d70 6c65 2074  ed on a simple t
-00000060: 656d 706c 6174 650a 4175 7468 6f72 2d65  emplate.Author-e
-00000070: 6d61 696c 3a20 2254 2e41 2e20 5072 6f67  mail: "T.A. Prog
-00000080: 7261 6d6d 696e 6720 5376 6373 2e22 203c  ramming Svcs." <
-00000090: 746f 6d61 737a 2e6d 6163 6965 6a2e 616e  tomasz.maciej.an
-000000a0: 696f 6c6f 7773 6b69 4067 6d61 696c 2e63  iolowski@gmail.c
-000000b0: 6f6d 3e0a 4c69 6365 6e73 653a 204d 4954  om>.License: MIT
-000000c0: 204c 6963 656e 7365 0a20 2020 2020 2020   License.       
-000000d0: 200a 2020 2020 2020 2020 436f 7079 7269   .        Copyri
-000000e0: 6768 7420 2863 2920 3230 3233 2054 6f6d  ght (c) 2023 Tom
-000000f0: 6173 7a20 416e 696f c582 6f77 736b 690a  asz Anio..owski.
-00000100: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000110: 2050 6572 6d69 7373 696f 6e20 6973 2068   Permission is h
-00000120: 6572 6562 7920 6772 616e 7465 642c 2066  ereby granted, f
-00000130: 7265 6520 6f66 2063 6861 7267 652c 2074  ree of charge, t
-00000140: 6f20 616e 7920 7065 7273 6f6e 206f 6274  o any person obt
-00000150: 6169 6e69 6e67 2061 2063 6f70 790a 2020  aining a copy.  
-00000160: 2020 2020 2020 6f66 2074 6869 7320 736f        of this so
-00000170: 6674 7761 7265 2061 6e64 2061 7373 6f63  ftware and assoc
-00000180: 6961 7465 6420 646f 6375 6d65 6e74 6174  iated documentat
-00000190: 696f 6e20 6669 6c65 7320 2874 6865 2022  ion files (the "
-000001a0: 536f 6674 7761 7265 2229 2c20 746f 2064  Software"), to d
-000001b0: 6561 6c0a 2020 2020 2020 2020 696e 2074  eal.        in t
-000001c0: 6865 2053 6f66 7477 6172 6520 7769 7468  he Software with
-000001d0: 6f75 7420 7265 7374 7269 6374 696f 6e2c  out restriction,
-000001e0: 2069 6e63 6c75 6469 6e67 2077 6974 686f   including witho
-000001f0: 7574 206c 696d 6974 6174 696f 6e20 7468  ut limitation th
-00000200: 6520 7269 6768 7473 0a20 2020 2020 2020  e rights.       
-00000210: 2074 6f20 7573 652c 2063 6f70 792c 206d   to use, copy, m
-00000220: 6f64 6966 792c 206d 6572 6765 2c20 7075  odify, merge, pu
-00000230: 626c 6973 682c 2064 6973 7472 6962 7574  blish, distribut
-00000240: 652c 2073 7562 6c69 6365 6e73 652c 2061  e, sublicense, a
-00000250: 6e64 2f6f 7220 7365 6c6c 0a20 2020 2020  nd/or sell.     
-00000260: 2020 2063 6f70 6965 7320 6f66 2074 6865     copies of the
-00000270: 2053 6f66 7477 6172 652c 2061 6e64 2074   Software, and t
-00000280: 6f20 7065 726d 6974 2070 6572 736f 6e73  o permit persons
-00000290: 2074 6f20 7768 6f6d 2074 6865 2053 6f66   to whom the Sof
-000002a0: 7477 6172 6520 6973 0a20 2020 2020 2020  tware is.       
-000002b0: 2066 7572 6e69 7368 6564 2074 6f20 646f   furnished to do
-000002c0: 2073 6f2c 2073 7562 6a65 6374 2074 6f20   so, subject to 
-000002d0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-000002e0: 6e64 6974 696f 6e73 3a0a 2020 2020 2020  nditions:.      
-000002f0: 2020 0a20 2020 2020 2020 2054 6865 2061    .        The a
-00000300: 626f 7665 2063 6f70 7972 6967 6874 206e  bove copyright n
-00000310: 6f74 6963 6520 616e 6420 7468 6973 2070  otice and this p
-00000320: 6572 6d69 7373 696f 6e20 6e6f 7469 6365  ermission notice
-00000330: 2073 6861 6c6c 2062 6520 696e 636c 7564   shall be includ
-00000340: 6564 2069 6e20 616c 6c0a 2020 2020 2020  ed in all.      
-00000350: 2020 636f 7069 6573 206f 7220 7375 6273    copies or subs
-00000360: 7461 6e74 6961 6c20 706f 7274 696f 6e73  tantial portions
-00000370: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
-00000380: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00000390: 2020 2054 4845 2053 4f46 5457 4152 4520     THE SOFTWARE 
-000003a0: 4953 2050 524f 5649 4445 4420 2241 5320  IS PROVIDED "AS 
-000003b0: 4953 222c 2057 4954 484f 5554 2057 4152  IS", WITHOUT WAR
-000003c0: 5241 4e54 5920 4f46 2041 4e59 204b 494e  RANTY OF ANY KIN
-000003d0: 442c 2045 5850 5245 5353 204f 520a 2020  D, EXPRESS OR.  
-000003e0: 2020 2020 2020 494d 504c 4945 442c 2049        IMPLIED, I
-000003f0: 4e43 4c55 4449 4e47 2042 5554 204e 4f54  NCLUDING BUT NOT
-00000400: 204c 494d 4954 4544 2054 4f20 5448 4520   LIMITED TO THE 
-00000410: 5741 5252 414e 5449 4553 204f 4620 4d45  WARRANTIES OF ME
-00000420: 5243 4841 4e54 4142 494c 4954 592c 0a20  RCHANTABILITY,. 
-00000430: 2020 2020 2020 2046 4954 4e45 5353 2046         FITNESS F
-00000440: 4f52 2041 2050 4152 5449 4355 4c41 5220  OR A PARTICULAR 
-00000450: 5055 5250 4f53 4520 414e 4420 4e4f 4e49  PURPOSE AND NONI
-00000460: 4e46 5249 4e47 454d 454e 542e 2049 4e20  NFRINGEMENT. IN 
-00000470: 4e4f 2045 5645 4e54 2053 4841 4c4c 2054  NO EVENT SHALL T
-00000480: 4845 0a20 2020 2020 2020 2041 5554 484f  HE.        AUTHO
-00000490: 5253 204f 5220 434f 5059 5249 4748 5420  RS OR COPYRIGHT 
-000004a0: 484f 4c44 4552 5320 4245 204c 4941 424c  HOLDERS BE LIABL
-000004b0: 4520 464f 5220 414e 5920 434c 4149 4d2c  E FOR ANY CLAIM,
-000004c0: 2044 414d 4147 4553 204f 5220 4f54 4845   DAMAGES OR OTHE
-000004d0: 520a 2020 2020 2020 2020 4c49 4142 494c  R.        LIABIL
-000004e0: 4954 592c 2057 4845 5448 4552 2049 4e20  ITY, WHETHER IN 
-000004f0: 414e 2041 4354 494f 4e20 4f46 2043 4f4e  AN ACTION OF CON
-00000500: 5452 4143 542c 2054 4f52 5420 4f52 204f  TRACT, TORT OR O
-00000510: 5448 4552 5749 5345 2c20 4152 4953 494e  THERWISE, ARISIN
-00000520: 4720 4652 4f4d 2c0a 2020 2020 2020 2020  G FROM,.        
-00000530: 4f55 5420 4f46 204f 5220 494e 2043 4f4e  OUT OF OR IN CON
-00000540: 4e45 4354 494f 4e20 5749 5448 2054 4845  NECTION WITH THE
-00000550: 2053 4f46 5457 4152 4520 4f52 2054 4845   SOFTWARE OR THE
-00000560: 2055 5345 204f 5220 4f54 4845 5220 4445   USE OR OTHER DE
-00000570: 414c 494e 4753 2049 4e20 5448 450a 2020  ALINGS IN THE.  
-00000580: 2020 2020 2020 534f 4654 5741 5245 2e0a        SOFTWARE..
-00000590: 2020 2020 2020 2020 0a50 726f 6a65 6374          .Project
-000005a0: 2d55 524c 3a20 4769 7448 7562 2c20 6874  -URL: GitHub, ht
-000005b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000005c0: 2f54 6f6d 6173 7a41 6e69 6f6c 6f77 736b  /TomaszAniolowsk
-000005d0: 692f 6d69 6d65 6f0a 4b65 7977 6f72 6473  i/mimeo.Keywords
-000005e0: 3a20 6d69 6d65 6f67 7261 7068 2c6d 696d  : mimeograph,mim
-000005f0: 656f 2c67 656e 6572 6174 652c 6765 6e65  eo,generate,gene
-00000600: 7261 746f 722c 6461 7461 2c78 6d6c 0a43  rator,data,xml.C
-00000610: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
-00000620: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000630: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-00000640: 650a 436c 6173 7369 6669 6572 3a20 4465  e.Classifier: De
-00000650: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000660: 203a 3a20 3420 2d20 4265 7461 0a43 6c61   :: 4 - Beta.Cla
-00000670: 7373 6966 6965 723a 2045 6e76 6972 6f6e  ssifier: Environ
-00000680: 6d65 6e74 203a 3a20 436f 6e73 6f6c 650a  ment :: Console.
-00000690: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
-000006a0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-000006b0: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
-000006c0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000006d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000006e0: 5079 7468 6f6e 0a43 6c61 7373 6966 6965  Python.Classifie
-000006f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000700: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000710: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
-00000720: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000730: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000740: 6e20 3a3a 2033 203a 3a20 4f6e 6c79 0a43  n :: 3 :: Only.C
-00000750: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000760: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000770: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000780: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000790: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000007a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000007b0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-000007c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000007d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000007e0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
-000007f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000800: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000810: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
-00000820: 6965 723a 2054 6f70 6963 203a 3a20 4461  ier: Topic :: Da
-00000830: 7461 6261 7365 0a43 6c61 7373 6966 6965  tabase.Classifie
-00000840: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
-00000850: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
-00000860: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-00000870: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
-00000880: 6576 656c 6f70 6d65 6e74 203a 3a20 5465  evelopment :: Te
-00000890: 7374 696e 670a 436c 6173 7369 6669 6572  sting.Classifier
-000008a0: 3a20 546f 7069 6320 3a3a 2055 7469 6c69  : Topic :: Utili
-000008b0: 7469 6573 0a52 6571 7569 7265 732d 5079  ties.Requires-Py
-000008c0: 7468 6f6e 3a20 3e3d 332e 380a 4465 7363  thon: >=3.8.Desc
-000008d0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-000008e0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-000008f0: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
-00000900: 7261 3a20 6465 760a 5072 6f76 6964 6573  ra: dev.Provides
-00000910: 2d45 7874 7261 3a20 7465 7374 0a4c 6963  -Extra: test.Lic
-00000920: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-00000930: 5345 0a0a 2320 4d69 6d65 6f20 284d 696d  SE..# Mimeo (Mim
-00000940: 656f 6772 6170 6829 0a0a 5b21 5b4c 6963  eograph)..[![Lic
-00000950: 656e 7365 5d28 6874 7470 733a 2f2f 696d  ense](https://im
-00000960: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00000970: 6875 622f 6c69 6365 6e73 652f 546f 6d61  hub/license/Toma
-00000980: 737a 416e 696f 6c6f 7773 6b69 2f6d 696d  szAniolowski/mim
-00000990: 656f 3f6c 6162 656c 3d4c 6963 656e 7365  eo?label=License
-000009a0: 2673 7479 6c65 3d70 6c61 7374 6963 295d  &style=plastic)]
-000009b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000009c0: 636f 6d2f 546f 6d61 737a 416e 696f 6c6f  com/TomaszAniolo
-000009d0: 7773 6b69 2f6d 696d 656f 2f62 6c6f 622f  wski/mimeo/blob/
-000009e0: 6465 7665 6c6f 702f 4c49 4345 4e53 4529  develop/LICENSE)
-000009f0: 0a5b 215b 5665 7273 696f 6e5d 2868 7474  .[![Version](htt
-00000a00: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000a10: 2e69 6f2f 7079 7069 2f76 2f6d 696d 656f  .io/pypi/v/mimeo
-00000a20: 6772 6170 683f 636f 6c6f 723d 626c 7565  graph?color=blue
-00000a30: 266c 6162 656c 3d50 7950 4926 7374 796c  &label=PyPI&styl
-00000a40: 653d 706c 6173 7469 6329 5d28 6874 7470  e=plastic)](http
-00000a50: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000a60: 6a65 6374 2f6d 696d 656f 6772 6170 682f  ject/mimeograph/
-00000a70: 290a 5b21 5b50 7974 686f 6e5d 2868 7474  ).[![Python](htt
-00000a80: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000a90: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-00000aa0: 6f6e 732f 6d69 6d65 6f67 7261 7068 3f6c  ons/mimeograph?l
-00000ab0: 6162 656c 3d50 7974 686f 6e26 7374 796c  abel=Python&styl
-00000ac0: 653d 706c 6173 7469 6329 5d28 6874 7470  e=plastic)](http
-00000ad0: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
-00000ae0: 7267 2f29 2020 0a5b 215b 4275 696c 645d  rg/)  .[![Build]
-00000af0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000b00: 656c 6473 2e69 6f2f 6769 7468 7562 2f61  elds.io/github/a
-00000b10: 6374 696f 6e73 2f77 6f72 6b66 6c6f 772f  ctions/workflow/
-00000b20: 7374 6174 7573 2f54 6f6d 6173 7a41 6e69  status/TomaszAni
-00000b30: 6f6c 6f77 736b 692f 6d69 6d65 6f2f 7465  olowski/mimeo/te
-00000b40: 7374 2e79 6d6c 3f63 6f6c 6f72 3d62 7269  st.yml?color=bri
-00000b50: 6768 7467 7265 656e 266c 6162 656c 3d54  ghtgreen&label=T
-00000b60: 6573 7425 3230 4d69 6d65 6f26 7374 796c  est%20Mimeo&styl
-00000b70: 653d 706c 6173 7469 6329 5d28 6874 7470  e=plastic)](http
-00000b80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00000b90: 6f6d 6173 7a41 6e69 6f6c 6f77 736b 692f  omaszAniolowski/
-00000ba0: 6d69 6d65 6f2f 6163 7469 6f6e 732f 776f  mimeo/actions/wo
-00000bb0: 726b 666c 6f77 732f 7465 7374 2e79 6d6c  rkflows/test.yml
-00000bc0: 3f71 7565 7279 3d62 7261 6e63 6825 3341  ?query=branch%3A
-00000bd0: 6d61 696e 290a 5b21 5b43 6f64 6520 436f  main).[![Code Co
-00000be0: 7665 7261 6765 5d28 6874 7470 733a 2f2f  verage](https://
-00000bf0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000c00: 6164 6765 2f43 6f64 6525 3230 436f 7665  adge/Code%20Cove
-00000c10: 7261 6765 2d31 3030 2532 352d 6272 6967  rage-100%25-brig
-00000c20: 6874 6772 6565 6e3f 7374 796c 653d 706c  htgreen?style=pl
-00000c30: 6173 7469 6329 5d28 6874 7470 733a 2f2f  astic)](https://
-00000c40: 6769 7468 7562 2e63 6f6d 2f54 6f6d 6173  github.com/Tomas
-00000c50: 7a41 6e69 6f6c 6f77 736b 692f 6d69 6d65  zAniolowski/mime
-00000c60: 6f2f 6163 7469 6f6e 732f 776f 726b 666c  o/actions/workfl
-00000c70: 6f77 732f 636f 7665 7261 6765 5f62 6164  ows/coverage_bad
-00000c80: 6765 2e79 6d6c 3f71 7565 7279 3d62 7261  ge.yml?query=bra
-00000c90: 6e63 6825 3341 6d61 696e 290a 0a5b 4d69  nch%3Amain)..[Mi
-00000ca0: 6d65 6f5d 2868 7474 7073 3a2f 2f67 6974  meo](https://git
-00000cb0: 6875 622e 636f 6d2f 546f 6d61 737a 416e  hub.com/TomaszAn
-00000cc0: 696f 6c6f 7773 6b69 2f6d 696d 656f 2920  iolowski/mimeo) 
-00000cd0: 6973 2061 2063 6f6d 6d61 6e64 206c 696e  is a command lin
-00000ce0: 6520 746f 6f6c 2061 6e64 2070 7974 686f  e tool and pytho
-00000cf0: 6e20 6c69 6272 6172 7920 6765 6e65 7261  n library genera
-00000d00: 7469 6e67 2063 7573 746f 6d20 6461 7461  ting custom data
-00000d10: 2062 6173 6564 206f 6e20 6120 7465 6d70   based on a temp
-00000d20: 6c61 7465 2e0a 4974 2063 616e 2062 6520  late..It can be 
-00000d30: 7573 6564 2062 7920 6465 7665 6c6f 7065  used by develope
-00000d40: 7273 2c20 7465 7374 6572 7320 6f72 2065  rs, testers or e
-00000d50: 7665 6e20 6275 7369 6e65 7373 2061 6e61  ven business ana
-00000d60: 6c79 7374 7320 696e 2074 6865 6972 2064  lysts in their d
-00000d70: 6169 6c79 2077 6f72 6b2e 0a0a 0a23 2320  aily work....## 
-00000d80: 496e 7374 616c 6c61 7469 6f6e 0a0a 496e  Installation..In
-00000d90: 7374 616c 6c20 4d69 6d65 6f20 7769 7468  stall Mimeo with
-00000da0: 2070 6970 0a0a 6060 6073 680a 7069 7020   pip..```sh.pip 
-00000db0: 696e 7374 616c 6c20 6d69 6d65 6f67 7261  install mimeogra
-00000dc0: 7068 0a60 6060 0a0a 0a23 2320 5573 6167  ph.```...## Usag
-00000dd0: 652f 4578 616d 706c 6573 0a0a 2323 2320  e/Examples..### 
-00000de0: 4d69 6d65 6f20 436f 6e66 6967 7572 6174  Mimeo Configurat
-00000df0: 696f 6e0a 0a50 7265 7061 7265 204d 696d  ion..Prepare Mim
-00000e00: 656f 2043 6f6e 6669 6775 7261 7469 6f6e  eo Configuration
-00000e10: 2066 6972 7374 0a2d 2066 6f72 2061 2063   first.- for a c
-00000e20: 6f6d 6d61 6e64 206c 696e 6520 746f 6f6c  ommand line tool
-00000e30: 3a20 696e 2061 204a 534f 4e20 6f72 2058  : in a JSON or X
-00000e40: 4d4c 2066 696c 650a 2d20 666f 7220 6120  ML file.- for a 
-00000e50: 604d 696d 656f 6772 6170 6860 2070 7974  `Mimeograph` pyt
-00000e60: 686f 6e20 636c 6173 733a 2069 6e20 6120  hon class: in a 
-00000e70: 6064 6963 7460 206f 7220 7374 7269 6e67  `dict` or string
-00000e80: 6966 6965 6420 584d 4c0a 0a60 6060 6a73  ified XML..```js
-00000e90: 6f6e 0a7b 0a20 2022 5f74 656d 706c 6174  on.{.  "_templat
-00000ea0: 6573 5f22 3a20 5b0a 2020 2020 7b0a 2020  es_": [.    {.  
-00000eb0: 2020 2020 2263 6f75 6e74 223a 2033 302c      "count": 30,
-00000ec0: 0a20 2020 2020 2022 6d6f 6465 6c22 3a20  .      "model": 
-00000ed0: 7b0a 2020 2020 2020 2020 2253 6f6d 6545  {.        "SomeE
-00000ee0: 6e74 6974 7922 3a20 7b0a 2020 2020 2020  ntity": {.      
-00000ef0: 2020 2020 2240 786d 6c6e 7322 3a20 2268      "@xmlns": "h
-00000f00: 7474 703a 2f2f 6d69 6d65 6f2e 6172 6368  ttp://mimeo.arch
-00000f10: 2e63 6f6d 2f64 6566 6175 6c74 2d6e 616d  .com/default-nam
-00000f20: 6573 7061 6365 222c 0a20 2020 2020 2020  espace",.       
-00000f30: 2020 2022 4078 6d6c 6e73 3a70 6e22 3a20     "@xmlns:pn": 
-00000f40: 2268 7474 703a 2f2f 6d69 6d65 6f2e 6172  "http://mimeo.ar
-00000f50: 6368 2e63 6f6d 2f70 7265 6669 7865 642d  ch.com/prefixed-
-00000f60: 6e61 6d65 7370 6163 6522 2c0a 2020 2020  namespace",.    
-00000f70: 2020 2020 2020 2243 6869 6c64 4e6f 6465        "ChildNode
-00000f80: 3122 3a20 312c 0a20 2020 2020 2020 2020  1": 1,.         
-00000f90: 2022 4368 696c 644e 6f64 6532 223a 2022   "ChildNode2": "
-00000fa0: 7661 6c75 652d 3222 2c0a 2020 2020 2020  value-2",.      
-00000fb0: 2020 2020 2243 6869 6c64 4e6f 6465 3322      "ChildNode3"
-00000fc0: 3a20 7472 7565 0a20 2020 2020 2020 207d  : true.        }
-00000fd0: 0a20 2020 2020 207d 0a20 2020 207d 0a20  .      }.    }. 
-00000fe0: 205d 0a7d 0a60 6060 0a60 6060 786d 6c0a   ].}.```.```xml.
-00000ff0: 3c6d 696d 656f 5f63 6f6e 6669 6775 7261  <mimeo_configura
-00001000: 7469 6f6e 3e0a 2020 2020 3c5f 7465 6d70  tion>.    <_temp
-00001010: 6c61 7465 735f 3e0a 2020 2020 2020 2020  lates_>.        
-00001020: 3c5f 7465 6d70 6c61 7465 5f3e 0a20 2020  <_template_>.   
-00001030: 2020 2020 2020 2020 203c 636f 756e 743e           <count>
-00001040: 3330 3c2f 636f 756e 743e 0a20 2020 2020  30</count>.     
-00001050: 2020 2020 2020 203c 6d6f 6465 6c3e 0a0a         <model>..
-00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 3c53 6f6d 6545 6e74 6974 790a 2020 2020  <SomeEntity.    
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 786d 6c6e 733d 2268 7474 703a 2f2f 6d69  xmlns="http://mi
-000010a0: 6d65 6f2e 6172 6368 2e63 6f6d 2f64 6566  meo.arch.com/def
-000010b0: 6175 6c74 2d6e 616d 6573 7061 6365 220a  ault-namespace".
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 2020 2020 786d 6c6e 733a 706e 3d22 6874      xmlns:pn="ht
-000010e0: 7470 3a2f 2f6d 696d 656f 2e61 7263 682e  tp://mimeo.arch.
-000010f0: 636f 6d2f 7072 6566 6978 6564 2d6e 616d  com/prefixed-nam
-00001100: 6573 7061 6365 223e 0a20 2020 2020 2020  espace">.       
-00001110: 2020 2020 2020 2020 2020 2020 203c 4368               <Ch
-00001120: 696c 644e 6f64 6531 3e31 3c2f 4368 696c  ildNode1>1</Chil
-00001130: 644e 6f64 6531 3e0a 2020 2020 2020 2020  dNode1>.        
-00001140: 2020 2020 2020 2020 2020 2020 3c70 6e3a              <pn:
-00001150: 4368 696c 644e 6f64 6532 3e76 616c 7565  ChildNode2>value
-00001160: 2d32 3c2f 706e 3a43 6869 6c64 4e6f 6465  -2</pn:ChildNode
-00001170: 323e 0a20 2020 2020 2020 2020 2020 2020  2>.             
-00001180: 2020 2020 2020 203c 4368 696c 644e 6f64         <ChildNod
-00001190: 6533 3e74 7275 653c 2f43 6869 6c64 4e6f  e3>true</ChildNo
-000011a0: 6465 333e 0a20 2020 2020 2020 2020 2020  de3>.           
-000011b0: 2020 2020 203c 2f53 6f6d 6545 6e74 6974       </SomeEntit
-000011c0: 793e 0a0a 2020 2020 2020 2020 2020 2020  y>..            
-000011d0: 3c2f 6d6f 6465 6c3e 0a20 2020 2020 2020  </model>.       
-000011e0: 203c 2f5f 7465 6d70 6c61 7465 5f3e 0a20   </_template_>. 
-000011f0: 2020 203c 2f5f 7465 6d70 6c61 7465 735f     </_templates_
-00001200: 3e0a 3c2f 6d69 6d65 6f5f 636f 6e66 6967  >.</mimeo_config
-00001210: 7572 6174 696f 6e3e 0a60 6060 0a5f 596f  uration>.```._Yo
-00001220: 7520 6361 6e20 6669 6e64 206d 6f72 6520  u can find more 
-00001230: 636f 6e66 6967 7572 6174 696f 6e20 6578  configuration ex
-00001240: 616d 706c 6573 2069 6e20 7468 6520 6065  amples in the `e
-00001250: 7861 6d70 6c65 7360 2066 6f6c 6465 722e  xamples` folder.
-00001260: 5f0a 0a23 2323 204d 696d 656f 6772 6170  _..### Mimeograp
-00001270: 680a 0a23 2323 2320 436f 6d6d 616e 6420  h..#### Command 
-00001280: 6c69 6e65 2074 6f6f 6c0a 0a60 6060 7368  line tool..```sh
-00001290: 0a6d 696d 656f 2053 6f6d 6545 6e74 6974  .mimeo SomeEntit
-000012a0: 792d 636f 6e66 6967 2e6a 736f 6e0a 6d69  y-config.json.mi
-000012b0: 6d65 6f20 536f 6d65 456e 7469 7479 2d63  meo SomeEntity-c
-000012c0: 6f6e 6669 672e 786d 6c0a 6060 600a 0a23  onfig.xml.```..#
-000012d0: 2323 2320 5079 7468 6f6e 206c 6962 7261  ### Python libra
-000012e0: 7279 0a0a 6060 6070 7974 686f 6e0a 6672  ry..```python.fr
-000012f0: 6f6d 206d 696d 656f 2069 6d70 6f72 7420  om mimeo import 
-00001300: 4d69 6d65 6f43 6f6e 6669 6746 6163 746f  MimeoConfigFacto
-00001310: 7279 2c20 4d69 6d65 6f67 7261 7068 0a0a  ry, Mimeograph..
-00001320: 636f 6e66 6967 203d 207b 0a20 2020 2023  config = {.    #
-00001330: 2059 6f75 7220 636f 6e66 6967 7572 6174   Your configurat
-00001340: 696f 6e20 696e 2061 2064 6963 740a 7d0a  ion in a dict.}.
-00001350: 636f 6e66 6967 203d 2022 2222 0a20 2020  config = """.   
-00001360: 2059 6f75 7220 636f 6e66 6967 7572 6174   Your configurat
-00001370: 696f 6e20 696e 2061 2073 7472 696e 6769  ion in a stringi
-00001380: 6669 6564 2058 4d4c 206e 6f64 650a 2222  fied XML node.""
-00001390: 220a 636f 6e66 6967 203d 2022 2220 2023  ".config = ""  #
-000013a0: 2041 2066 696c 6520 7061 7468 2074 6f20   A file path to 
-000013b0: 796f 7572 2063 6f6e 6669 6775 7261 7469  your configurati
-000013c0: 6f6e 2028 4a53 4f4e 202f 2058 4d4c 290a  on (JSON / XML).
-000013d0: 6d69 6d65 6f5f 636f 6e66 6967 203d 204d  mimeo_config = M
-000013e0: 696d 656f 436f 6e66 6967 4661 6374 6f72  imeoConfigFactor
-000013f0: 792e 7061 7273 6528 636f 6e66 6967 290a  y.parse(config).
-00001400: 4d69 6d65 6f67 7261 7068 286d 696d 656f  Mimeograph(mimeo
-00001410: 5f63 6f6e 6669 6729 2e70 726f 6365 7373  _config).process
-00001420: 2829 0a60 6060 0a2a 2a2a 0a54 6865 204d  ().```.***.The M
-00001430: 696d 656f 2043 6f6e 6669 6775 7261 7469  imeo Configurati
-00001440: 6f6e 2061 626f 7665 2077 696c 6c20 7072  on above will pr
-00001450: 6f64 7563 6520 3220 6669 6c65 733a 0a0a  oduce 2 files:..
-00001460: 6060 6078 6d6c 0a3c 212d 2d20 6d69 6d65  ```xml.<!-- mime
-00001470: 6f2d 6f75 7470 7574 2f6d 696d 656f 2d6f  o-output/mimeo-o
-00001480: 7574 7075 742d 312e 786d 6c2d 2d3e 0a3c  utput-1.xml-->.<
-00001490: 536f 6d65 456e 7469 7479 2078 6d6c 6e73  SomeEntity xmlns
-000014a0: 3d22 6874 7470 3a2f 2f6d 696d 656f 2e61  ="http://mimeo.a
-000014b0: 7263 682e 636f 6d2f 6465 6661 756c 742d  rch.com/default-
-000014c0: 6e61 6d65 7370 6163 6522 2078 6d6c 6e73  namespace" xmlns
-000014d0: 3a70 6e3d 2268 7474 703a 2f2f 6d69 6d65  :pn="http://mime
-000014e0: 6f2e 6172 6368 2e63 6f6d 2f70 7265 6669  o.arch.com/prefi
-000014f0: 7865 642d 6e61 6d65 7370 6163 6522 3e0a  xed-namespace">.
-00001500: 2020 2020 3c43 6869 6c64 4e6f 6465 313e      <ChildNode1>
-00001510: 313c 2f43 6869 6c64 4e6f 6465 313e 0a20  1</ChildNode1>. 
-00001520: 2020 203c 706e 3a43 6869 6c64 4e6f 6465     <pn:ChildNode
-00001530: 323e 7661 6c75 652d 323c 2f70 6e3a 4368  2>value-2</pn:Ch
-00001540: 696c 644e 6f64 6532 3e0a 2020 2020 3c43  ildNode2>.    <C
-00001550: 6869 6c64 4e6f 6465 333e 7472 7565 3c2f  hildNode3>true</
-00001560: 4368 696c 644e 6f64 6533 3e0a 3c2f 536f  ChildNode3>.</So
-00001570: 6d65 456e 7469 7479 3e0a 6060 600a 6060  meEntity>.```.``
-00001580: 6078 6d6c 0a3c 212d 2d20 6d69 6d65 6f2d  `xml.<!-- mimeo-
-00001590: 6f75 7470 7574 2f6d 696d 656f 2d6f 7574  output/mimeo-out
-000015a0: 7075 742d 322e 786d 6c2d 2d3e 0a3c 536f  put-2.xml-->.<So
-000015b0: 6d65 456e 7469 7479 2078 6d6c 6e73 3d22  meEntity xmlns="
-000015c0: 6874 7470 3a2f 2f6d 696d 656f 2e61 7263  http://mimeo.arc
-000015d0: 682e 636f 6d2f 6465 6661 756c 742d 6e61  h.com/default-na
-000015e0: 6d65 7370 6163 6522 2078 6d6c 6e73 3a70  mespace" xmlns:p
-000015f0: 6e3d 2268 7474 703a 2f2f 6d69 6d65 6f2e  n="http://mimeo.
-00001600: 6172 6368 2e63 6f6d 2f70 7265 6669 7865  arch.com/prefixe
-00001610: 642d 6e61 6d65 7370 6163 6522 3e0a 2020  d-namespace">.  
-00001620: 2020 3c43 6869 6c64 4e6f 6465 313e 313c    <ChildNode1>1<
-00001630: 2f43 6869 6c64 4e6f 6465 313e 0a20 2020  /ChildNode1>.   
-00001640: 203c 706e 3a43 6869 6c64 4e6f 6465 323e   <pn:ChildNode2>
-00001650: 7661 6c75 652d 323c 2f70 6e3a 4368 696c  value-2</pn:Chil
-00001660: 644e 6f64 6532 3e0a 2020 2020 3c43 6869  dNode2>.    <Chi
-00001670: 6c64 4e6f 6465 333e 7472 7565 3c2f 4368  ldNode3>true</Ch
-00001680: 696c 644e 6f64 6533 3e0a 3c2f 536f 6d65  ildNode3>.</Some
-00001690: 456e 7469 7479 3e0a 6060 600a 2a2a 2a0a  Entity>.```.***.
-000016a0: 0a23 2323 204d 696d 656f 2055 7469 6c73  .### Mimeo Utils
-000016b0: 0a0a 4d69 6d65 6f20 6578 706f 7365 7320  ..Mimeo exposes 
-000016c0: 7365 7665 7261 6c20 6675 6e63 7469 6f6e  several function
-000016d0: 7320 666f 7220 6461 7461 2067 656e 6572  s for data gener
-000016e0: 6174 696f 6e20 7468 6174 2077 696c 6c20  ation that will 
-000016f0: 6d61 6b65 2069 7420 6d6f 7265 2075 7365  make it more use
-00001700: 6675 6c20 666f 7220 7465 7374 696e 6720  ful for testing 
-00001710: 7075 7270 6f73 6573 2e0a 0a2a 2a54 656d  purposes...**Tem
-00001720: 706c 6174 652a 2a0a 6060 606a 736f 6e0a  plate**.```json.
-00001730: 7b0a 2020 2263 6f75 6e74 223a 2032 2c0a  {.  "count": 2,.
-00001740: 2020 226d 6f64 656c 223a 207b 0a20 2020    "model": {.   
-00001750: 2022 536f 6d65 456e 7469 7479 223a 207b   "SomeEntity": {
-00001760: 0a20 2020 2020 2022 6964 223a 2022 7b61  .      "id": "{a
-00001770: 7574 6f5f 696e 6372 656d 656e 747d 222c  uto_increment}",
-00001780: 0a20 2020 2020 2022 7261 6e64 6f6d 7374  .      "randomst
-00001790: 7269 6e67 223a 2022 7b72 616e 646f 6d5f  ring": "{random_
-000017a0: 7374 727d 222c 0a20 2020 2020 2022 7261  str}",.      "ra
-000017b0: 6e64 6f6d 696e 7422 3a20 227b 7261 6e64  ndomint": "{rand
-000017c0: 6f6d 5f69 6e74 7d22 0a20 2020 207d 0a20  om_int}".    }. 
-000017d0: 207d 0a7d 0a60 6060 0a60 6060 786d 6c0a   }.}.```.```xml.
-000017e0: 3c5f 7465 6d70 6c61 7465 5f3e 0a20 2020  <_template_>.   
-000017f0: 203c 636f 756e 743e 323c 2f63 6f75 6e74   <count>2</count
-00001800: 3e0a 2020 2020 3c6d 6f64 656c 3e0a 2020  >.    <model>.  
-00001810: 2020 2020 2020 0a20 2020 2020 2020 203c        .        <
-00001820: 536f 6d65 456e 7469 7479 3e0a 2020 2020  SomeEntity>.    
-00001830: 2020 2020 2020 2020 3c69 643e 7b61 7574          <id>{aut
-00001840: 6f5f 696e 6372 656d 656e 747d 3c2f 6964  o_increment}</id
-00001850: 3e0a 2020 2020 2020 2020 2020 2020 3c72  >.            <r
-00001860: 616e 646f 6d73 7472 696e 673e 7b72 616e  andomstring>{ran
-00001870: 646f 6d5f 7374 727d 3c2f 7261 6e64 6f6d  dom_str}</random
-00001880: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
-00001890: 2020 2020 3c72 616e 646f 6d69 6e74 3e7b      <randomint>{
-000018a0: 7261 6e64 6f6d 5f69 6e74 7d3c 2f72 616e  random_int}</ran
-000018b0: 646f 6d69 6e74 3e0a 2020 2020 2020 2020  domint>.        
-000018c0: 3c2f 536f 6d65 456e 7469 7479 3e0a 2020  </SomeEntity>.  
-000018d0: 2020 2020 2020 0a20 2020 203c 2f6d 6f64        .    </mod
-000018e0: 656c 3e0a 3c2f 5f74 656d 706c 6174 655f  el>.</_template_
-000018f0: 3e0a 6060 600a 0a2a 2a58 4d4c 2044 6174  >.```..**XML Dat
-00001900: 612a 2a0a 6060 6078 6d6c 0a3c 536f 6d65  a**.```xml.<Some
-00001910: 456e 7469 7479 3e0a 2020 2020 3c69 643e  Entity>.    <id>
-00001920: 3030 3030 313c 2f69 643e 0a20 2020 203c  00001</id>.    <
-00001930: 7261 6e64 6f6d 7374 7269 6e67 3e6d 4341  randomstring>mCA
-00001940: 7073 595a 7072 6179 596b 6d4b 6e59 5778  psYZprayYkmKnYWx
-00001950: 653c 2f72 616e 646f 6d73 7472 696e 673e  e</randomstring>
-00001960: 0a20 2020 203c 7261 6e64 6f6d 696e 743e  .    <randomint>
-00001970: 383c 2f72 616e 646f 6d69 6e74 3e0a 3c2f  8</randomint>.</
-00001980: 536f 6d65 456e 7469 7479 3e0a 6060 600a  SomeEntity>.```.
-00001990: 6060 6078 6d6c 0a3c 536f 6d65 456e 7469  ```xml.<SomeEnti
-000019a0: 7479 3e0a 2020 2020 3c69 643e 3030 3030  ty>.    <id>0000
-000019b0: 323c 2f69 643e 0a20 2020 203c 7261 6e64  2</id>.    <rand
-000019c0: 6f6d 7374 7269 6e67 3e63 6561 5055 7141  omstring>ceaPUqA
-000019d0: 5255 6b46 756b 5a49 5065 7571 4f3c 2f72  RUkFukZIPeuqO</r
-000019e0: 616e 646f 6d73 7472 696e 673e 0a20 2020  andomstring>.   
-000019f0: 203c 7261 6e64 6f6d 696e 743e 3939 3c2f   <randomint>99</
-00001a00: 7261 6e64 6f6d 696e 743e 0a3c 2f53 6f6d  randomint>.</Som
-00001a10: 6545 6e74 6974 793e 0a60 6060 0a0a 0a23  eEntity>.```...#
-00001a20: 2320 446f 6375 6d65 6e74 6174 696f 6e0a  # Documentation.
-00001a30: 0a23 2323 204d 696d 656f 2043 4c49 0a0a  .### Mimeo CLI..
-00001a40: 2323 2323 204d 696d 656f 2043 6f6e 6669  #### Mimeo Confi
-00001a50: 6775 7261 7469 6f6e 2061 7267 756d 656e  guration argumen
-00001a60: 7473 0a0a 5768 656e 2075 7369 6e67 204d  ts..When using M
-00001a70: 696d 656f 2063 6f6d 6d61 6e64 206c 696e  imeo command lin
-00001a80: 6520 746f 6f6c 2079 6f75 2063 616e 206f  e tool you can o
-00001a90: 7665 7277 7269 7465 204d 696d 656f 2043  verwrite Mimeo C
-00001aa0: 6f6e 6669 6775 7261 7469 6f6e 2070 726f  onfiguration pro
-00001ab0: 7065 7274 6965 733a 0a0a 7c20 5368 6f72  perties:..| Shor
-00001ac0: 7420 6f70 7469 6f6e 207c 204c 6f6e 6720  t option | Long 
-00001ad0: 6f70 7469 6f6e 2020 2020 2020 2020 207c  option         |
-00001ae0: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
-00001af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2020 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d        |.|:------
-00001b30: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
-00001b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d  -------------|:-
-00001b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b90: 2d2d 2d2d 7c0a 7c20 2020 2020 602d 6f60  ----|.|     `-o`
-00001ba0: 2020 2020 207c 2060 2d2d 6f75 7470 7574       | `--output
-00001bb0: 6020 2020 2020 2020 2020 207c 206f 7665  `          | ove
-00001bc0: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
-00001bd0: 7574 2f64 6972 6563 7469 6f6e 6020 7072  ut/direction` pr
-00001be0: 6f70 6572 7479 2020 2020 2020 2020 2020  operty          
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2020 7c0a 7c20 2020 2020 602d 7860 2020    |.|     `-x`  
-00001c10: 2020 207c 2060 2d2d 786d 6c2d 6465 636c     | `--xml-decl
-00001c20: 6172 6174 696f 6e60 207c 206f 7665 7277  aration` | overw
-00001c30: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
-00001c40: 2f78 6d6c 5f64 6563 6c61 7261 7469 6f6e  /xml_declaration
-00001c50: 6020 7072 6f70 6572 7479 2020 2020 2020  ` property      
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 7c0a 7c20 2020 2020 602d 6960 2020 2020  |.|     `-i`    
-00001c80: 207c 2060 2d2d 696e 6465 6e74 6020 2020   | `--indent`   
-00001c90: 2020 2020 2020 207c 206f 7665 7277 7269         | overwri
-00001ca0: 7465 2074 6865 2060 6f75 7470 7574 2f69  te the `output/i
-00001cb0: 6e64 656e 7460 2070 726f 7065 7274 7920  ndent` property 
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00001ce0: 7c20 2020 2020 602d 6460 2020 2020 207c  |     `-d`     |
-00001cf0: 2060 2d2d 6469 7265 6374 6f72 7960 2020   `--directory`  
-00001d00: 2020 2020 207c 206f 7665 7277 7269 7465       | overwrite
-00001d10: 2074 6865 2060 6f75 7470 7574 2f64 6972   the `output/dir
-00001d20: 6563 746f 7279 5f70 6174 6860 2070 726f  ectory_path` pro
-00001d30: 7065 7274 7920 2020 2020 2020 2020 2020  perty           
-00001d40: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00001d50: 2020 2020 602d 6660 2020 2020 207c 2060      `-f`     | `
-00001d60: 2d2d 6669 6c65 6020 2020 2020 2020 2020  --file`         
-00001d70: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
-00001d80: 6865 2060 6f75 7470 7574 2f66 696c 655f  he `output/file_
-00001d90: 6e61 6d65 6020 7072 6f70 6572 7479 2020  name` property  
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001db0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00001dc0: 2020 602d 4860 2020 2020 207c 2060 2d2d    `-H`     | `--
-00001dd0: 6874 7470 2d68 6f73 7460 2020 2020 2020  http-host`      
-00001de0: 207c 206f 7665 7277 7269 7465 2074 6865   | overwrite the
-00001df0: 2060 6f75 7470 7574 2f68 6f73 7460 2070   `output/host` p
-00001e00: 726f 7065 7274 7920 2020 2020 2020 2020  roperty         
-00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e20: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00001e30: 602d 7060 2020 2020 207c 2060 2d2d 6874  `-p`     | `--ht
-00001e40: 7470 2d70 6f72 7460 2020 2020 2020 207c  tp-port`       |
-00001e50: 206f 7665 7277 7269 7465 2074 6865 2060   overwrite the `
-00001e60: 6f75 7470 7574 2f70 6f72 7460 2070 726f  output/port` pro
-00001e70: 7065 7274 7920 2020 2020 2020 2020 2020  perty           
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 2020 2020 2020 7c0a 7c20 2020 2020 602d        |.|     `-
-00001ea0: 4560 2020 2020 207c 2060 2d2d 6874 7470  E`     | `--http
-00001eb0: 2d65 6e64 706f 696e 7460 2020 207c 206f  -endpoint`   | o
-00001ec0: 7665 7277 7269 7465 2074 6865 2060 6f75  verwrite the `ou
-00001ed0: 7470 7574 2f65 6e64 706f 696e 7460 2070  tput/endpoint` p
-00001ee0: 726f 7065 7274 7920 2020 2020 2020 2020  roperty         
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f00: 2020 2020 7c0a 7c20 2020 2020 602d 5560      |.|     `-U`
-00001f10: 2020 2020 207c 2060 2d2d 6874 7470 2d75       | `--http-u
-00001f20: 7365 7260 2020 2020 2020 207c 206f 7665  ser`       | ove
-00001f30: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
-00001f40: 7574 2f75 7365 726e 616d 6560 2070 726f  ut/username` pro
-00001f50: 7065 7274 7920 2020 2020 2020 2020 2020  perty           
-00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f70: 2020 7c0a 7c20 2020 2020 602d 5060 2020    |.|     `-P`  
-00001f80: 2020 207c 2060 2d2d 6874 7470 2d70 6173     | `--http-pas
-00001f90: 7377 6f72 6460 2020 207c 206f 7665 7277  sword`   | overw
-00001fa0: 7269 7465 2074 6865 2060 6f75 7470 7574  rite the `output
-00001fb0: 2f70 6173 7377 6f72 6460 2070 726f 7065  /password` prope
-00001fc0: 7274 7920 2020 2020 2020 2020 2020 2020  rty             
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00001ff0: 207c 2060 2d2d 6874 7470 2d6d 6574 686f   | `--http-metho
-00002000: 6460 2020 2020 207c 206f 7665 7277 7269  d`     | overwri
-00002010: 7465 2074 6865 2060 6f75 7470 7574 2f6d  te the `output/m
-00002020: 6574 686f 6460 2070 726f 7065 7274 7920  ethod` property 
-00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002040: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00002050: 7c20 2020 2020 2020 2020 2020 2020 207c  |              |
-00002060: 2060 2d2d 6874 7470 2d70 726f 746f 636f   `--http-protoco
-00002070: 6c60 2020 207c 206f 7665 7277 7269 7465  l`   | overwrite
-00002080: 2074 6865 2060 6f75 7470 7574 2f70 726f   the `output/pro
-00002090: 746f 636f 6c60 2070 726f 7065 7274 7920  tocol` property 
-000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020b0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-000020c0: 2020 2020 602d 6560 2020 2020 207c 2060      `-e`     | `
-000020d0: 2d2d 6874 7470 2d65 6e76 6020 2020 2020  --http-env`     
-000020e0: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
-000020f0: 6865 206f 7574 7075 7420 6874 7470 2070  he output http p
-00002100: 726f 7065 7274 6965 7320 7573 696e 6720  roperties using 
-00002110: 6120 6d69 6d65 6f20 656e 7620 636f 6e66  a mimeo env conf
-00002120: 6967 7572 6174 696f 6e20 7c0a 7c20 2020  iguration |.|   
-00002130: 2020 2020 2020 2020 2020 207c 2060 2d2d             | `--
-00002140: 6874 7470 2d65 6e76 732d 6669 6c65 6020  http-envs-file` 
-00002150: 207c 2075 7365 2061 2063 7573 746f 6d20   | use a custom 
-00002160: 656e 7669 726f 6e6d 656e 7473 2066 696c  environments fil
-00002170: 6520 2862 7920 6465 6661 756c 743a 206d  e (by default: m
-00002180: 696d 656f 2e65 6e76 732e 6a73 6f6e 2920  imeo.envs.json) 
-00002190: 2020 2020 2020 2020 7c0a 0a23 2323 2320          |..#### 
-000021a0: 4c6f 6767 696e 6720 6172 6775 6d65 6e74  Logging argument
-000021b0: 730a 0a7c 2053 686f 7274 206f 7074 696f  s..| Short optio
-000021c0: 6e20 7c20 4c6f 6e67 206f 7074 696f 6e20  n | Long option 
-000021d0: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
-000021e0: 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d      |.|:--------
-000021f0: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00002200: 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|:-----------
-00002210: 2d2d 2d2d 2d2d 2d7c 0a7c 2020 2020 2020  -------|.|      
-00002220: 2020 2020 2020 2020 7c20 602d 2d73 696c          | `--sil
-00002230: 656e 7460 2020 7c20 6469 7361 626c 6520  ent`  | disable 
-00002240: 494e 464f 206c 6f67 7320 7c0a 7c20 2020  INFO logs |.|   
-00002250: 2020 2020 2020 2020 2020 207c 2060 2d2d             | `--
-00002260: 6465 6275 6760 2020 207c 2065 6e61 626c  debug`   | enabl
-00002270: 6520 4445 4255 4720 6d6f 6465 207c 0a7c  e DEBUG mode |.|
-00002280: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00002290: 602d 2d66 696e 6560 2020 2020 7c20 656e  `--fine`    | en
-000022a0: 6162 6c65 2046 494e 4520 6d6f 6465 2020  able FINE mode  
-000022b0: 7c0a 0a23 2323 204d 696d 656f 2043 6f6e  |..### Mimeo Con
-000022c0: 6669 6775 7261 7469 6f6e 0a0a 4d69 6d65  figuration..Mime
-000022d0: 6f20 636f 6e66 6967 7572 6174 696f 6e20  o configuration 
-000022e0: 6973 2064 6566 696e 6564 2069 6e20 6120  is defined in a 
-000022f0: 4a53 4f4e 2066 696c 6520 7573 696e 6720  JSON file using 
-00002300: 696e 7465 726e 616c 2073 6574 7469 6e67  internal setting
-00002310: 7320 616e 6420 6461 7461 2074 656d 706c  s and data templ
-00002320: 6174 6573 2e0a 0a7c 204b 6579 2020 2020  ates...| Key    
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2020 2020 2020 2020 2020 7c20 204c 6576            |  Lev
-00002350: 656c 2020 207c 2020 2020 2020 5265 7175  el   |      Requ
-00002360: 6972 6564 2020 2020 2020 7c20 2020 2020  ired      |     
-00002370: 5375 7070 6f72 7465 6420 7661 6c75 6573  Supported values
-00002380: 2020 2020 207c 2020 2020 4465 6661 756c       |    Defaul
-00002390: 7420 2020 2020 7c20 4465 7363 7269 7074  t     | Descript
-000023a0: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000030: 312e 302e 330a 5375 6d6d 6172 793a 2047  1.0.3.Summary: G
+00000040: 656e 6572 6174 6520 4e6f 5351 4c20 6461  enerate NoSQL da
+00000050: 7461 2062 6173 6564 206f 6e20 6120 7369  ta based on a si
+00000060: 6d70 6c65 2074 656d 706c 6174 650a 4175  mple template.Au
+00000070: 7468 6f72 2d65 6d61 696c 3a20 2254 2e41  thor-email: "T.A
+00000080: 2e20 5072 6f67 7261 6d6d 696e 6720 5376  . Programming Sv
+00000090: 6373 2e22 203c 746f 6d61 737a 2e6d 6163  cs." <tomasz.mac
+000000a0: 6965 6a2e 616e 696f 6c6f 7773 6b69 4067  iej.aniolowski@g
+000000b0: 6d61 696c 2e63 6f6d 3e0a 4c69 6365 6e73  mail.com>.Licens
+000000c0: 653a 204d 4954 204c 6963 656e 7365 0a20  e: MIT License. 
+000000d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000000e0: 436f 7079 7269 6768 7420 2863 2920 3230  Copyright (c) 20
+000000f0: 3233 2054 6f6d 6173 7a20 416e 696f c582  23 Tomasz Anio..
+00000100: 6f77 736b 690a 2020 2020 2020 2020 0a20  owski.        . 
+00000110: 2020 2020 2020 2050 6572 6d69 7373 696f         Permissio
+00000120: 6e20 6973 2068 6572 6562 7920 6772 616e  n is hereby gran
+00000130: 7465 642c 2066 7265 6520 6f66 2063 6861  ted, free of cha
+00000140: 7267 652c 2074 6f20 616e 7920 7065 7273  rge, to any pers
+00000150: 6f6e 206f 6274 6169 6e69 6e67 2061 2063  on obtaining a c
+00000160: 6f70 790a 2020 2020 2020 2020 6f66 2074  opy.        of t
+00000170: 6869 7320 736f 6674 7761 7265 2061 6e64  his software and
+00000180: 2061 7373 6f63 6961 7465 6420 646f 6375   associated docu
+00000190: 6d65 6e74 6174 696f 6e20 6669 6c65 7320  mentation files 
+000001a0: 2874 6865 2022 536f 6674 7761 7265 2229  (the "Software")
+000001b0: 2c20 746f 2064 6561 6c0a 2020 2020 2020  , to deal.      
+000001c0: 2020 696e 2074 6865 2053 6f66 7477 6172    in the Softwar
+000001d0: 6520 7769 7468 6f75 7420 7265 7374 7269  e without restri
+000001e0: 6374 696f 6e2c 2069 6e63 6c75 6469 6e67  ction, including
+000001f0: 2077 6974 686f 7574 206c 696d 6974 6174   without limitat
+00000200: 696f 6e20 7468 6520 7269 6768 7473 0a20  ion the rights. 
+00000210: 2020 2020 2020 2074 6f20 7573 652c 2063         to use, c
+00000220: 6f70 792c 206d 6f64 6966 792c 206d 6572  opy, modify, mer
+00000230: 6765 2c20 7075 626c 6973 682c 2064 6973  ge, publish, dis
+00000240: 7472 6962 7574 652c 2073 7562 6c69 6365  tribute, sublice
+00000250: 6e73 652c 2061 6e64 2f6f 7220 7365 6c6c  nse, and/or sell
+00000260: 0a20 2020 2020 2020 2063 6f70 6965 7320  .        copies 
+00000270: 6f66 2074 6865 2053 6f66 7477 6172 652c  of the Software,
+00000280: 2061 6e64 2074 6f20 7065 726d 6974 2070   and to permit p
+00000290: 6572 736f 6e73 2074 6f20 7768 6f6d 2074  ersons to whom t
+000002a0: 6865 2053 6f66 7477 6172 6520 6973 0a20  he Software is. 
+000002b0: 2020 2020 2020 2066 7572 6e69 7368 6564         furnished
+000002c0: 2074 6f20 646f 2073 6f2c 2073 7562 6a65   to do so, subje
+000002d0: 6374 2074 6f20 7468 6520 666f 6c6c 6f77  ct to the follow
+000002e0: 696e 6720 636f 6e64 6974 696f 6e73 3a0a  ing conditions:.
+000002f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000300: 2054 6865 2061 626f 7665 2063 6f70 7972   The above copyr
+00000310: 6967 6874 206e 6f74 6963 6520 616e 6420  ight notice and 
+00000320: 7468 6973 2070 6572 6d69 7373 696f 6e20  this permission 
+00000330: 6e6f 7469 6365 2073 6861 6c6c 2062 6520  notice shall be 
+00000340: 696e 636c 7564 6564 2069 6e20 616c 6c0a  included in all.
+00000350: 2020 2020 2020 2020 636f 7069 6573 206f          copies o
+00000360: 7220 7375 6273 7461 6e74 6961 6c20 706f  r substantial po
+00000370: 7274 696f 6e73 206f 6620 7468 6520 536f  rtions of the So
+00000380: 6674 7761 7265 2e0a 2020 2020 2020 2020  ftware..        
+00000390: 0a20 2020 2020 2020 2054 4845 2053 4f46  .        THE SOF
+000003a0: 5457 4152 4520 4953 2050 524f 5649 4445  TWARE IS PROVIDE
+000003b0: 4420 2241 5320 4953 222c 2057 4954 484f  D "AS IS", WITHO
+000003c0: 5554 2057 4152 5241 4e54 5920 4f46 2041  UT WARRANTY OF A
+000003d0: 4e59 204b 494e 442c 2045 5850 5245 5353  NY KIND, EXPRESS
+000003e0: 204f 520a 2020 2020 2020 2020 494d 504c   OR.        IMPL
+000003f0: 4945 442c 2049 4e43 4c55 4449 4e47 2042  IED, INCLUDING B
+00000400: 5554 204e 4f54 204c 494d 4954 4544 2054  UT NOT LIMITED T
+00000410: 4f20 5448 4520 5741 5252 414e 5449 4553  O THE WARRANTIES
+00000420: 204f 4620 4d45 5243 4841 4e54 4142 494c   OF MERCHANTABIL
+00000430: 4954 592c 0a20 2020 2020 2020 2046 4954  ITY,.        FIT
+00000440: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
+00000450: 4355 4c41 5220 5055 5250 4f53 4520 414e  CULAR PURPOSE AN
+00000460: 4420 4e4f 4e49 4e46 5249 4e47 454d 454e  D NONINFRINGEMEN
+00000470: 542e 2049 4e20 4e4f 2045 5645 4e54 2053  T. IN NO EVENT S
+00000480: 4841 4c4c 2054 4845 0a20 2020 2020 2020  HALL THE.       
+00000490: 2041 5554 484f 5253 204f 5220 434f 5059   AUTHORS OR COPY
+000004a0: 5249 4748 5420 484f 4c44 4552 5320 4245  RIGHT HOLDERS BE
+000004b0: 204c 4941 424c 4520 464f 5220 414e 5920   LIABLE FOR ANY 
+000004c0: 434c 4149 4d2c 2044 414d 4147 4553 204f  CLAIM, DAMAGES O
+000004d0: 5220 4f54 4845 520a 2020 2020 2020 2020  R OTHER.        
+000004e0: 4c49 4142 494c 4954 592c 2057 4845 5448  LIABILITY, WHETH
+000004f0: 4552 2049 4e20 414e 2041 4354 494f 4e20  ER IN AN ACTION 
+00000500: 4f46 2043 4f4e 5452 4143 542c 2054 4f52  OF CONTRACT, TOR
+00000510: 5420 4f52 204f 5448 4552 5749 5345 2c20  T OR OTHERWISE, 
+00000520: 4152 4953 494e 4720 4652 4f4d 2c0a 2020  ARISING FROM,.  
+00000530: 2020 2020 2020 4f55 5420 4f46 204f 5220        OUT OF OR 
+00000540: 494e 2043 4f4e 4e45 4354 494f 4e20 5749  IN CONNECTION WI
+00000550: 5448 2054 4845 2053 4f46 5457 4152 4520  TH THE SOFTWARE 
+00000560: 4f52 2054 4845 2055 5345 204f 5220 4f54  OR THE USE OR OT
+00000570: 4845 5220 4445 414c 494e 4753 2049 4e20  HER DEALINGS IN 
+00000580: 5448 450a 2020 2020 2020 2020 534f 4654  THE.        SOFT
+00000590: 5741 5245 2e0a 2020 2020 2020 2020 0a50  WARE..        .P
+000005a0: 726f 6a65 6374 2d55 524c 3a20 4769 7448  roject-URL: GitH
+000005b0: 7562 2c20 6874 7470 733a 2f2f 6769 7468  ub, https://gith
+000005c0: 7562 2e63 6f6d 2f54 6f6d 6173 7a41 6e69  ub.com/TomaszAni
+000005d0: 6f6c 6f77 736b 692f 6d69 6d65 6f0a 4b65  olowski/mimeo.Ke
+000005e0: 7977 6f72 6473 3a20 6d69 6d65 6f67 7261  ywords: mimeogra
+000005f0: 7068 2c6d 696d 656f 2c67 656e 6572 6174  ph,mimeo,generat
+00000600: 652c 6765 6e65 7261 746f 722c 6461 7461  e,generator,data
+00000610: 2c78 6d6c 2c6a 736f 6e2c 6e6f 7371 6c0a  ,xml,json,nosql.
+00000620: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
+00000630: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000640: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000650: 7365 0a43 6c61 7373 6966 6965 723a 2044  se.Classifier: D
+00000660: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
+00000670: 7320 3a3a 2035 202d 2050 726f 6475 6374  s :: 5 - Product
+00000680: 696f 6e2f 5374 6162 6c65 0a43 6c61 7373  ion/Stable.Class
+00000690: 6966 6965 723a 2045 6e76 6972 6f6e 6d65  ifier: Environme
+000006a0: 6e74 203a 3a20 436f 6e73 6f6c 650a 436c  nt :: Console.Cl
+000006b0: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
+000006c0: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+000006d0: 6576 656c 6f70 6572 730a 436c 6173 7369  evelopers.Classi
+000006e0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000006f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000700: 7468 6f6e 0a43 6c61 7373 6966 6965 723a  thon.Classifier:
+00000710: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000720: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000730: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
+00000740: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000750: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000760: 3a3a 2033 203a 3a20 4f6e 6c79 0a43 6c61  :: 3 :: Only.Cla
+00000770: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000780: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000790: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
+000007a0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000007b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000007c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+000007d0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000007e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000007f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000800: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
+00000810: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000820: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000830: 3a20 332e 3131 0a43 6c61 7373 6966 6965  : 3.11.Classifie
+00000840: 723a 2054 6f70 6963 203a 3a20 4461 7461  r: Topic :: Data
+00000850: 6261 7365 0a43 6c61 7373 6966 6965 723a  base.Classifier:
+00000860: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
+00000870: 7265 2044 6576 656c 6f70 6d65 6e74 0a43  re Development.C
+00000880: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+00000890: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+000008a0: 656c 6f70 6d65 6e74 203a 3a20 5465 7374  elopment :: Test
+000008b0: 696e 670a 436c 6173 7369 6669 6572 3a20  ing.Classifier: 
+000008c0: 546f 7069 6320 3a3a 2055 7469 6c69 7469  Topic :: Utiliti
+000008d0: 6573 0a52 6571 7569 7265 732d 5079 7468  es.Requires-Pyth
+000008e0: 6f6e 3a20 3e3d 332e 380a 4465 7363 7269  on: >=3.8.Descri
+000008f0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+00000900: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+00000910: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
+00000920: 3a20 6465 760a 5072 6f76 6964 6573 2d45  : dev.Provides-E
+00000930: 7874 7261 3a20 7465 7374 0a4c 6963 656e  xtra: test.Licen
+00000940: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+00000950: 0a0a 2320 4d69 6d65 6f20 284d 696d 656f  ..# Mimeo (Mimeo
+00000960: 6772 6170 6829 0a0a 5b21 5b4c 6963 656e  graph)..[![Licen
+00000970: 7365 5d28 6874 7470 733a 2f2f 696d 672e  se](https://img.
+00000980: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00000990: 622f 6c69 6365 6e73 652f 546f 6d61 737a  b/license/Tomasz
+000009a0: 416e 696f 6c6f 7773 6b69 2f6d 696d 656f  Aniolowski/mimeo
+000009b0: 3f6c 6162 656c 3d4c 6963 656e 7365 2673  ?label=License&s
+000009c0: 7479 6c65 3d70 6c61 7374 6963 295d 2868  tyle=plastic)](h
+000009d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000009e0: 6d2f 546f 6d61 737a 416e 696f 6c6f 7773  m/TomaszAniolows
+000009f0: 6b69 2f6d 696d 656f 2f62 6c6f 622f 6465  ki/mimeo/blob/de
+00000a00: 7665 6c6f 702f 4c49 4345 4e53 4529 0a5b  velop/LICENSE).[
+00000a10: 215b 5665 7273 696f 6e5d 2868 7474 7073  ![Version](https
+00000a20: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000a30: 6f2f 7079 7069 2f76 2f6d 696d 656f 6772  o/pypi/v/mimeogr
+00000a40: 6170 683f 636f 6c6f 723d 626c 7565 266c  aph?color=blue&l
+00000a50: 6162 656c 3d50 7950 4926 7374 796c 653d  abel=PyPI&style=
+00000a60: 706c 6173 7469 6329 5d28 6874 7470 733a  plastic)](https:
+00000a70: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000a80: 6374 2f6d 696d 656f 6772 6170 682f 290a  ct/mimeograph/).
+00000a90: 5b21 5b50 7974 686f 6e5d 2868 7474 7073  [![Python](https
+00000aa0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000ab0: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
+00000ac0: 732f 6d69 6d65 6f67 7261 7068 3f6c 6162  s/mimeograph?lab
+00000ad0: 656c 3d50 7974 686f 6e26 7374 796c 653d  el=Python&style=
+00000ae0: 706c 6173 7469 6329 5d28 6874 7470 733a  plastic)](https:
+00000af0: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+00000b00: 2f29 2020 0a5b 215b 4275 696c 645d 2868  /)  .[![Build](h
+00000b10: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000b20: 6473 2e69 6f2f 6769 7468 7562 2f61 6374  ds.io/github/act
+00000b30: 696f 6e73 2f77 6f72 6b66 6c6f 772f 7374  ions/workflow/st
+00000b40: 6174 7573 2f54 6f6d 6173 7a41 6e69 6f6c  atus/TomaszAniol
+00000b50: 6f77 736b 692f 6d69 6d65 6f2f 7465 7374  owski/mimeo/test
+00000b60: 2e79 6d6c 3f63 6f6c 6f72 3d62 7269 6768  .yml?color=brigh
+00000b70: 7467 7265 656e 266c 6162 656c 3d54 6573  tgreen&label=Tes
+00000b80: 7425 3230 4d69 6d65 6f26 7374 796c 653d  t%20Mimeo&style=
+00000b90: 706c 6173 7469 6329 5d28 6874 7470 733a  plastic)](https:
+00000ba0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6f6d  //github.com/Tom
+00000bb0: 6173 7a41 6e69 6f6c 6f77 736b 692f 6d69  aszAniolowski/mi
+00000bc0: 6d65 6f2f 6163 7469 6f6e 732f 776f 726b  meo/actions/work
+00000bd0: 666c 6f77 732f 7465 7374 2e79 6d6c 3f71  flows/test.yml?q
+00000be0: 7565 7279 3d62 7261 6e63 6825 3341 6d61  uery=branch%3Ama
+00000bf0: 696e 290a 5b21 5b43 6f64 6520 436f 7665  in).[![Code Cove
+00000c00: 7261 6765 5d28 6874 7470 733a 2f2f 696d  rage](https://im
+00000c10: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000c20: 6765 2f43 6f64 6525 3230 436f 7665 7261  ge/Code%20Covera
+00000c30: 6765 2d31 3030 2532 352d 6272 6967 6874  ge-100%25-bright
+00000c40: 6772 6565 6e3f 7374 796c 653d 706c 6173  green?style=plas
+00000c50: 7469 6329 5d28 6874 7470 733a 2f2f 6769  tic)](https://gi
+00000c60: 7468 7562 2e63 6f6d 2f54 6f6d 6173 7a41  thub.com/TomaszA
+00000c70: 6e69 6f6c 6f77 736b 692f 6d69 6d65 6f2f  niolowski/mimeo/
+00000c80: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000c90: 732f 636f 7665 7261 6765 5f62 6164 6765  s/coverage_badge
+00000ca0: 2e79 6d6c 3f71 7565 7279 3d62 7261 6e63  .yml?query=branc
+00000cb0: 6825 3341 6d61 696e 290a 0a5b 4d69 6d65  h%3Amain)..[Mime
+00000cc0: 6f5d 2868 7474 7073 3a2f 2f67 6974 6875  o](https://githu
+00000cd0: 622e 636f 6d2f 546f 6d61 737a 416e 696f  b.com/TomaszAnio
+00000ce0: 6c6f 7773 6b69 2f6d 696d 656f 2920 6973  lowski/mimeo) is
+00000cf0: 2061 2063 6f6d 6d61 6e64 206c 696e 6520   a command line 
+00000d00: 746f 6f6c 2061 6e64 2061 2070 7974 686f  tool and a pytho
+00000d10: 6e20 6c69 6272 6172 7920 6765 6e65 7261  n library genera
+00000d20: 7469 6e67 204e 6f53 514c 2064 6174 6120  ting NoSQL data 
+00000d30: 6261 7365 6420 6f6e 2061 2074 656d 706c  based on a templ
+00000d40: 6174 652e 0a49 7420 6361 6e20 6265 2075  ate..It can be u
+00000d50: 7365 6420 6279 2064 6576 656c 6f70 6572  sed by developer
+00000d60: 732c 2074 6573 7465 7273 206f 7220 6275  s, testers or bu
+00000d70: 7369 6e65 7373 2061 6e61 6c79 7374 7320  siness analysts 
+00000d80: 696e 2074 6865 6972 2064 6169 6c79 2077  in their daily w
+00000d90: 6f72 6b2e 0a0a 0a23 2320 496e 7374 616c  ork....## Instal
+00000da0: 6c61 7469 6f6e 0a0a 496e 7374 616c 6c20  lation..Install 
+00000db0: 4d69 6d65 6f20 7769 7468 2070 6970 0a0a  Mimeo with pip..
+00000dc0: 6060 6073 680a 7069 7020 696e 7374 616c  ```sh.pip instal
+00000dd0: 6c20 6d69 6d65 6f67 7261 7068 0a60 6060  l mimeograph.```
+00000de0: 0a0a 0a23 2320 5573 6167 652f 4578 616d  ...## Usage/Exam
+00000df0: 706c 6573 0a0a 2323 2320 4d69 6d65 6f20  ples..### Mimeo 
+00000e00: 436f 6e66 6967 7572 6174 696f 6e0a 0a50  Configuration..P
+00000e10: 7265 7061 7265 204d 696d 656f 2043 6f6e  repare Mimeo Con
+00000e20: 6669 6775 7261 7469 6f6e 2066 6972 7374  figuration first
+00000e30: 0a0a 3c74 6162 6c65 3e0a 2020 2020 3c74  ..<table>.    <t
+00000e40: 723e 0a20 2020 2020 2020 203c 7468 3e4a  r>.        <th>J
+00000e50: 534f 4e3c 2f74 683e 0a20 2020 2020 2020  SON</th>.       
+00000e60: 203c 7468 3e58 4d4c 3c2f 7468 3e0a 2020   <th>XML</th>.  
+00000e70: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+00000e80: 0a20 2020 2020 2020 203c 7464 2076 616c  .        <td val
+00000e90: 6967 6e3d 2274 6f70 223e 0a0a 6060 606a  ign="top">..```j
+00000ea0: 736f 6e0a 7b0a 2020 225f 7465 6d70 6c61  son.{.  "_templa
+00000eb0: 7465 735f 223a 205b 0a20 2020 207b 0a20  tes_": [.    {. 
+00000ec0: 2020 2020 2022 636f 756e 7422 3a20 3330       "count": 30
+00000ed0: 2c0a 2020 2020 2020 226d 6f64 656c 223a  ,.      "model":
+00000ee0: 207b 0a20 2020 2020 2020 2022 536f 6d65   {.        "Some
+00000ef0: 456e 7469 7479 223a 207b 0a20 2020 2020  Entity": {.     
+00000f00: 2020 2020 2022 4078 6d6c 6e73 223a 2022       "@xmlns": "
+00000f10: 6874 7470 3a2f 2f6d 696d 656f 2e61 7263  http://mimeo.arc
+00000f20: 682e 636f 6d2f 6465 6661 756c 742d 6e61  h.com/default-na
+00000f30: 6d65 7370 6163 6522 2c0a 2020 2020 2020  mespace",.      
+00000f40: 2020 2020 2240 786d 6c6e 733a 706e 223a      "@xmlns:pn":
+00000f50: 2022 6874 7470 3a2f 2f6d 696d 656f 2e61   "http://mimeo.a
+00000f60: 7263 682e 636f 6d2f 7072 6566 6978 6564  rch.com/prefixed
+00000f70: 2d6e 616d 6573 7061 6365 222c 0a20 2020  -namespace",.   
+00000f80: 2020 2020 2020 2022 4368 696c 644e 6f64         "ChildNod
+00000f90: 6531 223a 2031 2c0a 2020 2020 2020 2020  e1": 1,.        
+00000fa0: 2020 2243 6869 6c64 4e6f 6465 3222 3a20    "ChildNode2": 
+00000fb0: 2276 616c 7565 2d32 222c 0a20 2020 2020  "value-2",.     
+00000fc0: 2020 2020 2022 4368 696c 644e 6f64 6533       "ChildNode3
+00000fd0: 223a 2074 7275 650a 2020 2020 2020 2020  ": true.        
+00000fe0: 7d0a 2020 2020 2020 7d0a 2020 2020 7d0a  }.      }.    }.
+00000ff0: 2020 5d0a 7d0a 6060 600a 3c2f 7464 3e0a    ].}.```.</td>.
+00001000: 2020 2020 2020 2020 3c74 6420 7661 6c69          <td vali
+00001010: 676e 3d22 746f 7022 3e0a 0a60 6060 786d  gn="top">..```xm
+00001020: 6c0a 3c6d 696d 656f 5f63 6f6e 6669 6775  l.<mimeo_configu
+00001030: 7261 7469 6f6e 3e0a 2020 2020 3c5f 7465  ration>.    <_te
+00001040: 6d70 6c61 7465 735f 3e0a 2020 2020 2020  mplates_>.      
+00001050: 2020 3c5f 7465 6d70 6c61 7465 5f3e 0a20    <_template_>. 
+00001060: 2020 2020 2020 2020 2020 203c 636f 756e             <coun
+00001070: 743e 3330 3c2f 636f 756e 743e 0a20 2020  t>30</count>.   
+00001080: 2020 2020 2020 2020 203c 6d6f 6465 6c3e           <model>
+00001090: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000010a0: 2020 3c53 6f6d 6545 6e74 6974 790a 2020    <SomeEntity.  
+000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010c0: 2020 786d 6c6e 733d 2268 7474 703a 2f2f    xmlns="http://
+000010d0: 6d69 6d65 6f2e 6172 6368 2e63 6f6d 2f64  mimeo.arch.com/d
+000010e0: 6566 6175 6c74 2d6e 616d 6573 7061 6365  efault-namespace
+000010f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00001100: 2020 2020 2020 786d 6c6e 733a 706e 3d22        xmlns:pn="
+00001110: 6874 7470 3a2f 2f6d 696d 656f 2e61 7263  http://mimeo.arc
+00001120: 682e 636f 6d2f 7072 6566 6978 6564 2d6e  h.com/prefixed-n
+00001130: 616d 6573 7061 6365 223e 0a20 2020 2020  amespace">.     
+00001140: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001150: 4368 696c 644e 6f64 6531 3e31 3c2f 4368  ChildNode1>1</Ch
+00001160: 696c 644e 6f64 6531 3e0a 2020 2020 2020  ildNode1>.      
+00001170: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00001180: 6e3a 4368 696c 644e 6f64 6532 3e76 616c  n:ChildNode2>val
+00001190: 7565 2d32 3c2f 706e 3a43 6869 6c64 4e6f  ue-2</pn:ChildNo
+000011a0: 6465 323e 0a20 2020 2020 2020 2020 2020  de2>.           
+000011b0: 2020 2020 2020 2020 203c 4368 696c 644e           <ChildN
+000011c0: 6f64 6533 3e74 7275 653c 2f43 6869 6c64  ode3>true</Child
+000011d0: 4e6f 6465 333e 0a20 2020 2020 2020 2020  Node3>.         
+000011e0: 2020 2020 2020 203c 2f53 6f6d 6545 6e74         </SomeEnt
+000011f0: 6974 793e 0a0a 2020 2020 2020 2020 2020  ity>..          
+00001200: 2020 3c2f 6d6f 6465 6c3e 0a20 2020 2020    </model>.     
+00001210: 2020 203c 2f5f 7465 6d70 6c61 7465 5f3e     </_template_>
+00001220: 0a20 2020 203c 2f5f 7465 6d70 6c61 7465  .    </_template
+00001230: 735f 3e0a 3c2f 6d69 6d65 6f5f 636f 6e66  s_>.</mimeo_conf
+00001240: 6967 7572 6174 696f 6e3e 0a60 6060 0a3c  iguration>.```.<
+00001250: 2f74 643e 0a20 203c 2f74 723e 0a3c 2f74  /td>.  </tr>.</t
+00001260: 6162 6c65 3e0a 0a0a 5f59 6f75 2063 616e  able>..._You can
+00001270: 2066 696e 6420 6d6f 7265 2063 6f6e 6669   find more confi
+00001280: 6775 7261 7469 6f6e 2065 7861 6d70 6c65  guration example
+00001290: 7320 696e 2074 6865 2060 6578 616d 706c  s in the `exampl
+000012a0: 6573 6020 666f 6c64 6572 2e5f 0a0a 2323  es` folder._..##
+000012b0: 2320 4461 7461 2067 656e 6572 6174 696f  # Data generatio
+000012c0: 6e0a 0a54 6865 204d 696d 656f 2043 6f6e  n..The Mimeo Con
+000012d0: 6669 6775 7261 7469 6f6e 2061 626f 7665  figuration above
+000012e0: 2077 696c 6c20 7072 6f64 7563 6520 3220   will produce 2 
+000012f0: 6669 6c65 733a 0a0a 6060 6078 6d6c 0a3c  files:..```xml.<
+00001300: 212d 2d20 6d69 6d65 6f2d 6f75 7470 7574  !-- mimeo-output
+00001310: 2f6d 696d 656f 2d6f 7574 7075 742d 312e  /mimeo-output-1.
+00001320: 786d 6c2d 2d3e 0a3c 536f 6d65 456e 7469  xml-->.<SomeEnti
+00001330: 7479 2078 6d6c 6e73 3d22 6874 7470 3a2f  ty xmlns="http:/
+00001340: 2f6d 696d 656f 2e61 7263 682e 636f 6d2f  /mimeo.arch.com/
+00001350: 6465 6661 756c 742d 6e61 6d65 7370 6163  default-namespac
+00001360: 6522 2078 6d6c 6e73 3a70 6e3d 2268 7474  e" xmlns:pn="htt
+00001370: 703a 2f2f 6d69 6d65 6f2e 6172 6368 2e63  p://mimeo.arch.c
+00001380: 6f6d 2f70 7265 6669 7865 642d 6e61 6d65  om/prefixed-name
+00001390: 7370 6163 6522 3e0a 2020 2020 3c43 6869  space">.    <Chi
+000013a0: 6c64 4e6f 6465 313e 313c 2f43 6869 6c64  ldNode1>1</Child
+000013b0: 4e6f 6465 313e 0a20 2020 203c 706e 3a43  Node1>.    <pn:C
+000013c0: 6869 6c64 4e6f 6465 323e 7661 6c75 652d  hildNode2>value-
+000013d0: 323c 2f70 6e3a 4368 696c 644e 6f64 6532  2</pn:ChildNode2
+000013e0: 3e0a 2020 2020 3c43 6869 6c64 4e6f 6465  >.    <ChildNode
+000013f0: 333e 7472 7565 3c2f 4368 696c 644e 6f64  3>true</ChildNod
+00001400: 6533 3e0a 3c2f 536f 6d65 456e 7469 7479  e3>.</SomeEntity
+00001410: 3e0a 6060 600a 6060 6078 6d6c 0a3c 212d  >.```.```xml.<!-
+00001420: 2d20 6d69 6d65 6f2d 6f75 7470 7574 2f6d  - mimeo-output/m
+00001430: 696d 656f 2d6f 7574 7075 742d 322e 786d  imeo-output-2.xm
+00001440: 6c2d 2d3e 0a3c 536f 6d65 456e 7469 7479  l-->.<SomeEntity
+00001450: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f6d   xmlns="http://m
+00001460: 696d 656f 2e61 7263 682e 636f 6d2f 6465  imeo.arch.com/de
+00001470: 6661 756c 742d 6e61 6d65 7370 6163 6522  fault-namespace"
+00001480: 2078 6d6c 6e73 3a70 6e3d 2268 7474 703a   xmlns:pn="http:
+00001490: 2f2f 6d69 6d65 6f2e 6172 6368 2e63 6f6d  //mimeo.arch.com
+000014a0: 2f70 7265 6669 7865 642d 6e61 6d65 7370  /prefixed-namesp
+000014b0: 6163 6522 3e0a 2020 2020 3c43 6869 6c64  ace">.    <Child
+000014c0: 4e6f 6465 313e 313c 2f43 6869 6c64 4e6f  Node1>1</ChildNo
+000014d0: 6465 313e 0a20 2020 203c 706e 3a43 6869  de1>.    <pn:Chi
+000014e0: 6c64 4e6f 6465 323e 7661 6c75 652d 323c  ldNode2>value-2<
+000014f0: 2f70 6e3a 4368 696c 644e 6f64 6532 3e0a  /pn:ChildNode2>.
+00001500: 2020 2020 3c43 6869 6c64 4e6f 6465 333e      <ChildNode3>
+00001510: 7472 7565 3c2f 4368 696c 644e 6f64 6533  true</ChildNode3
+00001520: 3e0a 3c2f 536f 6d65 456e 7469 7479 3e0a  >.</SomeEntity>.
+00001530: 6060 600a 0a57 6865 6e20 7765 2077 6f75  ```..When we wou
+00001540: 6c64 2063 6f6e 6669 6775 7265 206f 7574  ld configure out
+00001550: 7075 7420 666f 726d 6174 2061 7320 606a  put format as `j
+00001560: 736f 6e60 2074 6865 6e20 6974 2077 6f75  son` then it wou
+00001570: 6c64 2070 726f 6475 6365 204a 534f 4e20  ld produce JSON 
+00001580: 6e6f 6465 733a 0a0a 6060 606a 736f 6e0a  nodes:..```json.
+00001590: 7b0a 2020 2253 6f6d 6545 6e74 6974 7922  {.  "SomeEntity"
+000015a0: 3a20 7b0a 2020 2020 2240 786d 6c6e 7322  : {.    "@xmlns"
+000015b0: 3a20 2268 7474 703a 2f2f 6d69 6d65 6f2e  : "http://mimeo.
+000015c0: 6172 6368 2e63 6f6d 2f64 6566 6175 6c74  arch.com/default
+000015d0: 2d6e 616d 6573 7061 6365 222c 0a20 2020  -namespace",.   
+000015e0: 2022 4078 6d6c 6e73 3a70 6e22 3a20 2268   "@xmlns:pn": "h
+000015f0: 7474 703a 2f2f 6d69 6d65 6f2e 6172 6368  ttp://mimeo.arch
+00001600: 2e63 6f6d 2f70 7265 6669 7865 642d 6e61  .com/prefixed-na
+00001610: 6d65 7370 6163 6522 2c0a 2020 2020 2243  mespace",.    "C
+00001620: 6869 6c64 4e6f 6465 3122 3a20 312c 0a20  hildNode1": 1,. 
+00001630: 2020 2022 706e 3a43 6869 6c64 4e6f 6465     "pn:ChildNode
+00001640: 3222 3a20 2276 616c 7565 2d32 222c 0a20  2": "value-2",. 
+00001650: 2020 2022 4368 696c 644e 6f64 6533 223a     "ChildNode3":
+00001660: 2074 7275 650a 2020 7d0a 7d0a 6060 600a   true.  }.}.```.
+00001670: 6060 606a 736f 6e0a 7b0a 2020 2253 6f6d  ```json.{.  "Som
+00001680: 6545 6e74 6974 7922 3a20 7b0a 2020 2020  eEntity": {.    
+00001690: 2240 786d 6c6e 7322 3a20 2268 7474 703a  "@xmlns": "http:
+000016a0: 2f2f 6d69 6d65 6f2e 6172 6368 2e63 6f6d  //mimeo.arch.com
+000016b0: 2f64 6566 6175 6c74 2d6e 616d 6573 7061  /default-namespa
+000016c0: 6365 222c 0a20 2020 2022 4078 6d6c 6e73  ce",.    "@xmlns
+000016d0: 3a70 6e22 3a20 2268 7474 703a 2f2f 6d69  :pn": "http://mi
+000016e0: 6d65 6f2e 6172 6368 2e63 6f6d 2f70 7265  meo.arch.com/pre
+000016f0: 6669 7865 642d 6e61 6d65 7370 6163 6522  fixed-namespace"
+00001700: 2c0a 2020 2020 2243 6869 6c64 4e6f 6465  ,.    "ChildNode
+00001710: 3122 3a20 312c 0a20 2020 2022 706e 3a43  1": 1,.    "pn:C
+00001720: 6869 6c64 4e6f 6465 3222 3a20 2276 616c  hildNode2": "val
+00001730: 7565 2d32 222c 0a20 2020 2022 4368 696c  ue-2",.    "Chil
+00001740: 644e 6f64 6533 223a 2074 7275 650a 2020  dNode3": true.  
+00001750: 7d0a 7d0a 6060 600a 0a60 6060 7368 0a6d  }.}.```..```sh.m
+00001760: 696d 656f 2053 6f6d 6545 6e74 6974 792d  imeo SomeEntity-
+00001770: 636f 6e66 6967 2e6a 736f 6e0a 6d69 6d65  config.json.mime
+00001780: 6f20 536f 6d65 456e 7469 7479 2d63 6f6e  o SomeEntity-con
+00001790: 6669 672e 786d 6c0a 6060 600a 0a0a 2323  fig.xml.```...##
+000017a0: 2320 4d69 6d65 6f20 5574 696c 730a 0a4d  # Mimeo Utils..M
+000017b0: 696d 656f 2065 7870 6f73 6573 2073 6576  imeo exposes sev
+000017c0: 6572 616c 2066 756e 6374 696f 6e73 2066  eral functions f
+000017d0: 6f72 2064 6174 6120 6765 6e65 7261 7469  or data generati
+000017e0: 6f6e 2074 6861 7420 7769 6c6c 206d 616b  on that will mak
+000017f0: 6520 6974 206d 6f72 6520 7573 6566 756c  e it more useful
+00001800: 2066 6f72 2074 6573 7469 6e67 2070 7572   for testing pur
+00001810: 706f 7365 732e 0a54 6f20 7365 6520 616c  poses..To see al
+00001820: 6c20 4d69 6d65 6f20 5574 696c 732c 2067  l Mimeo Utils, g
+00001830: 6f20 746f 2074 6865 2064 6f63 756d 656e  o to the documen
+00001840: 7461 7469 6f6e 2062 656c 6f77 2e0a 0a2a  tation below...*
+00001850: 2a54 656d 706c 6174 652a 2a0a 6060 606a  *Template**.```j
+00001860: 736f 6e0a 7b0a 2020 2263 6f75 6e74 223a  son.{.  "count":
+00001870: 2032 2c0a 2020 226d 6f64 656c 223a 207b   2,.  "model": {
+00001880: 0a20 2020 2022 536f 6d65 456e 7469 7479  .    "SomeEntity
+00001890: 223a 207b 0a20 2020 2020 2022 6964 223a  ": {.      "id":
+000018a0: 2022 7b61 7574 6f5f 696e 6372 656d 656e   "{auto_incremen
+000018b0: 747d 222c 0a20 2020 2020 2022 7261 6e64  t}",.      "rand
+000018c0: 6f6d 7374 7269 6e67 223a 2022 7b72 616e  omstring": "{ran
+000018d0: 646f 6d5f 7374 727d 222c 0a20 2020 2020  dom_str}",.     
+000018e0: 2022 7261 6e64 6f6d 696e 7422 3a20 227b   "randomint": "{
+000018f0: 7261 6e64 6f6d 5f69 6e74 7d22 0a20 2020  random_int}".   
+00001900: 207d 0a20 207d 0a7d 0a60 6060 0a60 6060   }.  }.}.```.```
+00001910: 786d 6c0a 3c5f 7465 6d70 6c61 7465 5f3e  xml.<_template_>
+00001920: 0a20 2020 203c 636f 756e 743e 323c 2f63  .    <count>2</c
+00001930: 6f75 6e74 3e0a 2020 2020 3c6d 6f64 656c  ount>.    <model
+00001940: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
+00001950: 2020 203c 536f 6d65 456e 7469 7479 3e0a     <SomeEntity>.
+00001960: 2020 2020 2020 2020 2020 2020 3c69 643e              <id>
+00001970: 7b61 7574 6f5f 696e 6372 656d 656e 747d  {auto_increment}
+00001980: 3c2f 6964 3e0a 2020 2020 2020 2020 2020  </id>.          
+00001990: 2020 3c72 616e 646f 6d73 7472 696e 673e    <randomstring>
+000019a0: 7b72 616e 646f 6d5f 7374 727d 3c2f 7261  {random_str}</ra
+000019b0: 6e64 6f6d 7374 7269 6e67 3e0a 2020 2020  ndomstring>.    
+000019c0: 2020 2020 2020 2020 3c72 616e 646f 6d69          <randomi
+000019d0: 6e74 3e7b 7261 6e64 6f6d 5f69 6e74 7d3c  nt>{random_int}<
+000019e0: 2f72 616e 646f 6d69 6e74 3e0a 2020 2020  /randomint>.    
+000019f0: 2020 2020 3c2f 536f 6d65 456e 7469 7479      </SomeEntity
+00001a00: 3e0a 2020 2020 2020 2020 0a20 2020 203c  >.        .    <
+00001a10: 2f6d 6f64 656c 3e0a 3c2f 5f74 656d 706c  /model>.</_templ
+00001a20: 6174 655f 3e0a 6060 600a 0a2a 2a58 4d4c  ate_>.```..**XML
+00001a30: 2044 6174 612a 2a0a 6060 6078 6d6c 0a3c   Data**.```xml.<
+00001a40: 536f 6d65 456e 7469 7479 3e0a 2020 2020  SomeEntity>.    
+00001a50: 3c69 643e 3030 3030 313c 2f69 643e 0a20  <id>00001</id>. 
+00001a60: 2020 203c 7261 6e64 6f6d 7374 7269 6e67     <randomstring
+00001a70: 3e6d 4341 7073 595a 7072 6179 596b 6d4b  >mCApsYZprayYkmK
+00001a80: 6e59 5778 653c 2f72 616e 646f 6d73 7472  nYWxe</randomstr
+00001a90: 696e 673e 0a20 2020 203c 7261 6e64 6f6d  ing>.    <random
+00001aa0: 696e 743e 383c 2f72 616e 646f 6d69 6e74  int>8</randomint
+00001ab0: 3e0a 3c2f 536f 6d65 456e 7469 7479 3e0a  >.</SomeEntity>.
+00001ac0: 6060 600a 6060 6078 6d6c 0a3c 536f 6d65  ```.```xml.<Some
+00001ad0: 456e 7469 7479 3e0a 2020 2020 3c69 643e  Entity>.    <id>
+00001ae0: 3030 3030 323c 2f69 643e 0a20 2020 203c  00002</id>.    <
+00001af0: 7261 6e64 6f6d 7374 7269 6e67 3e63 6561  randomstring>cea
+00001b00: 5055 7141 5255 6b46 756b 5a49 5065 7571  PUqARUkFukZIPeuq
+00001b10: 4f3c 2f72 616e 646f 6d73 7472 696e 673e  O</randomstring>
+00001b20: 0a20 2020 203c 7261 6e64 6f6d 696e 743e  .    <randomint>
+00001b30: 3939 3c2f 7261 6e64 6f6d 696e 743e 0a3c  99</randomint>.<
+00001b40: 2f53 6f6d 6545 6e74 6974 793e 0a60 6060  /SomeEntity>.```
+00001b50: 0a0a 2a2a 4a53 4f4e 2044 6174 612a 2a0a  ..**JSON Data**.
+00001b60: 6060 606a 736f 6e0a 7b0a 2020 2253 6f6d  ```json.{.  "Som
+00001b70: 6545 6e74 6974 7922 3a20 7b0a 2020 2020  eEntity": {.    
+00001b80: 2269 6422 3a20 2230 3030 3031 222c 0a20  "id": "00001",. 
+00001b90: 2020 2022 7261 6e64 6f6d 7374 7269 6e67     "randomstring
+00001ba0: 223a 2022 6d43 4170 7359 5a70 7261 7959  ": "mCApsYZprayY
+00001bb0: 6b6d 4b6e 5957 7865 222c 0a20 2020 2022  kmKnYWxe",.    "
+00001bc0: 7261 6e64 6f6d 696e 7422 3a20 380a 2020  randomint": 8.  
+00001bd0: 7d0a 7d0a 6060 600a 6060 606a 736f 6e0a  }.}.```.```json.
+00001be0: 7b0a 2020 2253 6f6d 6545 6e74 6974 7922  {.  "SomeEntity"
+00001bf0: 3a20 7b0a 2020 2020 2269 6422 3a20 2230  : {.    "id": "0
+00001c00: 3030 3032 222c 0a20 2020 2022 7261 6e64  0002",.    "rand
+00001c10: 6f6d 7374 7269 6e67 223a 2022 6365 6150  omstring": "ceaP
+00001c20: 5571 4152 556b 4675 6b5a 4950 6575 714f  UqARUkFukZIPeuqO
+00001c30: 222c 0a20 2020 2022 7261 6e64 6f6d 696e  ",.    "randomin
+00001c40: 7422 3a20 3939 0a20 207d 0a7d 0a60 6060  t": 99.  }.}.```
+00001c50: 0a0a 0a23 2320 446f 6375 6d65 6e74 6174  ...## Documentat
+00001c60: 696f 6e0a 0a23 2323 204d 696d 656f 2043  ion..### Mimeo C
+00001c70: 4c49 0a0a 2323 2323 204d 696d 656f 2043  LI..#### Mimeo C
+00001c80: 6f6e 6669 6775 7261 7469 6f6e 2061 7267  onfiguration arg
+00001c90: 756d 656e 7473 0a0a 5768 656e 2075 7369  uments..When usi
+00001ca0: 6e67 204d 696d 656f 2063 6f6d 6d61 6e64  ng Mimeo command
+00001cb0: 206c 696e 6520 746f 6f6c 2079 6f75 2063   line tool you c
+00001cc0: 616e 206f 7665 7277 7269 7465 204d 696d  an overwrite Mim
+00001cd0: 656f 2043 6f6e 6669 6775 7261 7469 6f6e  eo Configuration
+00001ce0: 2070 726f 7065 7274 6965 733a 0a0a 7c20   properties:..| 
+00001cf0: 5368 6f72 7420 6f70 7469 6f6e 207c 204c  Short option | L
+00001d00: 6f6e 6720 6f70 7469 6f6e 2020 2020 2020  ong option      
+00001d10: 2020 207c 2044 6573 6372 6970 7469 6f6e     | Description
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d60: 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d      |.|:--------
+00001d70: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
+00001d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d  -----------|:---
+00001d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
+00001de0: 2020 2020 602d 4660 2020 2020 207c 2060      `-F`     | `
+00001df0: 2d2d 666f 726d 6174 6020 2020 2020 2020  --format`       
+00001e00: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
+00001e10: 6865 2060 6f75 7470 7574 2f66 6f72 6d61  he `output/forma
+00001e20: 7460 2070 726f 7065 7274 7920 2020 2020  t` property     
+00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e50: 2020 2020 7c0a 7c20 2020 2020 602d 6f60      |.|     `-o`
+00001e60: 2020 2020 207c 2060 2d2d 6f75 7470 7574       | `--output
+00001e70: 6020 2020 2020 2020 2020 207c 206f 7665  `          | ove
+00001e80: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
+00001e90: 7574 2f64 6972 6563 7469 6f6e 6020 7072  ut/direction` pr
+00001ea0: 6f70 6572 7479 2020 2020 2020 2020 2020  operty          
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ec0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00001ed0: 2020 2020 602d 7860 2020 2020 207c 2060      `-x`     | `
+00001ee0: 2d2d 786d 6c2d 6465 636c 6172 6174 696f  --xml-declaratio
+00001ef0: 6e60 207c 206f 7665 7277 7269 7465 2074  n` | overwrite t
+00001f00: 6865 2060 6f75 7470 7574 2f78 6d6c 5f64  he `output/xml_d
+00001f10: 6563 6c61 7261 7469 6f6e 6020 7072 6f70  eclaration` prop
+00001f20: 6572 7479 2020 2020 2020 2020 2020 2020  erty            
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2020 2020 7c0a 7c20 2020 2020 602d 6960      |.|     `-i`
+00001f50: 2020 2020 207c 2060 2d2d 696e 6465 6e74       | `--indent
+00001f60: 6020 2020 2020 2020 2020 207c 206f 7665  `          | ove
+00001f70: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
+00001f80: 7574 2f69 6e64 656e 7460 2070 726f 7065  ut/indent` prope
+00001f90: 7274 7920 2020 2020 2020 2020 2020 2020  rty             
+00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fb0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00001fc0: 2020 2020 602d 6460 2020 2020 207c 2060      `-d`     | `
+00001fd0: 2d2d 6469 7265 6374 6f72 7960 2020 2020  --directory`    
+00001fe0: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
+00001ff0: 6865 2060 6f75 7470 7574 2f64 6972 6563  he `output/direc
+00002000: 746f 7279 5f70 6174 6860 2070 726f 7065  tory_path` prope
+00002010: 7274 7920 2020 2020 2020 2020 2020 2020  rty             
+00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002030: 2020 2020 7c0a 7c20 2020 2020 602d 6660      |.|     `-f`
+00002040: 2020 2020 207c 2060 2d2d 6669 6c65 6020       | `--file` 
+00002050: 2020 2020 2020 2020 2020 207c 206f 7665             | ove
+00002060: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
+00002070: 7574 2f66 696c 655f 6e61 6d65 6020 7072  ut/file_name` pr
+00002080: 6f70 6572 7479 2020 2020 2020 2020 2020  operty          
+00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020a0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000020b0: 2020 2020 602d 4860 2020 2020 207c 2060      `-H`     | `
+000020c0: 2d2d 6874 7470 2d68 6f73 7460 2020 2020  --http-host`    
+000020d0: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
+000020e0: 6865 2060 6f75 7470 7574 2f68 6f73 7460  he `output/host`
+000020f0: 2070 726f 7065 7274 7920 2020 2020 2020   property       
+00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002120: 2020 2020 7c0a 7c20 2020 2020 602d 7060      |.|     `-p`
+00002130: 2020 2020 207c 2060 2d2d 6874 7470 2d70       | `--http-p
+00002140: 6f72 7460 2020 2020 2020 207c 206f 7665  ort`       | ove
+00002150: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
+00002160: 7574 2f70 6f72 7460 2070 726f 7065 7274  ut/port` propert
+00002170: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002190: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000021a0: 2020 2020 602d 4560 2020 2020 207c 2060      `-E`     | `
+000021b0: 2d2d 6874 7470 2d65 6e64 706f 696e 7460  --http-endpoint`
+000021c0: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
+000021d0: 6865 2060 6f75 7470 7574 2f65 6e64 706f  he `output/endpo
+000021e0: 696e 7460 2070 726f 7065 7274 7920 2020  int` property   
+000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002210: 2020 2020 7c0a 7c20 2020 2020 602d 5560      |.|     `-U`
+00002220: 2020 2020 207c 2060 2d2d 6874 7470 2d75       | `--http-u
+00002230: 7365 7260 2020 2020 2020 207c 206f 7665  ser`       | ove
+00002240: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
+00002250: 7574 2f75 7365 726e 616d 6560 2070 726f  ut/username` pro
+00002260: 7065 7274 7920 2020 2020 2020 2020 2020  perty           
+00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002280: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00002290: 2020 2020 602d 5060 2020 2020 207c 2060      `-P`     | `
+000022a0: 2d2d 6874 7470 2d70 6173 7377 6f72 6460  --http-password`
+000022b0: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
+000022c0: 6865 2060 6f75 7470 7574 2f70 6173 7377  he `output/passw
+000022d0: 6f72 6460 2070 726f 7065 7274 7920 2020  ord` property   
+000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002300: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+00002310: 2020 2020 207c 2060 2d2d 6874 7470 2d6d       | `--http-m
+00002320: 6574 686f 6460 2020 2020 207c 206f 7665  ethod`     | ove
+00002330: 7277 7269 7465 2074 6865 2060 6f75 7470  rwrite the `outp
+00002340: 7574 2f6d 6574 686f 6460 2070 726f 7065  ut/method` prope
+00002350: 7274 7920 2020 2020 2020 2020 2020 2020  rty             
+00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002370: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00002380: 2020 2020 2020 2020 2020 2020 207c 2060               | `
+00002390: 2d2d 6874 7470 2d70 726f 746f 636f 6c60  --http-protocol`
+000023a0: 2020 207c 206f 7665 7277 7269 7465 2074     | overwrite t
+000023b0: 6865 2060 6f75 7470 7574 2f70 726f 746f  he `output/proto
+000023c0: 636f 6c60 2070 726f 7065 7274 7920 2020  col` property   
 000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.|:------------
-00002440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002450: 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d3a  -----|:--------:
-00002460: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-00002470: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00002480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
-00002490: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-000024a0: 3a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|--------------
-000024b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000024c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000024d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000024e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000024f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2060  -----------|.| `
-00002540: 6f75 7470 7574 6020 2020 2020 2020 2020  output`         
-00002550: 2020 2020 2020 2020 7c20 2043 6f6e 6669          |  Confi
-00002560: 6720 207c 2020 2020 2020 2020 3a78 3a20  g  |        :x: 
-00002570: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00002580: 2020 206f 626a 6563 7420 2020 2020 2020     object       
-00002590: 2020 207c 2020 2020 2020 2d2d 2d20 2020     |      ---   
-000025a0: 2020 2020 7c20 4465 6669 6e65 7320 6f75      | Defines ou
-000025b0: 7470 7574 2064 6574 6169 6c73 206f 6e20  tput details on 
-000025c0: 686f 7720 6974 2077 696c 6c20 6265 2063  how it will be c
-000025d0: 6f6e 7375 6d65 6420 2020 2020 2020 2020  onsumed         
-000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00002640: 7c20 606f 7574 7075 742f 6469 7265 6374  | `output/direct
-00002650: 696f 6e60 2020 2020 2020 207c 2020 436f  ion`       |  Co
-00002660: 6e66 6967 2020 7c20 2020 2020 2020 203a  nfig  |        :
-00002670: 783a 2020 2020 2020 2020 207c 2060 6669  x:         | `fi
-00002680: 6c65 602c 2060 7374 646f 7574 602c 2060  le`, `stdout`, `
-00002690: 6874 7470 6020 7c20 2020 2020 6066 696c  http` |     `fil
-000026a0: 6560 2020 2020 207c 2044 6566 696e 6573  e`     | Defines
-000026b0: 2068 6f77 206f 7574 7075 7420 7769 6c6c   how output will
-000026c0: 2062 6520 636f 6e73 756d 6564 2020 2020   be consumed    
+000023f0: 2020 2020 7c0a 7c20 2020 2020 602d 6560      |.|     `-e`
+00002400: 2020 2020 207c 2060 2d2d 6874 7470 2d65       | `--http-e
+00002410: 6e76 6020 2020 2020 2020 207c 206f 7665  nv`        | ove
+00002420: 7277 7269 7465 2074 6865 206f 7574 7075  rwrite the outpu
+00002430: 7420 6874 7470 2070 726f 7065 7274 6965  t http propertie
+00002440: 7320 7573 696e 6720 6120 6d69 6d65 6f20  s using a mimeo 
+00002450: 656e 7620 636f 6e66 6967 7572 6174 696f  env configuratio
+00002460: 6e20 2020 2020 2020 2020 2020 7c0a 7c20  n           |.| 
+00002470: 2020 2020 2020 2020 2020 2020 207c 2060               | `
+00002480: 2d2d 6874 7470 2d65 6e76 732d 6669 6c65  --http-envs-file
+00002490: 6020 207c 2075 7365 2061 2063 7573 746f  `  | use a custo
+000024a0: 6d20 656e 7669 726f 6e6d 656e 7473 2066  m environments f
+000024b0: 696c 6520 2862 7920 6465 6661 756c 743a  ile (by default:
+000024c0: 206d 696d 656f 2e65 6e76 732e 6a73 6f6e   mimeo.envs.json
+000024d0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+000024e0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+000024f0: 2020 2020 207c 2060 2d2d 7261 7760 2020       | `--raw`  
+00002500: 2020 2020 2020 2020 2020 207c 2073 616d             | sam
+00002510: 6520 6173 2060 2d6f 2073 7464 6f75 7460  e as `-o stdout`
+00002520: 3c62 7220 2f3e 6f76 6572 7772 6974 6520  <br />overwrite 
+00002530: 7468 6520 606f 7574 7075 742f 6469 7265  the `output/dire
+00002540: 6374 696f 6e60 2070 726f 7065 7274 7920  ction` property 
+00002550: 746f 2060 7374 646f 7574 6020 7c0a 0a23  to `stdout` |..#
+00002560: 2323 2320 4c6f 6767 696e 6720 6172 6775  ### Logging argu
+00002570: 6d65 6e74 730a 0a7c 2053 686f 7274 206f  ments..| Short o
+00002580: 7074 696f 6e20 7c20 4c6f 6e67 206f 7074  ption | Long opt
+00002590: 696f 6e20 7c20 4465 7363 7269 7074 696f  ion | Descriptio
+000025a0: 6e20 2020 2020 2020 7c0a 7c3a 2d2d 2d2d  n       |.|:----
+000025b0: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
+000025c0: 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d  -------|:-------
+000025d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2020  -----------|.|  
+000025e0: 2020 2020 2020 2020 2020 2020 7c20 602d              | `-
+000025f0: 2d73 696c 656e 7460 2020 7c20 6469 7361  -silent`  | disa
+00002600: 626c 6520 494e 464f 206c 6f67 7320 7c0a  ble INFO logs |.
+00002610: 7c20 2020 2020 2020 2020 2020 2020 207c  |              |
+00002620: 2060 2d2d 6465 6275 6760 2020 207c 2065   `--debug`   | e
+00002630: 6e61 626c 6520 4445 4255 4720 6d6f 6465  nable DEBUG mode
+00002640: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00002650: 2020 7c20 602d 2d66 696e 6560 2020 2020    | `--fine`    
+00002660: 7c20 656e 6162 6c65 2046 494e 4520 6d6f  | enable FINE mo
+00002670: 6465 2020 7c0a 0a23 2323 2320 4f74 6865  de  |..#### Othe
+00002680: 7220 6172 6775 6d65 6e74 730a 0a7c 2053  r arguments..| S
+00002690: 686f 7274 206f 7074 696f 6e20 7c20 4c6f  hort option | Lo
+000026a0: 6e67 206f 7074 696f 6e20 2020 2020 207c  ng option      |
+000026b0: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
+000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 207c 0a7c 2060 6f75 7470 7574 2f66 6f72   |.| `output/for
-00002750: 6d61 7460 2020 2020 2020 2020 2020 7c20  mat`          | 
-00002760: 2043 6f6e 6669 6720 207c 2020 2020 2020   Config  |      
-00002770: 2020 3a78 3a20 2020 2020 2020 2020 7c20    :x:         | 
-00002780: 2020 2020 2020 2020 2060 786d 6c60 2020           `xml`  
-00002790: 2020 2020 2020 2020 207c 2020 2020 2060           |     `
-000027a0: 786d 6c60 2020 2020 2020 7c20 4465 6669  xml`      | Defi
-000027b0: 6e65 7320 6f75 7470 7574 2064 6174 6120  nes output data 
-000027c0: 666f 726d 6174 2020 2020 2020 2020 2020  format          
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 2020 7c0a 7c20 606f 7574 7075 742f      |.| `output/
-00002850: 696e 6465 6e74 6020 2020 2020 2020 2020  indent`         
-00002860: 207c 2020 436f 6e66 6967 2020 7c20 2020   |  Config  |   
-00002870: 2020 2020 203a 783a 2020 2020 2020 2020       :x:        
-00002880: 207c 2020 2020 2020 2020 2069 6e74 6567   |         integ
-00002890: 6572 2020 2020 2020 2020 2020 7c20 2020  er          |   
-000028a0: 2020 606e 756c 6c60 2020 2020 207c 2044    `null`     | D
-000028b0: 6566 696e 6573 2069 6e64 656e 7420 6170  efines indent ap
-000028c0: 706c 6965 6420 696e 206f 7574 7075 7420  plied in output 
-000028d0: 6461 7461 2020 2020 2020 2020 2020 2020  data            
+000026e0: 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.|:-----------
+000026f0: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
+00002700: 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d  -----|:---------
+00002710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002730: 2d2d 2d2d 2d2d 2d7c 0a7c 2020 2020 2020  -------|.|      
+00002740: 2020 2020 2020 2020 7c20 602d 2d73 6571          | `--seq
+00002750: 7565 6e74 6961 6c6c 7960 207c 2070 726f  uentially` | pro
+00002760: 6365 7373 204d 696d 656f 2043 6f6e 6669  cess Mimeo Confi
+00002770: 6775 7261 7469 6f6e 7320 696e 2061 2073  gurations in a s
+00002780: 696e 676c 6520 7468 7265 6164 207c 0a0a  ingle thread |..
+00002790: 2323 2320 4d69 6d65 6f20 436f 6e66 6967  ### Mimeo Config
+000027a0: 7572 6174 696f 6e0a 0a4d 696d 656f 2063  uration..Mimeo c
+000027b0: 6f6e 6669 6775 7261 7469 6f6e 2069 7320  onfiguration is 
+000027c0: 6465 6669 6e65 6420 696e 2061 204a 534f  defined in a JSO
+000027d0: 4e20 6669 6c65 2075 7369 6e67 2069 6e74  N file using int
+000027e0: 6572 6e61 6c20 7365 7474 696e 6773 2061  ernal settings a
+000027f0: 6e64 2064 6174 6120 7465 6d70 6c61 7465  nd data template
+00002800: 732e 0a0a 7c20 4b65 7920 2020 2020 2020  s...| Key       
+00002810: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002820: 2020 4c65 7665 6c20 2020 7c20 2020 2020    Level   |     
+00002830: 2052 6571 7569 7265 6420 2020 2020 207c   Required      |
+00002840: 2020 2020 2053 7570 706f 7274 6564 2076       Supported v
+00002850: 616c 7565 7320 2020 2020 7c20 2020 2044  alues     |    D
+00002860: 6566 6175 6c74 2020 2020 207c 2044 6573  efault     | Des
+00002870: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
+00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002940: 2020 2020 2020 207c 0a7c 2060 6f75 7470         |.| `outp
-00002950: 7574 2f78 6d6c 5f64 6563 6c61 7261 7469  ut/xml_declarati
-00002960: 6f6e 6020 7c20 2043 6f6e 6669 6720 207c  on` |  Config  |
-00002970: 2020 2020 2020 2020 3a78 3a20 2020 2020          :x:     
-00002980: 2020 2020 7c20 2020 2020 2020 2020 626f      |         bo
-00002990: 6f6c 6561 6e20 2020 2020 2020 2020 207c  olean          |
-000029a0: 2020 2020 6066 616c 7365 6020 2020 2020      `false`     
-000029b0: 7c20 496e 6469 6361 7465 7320 7768 6574  | Indicates whet
-000029c0: 6865 7220 616e 2078 6d6c 2064 6563 6c61  her an xml decla
-000029d0: 7261 7469 6f6e 2073 686f 756c 6420 6265  ration should be
-000029e0: 2061 6464 6564 2074 6f20 6f75 7470 7574   added to output
-000029f0: 2064 6174 6120 2020 2020 2020 2020 2020   data           
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 2020 2020 2020 2020 2020 7c0a 7c20 606f            |.| `o
-00002a50: 7574 7075 742f 6469 7265 6374 6f72 795f  utput/directory_
-00002a60: 7061 7468 6020 207c 2020 436f 6e66 6967  path`  |  Config
-00002a70: 2020 7c20 2020 2020 2020 203a 783a 2020    |        :x:  
-00002a80: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00002a90: 2020 7374 7269 6e67 2020 2020 2020 2020    string        
-00002aa0: 2020 7c20 606d 696d 656f 2d6f 7574 7075    | `mimeo-outpu
-00002ab0: 7460 207c 2046 6f72 2060 6669 6c65 6020  t` | For `file` 
-00002ac0: 6469 7265 6374 696f 6e20 2d20 6465 6669  direction - defi
-00002ad0: 6e65 7320 616e 206f 7574 7075 7420 6469  nes an output di
-00002ae0: 7265 6374 6f72 7920 2020 2020 2020 2020  rectory         
+00002900: 2020 2020 207c 0a7c 3a2d 2d2d 2d2d 2d2d       |.|:-------
+00002910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002920: 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  --|:--------:|:-
+00002930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002940: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
+00002950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  ------------:|:-
+00002960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c2d  -------------:|-
+00002970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000029a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000029b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000029c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000029d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000029e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000029f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002a00: 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 606f 7574  --------|.| `out
+00002a10: 7075 7460 2020 2020 2020 2020 2020 2020  put`            
+00002a20: 2020 2020 207c 2020 436f 6e66 6967 2020       |  Config  
+00002a30: 7c20 2020 2020 2020 203a 783a 2020 2020  |        :x:    
+00002a40: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00002a50: 6f62 6a65 6374 2020 2020 2020 2020 2020  object          
+00002a60: 7c20 2020 2020 202d 2d2d 2020 2020 2020  |      ---      
+00002a70: 207c 2044 6566 696e 6573 206f 7574 7075   | Defines outpu
+00002a80: 7420 6465 7461 696c 7320 6f6e 2068 6f77  t details on how
+00002a90: 2069 7420 7769 6c6c 2062 6520 636f 6e73   it will be cons
+00002aa0: 756d 6564 2020 2020 2020 2020 2020 2020  umed            
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00002b50: 2060 6f75 7470 7574 2f66 696c 655f 6e61   `output/file_na
-00002b60: 6d65 6020 2020 2020 2020 7c20 2043 6f6e  me`       |  Con
-00002b70: 6669 6720 207c 2020 2020 2020 2020 3a78  fig  |        :x
-00002b80: 3a20 2020 2020 2020 2020 7c20 2020 2020  :         |     
-00002b90: 2020 2020 2073 7472 696e 6720 2020 2020       string     
-00002ba0: 2020 2020 207c 2060 6d69 6d65 6f2d 6f75       | `mimeo-ou
-00002bb0: 7470 7574 6020 7c20 466f 7220 6066 696c  tput` | For `fil
-00002bc0: 6560 2064 6972 6563 7469 6f6e 202d 2064  e` direction - d
-00002bd0: 6566 696e 6573 2061 6e20 6f75 7470 7574  efines an output
-00002be0: 2066 696c 6520 6e61 6d65 2020 2020 2020   file name      
+00002b00: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
+00002b10: 6f75 7470 7574 2f64 6972 6563 7469 6f6e  output/direction
+00002b20: 6020 2020 2020 2020 7c20 2043 6f6e 6669  `       |  Confi
+00002b30: 6720 207c 2020 2020 2020 2020 3a78 3a20  g  |        :x: 
+00002b40: 2020 2020 2020 2020 7c20 6066 696c 6560          | `file`
+00002b50: 2c20 6073 7464 6f75 7460 2c20 6068 7474  , `stdout`, `htt
+00002b60: 7060 207c 2020 2020 2060 6669 6c65 6020  p` |     `file` 
+00002b70: 2020 2020 7c20 4465 6669 6e65 7320 686f      | Defines ho
+00002b80: 7720 6f75 7470 7574 2077 696c 6c20 6265  w output will be
+00002b90: 2063 6f6e 7375 6d65 6420 2020 2020 2020   consumed       
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c50: 7c0a 7c20 606f 7574 7075 742f 6d65 7468  |.| `output/meth
-00002c60: 6f64 6020 2020 2020 2020 2020 207c 2020  od`          |  
-00002c70: 436f 6e66 6967 2020 7c20 2020 2020 2020  Config  |       
-00002c80: 203a 783a 2020 2020 2020 2020 207c 2020   :x:         |  
-00002c90: 2020 2020 6050 4f53 5460 2c20 6050 5554      `POST`, `PUT
-00002ca0: 6020 2020 2020 2020 7c20 2020 2020 6050  `       |     `P
-00002cb0: 4f53 5460 2020 2020 207c 2046 6f72 2060  OST`     | For `
-00002cc0: 6874 7470 6020 6469 7265 6374 696f 6e20  http` direction 
-00002cd0: 2d20 6465 6669 6e65 7320 6120 7265 7175  - defines a requ
-00002ce0: 6573 7420 6d65 7468 6f64 2020 2020 2020  est method      
+00002c00: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00002c10: 7c20 606f 7574 7075 742f 666f 726d 6174  | `output/format
+00002c20: 6020 2020 2020 2020 2020 207c 2020 436f  `          |  Co
+00002c30: 6e66 6967 2020 7c20 2020 2020 2020 203a  nfig  |        :
+00002c40: 783a 2020 2020 2020 2020 207c 2020 2020  x:         |    
+00002c50: 2020 6078 6d6c 602c 2060 6a73 6f6e 6020    `xml`, `json` 
+00002c60: 2020 2020 2020 7c20 2020 2020 6078 6d6c        |     `xml
+00002c70: 6020 2020 2020 207c 2044 6566 696e 6573  `      | Defines
+00002c80: 206f 7574 7075 7420 6461 7461 2066 6f72   output data for
+00002c90: 6d61 7420 2020 2020 2020 2020 2020 2020  mat             
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d50: 2020 207c 0a7c 2060 6f75 7470 7574 2f70     |.| `output/p
-00002d60: 726f 746f 636f 6c60 2020 2020 2020 2020  rotocol`        
-00002d70: 7c20 2043 6f6e 6669 6720 207c 2020 2020  |  Config  |    
-00002d80: 2020 2020 3a78 3a20 2020 2020 2020 2020      :x:         
-00002d90: 7c20 2020 2020 6068 7474 7060 2c20 6068  |     `http`, `h
-00002da0: 7474 7073 6020 2020 2020 207c 2020 2020  ttps`      |    
-00002db0: 2060 6874 7470 6020 2020 2020 7c20 466f   `http`     | Fo
-00002dc0: 7220 6068 7474 7060 2064 6972 6563 7469  r `http` directi
-00002dd0: 6f6e 202d 2064 6566 696e 6573 2061 2075  on - defines a u
-00002de0: 726c 2070 726f 746f 636f 6c20 2020 2020  rl protocol     
+00002d10: 207c 0a7c 2060 6f75 7470 7574 2f69 6e64   |.| `output/ind
+00002d20: 656e 7460 2020 2020 2020 2020 2020 7c20  ent`          | 
+00002d30: 2043 6f6e 6669 6720 207c 2020 2020 2020   Config  |      
+00002d40: 2020 3a78 3a20 2020 2020 2020 2020 7c20    :x:         | 
+00002d50: 2020 2020 2020 2020 696e 7465 6765 7220          integer 
+00002d60: 2020 2020 2020 2020 207c 2020 2020 2060           |     `
+00002d70: 6e75 6c6c 6020 2020 2020 7c20 4465 6669  null`     | Defi
+00002d80: 6e65 7320 696e 6465 6e74 2061 7070 6c69  nes indent appli
+00002d90: 6564 2069 6e20 6f75 7470 7574 2064 6174  ed in output dat
+00002da0: 6120 2020 2020 2020 2020 2020 2020 2020  a               
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e50: 2020 2020 2020 7c0a 7c20 606f 7574 7075        |.| `outpu
-00002e60: 742f 686f 7374 6020 2020 2020 2020 2020  t/host`         
-00002e70: 2020 207c 2020 436f 6e66 6967 2020 7c20     |  Config  | 
-00002e80: 3a68 6561 7679 5f63 6865 636b 5f6d 6172  :heavy_check_mar
-00002e90: 6b3a 207c 2020 2020 2020 2020 2020 7374  k: |          st
-00002ea0: 7269 6e67 2020 2020 2020 2020 2020 7c20  ring          | 
-00002eb0: 2020 2020 202d 2d2d 2020 2020 2020 207c       ---       |
-00002ec0: 2046 6f72 2060 6874 7470 6020 6469 7265   For `http` dire
-00002ed0: 6374 696f 6e20 2d20 6465 6669 6e65 7320  ction - defines 
-00002ee0: 6120 7572 6c20 686f 7374 2020 2020 2020  a url host      
+00002e10: 2020 2020 7c0a 7c20 606f 7574 7075 742f      |.| `output/
+00002e20: 786d 6c5f 6465 636c 6172 6174 696f 6e60  xml_declaration`
+00002e30: 207c 2020 436f 6e66 6967 2020 7c20 2020   |  Config  |   
+00002e40: 2020 2020 203a 783a 2020 2020 2020 2020       :x:        
+00002e50: 207c 2020 2020 2020 2020 2062 6f6f 6c65   |         boole
+00002e60: 616e 2020 2020 2020 2020 2020 7c20 2020  an          |   
+00002e70: 2060 6661 6c73 6560 2020 2020 207c 2049   `false`     | I
+00002e80: 6e64 6963 6174 6573 2077 6865 7468 6572  ndicates whether
+00002e90: 2061 6e20 786d 6c20 6465 636c 6172 6174   an xml declarat
+00002ea0: 696f 6e20 7368 6f75 6c64 2062 6520 6164  ion should be ad
+00002eb0: 6465 6420 746f 206f 7574 7075 7420 6461  ded to output da
+00002ec0: 7461 2020 2020 2020 2020 2020 2020 2020  ta              
+00002ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2020 2020 2020 2020 207c 0a7c 2060 6f75           |.| `ou
-00002f60: 7470 7574 2f70 6f72 7460 2020 2020 2020  tput/port`      
-00002f70: 2020 2020 2020 7c20 2043 6f6e 6669 6720        |  Config 
-00002f80: 207c 2020 2020 2020 2020 3a78 3a20 2020   |        :x:   
-00002f90: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00002fa0: 696e 7465 6765 7220 2020 2020 2020 2020  integer         
-00002fb0: 207c 2020 2020 2060 6e75 6c6c 6020 2020   |     `null`   
-00002fc0: 2020 7c20 466f 7220 6068 7474 7060 2064    | For `http` d
-00002fd0: 6972 6563 7469 6f6e 202d 2064 6566 696e  irection - defin
-00002fe0: 6573 2061 2075 726c 2070 6f72 7420 2863  es a url port (c
-00002ff0: 616e 2062 6520 656d 7074 7929 2020 2020  an be empty)    
+00002f10: 2020 2020 2020 207c 0a7c 2060 6f75 7470         |.| `outp
+00002f20: 7574 2f64 6972 6563 746f 7279 5f70 6174  ut/directory_pat
+00002f30: 6860 2020 7c20 2043 6f6e 6669 6720 207c  h`  |  Config  |
+00002f40: 2020 2020 2020 2020 3a78 3a20 2020 2020          :x:     
+00002f50: 2020 2020 7c20 2020 2020 2020 2020 2073      |          s
+00002f60: 7472 696e 6720 2020 2020 2020 2020 207c  tring          |
+00002f70: 2060 6d69 6d65 6f2d 6f75 7470 7574 6020   `mimeo-output` 
+00002f80: 7c20 466f 7220 6066 696c 6560 2064 6972  | For `file` dir
+00002f90: 6563 7469 6f6e 202d 2064 6566 696e 6573  ection - defines
+00002fa0: 2061 6e20 6f75 7470 7574 2064 6972 6563   an output direc
+00002fb0: 746f 7279 2020 2020 2020 2020 2020 2020  tory            
+00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00003060: 606f 7574 7075 742f 656e 6470 6f69 6e74  `output/endpoint
-00003070: 6020 2020 2020 2020 207c 2020 436f 6e66  `        |  Conf
-00003080: 6967 2020 7c20 3a68 6561 7679 5f63 6865  ig  | :heavy_che
-00003090: 636b 5f6d 6172 6b3a 207c 2020 2020 2020  ck_mark: |      
-000030a0: 2020 2020 7374 7269 6e67 2020 2020 2020      string      
-000030b0: 2020 2020 7c20 2020 2020 202d 2d2d 2020      |      ---  
-000030c0: 2020 2020 207c 2046 6f72 2060 6874 7470       | For `http
-000030d0: 6020 6469 7265 6374 696f 6e20 2d20 6465  ` direction - de
-000030e0: 6669 6e65 7320 6120 7572 6c20 656e 6470  fines a url endp
-000030f0: 6f69 6e74 2020 2020 2020 2020 2020 2020  oint            
+00003010: 2020 2020 2020 2020 2020 7c0a 7c20 606f            |.| `o
+00003020: 7574 7075 742f 6669 6c65 5f6e 616d 6560  utput/file_name`
+00003030: 2020 2020 2020 207c 2020 436f 6e66 6967         |  Config
+00003040: 2020 7c20 2020 2020 2020 203a 783a 2020    |        :x:  
+00003050: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00003060: 2020 7374 7269 6e67 2020 2020 2020 2020    string        
+00003070: 2020 7c20 606d 696d 656f 2d6f 7574 7075    | `mimeo-outpu
+00003080: 7460 207c 2046 6f72 2060 6669 6c65 6020  t` | For `file` 
+00003090: 6469 7265 6374 696f 6e20 2d20 6465 6669  direction - defi
+000030a0: 6e65 7320 616e 206f 7574 7075 7420 6669  nes an output fi
+000030b0: 6c65 206e 616d 6520 2020 2020 2020 2020  le name         
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003150: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00003160: 0a7c 2060 6f75 7470 7574 2f75 7365 726e  .| `output/usern
-00003170: 616d 6560 2020 2020 2020 2020 7c20 2043  ame`        |  C
-00003180: 6f6e 6669 6720 207c 203a 6865 6176 795f  onfig  | :heavy_
-00003190: 6368 6563 6b5f 6d61 726b 3a20 7c20 2020  check_mark: |   
-000031a0: 2020 2020 2020 2073 7472 696e 6720 2020         string   
-000031b0: 2020 2020 2020 207c 2020 2020 2020 2d2d         |      --
-000031c0: 2d20 2020 2020 2020 7c20 466f 7220 6068  -       | For `h
-000031d0: 7474 7060 2064 6972 6563 7469 6f6e 202d  ttp` direction -
-000031e0: 2064 6566 696e 6573 2061 2075 7365 726e   defines a usern
-000031f0: 616d 6520 2020 2020 2020 2020 2020 2020  ame             
+00003110: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00003120: 2060 6f75 7470 7574 2f6d 6574 686f 6460   `output/method`
+00003130: 2020 2020 2020 2020 2020 7c20 2043 6f6e            |  Con
+00003140: 6669 6720 207c 2020 2020 2020 2020 3a78  fig  |        :x
+00003150: 3a20 2020 2020 2020 2020 7c20 2020 2020  :         |     
+00003160: 2060 504f 5354 602c 2060 5055 5460 2020   `POST`, `PUT`  
+00003170: 2020 2020 207c 2020 2020 2060 504f 5354       |     `POST
+00003180: 6020 2020 2020 7c20 466f 7220 6068 7474  `     | For `htt
+00003190: 7060 2064 6972 6563 7469 6f6e 202d 2064  p` direction - d
+000031a0: 6566 696e 6573 2061 2072 6571 7565 7374  efines a request
+000031b0: 206d 6574 686f 6420 2020 2020 2020 2020   method         
+000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003260: 2020 7c0a 7c20 606f 7574 7075 742f 7061    |.| `output/pa
-00003270: 7373 776f 7264 6020 2020 2020 2020 207c  ssword`        |
-00003280: 2020 436f 6e66 6967 2020 7c20 3a68 6561    Config  | :hea
-00003290: 7679 5f63 6865 636b 5f6d 6172 6b3a 207c  vy_check_mark: |
-000032a0: 2020 2020 2020 2020 2020 7374 7269 6e67            string
-000032b0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000032c0: 202d 2d2d 2020 2020 2020 207c 2046 6f72   ---       | For
-000032d0: 2060 6874 7470 6020 6469 7265 6374 696f   `http` directio
-000032e0: 6e20 2d20 6465 6669 6e65 7320 6120 7061  n - defines a pa
-000032f0: 7373 776f 7264 2020 2020 2020 2020 2020  ssword          
+00003220: 7c0a 7c20 606f 7574 7075 742f 7072 6f74  |.| `output/prot
+00003230: 6f63 6f6c 6020 2020 2020 2020 207c 2020  ocol`        |  
+00003240: 436f 6e66 6967 2020 7c20 2020 2020 2020  Config  |       
+00003250: 203a 783a 2020 2020 2020 2020 207c 2020   :x:         |  
+00003260: 2020 2060 6874 7470 602c 2060 6874 7470     `http`, `http
+00003270: 7360 2020 2020 2020 7c20 2020 2020 6068  s`      |     `h
+00003280: 7474 7060 2020 2020 207c 2046 6f72 2060  ttp`     | For `
+00003290: 6874 7470 6020 6469 7265 6374 696f 6e20  http` direction 
+000032a0: 2d20 6465 6669 6e65 7320 6120 7572 6c20  - defines a url 
+000032b0: 7072 6f74 6f63 6f6c 2020 2020 2020 2020  protocol        
+000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003360: 2020 2020 207c 0a7c 2060 7661 7273 6020       |.| `vars` 
-00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003380: 2020 2020 2020 2020 2020 7c20 2043 6f6e            |  Con
-00003390: 6669 6720 207c 2020 2020 2020 2020 3a78  fig  |        :x
-000033a0: 3a20 2020 2020 2020 2020 7c20 2020 2020  :         |     
-000033b0: 2020 2020 206f 626a 6563 7420 2020 2020       object     
-000033c0: 2020 2020 207c 2020 2020 2020 2d2d 2d20       |      --- 
-000033d0: 2020 2020 2020 7c20 4465 6669 6e65 7320        | Defines 
-000033e0: 7661 7269 6162 6c65 7320 746f 2062 6520  variables to be 
-000033f0: 7573 6564 2069 6e20 6120 4d69 6d65 6f20  used in a Mimeo 
-00003400: 5465 6d70 6c61 7465 2028 7265 6164 206d  Template (read m
-00003410: 6f72 6520 696e 206e 6578 7420 7365 6374  ore in next sect
-00003420: 696f 6e29 2020 2020 2020 2020 2020 2020  ion)            
-00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 7c0a 7c20 605f 7465 6d70 6c61 7465 735f  |.| `_templates_
-00003480: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00003490: 2020 2020 207c 2020 436f 6e66 6967 2020       |  Config  
-000034a0: 7c20 3a68 6561 7679 5f63 6865 636b 5f6d  | :heavy_check_m
-000034b0: 6172 6b3a 207c 2020 2020 2020 2020 2020  ark: |          
-000034c0: 6172 7261 7920 2020 2020 2020 2020 2020  array           
-000034d0: 7c20 2020 2020 202d 2d2d 2020 2020 2020  |      ---      
-000034e0: 207c 2053 746f 7265 7320 7465 6d70 6c61   | Stores templa
-000034f0: 7465 7320 666f 7220 6461 7461 2067 656e  tes for data gen
-00003500: 6572 6174 696f 6e20 2020 2020 2020 2020  eration         
+00003320: 2020 207c 0a7c 2060 6f75 7470 7574 2f68     |.| `output/h
+00003330: 6f73 7460 2020 2020 2020 2020 2020 2020  ost`            
+00003340: 7c20 2043 6f6e 6669 6720 207c 203a 6865  |  Config  | :he
+00003350: 6176 795f 6368 6563 6b5f 6d61 726b 3a20  avy_check_mark: 
+00003360: 7c20 2020 2020 2020 2020 2073 7472 696e  |          strin
+00003370: 6720 2020 2020 2020 2020 207c 2020 2020  g          |    
+00003380: 2020 2d2d 2d20 2020 2020 2020 7c20 466f    ---       | Fo
+00003390: 7220 6068 7474 7060 2064 6972 6563 7469  r `http` directi
+000033a0: 6f6e 202d 2064 6566 696e 6573 2061 2075  on - defines a u
+000033b0: 726c 2068 6f73 7420 2020 2020 2020 2020  rl host         
+000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003420: 2020 2020 2020 7c0a 7c20 606f 7574 7075        |.| `outpu
+00003430: 742f 706f 7274 6020 2020 2020 2020 2020  t/port`         
+00003440: 2020 207c 2020 436f 6e66 6967 2020 7c20     |  Config  | 
+00003450: 2020 2020 2020 203a 783a 2020 2020 2020         :x:      
+00003460: 2020 207c 2020 2020 2020 2020 2069 6e74     |         int
+00003470: 6567 6572 2020 2020 2020 2020 2020 7c20  eger          | 
+00003480: 2020 2020 606e 756c 6c60 2020 2020 207c      `null`     |
+00003490: 2046 6f72 2060 6874 7470 6020 6469 7265   For `http` dire
+000034a0: 6374 696f 6e20 2d20 6465 6669 6e65 7320  ction - defines 
+000034b0: 6120 7572 6c20 706f 7274 2028 6361 6e20  a url port (can 
+000034c0: 6265 2065 6d70 7479 2920 2020 2020 2020  be empty)       
+000034d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
-00003580: 636f 756e 7460 2020 2020 2020 2020 2020  count`          
-00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035a0: 7c20 5465 6d70 6c61 7465 207c 203a 6865  | Template | :he
-000035b0: 6176 795f 6368 6563 6b5f 6d61 726b 3a20  avy_check_mark: 
-000035c0: 7c20 2020 2020 2020 2020 696e 7465 6765  |         intege
-000035d0: 7220 2020 2020 2020 2020 207c 2020 2020  r          |    
-000035e0: 2020 2d2d 2d20 2020 2020 2020 7c20 496e    ---       | In
-000035f0: 6469 6361 7465 7320 6e75 6d62 6572 206f  dicates number o
-00003600: 6620 636f 7069 6573 2020 2020 2020 2020  f copies        
+00003520: 2020 2020 2020 2020 207c 0a7c 2060 6f75           |.| `ou
+00003530: 7470 7574 2f65 6e64 706f 696e 7460 2020  tput/endpoint`  
+00003540: 2020 2020 2020 7c20 2043 6f6e 6669 6720        |  Config 
+00003550: 207c 203a 6865 6176 795f 6368 6563 6b5f   | :heavy_check_
+00003560: 6d61 726b 3a20 7c20 2020 2020 2020 2020  mark: |         
+00003570: 2073 7472 696e 6720 2020 2020 2020 2020   string         
+00003580: 207c 2020 2020 2020 2d2d 2d20 2020 2020   |      ---     
+00003590: 2020 7c20 466f 7220 6068 7474 7060 2064    | For `http` d
+000035a0: 6972 6563 7469 6f6e 202d 2064 6566 696e  irection - defin
+000035b0: 6573 2061 2075 726c 2065 6e64 706f 696e  es a url endpoin
+000035c0: 7420 2020 2020 2020 2020 2020 2020 2020  t               
+000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003680: 2020 2020 2020 7c0a 7c20 606d 6f64 656c        |.| `model
-00003690: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-000036a0: 2020 2020 2020 2020 2020 207c 2054 656d             | Tem
-000036b0: 706c 6174 6520 7c20 3a68 6561 7679 5f63  plate | :heavy_c
-000036c0: 6865 636b 5f6d 6172 6b3a 207c 2020 2020  heck_mark: |    
-000036d0: 2020 2020 2020 6f62 6a65 6374 2020 2020        object    
-000036e0: 2020 2020 2020 7c20 2020 2020 202d 2d2d        |      ---
-000036f0: 2020 2020 2020 207c 2044 6566 696e 6573         | Defines
-00003700: 2064 6174 6120 7465 6d70 6c61 7465 2074   data template t
-00003710: 6f20 6265 2063 6f70 6965 6420 2020 2020  o be copied     
-00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003790: 207c 0a7c 2060 636f 6e74 6578 7460 2020   |.| `context`  
-000037a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037b0: 2020 2020 2020 7c20 204d 6f64 656c 2020        |  Model  
-000037c0: 207c 2020 2020 2020 2020 3a78 3a20 2020   |        :x:   
-000037d0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000037e0: 206f 626a 6563 7420 2020 2020 2020 2020   object         
-000037f0: 207c 2020 2020 2020 2d2d 2d20 2020 2020   |      ---     
-00003800: 2020 7c20 4465 6669 6e65 7320 6120 636f    | Defines a co
-00003810: 6e74 6578 7420 6e61 6d65 2074 6861 7420  ntext name that 
-00003820: 6973 2069 6e74 6572 6e61 6c6c 7920 7573  is internally us
-00003830: 6564 2065 2e67 2e20 7573 696e 6720 6063  ed e.g. using `c
-00003840: 7572 725f 6974 6572 2829 6020 616e 6420  urr_iter()` and 
-00003850: 6067 6574 5f6b 6579 2829 6020 6d69 6d65  `get_key()` mime
-00003860: 6f20 7574 696c 7320 2862 7920 6465 6661  o utils (by defa
-00003870: 756c 7420 6d6f 6465 6c20 6e61 6d65 2069  ult model name i
-00003880: 7320 7573 6564 2061 7320 7468 6520 636f  s used as the co
-00003890: 6e74 6578 7420 6e61 6d65 2920 7c0a 0a23  ntext name) |..#
-000038a0: 2323 2320 4d69 6d65 6f20 456e 7669 726f  ### Mimeo Enviro
-000038b0: 6e6d 656e 740a 0a54 6f20 6d61 6b65 2060  nment..To make `
-000038c0: 6874 7470 6020 6f75 7470 7574 2064 6972  http` output dir
-000038d0: 6563 746f 7279 2065 6173 6965 7220 746f  ectory easier to
-000038e0: 2075 7365 2c20 6d69 6d65 6f20 616c 6c6f   use, mimeo allo
-000038f0: 7773 2079 6f75 2074 6f20 636f 6e66 6967  ws you to config
-00003900: 7572 6520 4d69 6d65 6f20 456e 7669 726f  ure Mimeo Enviro
-00003910: 6e6d 656e 7473 2e0a 5468 6579 2061 7265  nments..They are
-00003920: 2063 6f6e 6669 6775 7265 6420 696e 2061   configured in a
-00003930: 204a 534f 4e20 6669 6c65 2028 6279 2064   JSON file (by d
-00003940: 6566 6175 6c74 3a20 6d69 6d65 6f2e 656e  efault: mimeo.en
-00003950: 7673 2e6a 736f 6e29 2061 6e64 2073 7570  vs.json) and sup
-00003960: 706f 7274 2074 6865 2066 6f6c 6c6f 7769  port the followi
-00003970: 6e67 206f 7574 7075 7420 6465 7461 696c  ng output detail
-00003980: 733a 0a2d 2060 7072 6f74 6f63 6f6c 600a  s:.- `protocol`.
-00003990: 2d20 6068 6f73 7460 0a2d 2060 706f 7274  - `host`.- `port
-000039a0: 600a 2d20 6075 7365 726e 616d 6560 0a2d  `.- `username`.-
-000039b0: 2060 7061 7373 776f 7264 600a 0a45 7861   `password`..Exa
-000039c0: 6d70 6c65 0a60 6060 6a73 6f6e 0a7b 0a20  mple.```json.{. 
-000039d0: 2020 2022 6c6f 6361 6c22 3a20 7b0a 2020     "local": {.  
-000039e0: 2020 2020 2020 2268 6f73 7422 3a20 226c        "host": "l
-000039f0: 6f63 616c 686f 7374 222c 0a20 2020 2020  ocalhost",.     
-00003a00: 2020 2022 706f 7274 223a 2038 3030 302c     "port": 8000,
-00003a10: 0a20 2020 2020 2020 2022 7573 6572 6e61  .        "userna
-00003a20: 6d65 223a 2022 6164 6d69 6e22 2c0a 2020  me": "admin",.  
-00003a30: 2020 2020 2020 2270 6173 7377 6f72 6422        "password"
-00003a40: 3a20 2261 646d 696e 220a 2020 2020 7d2c  : "admin".    },
-00003a50: 0a20 2020 2022 6465 7622 3a20 7b0a 2020  .    "dev": {.  
-00003a60: 2020 2020 2020 2270 726f 746f 636f 6c22        "protocol"
-00003a70: 3a20 2268 7474 7073 222c 0a20 2020 2020  : "https",.     
-00003a80: 2020 2022 686f 7374 223a 2022 3131 2e31     "host": "11.1
-00003a90: 3131 2e31 312e 3131 3122 2c0a 2020 2020  11.11.111",.    
-00003aa0: 2020 2020 2270 6f72 7422 3a20 3830 3030      "port": 8000
-00003ab0: 2c0a 2020 2020 2020 2020 2275 7365 726e  ,.        "usern
-00003ac0: 616d 6522 3a20 2273 6f6d 652d 7573 6572  ame": "some-user
-00003ad0: 222c 0a20 2020 2020 2020 2022 7061 7373  ",.        "pass
-00003ae0: 776f 7264 223a 2022 736f 6d65 2d70 6173  word": "some-pas
-00003af0: 7377 6f72 6422 0a20 2020 207d 0a7d 0a60  sword".    }.}.`
-00003b00: 6060 0a0a 546f 2075 7365 2061 2073 7065  ``..To use a spe
-00003b10: 6369 6669 6320 4d69 6d65 6f20 456e 7669  cific Mimeo Envi
-00003b20: 726f 6e6d 656e 7420 796f 7520 6361 6e20  ronment you can 
-00003b30: 7573 6520 7468 6520 666f 6c6c 6f77 696e  use the followin
-00003b40: 6720 636f 6d6d 616e 6473 3a0a 6060 6073  g commands:.```s
-00003b50: 680a 6d69 6d65 6f20 536f 6d65 456e 7469  h.mimeo SomeEnti
-00003b60: 7479 2d63 6f6e 6669 672e 6a73 6f6e 202d  ty-config.json -
-00003b70: 6520 6465 760a 6d69 6d65 6f20 536f 6d65  e dev.mimeo Some
-00003b80: 456e 7469 7479 2d63 6f6e 6669 672e 6a73  Entity-config.js
-00003b90: 6f6e 202d 6520 6465 7620 2d2d 6874 7470  on -e dev --http
-00003ba0: 2d65 6e76 732d 6669 6c65 2065 6e76 6972  -envs-file envir
-00003bb0: 6f6e 6d65 6e74 732e 6a73 6f6e 0a60 6060  onments.json.```
-00003bc0: 0a0a 2323 2323 204d 696d 656f 2056 6172  ..#### Mimeo Var
-00003bd0: 730a 0a4d 696d 656f 2061 6c6c 6f77 7320  s..Mimeo allows 
-00003be0: 796f 7520 746f 2064 6566 696e 6520 6120  you to define a 
-00003bf0: 6c69 7374 206f 6620 7661 7269 6162 6c65  list of variable
-00003c00: 732e 0a59 6f75 2063 616e 2075 7365 2074  s..You can use t
-00003c10: 6865 6d20 696e 2079 6f75 7220 4d69 6d65  hem in your Mime
-00003c20: 6f20 436f 6e66 6967 2062 7920 7772 6170  o Config by wrap
-00003c30: 7069 6e67 2074 6865 6d20 696e 2063 7572  ping them in cur
-00003c40: 6c79 2062 7261 636b 6574 7320 5b60 7b56  ly brackets [`{V
-00003c50: 4152 4941 424c 457d 605d 2e0a 0a54 6865  ARIABLE}`]...The
-00003c60: 7265 2061 7265 206f 6e6c 7920 3220 7275  re are only 2 ru
-00003c70: 6c65 7320 666f 7220 7661 7269 6162 6c65  les for variable
-00003c80: 206e 616d 6573 3a0a 2d20 5661 7269 6162   names:.- Variab
-00003c90: 6c65 206e 616d 6520 6361 6e20 696e 636c  le name can incl
-00003ca0: 7564 6520 7570 7065 722d 6361 7365 6420  ude upper-cased 
-00003cb0: 6c65 7474 6572 7320 5c5b 6041 2d5a 605c  letters \[`A-Z`\
-00003cc0: 5d2c 2075 6e64 6572 7363 6f72 6520 5c5b  ], underscore \[
-00003cd0: 605f 605c 5d20 616e 6420 6469 6769 7473  `_`\] and digits
-00003ce0: 205c 7b60 302d 3960 5c7d 206f 6e6c 790a   \{`0-9`\} only.
-00003cf0: 2d20 5661 7269 6162 6c65 206e 616d 6520  - Variable name 
-00003d00: 6d75 7374 2073 7461 7274 2077 6974 6820  must start with 
-00003d10: 6120 6c65 7474 6572 0a0a 5661 7269 6162  a letter..Variab
-00003d20: 6c65 2063 616e 2062 6520 6465 6669 6e65  le can be define
-00003d30: 6420 7769 7468 3a0a 2d20 616e 7920 6174  d with:.- any at
-00003d40: 6f6d 6963 2076 616c 7565 0a2d 2061 6e79  omic value.- any
-00003d50: 206f 7468 6572 2076 6172 6961 626c 6520   other variable 
-00003d60: 6465 6669 6e65 640a 2d20 616e 7920 4d69  defined.- any Mi
-00003d70: 6d65 6f20 5574 696c 0a0a 596f 7520 6361  meo Util..You ca
-00003d80: 6e20 7573 6520 4d69 6d65 6f20 5661 7273  n use Mimeo Vars
-00003d90: 2061 7320 7061 7274 6961 6c20 7661 6c75   as partial valu
-00003da0: 6573 2028 756e 6c65 7373 2074 6865 7920  es (unless they 
-00003db0: 6172 6520 6465 6669 6e65 6420 6173 204d  are defined as M
-00003dc0: 696d 656f 2055 7469 6c73 292e 0a0a 4578  imeo Utils)...Ex
-00003dd0: 616d 706c 653a 0a60 6060 6a73 6f6e 0a7b  ample:.```json.{
-00003de0: 0a20 2022 7661 7273 223a 207b 0a20 2020  .  "vars": {.   
-00003df0: 2022 4355 5354 4f4d 5f56 4152 5f31 223a   "CUSTOM_VAR_1":
-00003e00: 2022 6375 7374 6f6d 2d76 616c 7565 2d31   "custom-value-1
-00003e10: 222c 0a20 2020 2022 4355 5354 4f4d 5f56  ",.    "CUSTOM_V
-00003e20: 4152 5f32 223a 2031 2c0a 2020 2020 2243  AR_2": 1,.    "C
-00003e30: 5553 544f 4d5f 5641 525f 3322 3a20 7472  USTOM_VAR_3": tr
-00003e40: 7565 2c0a 2020 2020 2243 5553 544f 4d5f  ue,.    "CUSTOM_
-00003e50: 5641 525f 3422 3a20 227b 4355 5354 4f4d  VAR_4": "{CUSTOM
-00003e60: 5f56 4152 5f32 7d22 2c0a 2020 2020 2243  _VAR_2}",.    "C
-00003e70: 5553 544f 4d5f 5641 525f 3522 3a20 227b  USTOM_VAR_5": "{
-00003e80: 6175 746f 5f69 6e63 7265 6d65 6e74 7d22  auto_increment}"
-00003e90: 2c0a 2020 2020 2243 5553 544f 4d5f 5641  ,.    "CUSTOM_VA
-00003ea0: 525f 3622 3a20 7b0a 2020 2020 2020 225f  R_6": {.      "_
-00003eb0: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
-00003ec0: 2020 2020 2020 2022 5f6e 616d 6522 3a20         "_name": 
-00003ed0: 2272 616e 646f 6d5f 696e 7422 2c0a 2020  "random_int",.  
-00003ee0: 2020 2020 2020 226c 696d 6974 223a 2039        "limit": 9
-00003ef0: 390a 2020 2020 2020 7d0a 2020 2020 7d0a  9.      }.    }.
-00003f00: 2020 7d2c 0a20 2022 5f74 656d 706c 6174    },.  "_templat
-00003f10: 6573 5f22 3a20 5b0a 2020 2020 7b0a 2020  es_": [.    {.  
-00003f20: 2020 2020 2263 6f75 6e74 223a 2035 2c0a      "count": 5,.
-00003f30: 2020 2020 2020 226d 6f64 656c 223a 207b        "model": {
-00003f40: 0a20 2020 2020 2020 2022 536f 6d65 456e  .        "SomeEn
-00003f50: 7469 7479 223a 207b 0a20 2020 2020 2020  tity": {.       
-00003f60: 2020 2022 4368 696c 644e 6f64 6531 223a     "ChildNode1":
-00003f70: 2022 7b43 5553 544f 4d5f 5641 525f 317d   "{CUSTOM_VAR_1}
-00003f80: 222c 0a20 2020 2020 2020 2020 2022 4368  ",.          "Ch
-00003f90: 696c 644e 6f64 6532 223a 2022 7b43 5553  ildNode2": "{CUS
-00003fa0: 544f 4d5f 5641 525f 327d 222c 0a20 2020  TOM_VAR_2}",.   
-00003fb0: 2020 2020 2020 2022 4368 696c 644e 6f64         "ChildNod
-00003fc0: 6533 223a 2022 7b43 5553 544f 4d5f 5641  e3": "{CUSTOM_VA
-00003fd0: 525f 337d 222c 0a20 2020 2020 2020 2020  R_3}",.         
-00003fe0: 2022 4368 696c 644e 6f64 6534 223a 2022   "ChildNode4": "
-00003ff0: 7b43 5553 544f 4d5f 5641 525f 347d 222c  {CUSTOM_VAR_4}",
-00004000: 0a20 2020 2020 2020 2020 2022 4368 696c  .          "Chil
-00004010: 644e 6f64 6535 223a 2022 7b43 5553 544f  dNode5": "{CUSTO
-00004020: 4d5f 5641 525f 357d 222c 0a20 2020 2020  M_VAR_5}",.     
-00004030: 2020 2020 2022 4368 696c 644e 6f64 6536       "ChildNode6
-00004040: 223a 2022 7b43 5553 544f 4d5f 5641 525f  ": "{CUSTOM_VAR_
-00004050: 367d 222c 0a20 2020 2020 2020 2020 2022  6}",.          "
-00004060: 4368 696c 644e 6f64 6537 223a 2022 7b43  ChildNode7": "{C
-00004070: 5553 544f 4d5f 5641 525f 317d 2d77 6974  USTOM_VAR_1}-wit
-00004080: 682d 7375 6666 6978 220a 2020 2020 2020  h-suffix".      
-00004090: 2020 7d0a 2020 2020 2020 7d0a 2020 2020    }.      }.    
-000040a0: 7d0a 2020 5d0a 7d0a 6060 600a 0a23 2323  }.  ].}.```..###
-000040b0: 2320 4d69 6d65 6f20 5370 6563 6961 6c20  # Mimeo Special 
-000040c0: 4669 656c 6473 0a0a 496e 204d 696d 656f  Fields..In Mimeo
-000040d0: 2054 656d 706c 6174 6520 796f 7520 6361   Template you ca
-000040e0: 6e20 7573 6520 736f 2d63 616c 6c65 6420  n use so-called 
-000040f0: 5f73 7065 6369 616c 2066 6965 6c64 735f  _special fields_
-00004100: 2e0a 4576 6572 7920 6669 656c 6420 696e  ..Every field in
-00004110: 2061 2074 656d 706c 6174 6520 6361 6e20   a template can 
-00004120: 6265 2073 746f 7265 6420 696e 206d 656d  be stored in mem
-00004130: 6f72 7920 285f 7072 6f76 6964 6564 5f29  ory (_provided_)
-00004140: 2061 6e64 2075 7365 6420 6c61 7465 7220   and used later 
-00004150: 6173 2061 2076 616c 7565 206f 6620 6f74  as a value of ot
-00004160: 6865 7220 6669 656c 6473 2028 5f69 6e6a  her fields (_inj
-00004170: 6563 7465 645f 292e 0a54 6f20 7072 6f76  ected_)..To prov
-00004180: 6964 6520 6120 7370 6563 6961 6c20 6669  ide a special fi
-00004190: 656c 642c 2077 7261 7020 6974 7320 6e61  eld, wrap its na
-000041a0: 6d65 2077 6974 6820 636f 6c6f 6e73 3a20  me with colons: 
-000041b0: 5b60 3a53 6f6d 6546 6965 6c64 3a60 5d2e  [`:SomeField:`].
-000041c0: 2054 6f20 696e 6a65 6374 2c20 7573 6520   To inject, use 
-000041d0: 6164 6469 7469 6f6e 616c 6c79 2063 7572  additionally cur
-000041e0: 6c79 2062 7261 6365 7320 746f 0a6c 6574  ly braces to.let
-000041f0: 2069 6e74 6572 7072 6574 6572 206b 6e6f   interpreter kno
-00004200: 7720 6974 2073 686f 756c 6420 6265 2072  w it should be r
-00004210: 656e 6465 7265 6420 5b60 7b3a 536f 6d65  endered [`{:Some
-00004220: 4669 656c 643a 7d60 5d2e 0a54 6865 7920  Field:}`]..They 
-00004230: 6361 6e20 6265 2069 6e6a 6563 7465 6420  can be injected 
-00004240: 6173 2070 6172 7469 616c 2076 616c 7565  as partial value
-00004250: 732c 2073 696d 696c 6172 6c79 2074 6f20  s, similarly to 
-00004260: 4d69 6d65 6f20 5661 7273 2e0a 0a45 7861  Mimeo Vars...Exa
-00004270: 6d70 6c65 0a60 6060 6a73 6f6e 0a7b 0a20  mple.```json.{. 
-00004280: 2022 5f74 656d 706c 6174 6573 5f22 3a20   "_templates_": 
-00004290: 5b0a 2020 2020 7b0a 2020 2020 2020 2263  [.    {.      "c
-000042a0: 6f75 6e74 223a 2035 2c0a 2020 2020 2020  ount": 5,.      
-000042b0: 226d 6f64 656c 223a 207b 0a20 2020 2020  "model": {.     
-000042c0: 2020 2022 536f 6d65 456e 7469 7479 223a     "SomeEntity":
-000042d0: 207b 0a20 2020 2020 2020 2020 2022 3a43   {.          ":C
-000042e0: 6869 6c64 4e6f 6465 313a 223a 2022 6375  hildNode1:": "cu
-000042f0: 7374 6f6d 2d76 616c 7565 222c 0a20 2020  stom-value",.   
-00004300: 2020 2020 2020 2022 4368 696c 644e 6f64         "ChildNod
-00004310: 6532 223a 2022 7b3a 4368 696c 644e 6f64  e2": "{:ChildNod
-00004320: 6531 3a7d 222c 0a20 2020 2020 2020 2020  e1:}",.         
-00004330: 2022 4368 696c 644e 6f64 6533 223a 2022   "ChildNode3": "
-00004340: 7b3a 4368 696c 644e 6f64 6531 3a7d 2d77  {:ChildNode1:}-w
-00004350: 6974 682d 7375 6666 6978 220a 2020 2020  ith-suffix".    
-00004360: 2020 2020 7d0a 2020 2020 2020 7d0a 2020      }.      }.  
-00004370: 2020 7d0a 2020 5d0a 7d0a 6060 600a 0a23    }.  ].}.```..#
-00004380: 2323 2320 4d69 6d65 6f20 5574 696c 730a  ### Mimeo Utils.
-00004390: 0a59 6f75 2063 616e 2075 7365 2073 6576  .You can use sev
-000043a0: 6572 616c 2070 7265 6465 6669 6e65 6420  eral predefined 
-000043b0: 6675 6e63 7469 6f6e 7320 746f 2067 656e  functions to gen
-000043c0: 6572 6174 6520 6461 7461 2e20 5468 6579  erate data. They
-000043d0: 2063 616e 2062 6520 7573 6564 2069 6e20   can be used in 
-000043e0: 6120 5f72 6177 5f20 666f 726d 6174 206f  a _raw_ format o
-000043f0: 7220 5f70 6172 616d 6574 7269 7a65 645f  r _parametrized_
-00004400: 2e0a 0a23 2323 2323 2052 616e 646f 6d20  ...##### Random 
-00004410: 5374 7269 6e67 0a0a 4765 6e65 7261 7465  String..Generate
-00004420: 7320 6120 7261 6e64 6f6d 2073 7472 696e  s a random strin
-00004430: 6720 7661 6c75 652e 0a0a 7c20 5061 7261  g value...| Para
-00004440: 6d65 7465 7220 7c20 5375 7070 6f72 7465  meter | Supporte
-00004450: 6420 7661 6c75 6573 207c 2044 6566 6175  d values | Defau
-00004460: 6c74 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d  lt |.|:---------
-00004470: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|:-------------
-00004480: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d3a 7c0a  ---:|:-------:|.
-00004490: 7c20 206c 656e 6774 6820 2020 7c20 2020  |  length   |   
-000044a0: 2020 2060 696e 7460 2020 2020 2020 207c     `int`       |
-000044b0: 2020 6032 3060 2020 207c 0a0a 2323 2323    `20`   |..####
-000044c0: 2323 2052 6177 0a0a 5573 6573 2074 6865  ## Raw..Uses the
-000044d0: 2064 6566 6175 6c74 206c 656e 6774 683a   default length:
-000044e0: 2032 3020 6368 6172 6163 7465 7273 2e0a   20 characters..
-000044f0: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7261  .```json.{.  "ra
-00004500: 6e64 6f6d 7374 7269 6e67 223a 2022 7b72  ndomstring": "{r
-00004510: 616e 646f 6d5f 7374 727d 220a 7d0a 6060  andom_str}".}.``
-00004520: 600a 0a23 2323 2323 2320 5061 7261 6d65  `..###### Parame
-00004530: 7472 697a 6564 0a0a 5573 6573 2074 6865  trized..Uses the
-00004540: 2063 7573 746f 6d69 7a65 6420 6c65 6e67   customized leng
-00004550: 7468 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20  th...```json.{. 
-00004560: 2022 7261 6e64 6f6d 7374 7269 6e67 223a   "randomstring":
-00004570: 207b 0a20 2020 2022 5f6d 696d 656f 5f75   {.    "_mimeo_u
-00004580: 7469 6c22 3a20 7b0a 2020 2020 2020 225f  til": {.      "_
-00004590: 6e61 6d65 223a 2022 7261 6e64 6f6d 5f73  name": "random_s
-000045a0: 7472 222c 0a20 2020 2020 2022 6c65 6e67  tr",.      "leng
-000045b0: 7468 223a 2035 0a20 2020 207d 0a20 207d  th": 5.    }.  }
-000045c0: 0a7d 0a60 6060 0a0a 2323 2323 2320 5261  .}.```..##### Ra
-000045d0: 6e64 6f6d 2049 6e74 6567 6572 0a0a 4765  ndom Integer..Ge
-000045e0: 6e65 7261 7465 7320 6120 7261 6e64 6f6d  nerates a random
-000045f0: 2069 6e74 6567 6572 2076 616c 7565 2062   integer value b
-00004600: 6574 7765 656e 2060 7374 6172 7460 2061  etween `start` a
-00004610: 6e64 2060 6c69 6d69 7460 2070 6172 616d  nd `limit` param
-00004620: 6574 6572 7320 2869 6e63 6c75 7369 7665  eters (inclusive
-00004630: 292e 0a0a 7c20 5061 7261 6d65 7465 7220  )...| Parameter 
-00004640: 7c20 5375 7070 6f72 7465 6420 7661 6c75  | Supported valu
-00004650: 6573 207c 2044 6566 6175 6c74 207c 0a7c  es | Default |.|
-00004660: 3a2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d  :---------:|:---
-00004670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a  -------------:|:
-00004680: 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2020 7374  -------:|.|   st
-00004690: 6172 7420 2020 7c20 2020 2020 2060 696e  art   |      `in
-000046a0: 7460 2020 2020 2020 207c 2020 2060 3160  t`       |   `1`
-000046b0: 2020 207c 0a7c 2020 206c 696d 6974 2020     |.|   limit  
-000046c0: 207c 2020 2020 2020 6069 6e74 6020 2020   |      `int`   
-000046d0: 2020 2020 7c20 2060 3130 3060 2020 7c0a      |  `100`  |.
-000046e0: 0a23 2323 2323 2320 5261 770a 0a55 7365  .###### Raw..Use
-000046f0: 7320 7468 6520 6465 6661 756c 7420 7374  s the default st
-00004700: 6172 7420 2831 2920 616e 6420 6c69 6d69  art (1) and limi
-00004710: 7420 2831 3030 2920 7661 6c75 6573 2e0a  t (100) values..
-00004720: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7261  .```json.{.  "ra
-00004730: 6e64 6f6d 696e 7465 6765 7222 3a20 227b  ndominteger": "{
-00004740: 7261 6e64 6f6d 5f69 6e74 7d22 0a7d 0a60  random_int}".}.`
-00004750: 6060 0a0a 2323 2323 2323 2050 6172 616d  ``..###### Param
-00004760: 6574 7269 7a65 640a 0a55 7365 7320 7468  etrized..Uses th
-00004770: 6520 6375 7374 6f6d 697a 6564 206c 696d  e customized lim
-00004780: 6974 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20  it...```json.{. 
-00004790: 2022 7261 6e64 6f6d 696e 7465 6765 7231   "randominteger1
-000047a0: 223a 207b 0a20 2020 2022 5f6d 696d 656f  ": {.    "_mimeo
-000047b0: 5f75 7469 6c22 3a20 7b0a 2020 2020 2020  _util": {.      
-000047c0: 225f 6e61 6d65 223a 2022 7261 6e64 6f6d  "_name": "random
-000047d0: 5f69 6e74 222c 0a20 2020 2020 2022 7374  _int",.      "st
-000047e0: 6172 7422 3a20 300a 2020 2020 7d0a 2020  art": 0.    }.  
-000047f0: 7d2c 0a20 2022 7261 6e64 6f6d 696e 7465  },.  "randominte
-00004800: 6765 7232 223a 207b 0a20 2020 2022 5f6d  ger2": {.    "_m
-00004810: 696d 656f 5f75 7469 6c22 3a20 7b0a 2020  imeo_util": {.  
-00004820: 2020 2020 225f 6e61 6d65 223a 2022 7261      "_name": "ra
-00004830: 6e64 6f6d 5f69 6e74 222c 0a20 2020 2020  ndom_int",.     
-00004840: 2022 6c69 6d69 7422 3a20 350a 2020 2020   "limit": 5.    
-00004850: 7d0a 2020 7d2c 0a20 2022 7261 6e64 6f6d  }.  },.  "random
-00004860: 696e 7465 6765 7233 223a 207b 0a20 2020  integer3": {.   
-00004870: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
-00004880: 7b0a 2020 2020 2020 225f 6e61 6d65 223a  {.      "_name":
-00004890: 2022 7261 6e64 6f6d 5f69 6e74 222c 0a20   "random_int",. 
-000048a0: 2020 2020 2022 7374 6172 7422 3a20 302c       "start": 0,
-000048b0: 0a20 2020 2020 2022 6c69 6d69 7422 3a20  .      "limit": 
-000048c0: 350a 2020 2020 7d0a 2020 7d0a 7d0a 6060  5.    }.  }.}.``
-000048d0: 600a 0a23 2323 2323 2052 616e 646f 6d20  `..##### Random 
-000048e0: 4974 656d 0a0a 4765 6e65 7261 7465 7320  Item..Generates 
-000048f0: 6120 7261 6e64 6f6d 2076 616c 7565 2066  a random value f
-00004900: 726f 6d20 6974 656d 7320 7072 6f76 6964  rom items provid
-00004910: 6564 2e20 200a 4e4f 5449 4345 3a20 5468  ed.  .NOTICE: Th
-00004920: 6520 7261 7720 666f 726d 206f 6620 7468  e raw form of th
-00004930: 6973 204d 696d 656f 2055 7469 6c20 7769  is Mimeo Util wi
-00004940: 6c6c 2067 656e 6572 6174 6520 6120 626c  ll generate a bl
-00004950: 616e 6b20 7374 7269 6e67 2076 616c 7565  ank string value
-00004960: 2028 6173 2073 616d 6520 6173 206e 6f20   (as same as no 
-00004970: 6974 656d 7320 7061 7261 6d65 7472 697a  items parametriz
-00004980: 6564 292e 0a0a 7c20 5061 7261 6d65 7465  ed)...| Paramete
-00004990: 7220 7c20 5375 7070 6f72 7465 6420 7661  r | Supported va
-000049a0: 6c75 6573 207c 2044 6566 6175 6c74 207c  lues | Default |
-000049b0: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  .|:---------:|:-
-000049c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
-000049d0: 7c3a 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2020  |:-------:|.|   
-000049e0: 6974 656d 7320 2020 7c20 2020 2020 2060  items   |      `
-000049f0: 6c69 7374 6020 2020 2020 207c 2060 5b22  list`      | `["
-00004a00: 225d 6020 207c 0a0a 2323 2323 2323 2050  "]`  |..###### P
-00004a10: 6172 616d 6574 7269 7a65 640a 0a60 6060  arametrized..```
-00004a20: 6a73 6f6e 0a7b 0a20 2022 7261 6e64 6f6d  json.{.  "random
-00004a30: 223a 207b 0a20 2020 2022 5f6d 696d 656f  ": {.    "_mimeo
-00004a40: 5f75 7469 6c22 3a20 7b0a 2020 2020 2020  _util": {.      
-00004a50: 225f 6e61 6d65 223a 2022 7261 6e64 6f6d  "_name": "random
-00004a60: 5f69 7465 6d22 2c0a 2020 2020 2020 2269  _item",.      "i
-00004a70: 7465 6d73 223a 205b 2276 616c 7565 222c  tems": ["value",
-00004a80: 2031 2c20 7472 7565 5d0a 2020 2020 7d0a   1, true].    }.
-00004a90: 2020 7d0a 7d0a 6060 600a 0a23 2323 2323    }.}.```..#####
-00004aa0: 2044 6174 650a 0a47 656e 6572 6174 6573   Date..Generates
-00004ab0: 2061 2064 6174 6520 7661 6c75 6520 696e   a date value in
-00004ac0: 2066 6f72 6d61 7420 6059 5959 592d 4d4d   format `YYYY-MM
-00004ad0: 2d44 4460 2e0a 0a7c 2050 6172 616d 6574  -DD`...| Paramet
-00004ae0: 6572 2020 7c20 5375 7070 6f72 7465 6420  er  | Supported 
-00004af0: 7661 6c75 6573 207c 2044 6566 6175 6c74  values | Default
-00004b00: 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d3a   |.|:----------:
+00003620: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00003630: 606f 7574 7075 742f 7573 6572 6e61 6d65  `output/username
+00003640: 6020 2020 2020 2020 207c 2020 436f 6e66  `        |  Conf
+00003650: 6967 2020 7c20 3a68 6561 7679 5f63 6865  ig  | :heavy_che
+00003660: 636b 5f6d 6172 6b3a 207c 2020 2020 2020  ck_mark: |      
+00003670: 2020 2020 7374 7269 6e67 2020 2020 2020      string      
+00003680: 2020 2020 7c20 2020 2020 202d 2d2d 2020      |      ---  
+00003690: 2020 2020 207c 2046 6f72 2060 6874 7470       | For `http
+000036a0: 6020 6469 7265 6374 696f 6e20 2d20 6465  ` direction - de
+000036b0: 6669 6e65 7320 6120 7573 6572 6e61 6d65  fines a username
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003720: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00003730: 0a7c 2060 6f75 7470 7574 2f70 6173 7377  .| `output/passw
+00003740: 6f72 6460 2020 2020 2020 2020 7c20 2043  ord`        |  C
+00003750: 6f6e 6669 6720 207c 203a 6865 6176 795f  onfig  | :heavy_
+00003760: 6368 6563 6b5f 6d61 726b 3a20 7c20 2020  check_mark: |   
+00003770: 2020 2020 2020 2073 7472 696e 6720 2020         string   
+00003780: 2020 2020 2020 207c 2020 2020 2020 2d2d         |      --
+00003790: 2d20 2020 2020 2020 7c20 466f 7220 6068  -       | For `h
+000037a0: 7474 7060 2064 6972 6563 7469 6f6e 202d  ttp` direction -
+000037b0: 2064 6566 696e 6573 2061 2070 6173 7377   defines a passw
+000037c0: 6f72 6420 2020 2020 2020 2020 2020 2020  ord             
+000037d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003830: 2020 7c0a 7c20 6076 6172 7360 2020 2020    |.| `vars`    
+00003840: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00003850: 2020 436f 6e66 6967 2020 7c20 2020 2020    Config  |     
+00003860: 2020 203a 783a 2020 2020 2020 2020 207c     :x:         |
+00003870: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
+00003880: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00003890: 202d 2d2d 2020 2020 2020 207c 2044 6566   ---       | Def
+000038a0: 696e 6573 2076 6172 6961 626c 6573 2074  ines variables t
+000038b0: 6f20 6265 2075 7365 6420 696e 2061 204d  o be used in a M
+000038c0: 696d 656f 2054 656d 706c 6174 6520 2872  imeo Template (r
+000038d0: 6561 6420 6d6f 7265 2069 6e20 6e65 7874  ead more in next
+000038e0: 2073 6563 7469 6f6e 2920 2020 2020 2020   section)       
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003930: 2020 2020 207c 0a7c 2060 5f74 656d 706c       |.| `_templ
+00003940: 6174 6573 5f60 2020 2020 2020 2020 2020  ates_`          
+00003950: 2020 7c20 2043 6f6e 6669 6720 207c 203a    |  Config  | :
+00003960: 6865 6176 795f 6368 6563 6b5f 6d61 726b  heavy_check_mark
+00003970: 3a20 7c20 2020 2020 2020 2020 2061 7272  : |          arr
+00003980: 6179 2020 2020 2020 2020 2020 207c 2020  ay           |  
+00003990: 2020 2020 2d2d 2d20 2020 2020 2020 7c20      ---       | 
+000039a0: 5374 6f72 6573 2074 656d 706c 6174 6573  Stores templates
+000039b0: 2066 6f72 2064 6174 6120 6765 6e65 7261   for data genera
+000039c0: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a30: 2020 2020 2020 2020 7c0a 7c20 6063 6f75          |.| `cou
+00003a40: 6e74 6020 2020 2020 2020 2020 2020 2020  nt`             
+00003a50: 2020 2020 207c 2054 656d 706c 6174 6520       | Template 
+00003a60: 7c20 3a68 6561 7679 5f63 6865 636b 5f6d  | :heavy_check_m
+00003a70: 6172 6b3a 207c 2020 2020 2020 2020 2069  ark: |         i
+00003a80: 6e74 6567 6572 2020 2020 2020 2020 2020  nteger          
+00003a90: 7c20 2020 2020 202d 2d2d 2020 2020 2020  |      ---      
+00003aa0: 207c 2049 6e64 6963 6174 6573 206e 756d   | Indicates num
+00003ab0: 6265 7220 6f66 2063 6f70 6965 7320 2020  ber of copies   
+00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b30: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
+00003b40: 6d6f 6465 6c60 2020 2020 2020 2020 2020  model`          
+00003b50: 2020 2020 2020 2020 7c20 5465 6d70 6c61          | Templa
+00003b60: 7465 207c 203a 6865 6176 795f 6368 6563  te | :heavy_chec
+00003b70: 6b5f 6d61 726b 3a20 7c20 2020 2020 2020  k_mark: |       
+00003b80: 2020 206f 626a 6563 7420 2020 2020 2020     object       
+00003b90: 2020 207c 2020 2020 2020 2d2d 2d20 2020     |      ---   
+00003ba0: 2020 2020 7c20 4465 6669 6e65 7320 6461      | Defines da
+00003bb0: 7461 2074 656d 706c 6174 6520 746f 2062  ta template to b
+00003bc0: 6520 636f 7069 6564 2020 2020 2020 2020  e copied        
+00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c30: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00003c40: 7c20 6063 6f6e 7465 7874 6020 2020 2020  | `context`     
+00003c50: 2020 2020 2020 2020 2020 207c 2020 4d6f             |  Mo
+00003c60: 6465 6c20 2020 7c20 2020 2020 2020 203a  del   |        :
+00003c70: 783a 2020 2020 2020 2020 207c 2020 2020  x:         |    
+00003c80: 2020 2020 2020 6f62 6a65 6374 2020 2020        object    
+00003c90: 2020 2020 2020 7c20 2020 2020 202d 2d2d        |      ---
+00003ca0: 2020 2020 2020 207c 2044 6566 696e 6573         | Defines
+00003cb0: 2061 2063 6f6e 7465 7874 206e 616d 6520   a context name 
+00003cc0: 7468 6174 2069 7320 696e 7465 726e 616c  that is internal
+00003cd0: 6c79 2075 7365 6420 652e 672e 2075 7369  ly used e.g. usi
+00003ce0: 6e67 2060 6375 7272 5f69 7465 7228 2960  ng `curr_iter()`
+00003cf0: 2061 6e64 2060 6765 745f 6b65 7928 2960   and `get_key()`
+00003d00: 206d 696d 656f 2075 7469 6c73 2028 6279   mimeo utils (by
+00003d10: 2064 6566 6175 6c74 206d 6f64 656c 206e   default model n
+00003d20: 616d 6520 6973 2075 7365 6420 6173 2074  ame is used as t
+00003d30: 6865 2063 6f6e 7465 7874 206e 616d 6529  he context name)
+00003d40: 207c 0a0a 2323 2323 204d 696d 656f 2045   |..#### Mimeo E
+00003d50: 6e76 6972 6f6e 6d65 6e74 0a0a 546f 206d  nvironment..To m
+00003d60: 616b 6520 6068 7474 7060 206f 7574 7075  ake `http` outpu
+00003d70: 7420 6469 7265 6374 6f72 7920 6561 7369  t directory easi
+00003d80: 6572 2074 6f20 7573 652c 206d 696d 656f  er to use, mimeo
+00003d90: 2061 6c6c 6f77 7320 796f 7520 746f 2063   allows you to c
+00003da0: 6f6e 6669 6775 7265 204d 696d 656f 2045  onfigure Mimeo E
+00003db0: 6e76 6972 6f6e 6d65 6e74 732e 0a54 6865  nvironments..The
+00003dc0: 7920 6172 6520 636f 6e66 6967 7572 6564  y are configured
+00003dd0: 2069 6e20 6120 4a53 4f4e 2066 696c 6520   in a JSON file 
+00003de0: 2862 7920 6465 6661 756c 743a 206d 696d  (by default: mim
+00003df0: 656f 2e65 6e76 732e 6a73 6f6e 2920 616e  eo.envs.json) an
+00003e00: 6420 7375 7070 6f72 7420 7468 6520 666f  d support the fo
+00003e10: 6c6c 6f77 696e 6720 6f75 7470 7574 2064  llowing output d
+00003e20: 6574 6169 6c73 3a0a 2d20 6070 726f 746f  etails:.- `proto
+00003e30: 636f 6c60 0a2d 2060 686f 7374 600a 2d20  col`.- `host`.- 
+00003e40: 6070 6f72 7460 0a2d 2060 7573 6572 6e61  `port`.- `userna
+00003e50: 6d65 600a 2d20 6070 6173 7377 6f72 6460  me`.- `password`
+00003e60: 0a0a 4578 616d 706c 650a 6060 606a 736f  ..Example.```jso
+00003e70: 6e0a 7b0a 2020 2020 226c 6f63 616c 223a  n.{.    "local":
+00003e80: 207b 0a20 2020 2020 2020 2022 686f 7374   {.        "host
+00003e90: 223a 2022 6c6f 6361 6c68 6f73 7422 2c0a  ": "localhost",.
+00003ea0: 2020 2020 2020 2020 2270 6f72 7422 3a20          "port": 
+00003eb0: 3830 3030 2c0a 2020 2020 2020 2020 2275  8000,.        "u
+00003ec0: 7365 726e 616d 6522 3a20 2261 646d 696e  sername": "admin
+00003ed0: 222c 0a20 2020 2020 2020 2022 7061 7373  ",.        "pass
+00003ee0: 776f 7264 223a 2022 6164 6d69 6e22 0a20  word": "admin". 
+00003ef0: 2020 207d 2c0a 2020 2020 2264 6576 223a     },.    "dev":
+00003f00: 207b 0a20 2020 2020 2020 2022 7072 6f74   {.        "prot
+00003f10: 6f63 6f6c 223a 2022 6874 7470 7322 2c0a  ocol": "https",.
+00003f20: 2020 2020 2020 2020 2268 6f73 7422 3a20          "host": 
+00003f30: 2231 312e 3131 312e 3131 2e31 3131 222c  "11.111.11.111",
+00003f40: 0a20 2020 2020 2020 2022 706f 7274 223a  .        "port":
+00003f50: 2038 3030 302c 0a20 2020 2020 2020 2022   8000,.        "
+00003f60: 7573 6572 6e61 6d65 223a 2022 736f 6d65  username": "some
+00003f70: 2d75 7365 7222 2c0a 2020 2020 2020 2020  -user",.        
+00003f80: 2270 6173 7377 6f72 6422 3a20 2273 6f6d  "password": "som
+00003f90: 652d 7061 7373 776f 7264 220a 2020 2020  e-password".    
+00003fa0: 7d0a 7d0a 6060 600a 0a54 6f20 7573 6520  }.}.```..To use 
+00003fb0: 6120 7370 6563 6966 6963 204d 696d 656f  a specific Mimeo
+00003fc0: 2045 6e76 6972 6f6e 6d65 6e74 2079 6f75   Environment you
+00003fd0: 2063 616e 2075 7365 2074 6865 2066 6f6c   can use the fol
+00003fe0: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 733a  lowing commands:
+00003ff0: 0a60 6060 7368 0a6d 696d 656f 2053 6f6d  .```sh.mimeo Som
+00004000: 6545 6e74 6974 792d 636f 6e66 6967 2e6a  eEntity-config.j
+00004010: 736f 6e20 2d65 2064 6576 0a6d 696d 656f  son -e dev.mimeo
+00004020: 2053 6f6d 6545 6e74 6974 792d 636f 6e66   SomeEntity-conf
+00004030: 6967 2e6a 736f 6e20 2d65 2064 6576 202d  ig.json -e dev -
+00004040: 2d68 7474 702d 656e 7673 2d66 696c 6520  -http-envs-file 
+00004050: 656e 7669 726f 6e6d 656e 7473 2e6a 736f  environments.jso
+00004060: 6e0a 6060 600a 0a23 2323 2320 4d69 6d65  n.```..#### Mime
+00004070: 6f20 5661 7273 0a0a 4d69 6d65 6f20 616c  o Vars..Mimeo al
+00004080: 6c6f 7773 2079 6f75 2074 6f20 6465 6669  lows you to defi
+00004090: 6e65 2061 206c 6973 7420 6f66 2076 6172  ne a list of var
+000040a0: 6961 626c 6573 2e0a 596f 7520 6361 6e20  iables..You can 
+000040b0: 7573 6520 7468 656d 2069 6e20 796f 7572  use them in your
+000040c0: 204d 696d 656f 2043 6f6e 6669 6720 6279   Mimeo Config by
+000040d0: 2077 7261 7070 696e 6720 7468 656d 2069   wrapping them i
+000040e0: 6e20 6375 726c 7920 6272 6163 6b65 7473  n curly brackets
+000040f0: 205b 607b 5641 5249 4142 4c45 7d60 5d2e   [`{VARIABLE}`].
+00004100: 0a0a 5468 6572 6520 6172 6520 6f6e 6c79  ..There are only
+00004110: 2032 2072 756c 6573 2066 6f72 2076 6172   2 rules for var
+00004120: 6961 626c 6520 6e61 6d65 733a 0a2d 2056  iable names:.- V
+00004130: 6172 6961 626c 6520 6e61 6d65 2063 616e  ariable name can
+00004140: 2069 6e63 6c75 6465 2075 7070 6572 2d63   include upper-c
+00004150: 6173 6564 206c 6574 7465 7273 205c 5b60  ased letters \[`
+00004160: 412d 5a60 5c5d 2c20 756e 6465 7273 636f  A-Z`\], undersco
+00004170: 7265 205c 5b60 5f60 5c5d 2061 6e64 2064  re \[`_`\] and d
+00004180: 6967 6974 7320 5c7b 6030 2d39 605c 7d20  igits \{`0-9`\} 
+00004190: 6f6e 6c79 0a2d 2056 6172 6961 626c 6520  only.- Variable 
+000041a0: 6e61 6d65 206d 7573 7420 7374 6172 7420  name must start 
+000041b0: 7769 7468 2061 206c 6574 7465 720a 0a56  with a letter..V
+000041c0: 6172 6961 626c 6520 6361 6e20 6265 2064  ariable can be d
+000041d0: 6566 696e 6564 2077 6974 683a 0a2d 2061  efined with:.- a
+000041e0: 6e79 2061 746f 6d69 6320 7661 6c75 650a  ny atomic value.
+000041f0: 2d20 616e 7920 6f74 6865 7220 7661 7269  - any other vari
+00004200: 6162 6c65 2064 6566 696e 6564 0a2d 2061  able defined.- a
+00004210: 6e79 204d 696d 656f 2055 7469 6c0a 0a59  ny Mimeo Util..Y
+00004220: 6f75 2063 616e 2075 7365 204d 696d 656f  ou can use Mimeo
+00004230: 2056 6172 7320 6173 2070 6172 7469 616c   Vars as partial
+00004240: 2076 616c 7565 7320 2875 6e6c 6573 7320   values (unless 
+00004250: 7468 6579 2061 7265 2064 6566 696e 6564  they are defined
+00004260: 2061 7320 4d69 6d65 6f20 5574 696c 7329   as Mimeo Utils)
+00004270: 2e0a 0a45 7861 6d70 6c65 3a0a 6060 606a  ...Example:.```j
+00004280: 736f 6e0a 7b0a 2020 2276 6172 7322 3a20  son.{.  "vars": 
+00004290: 7b0a 2020 2020 2243 5553 544f 4d5f 5641  {.    "CUSTOM_VA
+000042a0: 525f 3122 3a20 2263 7573 746f 6d2d 7661  R_1": "custom-va
+000042b0: 6c75 652d 3122 2c0a 2020 2020 2243 5553  lue-1",.    "CUS
+000042c0: 544f 4d5f 5641 525f 3222 3a20 312c 0a20  TOM_VAR_2": 1,. 
+000042d0: 2020 2022 4355 5354 4f4d 5f56 4152 5f33     "CUSTOM_VAR_3
+000042e0: 223a 2074 7275 652c 0a20 2020 2022 4355  ": true,.    "CU
+000042f0: 5354 4f4d 5f56 4152 5f34 223a 2022 7b43  STOM_VAR_4": "{C
+00004300: 5553 544f 4d5f 5641 525f 327d 222c 0a20  USTOM_VAR_2}",. 
+00004310: 2020 2022 4355 5354 4f4d 5f56 4152 5f35     "CUSTOM_VAR_5
+00004320: 223a 2022 7b61 7574 6f5f 696e 6372 656d  ": "{auto_increm
+00004330: 656e 747d 222c 0a20 2020 2022 4355 5354  ent}",.    "CUST
+00004340: 4f4d 5f56 4152 5f36 223a 207b 0a20 2020  OM_VAR_6": {.   
+00004350: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
+00004360: 3a20 7b0a 2020 2020 2020 2020 225f 6e61  : {.        "_na
+00004370: 6d65 223a 2022 7261 6e64 6f6d 5f69 6e74  me": "random_int
+00004380: 222c 0a20 2020 2020 2020 2022 6c69 6d69  ",.        "limi
+00004390: 7422 3a20 3939 0a20 2020 2020 207d 0a20  t": 99.      }. 
+000043a0: 2020 207d 0a20 207d 2c0a 2020 225f 7465     }.  },.  "_te
+000043b0: 6d70 6c61 7465 735f 223a 205b 0a20 2020  mplates_": [.   
+000043c0: 207b 0a20 2020 2020 2022 636f 756e 7422   {.      "count"
+000043d0: 3a20 352c 0a20 2020 2020 2022 6d6f 6465  : 5,.      "mode
+000043e0: 6c22 3a20 7b0a 2020 2020 2020 2020 2253  l": {.        "S
+000043f0: 6f6d 6545 6e74 6974 7922 3a20 7b0a 2020  omeEntity": {.  
+00004400: 2020 2020 2020 2020 2243 6869 6c64 4e6f          "ChildNo
+00004410: 6465 3122 3a20 227b 4355 5354 4f4d 5f56  de1": "{CUSTOM_V
+00004420: 4152 5f31 7d22 2c0a 2020 2020 2020 2020  AR_1}",.        
+00004430: 2020 2243 6869 6c64 4e6f 6465 3222 3a20    "ChildNode2": 
+00004440: 227b 4355 5354 4f4d 5f56 4152 5f32 7d22  "{CUSTOM_VAR_2}"
+00004450: 2c0a 2020 2020 2020 2020 2020 2243 6869  ,.          "Chi
+00004460: 6c64 4e6f 6465 3322 3a20 227b 4355 5354  ldNode3": "{CUST
+00004470: 4f4d 5f56 4152 5f33 7d22 2c0a 2020 2020  OM_VAR_3}",.    
+00004480: 2020 2020 2020 2243 6869 6c64 4e6f 6465        "ChildNode
+00004490: 3422 3a20 227b 4355 5354 4f4d 5f56 4152  4": "{CUSTOM_VAR
+000044a0: 5f34 7d22 2c0a 2020 2020 2020 2020 2020  _4}",.          
+000044b0: 2243 6869 6c64 4e6f 6465 3522 3a20 227b  "ChildNode5": "{
+000044c0: 4355 5354 4f4d 5f56 4152 5f35 7d22 2c0a  CUSTOM_VAR_5}",.
+000044d0: 2020 2020 2020 2020 2020 2243 6869 6c64            "Child
+000044e0: 4e6f 6465 3622 3a20 227b 4355 5354 4f4d  Node6": "{CUSTOM
+000044f0: 5f56 4152 5f36 7d22 2c0a 2020 2020 2020  _VAR_6}",.      
+00004500: 2020 2020 2243 6869 6c64 4e6f 6465 3722      "ChildNode7"
+00004510: 3a20 227b 4355 5354 4f4d 5f56 4152 5f31  : "{CUSTOM_VAR_1
+00004520: 7d2d 7769 7468 2d73 7566 6669 7822 0a20  }-with-suffix". 
+00004530: 2020 2020 2020 207d 0a20 2020 2020 207d         }.      }
+00004540: 0a20 2020 207d 0a20 205d 0a7d 0a60 6060  .    }.  ].}.```
+00004550: 0a0a 2323 2323 204d 696d 656f 2053 7065  ..#### Mimeo Spe
+00004560: 6369 616c 2046 6965 6c64 730a 0a49 6e20  cial Fields..In 
+00004570: 4d69 6d65 6f20 5465 6d70 6c61 7465 2079  Mimeo Template y
+00004580: 6f75 2063 616e 2075 7365 2073 6f2d 6361  ou can use so-ca
+00004590: 6c6c 6564 205f 7370 6563 6961 6c20 6669  lled _special fi
+000045a0: 656c 6473 5f2e 0a45 7665 7279 2066 6965  elds_..Every fie
+000045b0: 6c64 2069 6e20 6120 7465 6d70 6c61 7465  ld in a template
+000045c0: 2063 616e 2062 6520 7374 6f72 6564 2069   can be stored i
+000045d0: 6e20 6d65 6d6f 7279 2028 5f70 726f 7669  n memory (_provi
+000045e0: 6465 645f 2920 616e 6420 7573 6564 206c  ded_) and used l
+000045f0: 6174 6572 2061 7320 6120 7661 6c75 6520  ater as a value 
+00004600: 6f66 206f 7468 6572 2066 6965 6c64 7320  of other fields 
+00004610: 285f 696e 6a65 6374 6564 5f29 2e0a 546f  (_injected_)..To
+00004620: 2070 726f 7669 6465 2061 2073 7065 6369   provide a speci
+00004630: 616c 2066 6965 6c64 2c20 7772 6170 2069  al field, wrap i
+00004640: 7473 206e 616d 6520 7769 7468 2063 6f6c  ts name with col
+00004650: 6f6e 733a 205b 603a 536f 6d65 4669 656c  ons: [`:SomeFiel
+00004660: 643a 605d 2e20 546f 2069 6e6a 6563 742c  d:`]. To inject,
+00004670: 2075 7365 2061 6464 6974 696f 6e61 6c6c   use additionall
+00004680: 7920 6375 726c 7920 6272 6163 6573 2074  y curly braces t
+00004690: 6f0a 6c65 7420 696e 7465 7270 7265 7465  o.let interprete
+000046a0: 7220 6b6e 6f77 2069 7420 7368 6f75 6c64  r know it should
+000046b0: 2062 6520 7265 6e64 6572 6564 205b 607b   be rendered [`{
+000046c0: 3a53 6f6d 6546 6965 6c64 3a7d 605d 2e0a  :SomeField:}`]..
+000046d0: 5468 6579 2063 616e 2062 6520 696e 6a65  They can be inje
+000046e0: 6374 6564 2061 7320 7061 7274 6961 6c20  cted as partial 
+000046f0: 7661 6c75 6573 2c20 7369 6d69 6c61 726c  values, similarl
+00004700: 7920 746f 204d 696d 656f 2056 6172 732e  y to Mimeo Vars.
+00004710: 0a0a 4578 616d 706c 650a 6060 606a 736f  ..Example.```jso
+00004720: 6e0a 7b0a 2020 225f 7465 6d70 6c61 7465  n.{.  "_template
+00004730: 735f 223a 205b 0a20 2020 207b 0a20 2020  s_": [.    {.   
+00004740: 2020 2022 636f 756e 7422 3a20 352c 0a20     "count": 5,. 
+00004750: 2020 2020 2022 6d6f 6465 6c22 3a20 7b0a       "model": {.
+00004760: 2020 2020 2020 2020 2253 6f6d 6545 6e74          "SomeEnt
+00004770: 6974 7922 3a20 7b0a 2020 2020 2020 2020  ity": {.        
+00004780: 2020 223a 4368 696c 644e 6f64 6531 3a22    ":ChildNode1:"
+00004790: 3a20 2263 7573 746f 6d2d 7661 6c75 6522  : "custom-value"
+000047a0: 2c0a 2020 2020 2020 2020 2020 2243 6869  ,.          "Chi
+000047b0: 6c64 4e6f 6465 3222 3a20 227b 3a43 6869  ldNode2": "{:Chi
+000047c0: 6c64 4e6f 6465 313a 7d22 2c0a 2020 2020  ldNode1:}",.    
+000047d0: 2020 2020 2020 2243 6869 6c64 4e6f 6465        "ChildNode
+000047e0: 3322 3a20 227b 3a43 6869 6c64 4e6f 6465  3": "{:ChildNode
+000047f0: 313a 7d2d 7769 7468 2d73 7566 6669 7822  1:}-with-suffix"
+00004800: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00004810: 207d 0a20 2020 207d 0a20 205d 0a7d 0a60   }.    }.  ].}.`
+00004820: 6060 0a0a 2323 2323 204d 696d 656f 2055  ``..#### Mimeo U
+00004830: 7469 6c73 0a0a 596f 7520 6361 6e20 7573  tils..You can us
+00004840: 6520 7365 7665 7261 6c20 7072 6564 6566  e several predef
+00004850: 696e 6564 2066 756e 6374 696f 6e73 2074  ined functions t
+00004860: 6f20 6765 6e65 7261 7465 2064 6174 612e  o generate data.
+00004870: 2054 6865 7920 6361 6e20 6265 2075 7365   They can be use
+00004880: 6420 696e 2061 205f 7261 775f 2066 6f72  d in a _raw_ for
+00004890: 6d61 7420 6f72 205f 7061 7261 6d65 7472  mat or _parametr
+000048a0: 697a 6564 5f2e 0a0a 2323 2323 2320 5261  ized_...##### Ra
+000048b0: 6e64 6f6d 2053 7472 696e 670a 0a47 656e  ndom String..Gen
+000048c0: 6572 6174 6573 2061 2072 616e 646f 6d20  erates a random 
+000048d0: 7374 7269 6e67 2076 616c 7565 2e0a 0a7c  string value...|
+000048e0: 2050 6172 616d 6574 6572 207c 2053 7570   Parameter | Sup
+000048f0: 706f 7274 6564 2076 616c 7565 7320 7c20  ported values | 
+00004900: 4465 6661 756c 7420 7c0a 7c3a 2d2d 2d2d  Default |.|:----
+00004910: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
+00004920: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
+00004930: 2d2d 3a7c 0a7c 2020 6c65 6e67 7468 2020  --:|.|  length  
+00004940: 207c 2020 2020 2020 6069 6e74 6020 2020   |      `int`   
+00004950: 2020 2020 7c20 2060 3230 6020 2020 7c0a      |  `20`   |.
+00004960: 0a23 2323 2323 2320 5261 770a 0a55 7365  .###### Raw..Use
+00004970: 7320 7468 6520 6465 6661 756c 7420 6c65  s the default le
+00004980: 6e67 7468 3a20 3230 2063 6861 7261 6374  ngth: 20 charact
+00004990: 6572 732e 0a0a 6060 606a 736f 6e0a 7b0a  ers...```json.{.
+000049a0: 2020 2272 616e 646f 6d73 7472 696e 6722    "randomstring"
+000049b0: 3a20 227b 7261 6e64 6f6d 5f73 7472 7d22  : "{random_str}"
+000049c0: 0a7d 0a60 6060 0a0a 2323 2323 2323 2050  .}.```..###### P
+000049d0: 6172 616d 6574 7269 7a65 640a 0a55 7365  arametrized..Use
+000049e0: 7320 7468 6520 6375 7374 6f6d 697a 6564  s the customized
+000049f0: 206c 656e 6774 682e 0a0a 6060 606a 736f   length...```jso
+00004a00: 6e0a 7b0a 2020 2272 616e 646f 6d73 7472  n.{.  "randomstr
+00004a10: 696e 6722 3a20 7b0a 2020 2020 225f 6d69  ing": {.    "_mi
+00004a20: 6d65 6f5f 7574 696c 223a 207b 0a20 2020  meo_util": {.   
+00004a30: 2020 2022 5f6e 616d 6522 3a20 2272 616e     "_name": "ran
+00004a40: 646f 6d5f 7374 7222 2c0a 2020 2020 2020  dom_str",.      
+00004a50: 226c 656e 6774 6822 3a20 350a 2020 2020  "length": 5.    
+00004a60: 7d0a 2020 7d0a 7d0a 6060 600a 0a23 2323  }.  }.}.```..###
+00004a70: 2323 2052 616e 646f 6d20 496e 7465 6765  ## Random Intege
+00004a80: 720a 0a47 656e 6572 6174 6573 2061 2072  r..Generates a r
+00004a90: 616e 646f 6d20 696e 7465 6765 7220 7661  andom integer va
+00004aa0: 6c75 6520 6265 7477 6565 6e20 6073 7461  lue between `sta
+00004ab0: 7274 6020 616e 6420 606c 696d 6974 6020  rt` and `limit` 
+00004ac0: 7061 7261 6d65 7465 7273 2028 696e 636c  parameters (incl
+00004ad0: 7573 6976 6529 2e0a 0a7c 2050 6172 616d  usive)...| Param
+00004ae0: 6574 6572 207c 2053 7570 706f 7274 6564  eter | Supported
+00004af0: 2076 616c 7565 7320 7c20 4465 6661 756c   values | Defaul
+00004b00: 7420 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a  t |.|:---------:
 00004b10: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
 00004b20: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 3a7c 0a7c  --:|:-------:|.|
-00004b30: 2064 6179 735f 6465 6c74 6120 7c20 2020   days_delta |   
-00004b40: 2020 2060 696e 7460 2020 2020 2020 207c     `int`       |
-00004b50: 2020 2060 3060 2020 207c 0a0a 2323 2323     `0`   |..####
-00004b60: 2323 2052 6177 0a0a 5573 6573 2074 6865  ## Raw..Uses the
-00004b70: 2074 6f64 6179 2773 2064 6174 652e 0a0a   today's date...
-00004b80: 6060 606a 736f 6e0a 7b0a 2020 2254 6f64  ```json.{.  "Tod
-00004b90: 6179 223a 2022 7b64 6174 657d 220a 7d0a  ay": "{date}".}.
-00004ba0: 6060 600a 0a23 2323 2323 2320 5061 7261  ```..###### Para
-00004bb0: 6d65 7472 697a 6564 0a0a 5573 6573 2074  metrized..Uses t
-00004bc0: 6865 2063 7573 746f 6d69 7a65 6420 6461  he customized da
-00004bd0: 7973 2064 656c 7461 2e0a 0a60 6060 6a73  ys delta...```js
-00004be0: 6f6e 0a7b 0a20 2022 5965 7374 6572 6461  on.{.  "Yesterda
-00004bf0: 7922 3a20 7b0a 2020 2020 225f 6d69 6d65  y": {.    "_mime
-00004c00: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
-00004c10: 2022 5f6e 616d 6522 3a20 2264 6174 6522   "_name": "date"
-00004c20: 2c0a 2020 2020 2020 2264 6179 735f 6465  ,.      "days_de
-00004c30: 6c74 6122 3a20 2d31 0a20 2020 207d 0a20  lta": -1.    }. 
-00004c40: 207d 2c0a 2020 2254 6f6d 6f72 726f 7722   },.  "Tomorrow"
-00004c50: 3a20 7b0a 2020 2020 225f 6d69 6d65 6f5f  : {.    "_mimeo_
-00004c60: 7574 696c 223a 207b 0a20 2020 2020 2022  util": {.      "
-00004c70: 5f6e 616d 6522 3a20 2264 6174 6522 2c0a  _name": "date",.
-00004c80: 2020 2020 2020 2264 6179 735f 6465 6c74        "days_delt
-00004c90: 6122 3a20 310a 2020 2020 7d0a 2020 7d0a  a": 1.    }.  }.
-00004ca0: 7d0a 6060 600a 0a23 2323 2323 2044 6174  }.```..##### Dat
-00004cb0: 6520 5469 6d65 0a0a 4765 6e65 7261 7465  e Time..Generate
-00004cc0: 7320 6120 6461 7465 2074 696d 6520 7661  s a date time va
-00004cd0: 6c75 6520 696e 2066 6f72 6d61 7420 6059  lue in format `Y
-00004ce0: 5959 592d 4d4d 2d44 4427 5427 4848 3a6d  YYY-MM-DD'T'HH:m
-00004cf0: 6d3a 5353 602e 0a0a 7c20 2020 5061 7261  m:SS`...|   Para
-00004d00: 6d65 7465 7220 2020 7c20 5375 7070 6f72  meter   | Suppor
-00004d10: 7465 6420 7661 6c75 6573 207c 2044 6566  ted values | Def
-00004d20: 6175 6c74 207c 0a7c 3a2d 2d2d 2d2d 2d2d  ault |.|:-------
-00004d30: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
-00004d40: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
-00004d50: 2d2d 2d3a 7c0a 7c20 2064 6179 735f 6465  ---:|.|  days_de
-00004d60: 6c74 6120 2020 7c20 2020 2020 2060 696e  lta   |      `in
-00004d70: 7460 2020 2020 2020 207c 2020 2060 3060  t`       |   `0`
-00004d80: 2020 207c 0a7c 2020 686f 7572 735f 6465     |.|  hours_de
-00004d90: 6c74 6120 207c 2020 2020 2020 6069 6e74  lta  |      `int
-00004da0: 6020 2020 2020 2020 7c20 2020 6030 6020  `       |   `0` 
-00004db0: 2020 7c0a 7c20 6d69 6e75 7465 735f 6465    |.| minutes_de
-00004dc0: 6c74 6120 7c20 2020 2020 2060 696e 7460  lta |      `int`
-00004dd0: 2020 2020 2020 207c 2020 2060 3060 2020         |   `0`  
-00004de0: 207c 0a7c 2073 6563 6f6e 6473 5f64 656c   |.| seconds_del
-00004df0: 7461 207c 2020 2020 2020 6069 6e74 6020  ta |      `int` 
-00004e00: 2020 2020 2020 7c20 2020 6030 6020 2020        |   `0`   
-00004e10: 7c0a 0a23 2323 2323 2320 5261 770a 0a55  |..###### Raw..U
-00004e20: 7365 7320 7468 6520 6375 7272 656e 7420  ses the current 
-00004e30: 7469 6d65 7374 616d 702e 0a0a 6060 606a  timestamp...```j
-00004e40: 736f 6e0a 7b0a 2020 224e 6f77 223a 2022  son.{.  "Now": "
-00004e50: 7b64 6174 655f 7469 6d65 7d22 0a7d 0a60  {date_time}".}.`
-00004e60: 6060 0a0a 2323 2323 2323 2050 6172 616d  ``..###### Param
-00004e70: 6574 7269 7a65 640a 0a55 7365 7320 7468  etrized..Uses th
-00004e80: 6520 6375 7374 6f6d 697a 6564 2064 656c  e customized del
-00004e90: 7461 732e 0a0a 6060 606a 736f 6e0a 7b0a  tas...```json.{.
-00004ea0: 2020 2254 6f6d 6f72 726f 7754 6872 6565    "TomorrowThree
-00004eb0: 486f 7572 734c 6174 6572 5477 656e 7479  HoursLaterTwenty
-00004ec0: 4d69 6e75 7465 7341 676f 5477 6f53 6563  MinutesAgoTwoSec
-00004ed0: 6f6e 6473 4c61 7465 7222 3a20 7b0a 2020  ondsLater": {.  
-00004ee0: 2020 225f 6d69 6d65 6f5f 7574 696c 223a    "_mimeo_util":
-00004ef0: 207b 0a20 2020 2020 2022 5f6e 616d 6522   {.      "_name"
-00004f00: 3a20 2264 6174 655f 7469 6d65 222c 0a20  : "date_time",. 
-00004f10: 2020 2020 2022 6461 7973 5f64 656c 7461       "days_delta
-00004f20: 223a 2031 2c0a 2020 2020 2020 2268 6f75  ": 1,.      "hou
-00004f30: 7273 5f64 656c 7461 223a 2033 2c0a 2020  rs_delta": 3,.  
-00004f40: 2020 2020 226d 696e 7574 6573 5f64 656c      "minutes_del
-00004f50: 7461 223a 202d 3230 2c0a 2020 2020 2020  ta": -20,.      
-00004f60: 2273 6563 6f6e 6473 5f64 656c 7461 223a  "seconds_delta":
-00004f70: 2032 0a20 2020 207d 0a20 207d 0a7d 0a60   2.    }.  }.}.`
-00004f80: 6060 0a0a 2323 2323 2320 4175 746f 2049  ``..##### Auto I
-00004f90: 6e63 7265 6d65 6e74 0a0a 4765 6e65 7261  ncrement..Genera
-00004fa0: 7465 7320 6120 6e65 7874 2069 6e74 6567  tes a next integ
-00004fb0: 6572 2069 6e20 636f 6e74 6578 7420 6f66  er in context of
-00004fc0: 2061 206d 6f64 656c 2028 696e 206e 6573   a model (in nes
-00004fd0: 7465 6420 7465 6d70 6c61 7465 7320 6974  ted templates it
-00004fe0: 2077 696c 6c20 7573 6520 6120 7365 7061   will use a sepa
-00004ff0: 7261 7465 6420 636f 6e74 6578 7429 2e0a  rated context)..
-00005000: 0a7c 2050 6172 616d 6574 6572 207c 2053  .| Parameter | S
-00005010: 7570 706f 7274 6564 2076 616c 7565 7320  upported values 
-00005020: 7c20 4465 6661 756c 7420 207c 0a7c 3a2d  | Default  |.|:-
-00005030: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
-00005040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
-00005050: 2d2d 2d2d 2d2d 3a7c 0a7c 2020 7061 7474  ------:|.|  patt
-00005060: 6572 6e20 207c 2020 2020 2020 6073 7472  ern  |      `str
-00005070: 6020 2020 2020 2020 7c20 607b 3a30 3564  `       | `{:05d
-00005080: 7d60 207c 0a0a 2323 2323 2323 2052 6177  }` |..###### Raw
-00005090: 0a0a 5573 6573 2061 2064 6566 6175 6c74  ..Uses a default
-000050a0: 2070 6174 7465 726e 3a20 2a2a 7b3a 3035   pattern: **{:05
-000050b0: 647d 2a2a 2028 616e 2069 6e74 6567 6572  d}** (an integer
-000050c0: 2077 6974 6820 3520 6c65 6164 696e 6720   with 5 leading 
-000050d0: 7a65 726f 7329 2e0a 0a60 6060 6a73 6f6e  zeros)...```json
-000050e0: 0a7b 0a20 2022 4944 223a 2022 7b61 7574  .{.  "ID": "{aut
-000050f0: 6f5f 696e 6372 656d 656e 747d 220a 7d0a  o_increment}".}.
-00005100: 6060 600a 0a23 2323 2323 2320 5061 7261  ```..###### Para
-00005110: 6d65 7472 697a 6564 0a0a 5573 6573 2074  metrized..Uses t
-00005120: 6865 2073 7472 696e 6720 7061 7474 6572  he string patter
-00005130: 6e20 7072 6f76 6964 6564 2e0a 0a60 6060  n provided...```
-00005140: 6a73 6f6e 0a7b 0a20 2022 4944 223a 207b  json.{.  "ID": {
-00005150: 0a20 2020 2022 5f6d 696d 656f 5f75 7469  .    "_mimeo_uti
-00005160: 6c22 3a20 7b0a 2020 2020 2020 225f 6e61  l": {.      "_na
-00005170: 6d65 223a 2022 6175 746f 5f69 6e63 7265  me": "auto_incre
-00005180: 6d65 6e74 222c 0a20 2020 2020 2022 7061  ment",.      "pa
-00005190: 7474 6572 6e22 3a20 224d 595f 4944 5f7b  ttern": "MY_ID_{
-000051a0: 3a30 3130 647d 220a 2020 2020 7d0a 2020  :010d}".    }.  
-000051b0: 7d0a 7d0a 6060 600a 0a23 2323 2323 2043  }.}.```..##### C
-000051c0: 7572 7265 6e74 2049 7465 7261 7469 6f6e  urrent Iteration
-000051d0: 0a0a 4765 6e65 7261 7465 7320 6120 7661  ..Generates a va
-000051e0: 6c75 6520 6f66 2074 6865 2063 7572 7265  lue of the curre
-000051f0: 6e74 2069 7465 7261 7469 6f6e 2069 6e20  nt iteration in 
-00005200: 6120 4d69 6d65 6f20 5465 6d70 6c61 7465  a Mimeo Template
-00005210: 2063 6f6e 7465 7874 2e0a 0a7c 2050 6172   context...| Par
-00005220: 616d 6574 6572 207c 2053 7570 706f 7274  ameter | Support
-00005230: 6564 2076 616c 7565 7320 7c20 2020 2020  ed values |     
-00005240: 2044 6566 6175 6c74 2020 2020 2020 7c0a   Default      |.
-00005250: 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  |:---------:|:--
-00005260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
-00005270: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-00005280: 2d2d 3a7c 0a7c 2020 636f 6e74 6578 7420  --:|.|  context 
-00005290: 207c 2020 2020 2020 6073 7472 6020 2020   |      `str`   
-000052a0: 2020 2020 7c20 6120 6375 7272 656e 7420      | a current 
-000052b0: 636f 6e74 6578 7420 7c0a 0a23 2323 2323  context |..#####
-000052c0: 2320 5261 770a 0a55 7365 7320 7468 6520  # Raw..Uses the 
-000052d0: 6375 7272 656e 7420 636f 6e74 6578 742e  current context.
-000052e0: 0a0a 6060 606a 736f 6e0a 7b0a 2020 2249  ..```json.{.  "I
-000052f0: 4422 3a20 227b 6375 7272 5f69 7465 727d  D": "{curr_iter}
+00004b30: 2020 2073 7461 7274 2020 207c 2020 2020     start   |    
+00004b40: 2020 6069 6e74 6020 2020 2020 2020 7c20    `int`       | 
+00004b50: 2020 6031 6020 2020 7c0a 7c20 2020 6c69    `1`   |.|   li
+00004b60: 6d69 7420 2020 7c20 2020 2020 2060 696e  mit   |      `in
+00004b70: 7460 2020 2020 2020 207c 2020 6031 3030  t`       |  `100
+00004b80: 6020 207c 0a0a 2323 2323 2323 2052 6177  `  |..###### Raw
+00004b90: 0a0a 5573 6573 2074 6865 2064 6566 6175  ..Uses the defau
+00004ba0: 6c74 2073 7461 7274 2028 3129 2061 6e64  lt start (1) and
+00004bb0: 206c 696d 6974 2028 3130 3029 2076 616c   limit (100) val
+00004bc0: 7565 732e 0a0a 6060 606a 736f 6e0a 7b0a  ues...```json.{.
+00004bd0: 2020 2272 616e 646f 6d69 6e74 6567 6572    "randominteger
+00004be0: 223a 2022 7b72 616e 646f 6d5f 696e 747d  ": "{random_int}
+00004bf0: 220a 7d0a 6060 600a 0a23 2323 2323 2320  ".}.```..###### 
+00004c00: 5061 7261 6d65 7472 697a 6564 0a0a 5573  Parametrized..Us
+00004c10: 6573 2074 6865 2063 7573 746f 6d69 7a65  es the customize
+00004c20: 6420 6c69 6d69 742e 0a0a 6060 606a 736f  d limit...```jso
+00004c30: 6e0a 7b0a 2020 2272 616e 646f 6d69 6e74  n.{.  "randomint
+00004c40: 6567 6572 3122 3a20 7b0a 2020 2020 225f  eger1": {.    "_
+00004c50: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
+00004c60: 2020 2020 2022 5f6e 616d 6522 3a20 2272       "_name": "r
+00004c70: 616e 646f 6d5f 696e 7422 2c0a 2020 2020  andom_int",.    
+00004c80: 2020 2273 7461 7274 223a 2030 0a20 2020    "start": 0.   
+00004c90: 207d 0a20 207d 2c0a 2020 2272 616e 646f   }.  },.  "rando
+00004ca0: 6d69 6e74 6567 6572 3222 3a20 7b0a 2020  minteger2": {.  
+00004cb0: 2020 225f 6d69 6d65 6f5f 7574 696c 223a    "_mimeo_util":
+00004cc0: 207b 0a20 2020 2020 2022 5f6e 616d 6522   {.      "_name"
+00004cd0: 3a20 2272 616e 646f 6d5f 696e 7422 2c0a  : "random_int",.
+00004ce0: 2020 2020 2020 226c 696d 6974 223a 2035        "limit": 5
+00004cf0: 0a20 2020 207d 0a20 207d 2c0a 2020 2272  .    }.  },.  "r
+00004d00: 616e 646f 6d69 6e74 6567 6572 3322 3a20  andominteger3": 
+00004d10: 7b0a 2020 2020 225f 6d69 6d65 6f5f 7574  {.    "_mimeo_ut
+00004d20: 696c 223a 207b 0a20 2020 2020 2022 5f6e  il": {.      "_n
+00004d30: 616d 6522 3a20 2272 616e 646f 6d5f 696e  ame": "random_in
+00004d40: 7422 2c0a 2020 2020 2020 2273 7461 7274  t",.      "start
+00004d50: 223a 2030 2c0a 2020 2020 2020 226c 696d  ": 0,.      "lim
+00004d60: 6974 223a 2035 0a20 2020 207d 0a20 207d  it": 5.    }.  }
+00004d70: 0a7d 0a60 6060 0a0a 2323 2323 2320 5261  .}.```..##### Ra
+00004d80: 6e64 6f6d 2049 7465 6d0a 0a47 656e 6572  ndom Item..Gener
+00004d90: 6174 6573 2061 2072 616e 646f 6d20 7661  ates a random va
+00004da0: 6c75 6520 6672 6f6d 2069 7465 6d73 2070  lue from items p
+00004db0: 726f 7669 6465 642e 2020 0a4e 4f54 4943  rovided.  .NOTIC
+00004dc0: 453a 2054 6865 2072 6177 2066 6f72 6d20  E: The raw form 
+00004dd0: 6f66 2074 6869 7320 4d69 6d65 6f20 5574  of this Mimeo Ut
+00004de0: 696c 2077 696c 6c20 6765 6e65 7261 7465  il will generate
+00004df0: 2061 2062 6c61 6e6b 2073 7472 696e 6720   a blank string 
+00004e00: 7661 6c75 6520 2861 7320 7361 6d65 2061  value (as same a
+00004e10: 7320 6e6f 2069 7465 6d73 2070 6172 616d  s no items param
+00004e20: 6574 7269 7a65 6429 2e0a 0a7c 2050 6172  etrized)...| Par
+00004e30: 616d 6574 6572 207c 2053 7570 706f 7274  ameter | Support
+00004e40: 6564 2076 616c 7565 7320 7c20 4465 6661  ed values | Defa
+00004e50: 756c 7420 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d  ult |.|:--------
+00004e60: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
+00004e70: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 3a7c  ----:|:-------:|
+00004e80: 0a7c 2020 2069 7465 6d73 2020 207c 2020  .|   items   |  
+00004e90: 2020 2020 606c 6973 7460 2020 2020 2020      `list`      
+00004ea0: 7c20 605b 2222 5d60 2020 7c0a 0a23 2323  | `[""]`  |..###
+00004eb0: 2323 2320 5061 7261 6d65 7472 697a 6564  ### Parametrized
+00004ec0: 0a0a 6060 606a 736f 6e0a 7b0a 2020 2272  ..```json.{.  "r
+00004ed0: 616e 646f 6d22 3a20 7b0a 2020 2020 225f  andom": {.    "_
+00004ee0: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
+00004ef0: 2020 2020 2022 5f6e 616d 6522 3a20 2272       "_name": "r
+00004f00: 616e 646f 6d5f 6974 656d 222c 0a20 2020  andom_item",.   
+00004f10: 2020 2022 6974 656d 7322 3a20 5b22 7661     "items": ["va
+00004f20: 6c75 6522 2c20 312c 2074 7275 655d 0a20  lue", 1, true]. 
+00004f30: 2020 207d 0a20 207d 0a7d 0a60 6060 0a0a     }.  }.}.```..
+00004f40: 2323 2323 2320 4461 7465 0a0a 4765 6e65  ##### Date..Gene
+00004f50: 7261 7465 7320 6120 6461 7465 2076 616c  rates a date val
+00004f60: 7565 2069 6e20 666f 726d 6174 2060 5959  ue in format `YY
+00004f70: 5959 2d4d 4d2d 4444 602e 0a0a 7c20 5061  YY-MM-DD`...| Pa
+00004f80: 7261 6d65 7465 7220 207c 2053 7570 706f  rameter  | Suppo
+00004f90: 7274 6564 2076 616c 7565 7320 7c20 4465  rted values | De
+00004fa0: 6661 756c 7420 7c0a 7c3a 2d2d 2d2d 2d2d  fault |.|:------
+00004fb0: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
+00004fc0: 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d  -------:|:------
+00004fd0: 2d3a 7c0a 7c20 6461 7973 5f64 656c 7461  -:|.| days_delta
+00004fe0: 207c 2020 2020 2020 6069 6e74 6020 2020   |      `int`   
+00004ff0: 2020 2020 7c20 2020 6030 6020 2020 7c0a      |   `0`   |.
+00005000: 0a23 2323 2323 2320 5261 770a 0a55 7365  .###### Raw..Use
+00005010: 7320 7468 6520 746f 6461 7927 7320 6461  s the today's da
+00005020: 7465 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20  te...```json.{. 
+00005030: 2022 546f 6461 7922 3a20 227b 6461 7465   "Today": "{date
+00005040: 7d22 0a7d 0a60 6060 0a0a 2323 2323 2323  }".}.```..######
+00005050: 2050 6172 616d 6574 7269 7a65 640a 0a55   Parametrized..U
+00005060: 7365 7320 7468 6520 6375 7374 6f6d 697a  ses the customiz
+00005070: 6564 2064 6179 7320 6465 6c74 612e 0a0a  ed days delta...
+00005080: 6060 606a 736f 6e0a 7b0a 2020 2259 6573  ```json.{.  "Yes
+00005090: 7465 7264 6179 223a 207b 0a20 2020 2022  terday": {.    "
+000050a0: 5f6d 696d 656f 5f75 7469 6c22 3a20 7b0a  _mimeo_util": {.
+000050b0: 2020 2020 2020 225f 6e61 6d65 223a 2022        "_name": "
+000050c0: 6461 7465 222c 0a20 2020 2020 2022 6461  date",.      "da
+000050d0: 7973 5f64 656c 7461 223a 202d 310a 2020  ys_delta": -1.  
+000050e0: 2020 7d0a 2020 7d2c 0a20 2022 546f 6d6f    }.  },.  "Tomo
+000050f0: 7272 6f77 223a 207b 0a20 2020 2022 5f6d  rrow": {.    "_m
+00005100: 696d 656f 5f75 7469 6c22 3a20 7b0a 2020  imeo_util": {.  
+00005110: 2020 2020 225f 6e61 6d65 223a 2022 6461      "_name": "da
+00005120: 7465 222c 0a20 2020 2020 2022 6461 7973  te",.      "days
+00005130: 5f64 656c 7461 223a 2031 0a20 2020 207d  _delta": 1.    }
+00005140: 0a20 207d 0a7d 0a60 6060 0a0a 2323 2323  .  }.}.```..####
+00005150: 2320 4461 7465 2054 696d 650a 0a47 656e  # Date Time..Gen
+00005160: 6572 6174 6573 2061 2064 6174 6520 7469  erates a date ti
+00005170: 6d65 2076 616c 7565 2069 6e20 666f 726d  me value in form
+00005180: 6174 2060 5959 5959 2d4d 4d2d 4444 2754  at `YYYY-MM-DD'T
+00005190: 2748 483a 6d6d 3a53 5360 2e0a 0a7c 2020  'HH:mm:SS`...|  
+000051a0: 2050 6172 616d 6574 6572 2020 207c 2053   Parameter   | S
+000051b0: 7570 706f 7274 6564 2076 616c 7565 7320  upported values 
+000051c0: 7c20 4465 6661 756c 7420 7c0a 7c3a 2d2d  | Default |.|:--
+000051d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
+000051e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
+000051f0: 3a2d 2d2d 2d2d 2d2d 3a7c 0a7c 2020 6461  :-------:|.|  da
+00005200: 7973 5f64 656c 7461 2020 207c 2020 2020  ys_delta   |    
+00005210: 2020 6069 6e74 6020 2020 2020 2020 7c20    `int`       | 
+00005220: 2020 6030 6020 2020 7c0a 7c20 2068 6f75    `0`   |.|  hou
+00005230: 7273 5f64 656c 7461 2020 7c20 2020 2020  rs_delta  |     
+00005240: 2060 696e 7460 2020 2020 2020 207c 2020   `int`       |  
+00005250: 2060 3060 2020 207c 0a7c 206d 696e 7574   `0`   |.| minut
+00005260: 6573 5f64 656c 7461 207c 2020 2020 2020  es_delta |      
+00005270: 6069 6e74 6020 2020 2020 2020 7c20 2020  `int`       |   
+00005280: 6030 6020 2020 7c0a 7c20 7365 636f 6e64  `0`   |.| second
+00005290: 735f 6465 6c74 6120 7c20 2020 2020 2060  s_delta |      `
+000052a0: 696e 7460 2020 2020 2020 207c 2020 2060  int`       |   `
+000052b0: 3060 2020 207c 0a0a 2323 2323 2323 2052  0`   |..###### R
+000052c0: 6177 0a0a 5573 6573 2074 6865 2063 7572  aw..Uses the cur
+000052d0: 7265 6e74 2074 696d 6573 7461 6d70 2e0a  rent timestamp..
+000052e0: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 4e6f  .```json.{.  "No
+000052f0: 7722 3a20 227b 6461 7465 5f74 696d 657d  w": "{date_time}
 00005300: 220a 7d0a 6060 600a 0a23 2323 2323 2320  ".}.```..###### 
 00005310: 5061 7261 6d65 7472 697a 6564 0a0a 5573  Parametrized..Us
-00005320: 6573 2061 2073 7065 6369 6669 6320 4d69  es a specific Mi
-00005330: 6d65 6f20 4d6f 6465 6c20 636f 6e74 6578  meo Model contex
-00005340: 7420 286d 6f64 656c 206e 616d 6520 7768  t (model name wh
-00005350: 656e 2060 636f 6e74 6578 7460 2069 7320  en `context` is 
-00005360: 6e6f 7420 636f 6e66 6967 7572 6564 292e  not configured).
-00005370: 0a0a 6060 606a 736f 6e0a 7b0a 2020 2250  ..```json.{.  "P
-00005380: 6172 656e 7422 3a20 7b0a 2020 2020 225f  arent": {.    "_
-00005390: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
-000053a0: 2020 2020 2022 5f6e 616d 6522 3a20 2263       "_name": "c
-000053b0: 7572 725f 6974 6572 222c 0a20 2020 2020  urr_iter",.     
-000053c0: 2022 636f 6e74 6578 7422 3a20 2253 6f6d   "context": "Som
-000053d0: 6545 6e74 6974 7922 0a20 2020 207d 0a20  eEntity".    }. 
-000053e0: 207d 0a7d 0a60 6060 0a0a 2323 2323 2320   }.}.```..##### 
-000053f0: 4b65 790a 0a47 656e 6572 6174 6573 2061  Key..Generates a
-00005400: 206b 6579 2075 6e69 7175 6520 6163 726f   key unique acro
-00005410: 7373 2061 6c6c 204d 696d 656f 204d 6f64  ss all Mimeo Mod
-00005420: 656c 7320 616e 6420 6265 696e 6720 7468  els and being th
-00005430: 6520 7361 6d65 2077 6974 6869 6e20 6120  e same within a 
-00005440: 7369 6e67 6c65 204d 696d 656f 204d 6f64  single Mimeo Mod
-00005450: 656c 2063 6f6e 7465 7874 2e0a 0a7c 2050  el context...| P
-00005460: 6172 616d 6574 6572 207c 2053 7570 706f  arameter | Suppo
-00005470: 7274 6564 2076 616c 7565 7320 7c20 2020  rted values |   
-00005480: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00005490: 6c74 2020 2020 2020 2020 2020 2020 2020  lt              
-000054a0: 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 3a7c   |.|:---------:|
-000054b0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-000054c0: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
-000054d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000054e0: 2d2d 2d2d 2d2d 3a7c 0a7c 2020 636f 6e74  ------:|.|  cont
-000054f0: 6578 7420 207c 2020 2020 2020 6073 7472  ext  |      `str
-00005500: 6020 2020 2020 2020 7c20 2020 2020 2020  `       |       
-00005510: 2020 6120 6375 7272 656e 7420 636f 6e74    a current cont
-00005520: 6578 7420 2020 2020 2020 2020 207c 0a7c  ext          |.|
-00005530: 2069 7465 7261 7469 6f6e 207c 2020 2020   iteration |    
-00005540: 2020 6069 6e74 6020 2020 2020 2020 7c20    `int`       | 
-00005550: 6120 6375 7272 656e 7420 6974 6572 6174  a current iterat
-00005560: 696f 6e20 6f66 2074 6865 2063 6f6e 7465  ion of the conte
-00005570: 7874 207c 0a0a 2323 2323 2323 2052 6177  xt |..###### Raw
-00005580: 0a0a 5573 6573 2061 206b 6579 2066 726f  ..Uses a key fro
-00005590: 6d20 7468 6520 6375 7272 656e 7420 636f  m the current co
-000055a0: 6e74 6578 7420 616e 6420 6974 6572 6174  ntext and iterat
-000055b0: 696f 6e2e 0a0a 6060 606a 736f 6e0a 7b0a  ion...```json.{.
-000055c0: 2020 2249 4422 3a20 227b 6b65 797d 220a    "ID": "{key}".
-000055d0: 7d0a 6060 600a 0a23 2323 2323 2320 5061  }.```..###### Pa
-000055e0: 7261 6d65 7472 697a 6564 0a0a 5573 6573  rametrized..Uses
-000055f0: 2061 206b 6579 2066 726f 6d20 7468 6520   a key from the 
-00005600: 7370 6563 6966 6963 2063 6f6e 7465 7874  specific context
-00005610: 2061 6e64 2069 7465 7261 7469 6f6e 2e20   and iteration. 
-00005620: 200a 5768 656e 2063 6f6e 7465 7874 2069   .When context i
-00005630: 7320 696e 6469 6361 7465 6420 616e 6420  s indicated and 
-00005640: 6974 6572 6174 696f 6e20 6973 206e 6f74  iteration is not
-00005650: 2c20 7468 656e 2074 6865 2063 7572 7265  , then the curre
-00005660: 6e74 2069 7465 7261 7469 6f6e 202a 2a6f  nt iteration **o
-00005670: 6620 7468 6520 696e 6469 6361 7465 6420  f the indicated 
-00005680: 636f 6e74 6578 742a 2a20 6973 2062 6569  context** is bei
-00005690: 6e67 2075 7365 642e 0a0a 6060 606a 736f  ng used...```jso
-000056a0: 6e0a 7b0a 2020 2253 6f6d 6545 6e74 6974  n.{.  "SomeEntit
-000056b0: 7932 223a 207b 0a20 2020 2022 5f6d 696d  y2": {.    "_mim
-000056c0: 656f 5f75 7469 6c22 3a20 7b0a 2020 2020  eo_util": {.    
-000056d0: 2020 225f 6e61 6d65 223a 2022 6b65 7922    "_name": "key"
-000056e0: 2c0a 2020 2020 2020 2263 6f6e 7465 7874  ,.      "context
-000056f0: 223a 2022 536f 6d65 456e 7469 7479 222c  ": "SomeEntity",
-00005700: 0a20 2020 2020 2022 6974 6572 6174 696f  .      "iteratio
-00005710: 6e22 3a20 227b 6375 7272 5f69 7465 727d  n": "{curr_iter}
-00005720: 220a 2020 2020 7d0a 2020 7d0a 7d0a 6060  ".    }.  }.}.``
-00005730: 600a 0a23 2323 2323 2043 6974 790a 0a47  `..##### City..G
-00005740: 656e 6572 6174 6573 2061 2063 6974 7920  enerates a city 
-00005750: 6e61 6d65 2e0a 0a7c 2050 6172 616d 6574  name...| Paramet
-00005760: 6572 207c 2053 7570 706f 7274 6564 2076  er | Supported v
-00005770: 616c 7565 7320 7c20 4465 6661 756c 7420  alues | Default 
-00005780: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a  |.|:---------:|:
-00005790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000057a0: 3a7c 3a2d 2d2d 2d2d 2d2d 3a7c 0a7c 2020  :|:-------:|.|  
-000057b0: 756e 6971 7565 2020 207c 2020 2020 2020  unique   |      
-000057c0: 6062 6f6f 6c60 2020 2020 2020 7c20 6054  `bool`      | `T
-000057d0: 7275 6560 2020 7c0a 7c20 2063 6f75 6e74  rue`  |.|  count
-000057e0: 7279 2020 7c20 2020 2020 2060 7374 7260  ry  |      `str`
-000057f0: 2020 2020 2020 207c 2060 4e6f 6e65 6020         | `None` 
-00005800: 207c 0a0a 2323 2323 2323 2052 6177 0a0a   |..###### Raw..
-00005810: 4279 2064 6566 6175 6c74 2063 6974 7920  By default city 
-00005820: 6e61 6d65 7320 7769 6c6c 2062 6520 756e  names will be un
-00005830: 6971 7565 2061 6372 6f73 7320 6120 4d69  ique across a Mi
-00005840: 6d65 6f20 436f 6e74 6578 742e 0a0a 6060  meo Context...``
-00005850: 606a 736f 6e0a 7b0a 2020 2243 6974 7922  `json.{.  "City"
-00005860: 3a20 227b 6369 7479 7d22 0a7d 0a60 6060  : "{city}".}.```
-00005870: 0a0a 2323 2323 2323 2050 6172 616d 6574  ..###### Paramet
-00005880: 7269 7a65 640a 0a55 7365 7320 636f 756e  rized..Uses coun
-00005890: 7472 7920 286e 616d 652c 2069 736f 322c  try (name, iso2,
-000058a0: 2069 736f 3329 2061 6e64 2060 756e 6971   iso3) and `uniq
-000058b0: 7565 6020 666c 6167 2074 6f20 6765 6e65  ue` flag to gene
-000058c0: 7261 7465 2061 2063 6974 7920 6e61 6d65  rate a city name
-000058d0: 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  ...```json.{.  "
-000058e0: 4369 7479 5769 7468 4475 706c 6963 6174  CityWithDuplicat
-000058f0: 6573 223a 207b 0a20 2020 2022 5f6d 696d  es": {.    "_mim
-00005900: 656f 5f75 7469 6c22 3a20 7b0a 2020 2020  eo_util": {.    
-00005910: 2020 225f 6e61 6d65 223a 2022 6369 7479    "_name": "city
-00005920: 222c 0a20 2020 2020 2022 756e 6971 7565  ",.      "unique
-00005930: 223a 2066 616c 7365 0a20 2020 207d 0a20  ": false.    }. 
-00005940: 207d 2c0a 2020 2243 6974 794f 6643 6f75   },.  "CityOfCou
-00005950: 6e74 7279 4e61 6d65 223a 207b 0a20 2020  ntryName": {.   
-00005960: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
-00005970: 7b0a 2020 2020 2020 225f 6e61 6d65 223a  {.      "_name":
-00005980: 2022 6369 7479 222c 0a20 2020 2020 2022   "city",.      "
-00005990: 636f 756e 7472 7922 3a20 2255 6e69 7465  country": "Unite
-000059a0: 6420 4b69 6e67 646f 6d22 0a20 2020 207d  d Kingdom".    }
-000059b0: 0a20 207d 2c0a 2020 2243 6974 794f 6643  .  },.  "CityOfC
-000059c0: 6f75 6e74 7279 4953 4f32 223a 207b 0a20  ountryISO2": {. 
-000059d0: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
-000059e0: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
-000059f0: 223a 2022 6369 7479 222c 0a20 2020 2020  ": "city",.     
-00005a00: 2022 636f 756e 7472 7922 3a20 2247 4222   "country": "GB"
-00005a10: 0a20 2020 207d 0a20 207d 2c0a 2020 2243  .    }.  },.  "C
-00005a20: 6974 794f 6643 6f75 6e74 7279 4953 4f33  ityOfCountryISO3
-00005a30: 223a 207b 0a20 2020 2022 5f6d 696d 656f  ": {.    "_mimeo
-00005a40: 5f75 7469 6c22 3a20 7b0a 2020 2020 2020  _util": {.      
-00005a50: 225f 6e61 6d65 223a 2022 6369 7479 222c  "_name": "city",
-00005a60: 0a20 2020 2020 2022 636f 756e 7472 7922  .      "country"
-00005a70: 3a20 2247 4252 220a 2020 2020 7d0a 2020  : "GBR".    }.  
-00005a80: 7d2c 0a20 2022 4369 7479 4f66 436f 756e  },.  "CityOfCoun
-00005a90: 7472 7957 6974 6844 7570 6c69 6361 7465  tryWithDuplicate
-00005aa0: 7322 3a20 7b0a 2020 2020 225f 6d69 6d65  s": {.    "_mime
-00005ab0: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
-00005ac0: 2022 5f6e 616d 6522 3a20 2263 6974 7922   "_name": "city"
-00005ad0: 2c0a 2020 2020 2020 2263 6f75 6e74 7279  ,.      "country
-00005ae0: 223a 2022 556e 6974 6564 204b 696e 6764  ": "United Kingd
-00005af0: 6f6d 222c 0a20 2020 2020 2022 756e 6971  om",.      "uniq
-00005b00: 7565 223a 2066 616c 7365 0a20 2020 207d  ue": false.    }
-00005b10: 0a20 207d 0a7d 0a60 6060 0a0a 2323 2323  .  }.}.```..####
-00005b20: 2320 436f 756e 7472 790a 0a47 656e 6572  # Country..Gener
-00005b30: 6174 6573 2061 2063 6f75 6e74 7279 206e  ates a country n
-00005b40: 616d 6520 2862 7920 6465 6661 756c 7429  ame (by default)
-00005b50: 2c20 6973 6f32 206f 7220 6973 6f33 2e0a  , iso2 or iso3..
-00005b60: 0a7c 2050 6172 616d 6574 6572 207c 2020  .| Parameter |  
-00005b70: 2020 2020 2053 7570 706f 7274 6564 2076       Supported v
-00005b80: 616c 7565 7320 2020 2020 2020 7c20 4465  alues       | De
-00005b90: 6661 756c 7420 207c 0a7c 3a2d 2d2d 2d2d  fault  |.|:-----
-00005ba0: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00005bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005bc0: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 3a7c  ---:|:--------:|
-00005bd0: 0a7c 2020 756e 6971 7565 2020 207c 2020  .|  unique   |  
-00005be0: 2020 2020 2020 2020 2020 6062 6f6f 6c60            `bool`
-00005bf0: 2020 2020 2020 2020 2020 2020 7c20 2060              |  `
-00005c00: 5472 7565 6020 207c 0a7c 2020 2076 616c  True`  |.|   val
-00005c10: 7565 2020 207c 2060 226e 616d 6522 602c  ue   | `"name"`,
-00005c20: 2060 2269 736f 3322 602c 2060 2269 736f   `"iso3"`, `"iso
-00005c30: 3222 6020 7c20 6022 6e61 6d65 2260 207c  2"` | `"name"` |
-00005c40: 0a7c 2020 636f 756e 7472 7920 207c 2020  .|  country  |  
-00005c50: 2020 2020 2020 2020 2020 6073 7472 6020            `str` 
-00005c60: 2020 2020 2020 2020 2020 2020 7c20 2060              |  `
-00005c70: 4e6f 6e65 6020 207c 0a0a 2323 2323 2323  None`  |..######
-00005c80: 2052 6177 0a0a 4279 2064 6566 6175 6c74   Raw..By default
-00005c90: 2063 6f75 6e74 7279 206e 616d 6573 2077   country names w
-00005ca0: 696c 6c20 6265 2075 6e69 7175 6520 6163  ill be unique ac
-00005cb0: 726f 7373 2061 204d 696d 656f 2043 6f6e  ross a Mimeo Con
-00005cc0: 7465 7874 2e0a 0a60 6060 6a73 6f6e 0a7b  text...```json.{
-00005cd0: 0a20 2022 436f 756e 7472 7922 3a20 227b  .  "Country": "{
-00005ce0: 636f 756e 7472 797d 220a 7d0a 6060 600a  country}".}.```.
-00005cf0: 0a23 2323 2323 2320 5061 7261 6d65 7472  .###### Parametr
-00005d00: 697a 6564 0a0a 4974 2063 616e 2067 656e  ized..It can gen
-00005d10: 6572 6174 653a 0a2d 2063 6f75 6e74 7279  erate:.- country
-00005d20: 2069 736f 3320 6f72 2069 736f 2032 2069   iso3 or iso 2 i
-00005d30: 6e73 7465 6164 206f 6620 6e61 6d65 0a2d  nstead of name.-
-00005d40: 2063 6f75 6e74 7279 2077 6974 6820 6475   country with du
-00005d50: 706c 6963 6174 6573 0a2d 2063 6f75 6e74  plicates.- count
-00005d60: 7279 206e 616d 6520 666f 7220 6120 7072  ry name for a pr
-00005d70: 6f76 6964 6564 2069 736f 3320 6f72 2069  ovided iso3 or i
-00005d80: 736f 320a 2d20 636f 756e 7472 7920 6973  so2.- country is
-00005d90: 6f32 2066 6f72 2061 2070 726f 7669 6465  o2 for a provide
-00005da0: 6420 6e61 6d65 206f 7220 6973 6f33 0a2d  d name or iso3.-
-00005db0: 2063 6f75 6e74 7279 2069 736f 3320 666f   country iso3 fo
-00005dc0: 7220 6120 7072 6f76 6964 6564 206e 616d  r a provided nam
-00005dd0: 6520 6f72 2069 736f 320a 0a57 6865 6e20  e or iso2..When 
-00005de0: 7468 6520 6063 6f75 6e74 7279 6020 7061  the `country` pa
-00005df0: 7261 6d20 6973 2070 726f 7669 6465 6420  ram is provided 
-00005e00: 7468 656e 2074 6865 2060 756e 6971 7565  then the `unique
-00005e10: 6020 666c 6167 2069 7320 6967 6e6f 7265  ` flag is ignore
-00005e20: 642e 0a0a 6060 606a 736f 6e0a 7b0a 2020  d...```json.{.  
-00005e30: 2243 6f75 6e74 7279 4e61 6d65 5769 7468  "CountryNameWith
-00005e40: 4475 706c 6963 6174 6573 223a 207b 0a20  Duplicates": {. 
-00005e50: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
-00005e60: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
-00005e70: 223a 2022 636f 756e 7472 7922 2c0a 2020  ": "country",.  
-00005e80: 2020 2020 2275 6e69 7175 6522 3a20 6661      "unique": fa
-00005e90: 6c73 650a 2020 2020 7d0a 2020 7d2c 0a20  lse.    }.  },. 
-00005ea0: 2022 436f 756e 7472 7949 534f 3222 3a20   "CountryISO2": 
-00005eb0: 7b0a 2020 2020 225f 6d69 6d65 6f5f 7574  {.    "_mimeo_ut
-00005ec0: 696c 223a 207b 0a20 2020 2020 2022 5f6e  il": {.      "_n
-00005ed0: 616d 6522 3a20 2263 6f75 6e74 7279 222c  ame": "country",
-00005ee0: 0a20 2020 2020 2022 7661 6c75 6522 3a20  .      "value": 
-00005ef0: 2269 736f 3222 0a20 2020 207d 0a20 207d  "iso2".    }.  }
-00005f00: 2c0a 2020 2243 6f75 6e74 7279 4953 4f33  ,.  "CountryISO3
-00005f10: 223a 207b 0a20 2020 2022 5f6d 696d 656f  ": {.    "_mimeo
-00005f20: 5f75 7469 6c22 3a20 7b0a 2020 2020 2020  _util": {.      
-00005f30: 225f 6e61 6d65 223a 2022 636f 756e 7472  "_name": "countr
-00005f40: 7922 2c0a 2020 2020 2020 2276 616c 7565  y",.      "value
-00005f50: 223a 2022 6973 6f33 220a 2020 2020 7d0a  ": "iso3".    }.
-00005f60: 2020 7d2c 0a20 2022 436f 756e 7472 794e    },.  "CountryN
-00005f70: 616d 6546 6f72 4953 4f33 223a 207b 0a20  ameForISO3": {. 
-00005f80: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
-00005f90: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
-00005fa0: 223a 2022 636f 756e 7472 7922 2c0a 2020  ": "country",.  
-00005fb0: 2020 2020 2263 6f75 6e74 7279 223a 2022      "country": "
-00005fc0: 4742 5222 0a20 2020 207d 0a20 207d 2c0a  GBR".    }.  },.
-00005fd0: 2020 2243 6f75 6e74 7279 4953 4f32 466f    "CountryISO2Fo
-00005fe0: 724e 616d 6522 3a20 7b0a 2020 2020 225f  rName": {.    "_
-00005ff0: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
-00006000: 2020 2020 2022 5f6e 616d 6522 3a20 2263       "_name": "c
-00006010: 6f75 6e74 7279 222c 0a20 2020 2020 2022  ountry",.      "
-00006020: 7661 6c75 6522 3a20 2269 736f 3222 2c0a  value": "iso2",.
-00006030: 2020 2020 2020 2263 6f75 6e74 7279 223a        "country":
-00006040: 2022 556e 6974 6564 204b 696e 6764 6f6d   "United Kingdom
-00006050: 220a 2020 2020 7d0a 2020 7d0a 7d0a 6060  ".    }.  }.}.``
-00006060: 600a 0a23 2323 2323 2043 7572 7265 6e63  `..##### Currenc
-00006070: 790a 0a47 656e 6572 6174 6573 2061 2063  y..Generates a c
-00006080: 7572 7265 6e63 7920 636f 6465 2028 6279  urrency code (by
-00006090: 2064 6566 6175 6c74 2920 6f72 206e 616d   default) or nam
-000060a0: 652e 0a0a 7c20 5061 7261 6d65 7465 7220  e...| Parameter 
-000060b0: 7c20 2053 7570 706f 7274 6564 2076 616c  |  Supported val
-000060c0: 7565 7320 207c 2044 6566 6175 6c74 2020  ues  | Default  
-000060d0: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a  |.|:---------:|:
-000060e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000060f0: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d3a 7c0a  --:|:--------:|.
-00006100: 7c20 2075 6e69 7175 6520 2020 7c20 2020  |  unique   |   
-00006110: 2020 2020 6062 6f6f 6c60 2020 2020 2020      `bool`      
-00006120: 207c 2060 4661 6c73 6560 2020 7c0a 7c20   | `False`  |.| 
-00006130: 2020 7661 6c75 6520 2020 7c20 6022 636f    value   | `"co
-00006140: 6465 2260 2c20 6022 6e61 6d65 2260 207c  de"`, `"name"` |
-00006150: 2060 2263 6f64 6522 6020 7c0a 7c20 2063   `"code"` |.|  c
-00006160: 6f75 6e74 7279 2020 7c20 2020 2020 2020  ountry  |       
-00006170: 6073 7472 6020 2020 2020 2020 207c 2020  `str`        |  
-00006180: 604e 6f6e 6560 2020 7c0a 0a23 2323 2323  `None`  |..#####
-00006190: 2320 5261 770a 0a42 7920 6465 6661 756c  # Raw..By defaul
-000061a0: 7420 6369 7479 206e 616d 6573 2077 696c  t city names wil
-000061b0: 6c20 5f4e 4f54 5f20 6265 2075 6e69 7175  l _NOT_ be uniqu
-000061c0: 6520 6163 726f 7373 2061 204d 696d 656f  e across a Mimeo
-000061d0: 2043 6f6e 7465 7874 2e0a 0a60 6060 6a73   Context...```js
-000061e0: 6f6e 0a7b 0a20 2022 4375 7272 656e 6379  on.{.  "Currency
-000061f0: 223a 2022 7b63 7572 7265 6e63 797d 220a  ": "{currency}".
-00006200: 7d0a 6060 600a 0a23 2323 2323 2320 5061  }.```..###### Pa
-00006210: 7261 6d65 7472 697a 6564 0a0a 4974 2063  rametrized..It c
-00006220: 616e 2067 656e 6572 6174 653a 0a2d 2075  an generate:.- u
-00006230: 6e69 7175 6520 6375 7272 656e 6369 6573  nique currencies
-00006240: 0a2d 2063 7572 7265 6e63 7920 6e61 6d65  .- currency name
-00006250: 2069 6e73 7465 6164 206f 6620 636f 6465   instead of code
-00006260: 0a2d 2063 7572 7265 6e63 7920 636f 6465  .- currency code
-00006270: 206f 7220 6e61 6d65 206f 6620 6120 7370   or name of a sp
-00006280: 6563 6966 6963 2063 6f75 6e74 7279 2028  ecific country (
-00006290: 7573 696e 6720 6973 6f33 2c20 6973 6f32  using iso3, iso2
-000062a0: 206f 7220 6e61 6d65 290a 0a57 6865 6e20   or name)..When 
-000062b0: 7468 6520 6063 6f75 6e74 7279 6020 7061  the `country` pa
-000062c0: 7261 6d20 6973 2070 726f 7669 6465 6420  ram is provided 
-000062d0: 7468 656e 2074 6865 2060 756e 6971 7565  then the `unique
-000062e0: 6020 666c 6167 2069 7320 6967 6e6f 7265  ` flag is ignore
-000062f0: 642e 0a0a 6060 606a 736f 6e0a 7b0a 2020  d...```json.{.  
-00006300: 2255 6e69 7175 6543 7572 7265 6e63 7943  "UniqueCurrencyC
-00006310: 6f64 6522 3a20 7b0a 2020 2020 225f 6d69  ode": {.    "_mi
-00006320: 6d65 6f5f 7574 696c 223a 207b 0a20 2020  meo_util": {.   
-00006330: 2020 2022 5f6e 616d 6522 3a20 2263 7572     "_name": "cur
-00006340: 7265 6e63 7922 2c0a 2020 2020 2020 2275  rency",.      "u
-00006350: 6e69 7175 6522 3a20 7472 7565 0a20 2020  nique": true.   
-00006360: 207d 0a20 207d 2c0a 2020 2243 7572 7265   }.  },.  "Curre
-00006370: 6e63 794e 616d 6522 3a20 7b0a 2020 2020  ncyName": {.    
-00006380: 225f 6d69 6d65 6f5f 7574 696c 223a 207b  "_mimeo_util": {
-00006390: 0a20 2020 2020 2022 5f6e 616d 6522 3a20  .      "_name": 
-000063a0: 2263 7572 7265 6e63 7922 2c0a 2020 2020  "currency",.    
-000063b0: 2020 2276 616c 7565 223a 2022 6e61 6d65    "value": "name
-000063c0: 220a 2020 2020 7d0a 2020 7d2c 0a20 2022  ".    }.  },.  "
-000063d0: 4375 7272 656e 6379 436f 6465 466f 7243  CurrencyCodeForC
-000063e0: 6f75 6e74 7279 4953 4f33 223a 207b 0a20  ountryISO3": {. 
-000063f0: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
-00006400: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
-00006410: 223a 2022 6375 7272 656e 6379 222c 0a20  ": "currency",. 
-00006420: 2020 2020 2022 636f 756e 7472 7922 3a20       "country": 
-00006430: 2247 4252 220a 2020 2020 7d0a 2020 7d2c  "GBR".    }.  },
-00006440: 0a20 2022 4375 7272 656e 6379 4e61 6d65  .  "CurrencyName
-00006450: 466f 7243 6f75 6e74 7279 4953 4f32 223a  ForCountryISO2":
-00006460: 207b 0a20 2020 2022 5f6d 696d 656f 5f75   {.    "_mimeo_u
-00006470: 7469 6c22 3a20 7b0a 2020 2020 2020 225f  til": {.      "_
-00006480: 6e61 6d65 223a 2022 6375 7272 656e 6379  name": "currency
-00006490: 222c 0a20 2020 2020 2022 7661 6c75 6522  ",.      "value"
-000064a0: 3a20 226e 616d 6522 2c0a 2020 2020 2020  : "name",.      
-000064b0: 2263 6f75 6e74 7279 223a 2022 4742 220a  "country": "GB".
-000064c0: 2020 2020 7d0a 2020 7d2c 0a20 2022 4375      }.  },.  "Cu
-000064d0: 7272 656e 6379 4e61 6d65 466f 7243 6f75  rrencyNameForCou
-000064e0: 6e74 7279 4e61 6d65 223a 207b 0a20 2020  ntryName": {.   
-000064f0: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
-00006500: 7b0a 2020 2020 2020 225f 6e61 6d65 223a  {.      "_name":
-00006510: 2022 6375 7272 656e 6379 222c 0a20 2020   "currency",.   
-00006520: 2020 2022 7661 6c75 6522 3a20 226e 616d     "value": "nam
-00006530: 6522 2c0a 2020 2020 2020 2263 6f75 6e74  e",.      "count
-00006540: 7279 223a 2022 556e 6974 6564 204b 696e  ry": "United Kin
-00006550: 6764 6f6d 220a 2020 2020 7d0a 2020 7d0a  gdom".    }.  }.
-00006560: 7d0a 6060 600a 0a23 2323 2323 2046 6972  }.```..##### Fir
-00006570: 7374 204e 616d 650a 0a47 656e 6572 6174  st Name..Generat
-00006580: 6573 2061 2066 6972 7374 206e 616d 652e  es a first name.
-00006590: 0a0a 7c20 5061 7261 6d65 7465 7220 7c20  ..| Parameter | 
-000065a0: 2020 2020 2053 7570 706f 7274 6564 2076       Supported v
-000065b0: 616c 7565 7320 2020 2020 207c 2044 6566  alues      | Def
-000065c0: 6175 6c74 2020 7c0a 7c3a 2d2d 2d2d 2d2d  ault  |.|:------
-000065d0: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
-000065e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000065f0: 3a7c 3a2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20  :|:--------:|.| 
-00006600: 2075 6e69 7175 6520 2020 7c20 2020 2020   unique   |     
-00006610: 2020 2020 2020 6062 6f6f 6c60 2020 2020        `bool`    
-00006620: 2020 2020 2020 207c 2020 6054 7275 6560         |  `True`
-00006630: 2020 7c0a 7c20 2020 2073 6578 2020 2020    |.|    sex    
-00006640: 7c20 604d 602c 2060 4d61 6c65 602c 2060  | `M`, `Male`, `
-00006650: 4660 2c20 6046 656d 616c 6560 207c 2020  F`, `Female` |  
-00006660: 604e 6f6e 6560 2020 7c0a 0a23 2323 2323  `None`  |..#####
-00006670: 2320 5261 770a 0a42 7920 6465 6661 756c  # Raw..By defaul
-00006680: 7420 6669 7273 7420 6e61 6d65 7320 7769  t first names wi
-00006690: 6c6c 2062 6520 756e 6971 7565 2061 6372  ll be unique acr
-000066a0: 6f73 7320 6120 4d69 6d65 6f20 436f 6e74  oss a Mimeo Cont
-000066b0: 6578 742e 0a0a 6060 606a 736f 6e0a 7b0a  ext...```json.{.
-000066c0: 2020 2246 6972 7374 4e61 6d65 223a 2022    "FirstName": "
-000066d0: 7b66 6972 7374 5f6e 616d 657d 220a 7d0a  {first_name}".}.
-000066e0: 6060 600a 0a23 2323 2323 2320 5061 7261  ```..###### Para
-000066f0: 6d65 7472 697a 6564 0a0a 5573 6573 2073  metrized..Uses s
-00006700: 6578 2028 604d 6020 2f20 604d 616c 6560  ex (`M` / `Male`
-00006710: 202f 2060 4660 202f 2060 4665 6d61 6c65   / `F` / `Female
-00006720: 6029 2061 6e64 2060 756e 6971 7565 6020  `) and `unique` 
-00006730: 666c 6167 2074 6f20 6765 6e65 7261 7465  flag to generate
-00006740: 2061 2066 6972 7374 206e 616d 652e 0a0a   a first name...
-00006750: 6060 606a 736f 6e0a 7b0a 2020 2246 6972  ```json.{.  "Fir
-00006760: 7374 4e61 6d65 5769 7468 4475 706c 6963  stNameWithDuplic
-00006770: 6174 6573 223a 207b 0a20 2020 2022 5f6d  ates": {.    "_m
-00006780: 696d 656f 5f75 7469 6c22 3a20 7b0a 2020  imeo_util": {.  
-00006790: 2020 2020 225f 6e61 6d65 223a 2022 6669      "_name": "fi
-000067a0: 7273 745f 6e61 6d65 222c 0a20 2020 2020  rst_name",.     
-000067b0: 2022 756e 6971 7565 223a 2066 616c 7365   "unique": false
-000067c0: 0a20 2020 207d 0a20 207d 2c0a 2020 224d  .    }.  },.  "M
-000067d0: 616c 6546 6972 7374 4e61 6d65 223a 207b  aleFirstName": {
-000067e0: 0a20 2020 2022 5f6d 696d 656f 5f75 7469  .    "_mimeo_uti
-000067f0: 6c22 3a20 7b0a 2020 2020 2020 225f 6e61  l": {.      "_na
-00006800: 6d65 223a 2022 6669 7273 745f 6e61 6d65  me": "first_name
-00006810: 222c 0a20 2020 2020 2022 7365 7822 3a20  ",.      "sex": 
-00006820: 224d 220a 2020 2020 7d0a 2020 7d2c 0a20  "M".    }.  },. 
-00006830: 2022 4665 6d61 6c65 4669 7273 744e 616d   "FemaleFirstNam
-00006840: 6522 3a20 7b0a 2020 2020 225f 6d69 6d65  e": {.    "_mime
-00006850: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
-00006860: 2022 5f6e 616d 6522 3a20 2266 6972 7374   "_name": "first
-00006870: 5f6e 616d 6522 2c0a 2020 2020 2020 2273  _name",.      "s
-00006880: 6578 223a 2022 4622 0a20 2020 207d 0a20  ex": "F".    }. 
-00006890: 207d 2c0a 2020 224d 616c 6546 6972 7374   },.  "MaleFirst
-000068a0: 4e61 6d65 5769 7468 4475 706c 6963 6174  NameWithDuplicat
-000068b0: 6573 223a 207b 0a20 2020 2022 5f6d 696d  es": {.    "_mim
-000068c0: 656f 5f75 7469 6c22 3a20 7b0a 2020 2020  eo_util": {.    
-000068d0: 2020 225f 6e61 6d65 223a 2022 6669 7273    "_name": "firs
-000068e0: 745f 6e61 6d65 222c 0a20 2020 2020 2022  t_name",.      "
-000068f0: 7365 7822 3a20 224d 222c 0a20 2020 2020  sex": "M",.     
-00006900: 2022 756e 6971 7565 223a 2066 616c 7365   "unique": false
-00006910: 0a20 2020 207d 0a20 207d 0a7d 0a60 6060  .    }.  }.}.```
-00006920: 0a0a 2323 2323 2320 4c61 7374 204e 616d  ..##### Last Nam
-00006930: 650a 0a47 656e 6572 6174 6573 2061 206c  e..Generates a l
-00006940: 6173 7420 6e61 6d65 2e0a 0a7c 2050 6172  ast name...| Par
-00006950: 616d 6574 6572 207c 2053 7570 706f 7274  ameter | Support
-00006960: 6564 2076 616c 7565 7320 7c20 4465 6661  ed values | Defa
-00006970: 756c 7420 207c 0a7c 3a2d 2d2d 2d2d 2d2d  ult  |.|:-------
-00006980: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
-00006990: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-000069a0: 3a7c 0a7c 2020 756e 6971 7565 2020 207c  :|.|  unique   |
-000069b0: 2020 2020 2020 6062 6f6f 6c60 2020 2020        `bool`    
-000069c0: 2020 7c20 2060 5472 7565 6020 207c 0a0a    |  `True`  |..
-000069d0: 2323 2323 2323 2052 6177 0a0a 4279 2064  ###### Raw..By d
-000069e0: 6566 6175 6c74 206c 6173 7420 6e61 6d65  efault last name
-000069f0: 7320 7769 6c6c 2062 6520 756e 6971 7565  s will be unique
-00006a00: 2061 6372 6f73 7320 6120 4d69 6d65 6f20   across a Mimeo 
-00006a10: 436f 6e74 6578 742e 0a0a 6060 606a 736f  Context...```jso
-00006a20: 6e0a 7b0a 2020 224c 6173 744e 616d 6522  n.{.  "LastName"
-00006a30: 3a20 227b 6c61 7374 5f6e 616d 657d 220a  : "{last_name}".
-00006a40: 7d0a 6060 600a 0a23 2323 2323 2320 5061  }.```..###### Pa
-00006a50: 7261 6d65 7472 697a 6564 0a0a 5573 6573  rametrized..Uses
-00006a60: 2060 756e 6971 7565 6020 666c 6167 2074   `unique` flag t
-00006a70: 6f20 6765 6e65 7261 7465 2061 206c 6173  o generate a las
-00006a80: 7420 6e61 6d65 2e0a 0a60 6060 6a73 6f6e  t name...```json
-00006a90: 0a7b 0a20 2022 4c61 7374 4e61 6d65 5769  .{.  "LastNameWi
-00006aa0: 7468 4475 706c 6963 6174 6573 223a 207b  thDuplicates": {
-00006ab0: 0a20 2020 2022 5f6d 696d 656f 5f75 7469  .    "_mimeo_uti
-00006ac0: 6c22 3a20 7b0a 2020 2020 2020 225f 6e61  l": {.      "_na
-00006ad0: 6d65 223a 2022 6c61 7374 5f6e 616d 6522  me": "last_name"
-00006ae0: 2c0a 2020 2020 2020 2275 6e69 7175 6522  ,.      "unique"
-00006af0: 3a20 6661 6c73 650a 2020 2020 7d0a 2020  : false.    }.  
-00006b00: 7d0a 7d0a 6060 600a 0a0a 2323 204c 6963  }.}.```...## Lic
-00006b10: 656e 7365 0a0a 4d49 540a 0a0a 2323 2041  ense..MIT...## A
-00006b20: 7574 686f 7273 0a0a 2d20 5b40 546f 6d61  uthors..- [@Toma
-00006b30: 737a 416e 696f 6c6f 7773 6b69 5d28 6874  szAniolowski](ht
-00006b40: 7470 733a 2f2f 7777 772e 6769 7468 7562  tps://www.github
-00006b50: 2e63 6f6d 2f54 6f6d 6173 7a41 6e69 6f6c  .com/TomaszAniol
-00006b60: 6f77 736b 6929 0a0a 0a23 2320 4163 6b6e  owski)...## Ackn
-00006b70: 6f77 6c65 6467 656d 656e 7473 0a0a 202d  owledgements.. -
-00006b80: 205b 5369 6d70 6c65 4d61 7073 2e63 6f6d   [SimpleMaps.com
-00006b90: 5d28 6874 7470 733a 2f2f 7369 6d70 6c65  ](https://simple
-00006ba0: 6d61 7073 2e63 6f6d 2f64 6174 612f 776f  maps.com/data/wo
-00006bb0: 726c 642d 6369 7469 6573 2920 2843 6974  rld-cities) (Cit
-00006bc0: 6965 7320 2620 636f 756e 7472 6965 7320  ies & countries 
-00006bd0: 6461 7461 290a 202d 205b 4068 6164 6c65  data). - [@hadle
-00006be0: 792f 6461 7461 2d62 6162 792d 6e61 6d65  y/data-baby-name
-00006bf0: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00006c00: 622e 636f 6d2f 6861 646c 6579 2f64 6174  b.com/hadley/dat
-00006c10: 612d 6261 6279 2d6e 616d 6573 2f29 2028  a-baby-names/) (
-00006c20: 466f 7265 6e61 6d65 7320 6461 7461 290a  Forenames data).
-00006c30: 202d 205b 4066 6976 6574 6869 7274 7965   - [@fivethirtye
-00006c40: 6967 682f 6461 7461 2f6d 6f73 742d 636f  igh/data/most-co
-00006c50: 6d6d 6f6e 2d6e 616d 655d 2868 7474 7073  mmon-name](https
-00006c60: 3a2f 2f67 6974 6875 622e 636f 6d2f 6669  ://github.com/fi
-00006c70: 7665 7468 6972 7479 6569 6768 742f 6461  vethirtyeight/da
-00006c80: 7461 2f74 7265 652f 6d61 7374 6572 2f6d  ta/tree/master/m
-00006c90: 6f73 742d 636f 6d6d 6f6e 2d6e 616d 6529  ost-common-name)
-00006ca0: 2028 5375 726e 616d 6573 2064 6174 6129   (Surnames data)
-00006cb0: 0a0a                                     ..
+00005320: 6573 2074 6865 2063 7573 746f 6d69 7a65  es the customize
+00005330: 6420 6465 6c74 6173 2e0a 0a60 6060 6a73  d deltas...```js
+00005340: 6f6e 0a7b 0a20 2022 546f 6d6f 7272 6f77  on.{.  "Tomorrow
+00005350: 5468 7265 6548 6f75 7273 4c61 7465 7254  ThreeHoursLaterT
+00005360: 7765 6e74 794d 696e 7574 6573 4167 6f54  wentyMinutesAgoT
+00005370: 776f 5365 636f 6e64 734c 6174 6572 223a  woSecondsLater":
+00005380: 207b 0a20 2020 2022 5f6d 696d 656f 5f75   {.    "_mimeo_u
+00005390: 7469 6c22 3a20 7b0a 2020 2020 2020 225f  til": {.      "_
+000053a0: 6e61 6d65 223a 2022 6461 7465 5f74 696d  name": "date_tim
+000053b0: 6522 2c0a 2020 2020 2020 2264 6179 735f  e",.      "days_
+000053c0: 6465 6c74 6122 3a20 312c 0a20 2020 2020  delta": 1,.     
+000053d0: 2022 686f 7572 735f 6465 6c74 6122 3a20   "hours_delta": 
+000053e0: 332c 0a20 2020 2020 2022 6d69 6e75 7465  3,.      "minute
+000053f0: 735f 6465 6c74 6122 3a20 2d32 302c 0a20  s_delta": -20,. 
+00005400: 2020 2020 2022 7365 636f 6e64 735f 6465       "seconds_de
+00005410: 6c74 6122 3a20 320a 2020 2020 7d0a 2020  lta": 2.    }.  
+00005420: 7d0a 7d0a 6060 600a 0a23 2323 2323 2041  }.}.```..##### A
+00005430: 7574 6f20 496e 6372 656d 656e 740a 0a47  uto Increment..G
+00005440: 656e 6572 6174 6573 2061 206e 6578 7420  enerates a next 
+00005450: 696e 7465 6765 7220 696e 2063 6f6e 7465  integer in conte
+00005460: 7874 206f 6620 6120 6d6f 6465 6c20 2869  xt of a model (i
+00005470: 6e20 6e65 7374 6564 2074 656d 706c 6174  n nested templat
+00005480: 6573 2069 7420 7769 6c6c 2075 7365 2061  es it will use a
+00005490: 2073 6570 6172 6174 6564 2063 6f6e 7465   separated conte
+000054a0: 7874 292e 0a0a 7c20 5061 7261 6d65 7465  xt)...| Paramete
+000054b0: 7220 7c20 5375 7070 6f72 7465 6420 7661  r | Supported va
+000054c0: 6c75 6573 207c 2044 6566 6175 6c74 2020  lues | Default  
+000054d0: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a  |.|:---------:|:
+000054e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000054f0: 3a7c 3a2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20  :|:--------:|.| 
+00005500: 2070 6174 7465 726e 2020 7c20 2020 2020   pattern  |     
+00005510: 2060 7374 7260 2020 2020 2020 207c 2060   `str`       | `
+00005520: 7b3a 3035 647d 6020 7c0a 0a23 2323 2323  {:05d}` |..#####
+00005530: 2320 5261 770a 0a55 7365 7320 6120 6465  # Raw..Uses a de
+00005540: 6661 756c 7420 7061 7474 6572 6e3a 202a  fault pattern: *
+00005550: 2a7b 3a30 3564 7d2a 2a20 2861 6e20 696e  *{:05d}** (an in
+00005560: 7465 6765 7220 7769 7468 2035 206c 6561  teger with 5 lea
+00005570: 6469 6e67 207a 6572 6f73 292e 0a0a 6060  ding zeros)...``
+00005580: 606a 736f 6e0a 7b0a 2020 2249 4422 3a20  `json.{.  "ID": 
+00005590: 227b 6175 746f 5f69 6e63 7265 6d65 6e74  "{auto_increment
+000055a0: 7d22 0a7d 0a60 6060 0a0a 2323 2323 2323  }".}.```..######
+000055b0: 2050 6172 616d 6574 7269 7a65 640a 0a55   Parametrized..U
+000055c0: 7365 7320 7468 6520 7374 7269 6e67 2070  ses the string p
+000055d0: 6174 7465 726e 2070 726f 7669 6465 642e  attern provided.
+000055e0: 0a0a 6060 606a 736f 6e0a 7b0a 2020 2249  ..```json.{.  "I
+000055f0: 4422 3a20 7b0a 2020 2020 225f 6d69 6d65  D": {.    "_mime
+00005600: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
+00005610: 2022 5f6e 616d 6522 3a20 2261 7574 6f5f   "_name": "auto_
+00005620: 696e 6372 656d 656e 7422 2c0a 2020 2020  increment",.    
+00005630: 2020 2270 6174 7465 726e 223a 2022 4d59    "pattern": "MY
+00005640: 5f49 445f 7b3a 3031 3064 7d22 0a20 2020  _ID_{:010d}".   
+00005650: 207d 0a20 207d 0a7d 0a60 6060 0a0a 2323   }.  }.}.```..##
+00005660: 2323 2320 4375 7272 656e 7420 4974 6572  ### Current Iter
+00005670: 6174 696f 6e0a 0a47 656e 6572 6174 6573  ation..Generates
+00005680: 2061 2076 616c 7565 206f 6620 7468 6520   a value of the 
+00005690: 6375 7272 656e 7420 6974 6572 6174 696f  current iteratio
+000056a0: 6e20 696e 2061 204d 696d 656f 2054 656d  n in a Mimeo Tem
+000056b0: 706c 6174 6520 636f 6e74 6578 742e 0a0a  plate context...
+000056c0: 7c20 5061 7261 6d65 7465 7220 7c20 5375  | Parameter | Su
+000056d0: 7070 6f72 7465 6420 7661 6c75 6573 207c  pported values |
+000056e0: 2020 2020 2020 4465 6661 756c 7420 2020        Default   
+000056f0: 2020 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d     |.|:---------
+00005700: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|:-------------
+00005710: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00005720: 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2063 6f6e  -------:|.|  con
+00005730: 7465 7874 2020 7c20 2020 2020 2060 7374  text  |      `st
+00005740: 7260 2020 2020 2020 207c 2061 2063 7572  r`       | a cur
+00005750: 7265 6e74 2063 6f6e 7465 7874 207c 0a0a  rent context |..
+00005760: 2323 2323 2323 2052 6177 0a0a 5573 6573  ###### Raw..Uses
+00005770: 2074 6865 2063 7572 7265 6e74 2063 6f6e   the current con
+00005780: 7465 7874 2e0a 0a60 6060 6a73 6f6e 0a7b  text...```json.{
+00005790: 0a20 2022 4944 223a 2022 7b63 7572 725f  .  "ID": "{curr_
+000057a0: 6974 6572 7d22 0a7d 0a60 6060 0a0a 2323  iter}".}.```..##
+000057b0: 2323 2323 2050 6172 616d 6574 7269 7a65  #### Parametrize
+000057c0: 640a 0a55 7365 7320 6120 7370 6563 6966  d..Uses a specif
+000057d0: 6963 204d 696d 656f 204d 6f64 656c 2063  ic Mimeo Model c
+000057e0: 6f6e 7465 7874 2028 6d6f 6465 6c20 6e61  ontext (model na
+000057f0: 6d65 2077 6865 6e20 6063 6f6e 7465 7874  me when `context
+00005800: 6020 6973 206e 6f74 2063 6f6e 6669 6775  ` is not configu
+00005810: 7265 6429 2e0a 0a60 6060 6a73 6f6e 0a7b  red)...```json.{
+00005820: 0a20 2022 5061 7265 6e74 223a 207b 0a20  .  "Parent": {. 
+00005830: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
+00005840: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
+00005850: 223a 2022 6375 7272 5f69 7465 7222 2c0a  ": "curr_iter",.
+00005860: 2020 2020 2020 2263 6f6e 7465 7874 223a        "context":
+00005870: 2022 536f 6d65 456e 7469 7479 220a 2020   "SomeEntity".  
+00005880: 2020 7d0a 2020 7d0a 7d0a 6060 600a 0a23    }.  }.}.```..#
+00005890: 2323 2323 204b 6579 0a0a 4765 6e65 7261  #### Key..Genera
+000058a0: 7465 7320 6120 6b65 7920 756e 6971 7565  tes a key unique
+000058b0: 2061 6372 6f73 7320 616c 6c20 4d69 6d65   across all Mime
+000058c0: 6f20 4d6f 6465 6c73 2061 6e64 2062 6569  o Models and bei
+000058d0: 6e67 2074 6865 2073 616d 6520 7769 7468  ng the same with
+000058e0: 696e 2061 2073 696e 676c 6520 4d69 6d65  in a single Mime
+000058f0: 6f20 4d6f 6465 6c20 636f 6e74 6578 742e  o Model context.
+00005900: 0a0a 7c20 5061 7261 6d65 7465 7220 7c20  ..| Parameter | 
+00005910: 5375 7070 6f72 7465 6420 7661 6c75 6573  Supported values
+00005920: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00005930: 4465 6661 756c 7420 2020 2020 2020 2020  Default         
+00005940: 2020 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d        |.|:------
+00005950: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00005960: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
+00005970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20  -----------:|.| 
+00005990: 2063 6f6e 7465 7874 2020 7c20 2020 2020   context  |     
+000059a0: 2060 7374 7260 2020 2020 2020 207c 2020   `str`       |  
+000059b0: 2020 2020 2020 2061 2063 7572 7265 6e74         a current
+000059c0: 2063 6f6e 7465 7874 2020 2020 2020 2020   context        
+000059d0: 2020 7c0a 7c20 6974 6572 6174 696f 6e20    |.| iteration 
+000059e0: 7c20 2020 2020 2060 696e 7460 2020 2020  |      `int`    
+000059f0: 2020 207c 2061 2063 7572 7265 6e74 2069     | a current i
+00005a00: 7465 7261 7469 6f6e 206f 6620 7468 6520  teration of the 
+00005a10: 636f 6e74 6578 7420 7c0a 0a23 2323 2323  context |..#####
+00005a20: 2320 5261 770a 0a55 7365 7320 6120 6b65  # Raw..Uses a ke
+00005a30: 7920 6672 6f6d 2074 6865 2063 7572 7265  y from the curre
+00005a40: 6e74 2063 6f6e 7465 7874 2061 6e64 2069  nt context and i
+00005a50: 7465 7261 7469 6f6e 2e0a 0a60 6060 6a73  teration...```js
+00005a60: 6f6e 0a7b 0a20 2022 4944 223a 2022 7b6b  on.{.  "ID": "{k
+00005a70: 6579 7d22 0a7d 0a60 6060 0a0a 2323 2323  ey}".}.```..####
+00005a80: 2323 2050 6172 616d 6574 7269 7a65 640a  ## Parametrized.
+00005a90: 0a55 7365 7320 6120 6b65 7920 6672 6f6d  .Uses a key from
+00005aa0: 2074 6865 2073 7065 6369 6669 6320 636f   the specific co
+00005ab0: 6e74 6578 7420 616e 6420 6974 6572 6174  ntext and iterat
+00005ac0: 696f 6e2e 2020 0a57 6865 6e20 636f 6e74  ion.  .When cont
+00005ad0: 6578 7420 6973 2069 6e64 6963 6174 6564  ext is indicated
+00005ae0: 2061 6e64 2069 7465 7261 7469 6f6e 2069   and iteration i
+00005af0: 7320 6e6f 742c 2074 6865 6e20 7468 6520  s not, then the 
+00005b00: 6375 7272 656e 7420 6974 6572 6174 696f  current iteratio
+00005b10: 6e20 2a2a 6f66 2074 6865 2069 6e64 6963  n **of the indic
+00005b20: 6174 6564 2063 6f6e 7465 7874 2a2a 2069  ated context** i
+00005b30: 7320 6265 696e 6720 7573 6564 2e0a 0a60  s being used...`
+00005b40: 6060 6a73 6f6e 0a7b 0a20 2022 536f 6d65  ``json.{.  "Some
+00005b50: 456e 7469 7479 3222 3a20 7b0a 2020 2020  Entity2": {.    
+00005b60: 225f 6d69 6d65 6f5f 7574 696c 223a 207b  "_mimeo_util": {
+00005b70: 0a20 2020 2020 2022 5f6e 616d 6522 3a20  .      "_name": 
+00005b80: 226b 6579 222c 0a20 2020 2020 2022 636f  "key",.      "co
+00005b90: 6e74 6578 7422 3a20 2253 6f6d 6545 6e74  ntext": "SomeEnt
+00005ba0: 6974 7922 2c0a 2020 2020 2020 2269 7465  ity",.      "ite
+00005bb0: 7261 7469 6f6e 223a 2022 7b63 7572 725f  ration": "{curr_
+00005bc0: 6974 6572 7d22 0a20 2020 207d 0a20 207d  iter}".    }.  }
+00005bd0: 0a7d 0a60 6060 0a0a 2323 2323 2320 4369  .}.```..##### Ci
+00005be0: 7479 0a0a 4765 6e65 7261 7465 7320 6120  ty..Generates a 
+00005bf0: 6369 7479 206e 616d 652e 0a0a 7c20 5061  city name...| Pa
+00005c00: 7261 6d65 7465 7220 7c20 5375 7070 6f72  rameter | Suppor
+00005c10: 7465 6420 7661 6c75 6573 207c 2044 6566  ted values | Def
+00005c20: 6175 6c74 207c 0a7c 3a2d 2d2d 2d2d 2d2d  ault |.|:-------
+00005c30: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
+00005c40: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d3a  -----:|:-------:
+00005c50: 7c0a 7c20 2075 6e69 7175 6520 2020 7c20  |.|  unique   | 
+00005c60: 2020 2020 2060 626f 6f6c 6020 2020 2020       `bool`     
+00005c70: 207c 2060 5472 7565 6020 207c 0a7c 2020   | `True`  |.|  
+00005c80: 636f 756e 7472 7920 207c 2020 2020 2020  country  |      
+00005c90: 6073 7472 6020 2020 2020 2020 7c20 604e  `str`       | `N
+00005ca0: 6f6e 6560 2020 7c0a 0a23 2323 2323 2320  one`  |..###### 
+00005cb0: 5261 770a 0a42 7920 6465 6661 756c 7420  Raw..By default 
+00005cc0: 6369 7479 206e 616d 6573 2077 696c 6c20  city names will 
+00005cd0: 6265 2075 6e69 7175 6520 6163 726f 7373  be unique across
+00005ce0: 2061 204d 696d 656f 2043 6f6e 7465 7874   a Mimeo Context
+00005cf0: 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  ...```json.{.  "
+00005d00: 4369 7479 223a 2022 7b63 6974 797d 220a  City": "{city}".
+00005d10: 7d0a 6060 600a 0a23 2323 2323 2320 5061  }.```..###### Pa
+00005d20: 7261 6d65 7472 697a 6564 0a0a 5573 6573  rametrized..Uses
+00005d30: 2063 6f75 6e74 7279 2028 6e61 6d65 2c20   country (name, 
+00005d40: 6973 6f32 2c20 6973 6f33 2920 616e 6420  iso2, iso3) and 
+00005d50: 6075 6e69 7175 6560 2066 6c61 6720 746f  `unique` flag to
+00005d60: 2067 656e 6572 6174 6520 6120 6369 7479   generate a city
+00005d70: 206e 616d 652e 0a0a 6060 606a 736f 6e0a   name...```json.
+00005d80: 7b0a 2020 2243 6974 7957 6974 6844 7570  {.  "CityWithDup
+00005d90: 6c69 6361 7465 7322 3a20 7b0a 2020 2020  licates": {.    
+00005da0: 225f 6d69 6d65 6f5f 7574 696c 223a 207b  "_mimeo_util": {
+00005db0: 0a20 2020 2020 2022 5f6e 616d 6522 3a20  .      "_name": 
+00005dc0: 2263 6974 7922 2c0a 2020 2020 2020 2275  "city",.      "u
+00005dd0: 6e69 7175 6522 3a20 6661 6c73 650a 2020  nique": false.  
+00005de0: 2020 7d0a 2020 7d2c 0a20 2022 4369 7479    }.  },.  "City
+00005df0: 4f66 436f 756e 7472 794e 616d 6522 3a20  OfCountryName": 
+00005e00: 7b0a 2020 2020 225f 6d69 6d65 6f5f 7574  {.    "_mimeo_ut
+00005e10: 696c 223a 207b 0a20 2020 2020 2022 5f6e  il": {.      "_n
+00005e20: 616d 6522 3a20 2263 6974 7922 2c0a 2020  ame": "city",.  
+00005e30: 2020 2020 2263 6f75 6e74 7279 223a 2022      "country": "
+00005e40: 556e 6974 6564 204b 696e 6764 6f6d 220a  United Kingdom".
+00005e50: 2020 2020 7d0a 2020 7d2c 0a20 2022 4369      }.  },.  "Ci
+00005e60: 7479 4f66 436f 756e 7472 7949 534f 3222  tyOfCountryISO2"
+00005e70: 3a20 7b0a 2020 2020 225f 6d69 6d65 6f5f  : {.    "_mimeo_
+00005e80: 7574 696c 223a 207b 0a20 2020 2020 2022  util": {.      "
+00005e90: 5f6e 616d 6522 3a20 2263 6974 7922 2c0a  _name": "city",.
+00005ea0: 2020 2020 2020 2263 6f75 6e74 7279 223a        "country":
+00005eb0: 2022 4742 220a 2020 2020 7d0a 2020 7d2c   "GB".    }.  },
+00005ec0: 0a20 2022 4369 7479 4f66 436f 756e 7472  .  "CityOfCountr
+00005ed0: 7949 534f 3322 3a20 7b0a 2020 2020 225f  yISO3": {.    "_
+00005ee0: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
+00005ef0: 2020 2020 2022 5f6e 616d 6522 3a20 2263       "_name": "c
+00005f00: 6974 7922 2c0a 2020 2020 2020 2263 6f75  ity",.      "cou
+00005f10: 6e74 7279 223a 2022 4742 5222 0a20 2020  ntry": "GBR".   
+00005f20: 207d 0a20 207d 2c0a 2020 2243 6974 794f   }.  },.  "CityO
+00005f30: 6643 6f75 6e74 7279 5769 7468 4475 706c  fCountryWithDupl
+00005f40: 6963 6174 6573 223a 207b 0a20 2020 2022  icates": {.    "
+00005f50: 5f6d 696d 656f 5f75 7469 6c22 3a20 7b0a  _mimeo_util": {.
+00005f60: 2020 2020 2020 225f 6e61 6d65 223a 2022        "_name": "
+00005f70: 6369 7479 222c 0a20 2020 2020 2022 636f  city",.      "co
+00005f80: 756e 7472 7922 3a20 2255 6e69 7465 6420  untry": "United 
+00005f90: 4b69 6e67 646f 6d22 2c0a 2020 2020 2020  Kingdom",.      
+00005fa0: 2275 6e69 7175 6522 3a20 6661 6c73 650a  "unique": false.
+00005fb0: 2020 2020 7d0a 2020 7d0a 7d0a 6060 600a      }.  }.}.```.
+00005fc0: 0a23 2323 2323 2043 6f75 6e74 7279 0a0a  .##### Country..
+00005fd0: 4765 6e65 7261 7465 7320 6120 636f 756e  Generates a coun
+00005fe0: 7472 7920 6e61 6d65 2028 6279 2064 6566  try name (by def
+00005ff0: 6175 6c74 292c 2069 736f 3220 6f72 2069  ault), iso2 or i
+00006000: 736f 332e 0a0a 7c20 5061 7261 6d65 7465  so3...| Paramete
+00006010: 7220 7c20 2020 2020 2020 5375 7070 6f72  r |       Suppor
+00006020: 7465 6420 7661 6c75 6573 2020 2020 2020  ted values      
+00006030: 207c 2044 6566 6175 6c74 2020 7c0a 7c3a   | Default  |.|:
+00006040: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
+00006050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006060: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
+00006070: 2d2d 2d3a 7c0a 7c20 2075 6e69 7175 6520  ---:|.|  unique 
+00006080: 2020 7c20 2020 2020 2020 2020 2020 2060    |            `
+00006090: 626f 6f6c 6020 2020 2020 2020 2020 2020  bool`           
+000060a0: 207c 2020 6054 7275 6560 2020 7c0a 7c20   |  `True`  |.| 
+000060b0: 2020 7661 6c75 6520 2020 7c20 6022 6e61    value   | `"na
+000060c0: 6d65 2260 2c20 6022 6973 6f33 2260 2c20  me"`, `"iso3"`, 
+000060d0: 6022 6973 6f32 2260 207c 2060 226e 616d  `"iso2"` | `"nam
+000060e0: 6522 6020 7c0a 7c20 2063 6f75 6e74 7279  e"` |.|  country
+000060f0: 2020 7c20 2020 2020 2020 2020 2020 2060    |            `
+00006100: 7374 7260 2020 2020 2020 2020 2020 2020  str`            
+00006110: 207c 2020 604e 6f6e 6560 2020 7c0a 0a23   |  `None`  |..#
+00006120: 2323 2323 2320 5261 770a 0a42 7920 6465  ##### Raw..By de
+00006130: 6661 756c 7420 636f 756e 7472 7920 6e61  fault country na
+00006140: 6d65 7320 7769 6c6c 2062 6520 756e 6971  mes will be uniq
+00006150: 7565 2061 6372 6f73 7320 6120 4d69 6d65  ue across a Mime
+00006160: 6f20 436f 6e74 6578 742e 0a0a 6060 606a  o Context...```j
+00006170: 736f 6e0a 7b0a 2020 2243 6f75 6e74 7279  son.{.  "Country
+00006180: 223a 2022 7b63 6f75 6e74 7279 7d22 0a7d  ": "{country}".}
+00006190: 0a60 6060 0a0a 2323 2323 2323 2050 6172  .```..###### Par
+000061a0: 616d 6574 7269 7a65 640a 0a49 7420 6361  ametrized..It ca
+000061b0: 6e20 6765 6e65 7261 7465 3a0a 2d20 636f  n generate:.- co
+000061c0: 756e 7472 7920 6973 6f33 206f 7220 6973  untry iso3 or is
+000061d0: 6f20 3220 696e 7374 6561 6420 6f66 206e  o 2 instead of n
+000061e0: 616d 650a 2d20 636f 756e 7472 7920 7769  ame.- country wi
+000061f0: 7468 2064 7570 6c69 6361 7465 730a 2d20  th duplicates.- 
+00006200: 636f 756e 7472 7920 6e61 6d65 2066 6f72  country name for
+00006210: 2061 2070 726f 7669 6465 6420 6973 6f33   a provided iso3
+00006220: 206f 7220 6973 6f32 0a2d 2063 6f75 6e74   or iso2.- count
+00006230: 7279 2069 736f 3220 666f 7220 6120 7072  ry iso2 for a pr
+00006240: 6f76 6964 6564 206e 616d 6520 6f72 2069  ovided name or i
+00006250: 736f 330a 2d20 636f 756e 7472 7920 6973  so3.- country is
+00006260: 6f33 2066 6f72 2061 2070 726f 7669 6465  o3 for a provide
+00006270: 6420 6e61 6d65 206f 7220 6973 6f32 0a0a  d name or iso2..
+00006280: 5768 656e 2074 6865 2060 636f 756e 7472  When the `countr
+00006290: 7960 2070 6172 616d 2069 7320 7072 6f76  y` param is prov
+000062a0: 6964 6564 2074 6865 6e20 7468 6520 6075  ided then the `u
+000062b0: 6e69 7175 6560 2066 6c61 6720 6973 2069  nique` flag is i
+000062c0: 676e 6f72 6564 2e0a 0a60 6060 6a73 6f6e  gnored...```json
+000062d0: 0a7b 0a20 2022 436f 756e 7472 794e 616d  .{.  "CountryNam
+000062e0: 6557 6974 6844 7570 6c69 6361 7465 7322  eWithDuplicates"
+000062f0: 3a20 7b0a 2020 2020 225f 6d69 6d65 6f5f  : {.    "_mimeo_
+00006300: 7574 696c 223a 207b 0a20 2020 2020 2022  util": {.      "
+00006310: 5f6e 616d 6522 3a20 2263 6f75 6e74 7279  _name": "country
+00006320: 222c 0a20 2020 2020 2022 756e 6971 7565  ",.      "unique
+00006330: 223a 2066 616c 7365 0a20 2020 207d 0a20  ": false.    }. 
+00006340: 207d 2c0a 2020 2243 6f75 6e74 7279 4953   },.  "CountryIS
+00006350: 4f32 223a 207b 0a20 2020 2022 5f6d 696d  O2": {.    "_mim
+00006360: 656f 5f75 7469 6c22 3a20 7b0a 2020 2020  eo_util": {.    
+00006370: 2020 225f 6e61 6d65 223a 2022 636f 756e    "_name": "coun
+00006380: 7472 7922 2c0a 2020 2020 2020 2276 616c  try",.      "val
+00006390: 7565 223a 2022 6973 6f32 220a 2020 2020  ue": "iso2".    
+000063a0: 7d0a 2020 7d2c 0a20 2022 436f 756e 7472  }.  },.  "Countr
+000063b0: 7949 534f 3322 3a20 7b0a 2020 2020 225f  yISO3": {.    "_
+000063c0: 6d69 6d65 6f5f 7574 696c 223a 207b 0a20  mimeo_util": {. 
+000063d0: 2020 2020 2022 5f6e 616d 6522 3a20 2263       "_name": "c
+000063e0: 6f75 6e74 7279 222c 0a20 2020 2020 2022  ountry",.      "
+000063f0: 7661 6c75 6522 3a20 2269 736f 3322 0a20  value": "iso3". 
+00006400: 2020 207d 0a20 207d 2c0a 2020 2243 6f75     }.  },.  "Cou
+00006410: 6e74 7279 4e61 6d65 466f 7249 534f 3322  ntryNameForISO3"
+00006420: 3a20 7b0a 2020 2020 225f 6d69 6d65 6f5f  : {.    "_mimeo_
+00006430: 7574 696c 223a 207b 0a20 2020 2020 2022  util": {.      "
+00006440: 5f6e 616d 6522 3a20 2263 6f75 6e74 7279  _name": "country
+00006450: 222c 0a20 2020 2020 2022 636f 756e 7472  ",.      "countr
+00006460: 7922 3a20 2247 4252 220a 2020 2020 7d0a  y": "GBR".    }.
+00006470: 2020 7d2c 0a20 2022 436f 756e 7472 7949    },.  "CountryI
+00006480: 534f 3246 6f72 4e61 6d65 223a 207b 0a20  SO2ForName": {. 
+00006490: 2020 2022 5f6d 696d 656f 5f75 7469 6c22     "_mimeo_util"
+000064a0: 3a20 7b0a 2020 2020 2020 225f 6e61 6d65  : {.      "_name
+000064b0: 223a 2022 636f 756e 7472 7922 2c0a 2020  ": "country",.  
+000064c0: 2020 2020 2276 616c 7565 223a 2022 6973      "value": "is
+000064d0: 6f32 222c 0a20 2020 2020 2022 636f 756e  o2",.      "coun
+000064e0: 7472 7922 3a20 2255 6e69 7465 6420 4b69  try": "United Ki
+000064f0: 6e67 646f 6d22 0a20 2020 207d 0a20 207d  ngdom".    }.  }
+00006500: 0a7d 0a60 6060 0a0a 2323 2323 2320 4375  .}.```..##### Cu
+00006510: 7272 656e 6379 0a0a 4765 6e65 7261 7465  rrency..Generate
+00006520: 7320 6120 6375 7272 656e 6379 2063 6f64  s a currency cod
+00006530: 6520 2862 7920 6465 6661 756c 7429 206f  e (by default) o
+00006540: 7220 6e61 6d65 2e0a 0a7c 2050 6172 616d  r name...| Param
+00006550: 6574 6572 207c 2020 5375 7070 6f72 7465  eter |  Supporte
+00006560: 6420 7661 6c75 6573 2020 7c20 4465 6661  d values  | Defa
+00006570: 756c 7420 207c 0a7c 3a2d 2d2d 2d2d 2d2d  ult  |.|:-------
+00006580: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
+00006590: 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d  -------:|:------
+000065a0: 2d2d 3a7c 0a7c 2020 756e 6971 7565 2020  --:|.|  unique  
+000065b0: 207c 2020 2020 2020 2060 626f 6f6c 6020   |       `bool` 
+000065c0: 2020 2020 2020 7c20 6046 616c 7365 6020        | `False` 
+000065d0: 207c 0a7c 2020 2076 616c 7565 2020 207c   |.|   value   |
+000065e0: 2060 2263 6f64 6522 602c 2060 226e 616d   `"code"`, `"nam
+000065f0: 6522 6020 7c20 6022 636f 6465 2260 207c  e"` | `"code"` |
+00006600: 0a7c 2020 636f 756e 7472 7920 207c 2020  .|  country  |  
+00006610: 2020 2020 2060 7374 7260 2020 2020 2020       `str`      
+00006620: 2020 7c20 2060 4e6f 6e65 6020 207c 0a0a    |  `None`  |..
+00006630: 2323 2323 2323 2052 6177 0a0a 4279 2064  ###### Raw..By d
+00006640: 6566 6175 6c74 2063 6974 7920 6e61 6d65  efault city name
+00006650: 7320 7769 6c6c 205f 4e4f 545f 2062 6520  s will _NOT_ be 
+00006660: 756e 6971 7565 2061 6372 6f73 7320 6120  unique across a 
+00006670: 4d69 6d65 6f20 436f 6e74 6578 742e 0a0a  Mimeo Context...
+00006680: 6060 606a 736f 6e0a 7b0a 2020 2243 7572  ```json.{.  "Cur
+00006690: 7265 6e63 7922 3a20 227b 6375 7272 656e  rency": "{curren
+000066a0: 6379 7d22 0a7d 0a60 6060 0a0a 2323 2323  cy}".}.```..####
+000066b0: 2323 2050 6172 616d 6574 7269 7a65 640a  ## Parametrized.
+000066c0: 0a49 7420 6361 6e20 6765 6e65 7261 7465  .It can generate
+000066d0: 3a0a 2d20 756e 6971 7565 2063 7572 7265  :.- unique curre
+000066e0: 6e63 6965 730a 2d20 6375 7272 656e 6379  ncies.- currency
+000066f0: 206e 616d 6520 696e 7374 6561 6420 6f66   name instead of
+00006700: 2063 6f64 650a 2d20 6375 7272 656e 6379   code.- currency
+00006710: 2063 6f64 6520 6f72 206e 616d 6520 6f66   code or name of
+00006720: 2061 2073 7065 6369 6669 6320 636f 756e   a specific coun
+00006730: 7472 7920 2875 7369 6e67 2069 736f 332c  try (using iso3,
+00006740: 2069 736f 3220 6f72 206e 616d 6529 0a0a   iso2 or name)..
+00006750: 5768 656e 2074 6865 2060 636f 756e 7472  When the `countr
+00006760: 7960 2070 6172 616d 2069 7320 7072 6f76  y` param is prov
+00006770: 6964 6564 2074 6865 6e20 7468 6520 6075  ided then the `u
+00006780: 6e69 7175 6560 2066 6c61 6720 6973 2069  nique` flag is i
+00006790: 676e 6f72 6564 2e0a 0a60 6060 6a73 6f6e  gnored...```json
+000067a0: 0a7b 0a20 2022 556e 6971 7565 4375 7272  .{.  "UniqueCurr
+000067b0: 656e 6379 436f 6465 223a 207b 0a20 2020  encyCode": {.   
+000067c0: 2022 5f6d 696d 656f 5f75 7469 6c22 3a20   "_mimeo_util": 
+000067d0: 7b0a 2020 2020 2020 225f 6e61 6d65 223a  {.      "_name":
+000067e0: 2022 6375 7272 656e 6379 222c 0a20 2020   "currency",.   
+000067f0: 2020 2022 756e 6971 7565 223a 2074 7275     "unique": tru
+00006800: 650a 2020 2020 7d0a 2020 7d2c 0a20 2022  e.    }.  },.  "
+00006810: 4375 7272 656e 6379 4e61 6d65 223a 207b  CurrencyName": {
+00006820: 0a20 2020 2022 5f6d 696d 656f 5f75 7469  .    "_mimeo_uti
+00006830: 6c22 3a20 7b0a 2020 2020 2020 225f 6e61  l": {.      "_na
+00006840: 6d65 223a 2022 6375 7272 656e 6379 222c  me": "currency",
+00006850: 0a20 2020 2020 2022 7661 6c75 6522 3a20  .      "value": 
+00006860: 226e 616d 6522 0a20 2020 207d 0a20 207d  "name".    }.  }
+00006870: 2c0a 2020 2243 7572 7265 6e63 7943 6f64  ,.  "CurrencyCod
+00006880: 6546 6f72 436f 756e 7472 7949 534f 3322  eForCountryISO3"
+00006890: 3a20 7b0a 2020 2020 225f 6d69 6d65 6f5f  : {.    "_mimeo_
+000068a0: 7574 696c 223a 207b 0a20 2020 2020 2022  util": {.      "
+000068b0: 5f6e 616d 6522 3a20 2263 7572 7265 6e63  _name": "currenc
+000068c0: 7922 2c0a 2020 2020 2020 2263 6f75 6e74  y",.      "count
+000068d0: 7279 223a 2022 4742 5222 0a20 2020 207d  ry": "GBR".    }
+000068e0: 0a20 207d 2c0a 2020 2243 7572 7265 6e63  .  },.  "Currenc
+000068f0: 794e 616d 6546 6f72 436f 756e 7472 7949  yNameForCountryI
+00006900: 534f 3222 3a20 7b0a 2020 2020 225f 6d69  SO2": {.    "_mi
+00006910: 6d65 6f5f 7574 696c 223a 207b 0a20 2020  meo_util": {.   
+00006920: 2020 2022 5f6e 616d 6522 3a20 2263 7572     "_name": "cur
+00006930: 7265 6e63 7922 2c0a 2020 2020 2020 2276  rency",.      "v
+00006940: 616c 7565 223a 2022 6e61 6d65 222c 0a20  alue": "name",. 
+00006950: 2020 2020 2022 636f 756e 7472 7922 3a20       "country": 
+00006960: 2247 4222 0a20 2020 207d 0a20 207d 2c0a  "GB".    }.  },.
+00006970: 2020 2243 7572 7265 6e63 794e 616d 6546    "CurrencyNameF
+00006980: 6f72 436f 756e 7472 794e 616d 6522 3a20  orCountryName": 
+00006990: 7b0a 2020 2020 225f 6d69 6d65 6f5f 7574  {.    "_mimeo_ut
+000069a0: 696c 223a 207b 0a20 2020 2020 2022 5f6e  il": {.      "_n
+000069b0: 616d 6522 3a20 2263 7572 7265 6e63 7922  ame": "currency"
+000069c0: 2c0a 2020 2020 2020 2276 616c 7565 223a  ,.      "value":
+000069d0: 2022 6e61 6d65 222c 0a20 2020 2020 2022   "name",.      "
+000069e0: 636f 756e 7472 7922 3a20 2255 6e69 7465  country": "Unite
+000069f0: 6420 4b69 6e67 646f 6d22 0a20 2020 207d  d Kingdom".    }
+00006a00: 0a20 207d 0a7d 0a60 6060 0a0a 2323 2323  .  }.}.```..####
+00006a10: 2320 4669 7273 7420 4e61 6d65 0a0a 4765  # First Name..Ge
+00006a20: 6e65 7261 7465 7320 6120 6669 7273 7420  nerates a first 
+00006a30: 6e61 6d65 2e0a 0a7c 2050 6172 616d 6574  name...| Paramet
+00006a40: 6572 207c 2020 2020 2020 5375 7070 6f72  er |      Suppor
+00006a50: 7465 6420 7661 6c75 6573 2020 2020 2020  ted values      
+00006a60: 7c20 4465 6661 756c 7420 207c 0a7c 3a2d  | Default  |.|:-
+00006a70: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
+00006a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006a90: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
+00006aa0: 3a7c 0a7c 2020 756e 6971 7565 2020 207c  :|.|  unique   |
+00006ab0: 2020 2020 2020 2020 2020 2060 626f 6f6c             `bool
+00006ac0: 6020 2020 2020 2020 2020 2020 7c20 2060  `           |  `
+00006ad0: 5472 7565 6020 207c 0a7c 2020 2020 7365  True`  |.|    se
+00006ae0: 7820 2020 207c 2060 4d60 2c20 604d 616c  x    | `M`, `Mal
+00006af0: 6560 2c20 6046 602c 2060 4665 6d61 6c65  e`, `F`, `Female
+00006b00: 6020 7c20 2060 4e6f 6e65 6020 207c 0a0a  ` |  `None`  |..
+00006b10: 2323 2323 2323 2052 6177 0a0a 4279 2064  ###### Raw..By d
+00006b20: 6566 6175 6c74 2066 6972 7374 206e 616d  efault first nam
+00006b30: 6573 2077 696c 6c20 6265 2075 6e69 7175  es will be uniqu
+00006b40: 6520 6163 726f 7373 2061 204d 696d 656f  e across a Mimeo
+00006b50: 2043 6f6e 7465 7874 2e0a 0a60 6060 6a73   Context...```js
+00006b60: 6f6e 0a7b 0a20 2022 4669 7273 744e 616d  on.{.  "FirstNam
+00006b70: 6522 3a20 227b 6669 7273 745f 6e61 6d65  e": "{first_name
+00006b80: 7d22 0a7d 0a60 6060 0a0a 2323 2323 2323  }".}.```..######
+00006b90: 2050 6172 616d 6574 7269 7a65 640a 0a55   Parametrized..U
+00006ba0: 7365 7320 7365 7820 2860 4d60 202f 2060  ses sex (`M` / `
+00006bb0: 4d61 6c65 6020 2f20 6046 6020 2f20 6046  Male` / `F` / `F
+00006bc0: 656d 616c 6560 2920 616e 6420 6075 6e69  emale`) and `uni
+00006bd0: 7175 6560 2066 6c61 6720 746f 2067 656e  que` flag to gen
+00006be0: 6572 6174 6520 6120 6669 7273 7420 6e61  erate a first na
+00006bf0: 6d65 2e0a 0a60 6060 6a73 6f6e 0a7b 0a20  me...```json.{. 
+00006c00: 2022 4669 7273 744e 616d 6557 6974 6844   "FirstNameWithD
+00006c10: 7570 6c69 6361 7465 7322 3a20 7b0a 2020  uplicates": {.  
+00006c20: 2020 225f 6d69 6d65 6f5f 7574 696c 223a    "_mimeo_util":
+00006c30: 207b 0a20 2020 2020 2022 5f6e 616d 6522   {.      "_name"
+00006c40: 3a20 2266 6972 7374 5f6e 616d 6522 2c0a  : "first_name",.
+00006c50: 2020 2020 2020 2275 6e69 7175 6522 3a20        "unique": 
+00006c60: 6661 6c73 650a 2020 2020 7d0a 2020 7d2c  false.    }.  },
+00006c70: 0a20 2022 4d61 6c65 4669 7273 744e 616d  .  "MaleFirstNam
+00006c80: 6522 3a20 7b0a 2020 2020 225f 6d69 6d65  e": {.    "_mime
+00006c90: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
+00006ca0: 2022 5f6e 616d 6522 3a20 2266 6972 7374   "_name": "first
+00006cb0: 5f6e 616d 6522 2c0a 2020 2020 2020 2273  _name",.      "s
+00006cc0: 6578 223a 2022 4d22 0a20 2020 207d 0a20  ex": "M".    }. 
+00006cd0: 207d 2c0a 2020 2246 656d 616c 6546 6972   },.  "FemaleFir
+00006ce0: 7374 4e61 6d65 223a 207b 0a20 2020 2022  stName": {.    "
+00006cf0: 5f6d 696d 656f 5f75 7469 6c22 3a20 7b0a  _mimeo_util": {.
+00006d00: 2020 2020 2020 225f 6e61 6d65 223a 2022        "_name": "
+00006d10: 6669 7273 745f 6e61 6d65 222c 0a20 2020  first_name",.   
+00006d20: 2020 2022 7365 7822 3a20 2246 220a 2020     "sex": "F".  
+00006d30: 2020 7d0a 2020 7d2c 0a20 2022 4d61 6c65    }.  },.  "Male
+00006d40: 4669 7273 744e 616d 6557 6974 6844 7570  FirstNameWithDup
+00006d50: 6c69 6361 7465 7322 3a20 7b0a 2020 2020  licates": {.    
+00006d60: 225f 6d69 6d65 6f5f 7574 696c 223a 207b  "_mimeo_util": {
+00006d70: 0a20 2020 2020 2022 5f6e 616d 6522 3a20  .      "_name": 
+00006d80: 2266 6972 7374 5f6e 616d 6522 2c0a 2020  "first_name",.  
+00006d90: 2020 2020 2273 6578 223a 2022 4d22 2c0a      "sex": "M",.
+00006da0: 2020 2020 2020 2275 6e69 7175 6522 3a20        "unique": 
+00006db0: 6661 6c73 650a 2020 2020 7d0a 2020 7d0a  false.    }.  }.
+00006dc0: 7d0a 6060 600a 0a23 2323 2323 204c 6173  }.```..##### Las
+00006dd0: 7420 4e61 6d65 0a0a 4765 6e65 7261 7465  t Name..Generate
+00006de0: 7320 6120 6c61 7374 206e 616d 652e 0a0a  s a last name...
+00006df0: 7c20 5061 7261 6d65 7465 7220 7c20 5375  | Parameter | Su
+00006e00: 7070 6f72 7465 6420 7661 6c75 6573 207c  pported values |
+00006e10: 2044 6566 6175 6c74 2020 7c0a 7c3a 2d2d   Default  |.|:--
+00006e20: 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d  -------:|:------
+00006e30: 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d  ----------:|:---
+00006e40: 2d2d 2d2d 2d3a 7c0a 7c20 2075 6e69 7175  -----:|.|  uniqu
+00006e50: 6520 2020 7c20 2020 2020 2060 626f 6f6c  e   |      `bool
+00006e60: 6020 2020 2020 207c 2020 6054 7275 6560  `      |  `True`
+00006e70: 2020 7c0a 0a23 2323 2323 2320 5261 770a    |..###### Raw.
+00006e80: 0a42 7920 6465 6661 756c 7420 6c61 7374  .By default last
+00006e90: 206e 616d 6573 2077 696c 6c20 6265 2075   names will be u
+00006ea0: 6e69 7175 6520 6163 726f 7373 2061 204d  nique across a M
+00006eb0: 696d 656f 2043 6f6e 7465 7874 2e0a 0a60  imeo Context...`
+00006ec0: 6060 6a73 6f6e 0a7b 0a20 2022 4c61 7374  ``json.{.  "Last
+00006ed0: 4e61 6d65 223a 2022 7b6c 6173 745f 6e61  Name": "{last_na
+00006ee0: 6d65 7d22 0a7d 0a60 6060 0a0a 2323 2323  me}".}.```..####
+00006ef0: 2323 2050 6172 616d 6574 7269 7a65 640a  ## Parametrized.
+00006f00: 0a55 7365 7320 6075 6e69 7175 6560 2066  .Uses `unique` f
+00006f10: 6c61 6720 746f 2067 656e 6572 6174 6520  lag to generate 
+00006f20: 6120 6c61 7374 206e 616d 652e 0a0a 6060  a last name...``
+00006f30: 606a 736f 6e0a 7b0a 2020 224c 6173 744e  `json.{.  "LastN
+00006f40: 616d 6557 6974 6844 7570 6c69 6361 7465  ameWithDuplicate
+00006f50: 7322 3a20 7b0a 2020 2020 225f 6d69 6d65  s": {.    "_mime
+00006f60: 6f5f 7574 696c 223a 207b 0a20 2020 2020  o_util": {.     
+00006f70: 2022 5f6e 616d 6522 3a20 226c 6173 745f   "_name": "last_
+00006f80: 6e61 6d65 222c 0a20 2020 2020 2022 756e  name",.      "un
+00006f90: 6971 7565 223a 2066 616c 7365 0a20 2020  ique": false.   
+00006fa0: 207d 0a20 207d 0a7d 0a60 6060 0a0a 2323   }.  }.}.```..##
+00006fb0: 2320 5079 7468 6f6e 204c 6962 0a0a 546f  # Python Lib..To
+00006fc0: 2067 656e 6572 6174 6520 6461 7461 2075   generate data u
+00006fd0: 7369 6e67 204d 696d 656f 2061 7320 6120  sing Mimeo as a 
+00006fe0: 7079 7468 6f6e 206c 6962 7261 7279 2079  python library y
+00006ff0: 6f75 206e 6565 6420 3320 636c 6173 7365  ou need 3 classe
+00007000: 733a 0a2a 2060 4d69 6d65 6f43 6f6e 6669  s:.* `MimeoConfi
+00007010: 6760 2028 4120 7079 7468 6f6e 2072 6570  g` (A python rep
+00007020: 7265 7365 6e74 6174 696f 6e20 6f66 2061  resentation of a
+00007030: 204d 696d 656f 2043 6f6e 6669 6775 7261   Mimeo Configura
+00007040: 7469 6f6e 290a 2a20 604d 696d 656f 436f  tion).* `MimeoCo
+00007050: 6e66 6967 4661 6374 6f72 7960 2028 4120  nfigFactory` (A 
+00007060: 6661 6374 6f72 7920 7061 7273 696e 6720  factory parsing 
+00007070: 6120 4d69 6d65 6f20 436f 6e66 6967 7572  a Mimeo Configur
+00007080: 6174 696f 6e29 0a2a 2060 4d69 6d65 6f67  ation).* `Mimeog
+00007090: 7261 7068 6020 2861 2063 6c61 7373 2067  raph` (a class g
+000070a0: 656e 6572 6174 696e 6720 616e 6420 636f  enerating and co
+000070b0: 6e73 756d 696e 6720 6461 7461 2066 726f  nsuming data fro
+000070c0: 6d20 6120 4d69 6d65 6f20 436f 6e66 6967  m a Mimeo Config
+000070d0: 7572 6174 696f 6e29 0a0a 2323 2323 2050  uration)..#### P
+000070e0: 6172 7369 6e67 204d 696d 656f 2043 6f6e  arsing Mimeo Con
+000070f0: 6669 6775 7261 7469 6f6e 0a0a 2323 2323  figuration..####
+00007100: 2320 604d 696d 656f 436f 6e66 6967 600a  # `MimeoConfig`.
+00007110: 0a54 6865 2060 4d69 6d65 6f43 6f6e 6669  .The `MimeoConfi
+00007120: 6760 2063 6c61 7373 2074 616b 6573 2061  g` class takes a
+00007130: 2064 6963 7469 6f6e 6172 7920 6173 2061   dictionary as a
+00007140: 2070 6172 616d 6574 6572 2061 6e64 2069   parameter and i
+00007150: 6e69 7469 616c 697a 6573 2061 6c6c 2073  nitializes all s
+00007160: 6574 7469 6e67 732e 0a0a 6060 6070 7974  ettings...```pyt
+00007170: 686f 6e0a 6672 6f6d 206d 696d 656f 2069  hon.from mimeo i
+00007180: 6d70 6f72 7420 4d69 6d65 6f43 6f6e 6669  mport MimeoConfi
+00007190: 670a 0a63 6f6e 6669 6720 3d20 7b0a 2020  g..config = {.  
+000071a0: 225f 7465 6d70 6c61 7465 735f 223a 205b  "_templates_": [
+000071b0: 0a20 2020 207b 0a20 2020 2020 2022 636f  .    {.      "co
+000071c0: 756e 7422 3a20 3330 2c0a 2020 2020 2020  unt": 30,.      
+000071d0: 226d 6f64 656c 223a 207b 0a20 2020 2020  "model": {.     
+000071e0: 2020 2022 536f 6d65 456e 7469 7479 223a     "SomeEntity":
+000071f0: 207b 0a20 2020 2020 2020 2020 2022 4078   {.          "@x
+00007200: 6d6c 6e73 223a 2022 6874 7470 3a2f 2f6d  mlns": "http://m
+00007210: 696d 656f 2e61 7263 682e 636f 6d2f 6465  imeo.arch.com/de
+00007220: 6661 756c 742d 6e61 6d65 7370 6163 6522  fault-namespace"
+00007230: 2c0a 2020 2020 2020 2020 2020 2240 786d  ,.          "@xm
+00007240: 6c6e 733a 706e 223a 2022 6874 7470 3a2f  lns:pn": "http:/
+00007250: 2f6d 696d 656f 2e61 7263 682e 636f 6d2f  /mimeo.arch.com/
+00007260: 7072 6566 6978 6564 2d6e 616d 6573 7061  prefixed-namespa
+00007270: 6365 222c 0a20 2020 2020 2020 2020 2022  ce",.          "
+00007280: 4368 696c 644e 6f64 6531 223a 2031 2c0a  ChildNode1": 1,.
+00007290: 2020 2020 2020 2020 2020 2243 6869 6c64            "Child
+000072a0: 4e6f 6465 3222 3a20 2276 616c 7565 2d32  Node2": "value-2
+000072b0: 222c 0a20 2020 2020 2020 2020 2022 4368  ",.          "Ch
+000072c0: 696c 644e 6f64 6533 223a 2054 7275 650a  ildNode3": True.
+000072d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000072e0: 7d0a 2020 2020 7d0a 2020 5d0a 7d0a 6d69  }.    }.  ].}.mi
+000072f0: 6d65 6f5f 636f 6e66 6967 203d 204d 696d  meo_config = Mim
+00007300: 656f 436f 6e66 6967 2863 6f6e 6669 6729  eoConfig(config)
+00007310: 0a60 6060 0a0a 2323 2323 2320 604d 696d  .```..##### `Mim
+00007320: 656f 436f 6e66 6967 4661 6374 6f72 7960  eoConfigFactory`
+00007330: 0a0a 546f 2065 6173 696c 7920 7061 7273  ..To easily pars
+00007340: 6520 4d69 6d65 6f20 436f 6e66 6967 7572  e Mimeo Configur
+00007350: 6174 696f 6e20 796f 7520 6361 6e20 7573  ation you can us
+00007360: 6520 7468 6520 604d 696d 656f 436f 6e66  e the `MimeoConf
+00007370: 6967 4661 6374 6f72 7960 2e0a 4974 2061  igFactory`..It a
+00007380: 6c6c 6f77 7320 796f 7520 746f 2070 726f  llows you to pro
+00007390: 7669 6465 2061 2072 6177 2063 6f6e 6669  vide a raw confi
+000073a0: 6720 6173 3a0a 2a20 6120 6469 6374 696f  g as:.* a dictio
+000073b0: 6e61 7279 0a2a 2061 2073 7472 696e 6769  nary.* a stringi
+000073c0: 6669 6564 2058 4d4c 206e 6f64 650a 2a20  fied XML node.* 
+000073d0: 6120 6669 6c65 2070 6174 680a 0a3c 7461  a file path..<ta
+000073e0: 626c 653e 0a20 2020 203c 7472 3e0a 2020  ble>.    <tr>.  
+000073f0: 2020 2020 2020 3c74 683e 3c2f 7468 3e0a        <th></th>.
+00007400: 2020 2020 2020 2020 3c74 683e 4a53 4f4e          <th>JSON
+00007410: 3c2f 7468 3e0a 2020 2020 2020 2020 3c74  </th>.        <t
+00007420: 683e 584d 4c3c 2f74 683e 0a20 2020 203c  h>XML</th>.    <
+00007430: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
+00007440: 2020 2020 2020 3c74 643e 3c62 3e52 6177        <td><b>Raw
+00007450: 2064 6174 613c 2f62 3e3c 2f74 643e 0a20   data</b></td>. 
+00007460: 2020 2020 2020 203c 7464 2076 616c 6967         <td valig
+00007470: 6e3d 2274 6f70 223e 0a0a 6060 6070 7974  n="top">..```pyt
+00007480: 686f 6e0a 6672 6f6d 206d 696d 656f 2069  hon.from mimeo i
+00007490: 6d70 6f72 7420 4d69 6d65 6f43 6f6e 6669  mport MimeoConfi
+000074a0: 6746 6163 746f 7279 0a0a 636f 6e66 6967  gFactory..config
+000074b0: 203d 207b 0a20 2022 5f74 656d 706c 6174   = {.  "_templat
+000074c0: 6573 5f22 3a20 5b0a 2020 2020 7b0a 2020  es_": [.    {.  
+000074d0: 2020 2020 2263 6f75 6e74 223a 2033 302c      "count": 30,
+000074e0: 0a20 2020 2020 2022 6d6f 6465 6c22 3a20  .      "model": 
+000074f0: 7b0a 2020 2020 2020 2020 2253 6f6d 6545  {.        "SomeE
+00007500: 6e74 6974 7922 3a20 7b0a 2020 2020 2020  ntity": {.      
+00007510: 2020 2020 2240 786d 6c6e 7322 3a20 2268      "@xmlns": "h
+00007520: 7474 703a 2f2f 6d69 6d65 6f2e 6172 6368  ttp://mimeo.arch
+00007530: 2e63 6f6d 2f64 6566 6175 6c74 2d6e 616d  .com/default-nam
+00007540: 6573 7061 6365 222c 0a20 2020 2020 2020  espace",.       
+00007550: 2020 2022 4078 6d6c 6e73 3a70 6e22 3a20     "@xmlns:pn": 
+00007560: 2268 7474 703a 2f2f 6d69 6d65 6f2e 6172  "http://mimeo.ar
+00007570: 6368 2e63 6f6d 2f70 7265 6669 7865 642d  ch.com/prefixed-
+00007580: 6e61 6d65 7370 6163 6522 2c0a 2020 2020  namespace",.    
+00007590: 2020 2020 2020 2243 6869 6c64 4e6f 6465        "ChildNode
+000075a0: 3122 3a20 312c 0a20 2020 2020 2020 2020  1": 1,.         
+000075b0: 2022 4368 696c 644e 6f64 6532 223a 2022   "ChildNode2": "
+000075c0: 7661 6c75 652d 3222 2c0a 2020 2020 2020  value-2",.      
+000075d0: 2020 2020 2243 6869 6c64 4e6f 6465 3322      "ChildNode3"
+000075e0: 3a20 5472 7565 0a20 2020 2020 2020 207d  : True.        }
+000075f0: 0a20 2020 2020 207d 0a20 2020 207d 0a20  .      }.    }. 
+00007600: 205d 0a7d 0a6d 696d 656f 5f63 6f6e 6669   ].}.mimeo_confi
+00007610: 6720 3d20 4d69 6d65 6f43 6f6e 6669 6746  g = MimeoConfigF
+00007620: 6163 746f 7279 2e70 6172 7365 2863 6f6e  actory.parse(con
+00007630: 6669 6729 0a60 6060 0a3c 2f74 643e 0a20  fig).```.</td>. 
+00007640: 2020 203c 7464 2076 616c 6967 6e3d 2274     <td valign="t
+00007650: 6f70 223e 0a0a 6060 6070 7974 686f 6e0a  op">..```python.
+00007660: 6672 6f6d 206d 696d 656f 2069 6d70 6f72  from mimeo impor
+00007670: 7420 4d69 6d65 6f43 6f6e 6669 6746 6163  t MimeoConfigFac
+00007680: 746f 7279 0a0a 636f 6e66 6967 203d 2028  tory..config = (
+00007690: 0a20 2020 2027 3c6d 696d 656f 5f63 6f6e  .    '<mimeo_con
+000076a0: 6669 6775 7261 7469 6f6e 3e27 0a20 2020  figuration>'.   
+000076b0: 2027 2020 2020 3c5f 7465 6d70 6c61 7465   '    <_template
+000076c0: 735f 3e27 0a20 2020 2027 2020 2020 2020  s_>'.    '      
+000076d0: 2020 3c5f 7465 6d70 6c61 7465 5f3e 270a    <_template_>'.
+000076e0: 2020 2020 2720 2020 2020 2020 2020 2020      '           
+000076f0: 203c 636f 756e 743e 3330 3c2f 636f 756e   <count>30</coun
+00007700: 743e 270a 2020 2020 2720 2020 2020 2020  t>'.    '       
+00007710: 2020 2020 203c 6d6f 6465 6c3e 270a 2020       <model>'.  
+00007720: 2020 2727 0a20 2020 2027 2020 2020 2020    ''.    '      
+00007730: 2020 2020 2020 2020 2020 3c53 6f6d 6545            <SomeE
+00007740: 6e74 6974 7927 0a20 2020 2027 2020 2020  ntity'.    '    
+00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007760: 786d 6c6e 733d 2268 7474 703a 2f2f 6d69  xmlns="http://mi
+00007770: 6d65 6f2e 6172 6368 2e63 6f6d 2f64 6566  meo.arch.com/def
+00007780: 6175 6c74 2d6e 616d 6573 7061 6365 2227  ault-namespace"'
+00007790: 0a20 2020 2027 2020 2020 2020 2020 2020  .    '          
+000077a0: 2020 2020 2020 2020 2020 786d 6c6e 733a            xmlns:
+000077b0: 706e 3d22 6874 7470 3a2f 2f6d 696d 656f  pn="http://mimeo
+000077c0: 2e61 7263 682e 636f 6d2f 7072 6566 6978  .arch.com/prefix
+000077d0: 6564 2d6e 616d 6573 7061 6365 223e 270a  ed-namespace">'.
+000077e0: 2020 2020 2720 2020 2020 2020 2020 2020      '           
+000077f0: 2020 2020 2020 2020 203c 4368 696c 644e           <ChildN
+00007800: 6f64 6531 3e31 3c2f 4368 696c 644e 6f64  ode1>1</ChildNod
+00007810: 6531 3e27 0a20 2020 2027 2020 2020 2020  e1>'.    '      
+00007820: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00007830: 6e3a 4368 696c 644e 6f64 6532 3e76 616c  n:ChildNode2>val
+00007840: 7565 2d32 3c2f 706e 3a43 6869 6c64 4e6f  ue-2</pn:ChildNo
+00007850: 6465 323e 270a 2020 2020 2720 2020 2020  de2>'.    '     
+00007860: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007870: 4368 696c 644e 6f64 6533 3e74 7275 653c  ChildNode3>true<
+00007880: 2f43 6869 6c64 4e6f 6465 333e 270a 2020  /ChildNode3>'.  
+00007890: 2020 2720 2020 2020 2020 2020 2020 2020    '             
+000078a0: 2020 203c 2f53 6f6d 6545 6e74 6974 793e     </SomeEntity>
+000078b0: 270a 2020 2020 2727 0a20 2020 2027 2020  '.    ''.    '  
+000078c0: 2020 2020 2020 2020 2020 3c2f 6d6f 6465            </mode
+000078d0: 6c3e 270a 2020 2020 2720 2020 2020 2020  l>'.    '       
+000078e0: 203c 2f5f 7465 6d70 6c61 7465 5f3e 270a   </_template_>'.
+000078f0: 2020 2020 2720 2020 203c 2f5f 7465 6d70      '    </_temp
+00007900: 6c61 7465 735f 3e27 0a20 2020 2027 3c2f  lates_>'.    '</
+00007910: 6d69 6d65 6f5f 636f 6e66 6967 7572 6174  mimeo_configurat
+00007920: 696f 6e3e 2729 0a6d 696d 656f 5f63 6f6e  ion>').mimeo_con
+00007930: 6669 6720 3d20 4d69 6d65 6f43 6f6e 6669  fig = MimeoConfi
+00007940: 6746 6163 746f 7279 2e70 6172 7365 2863  gFactory.parse(c
+00007950: 6f6e 6669 6729 0a60 6060 0a3c 2f74 643e  onfig).```.</td>
+00007960: 0a20 203c 2f74 723e 0a20 2020 203c 7472  .  </tr>.    <tr
+00007970: 3e0a 2020 2020 2020 2020 3c74 643e 3c62  >.        <td><b
+00007980: 3e46 696c 6520 7061 7468 3c2f 623e 3c2f  >File path</b></
+00007990: 7464 3e0a 2020 2020 2020 2020 3c74 6420  td>.        <td 
+000079a0: 7661 6c69 676e 3d22 746f 7022 3e0a 0a60  valign="top">..`
+000079b0: 6060 7079 7468 6f6e 0a66 726f 6d20 6d69  ``python.from mi
+000079c0: 6d65 6f20 696d 706f 7274 204d 696d 656f  meo import Mimeo
+000079d0: 436f 6e66 6967 4661 6374 6f72 790a 0a63  ConfigFactory..c
+000079e0: 6f6e 6669 6720 3d20 2253 6f6d 6545 6e74  onfig = "SomeEnt
+000079f0: 6974 792d 636f 6e66 6967 2e6a 736f 6e22  ity-config.json"
+00007a00: 0a6d 696d 656f 5f63 6f6e 6669 6720 3d20  .mimeo_config = 
+00007a10: 4d69 6d65 6f43 6f6e 6669 6746 6163 746f  MimeoConfigFacto
+00007a20: 7279 2e70 6172 7365 2863 6f6e 6669 6729  ry.parse(config)
+00007a30: 0a60 6060 0a3c 2f74 643e 0a20 2020 203c  .```.</td>.    <
+00007a40: 7464 2076 616c 6967 6e3d 2274 6f70 223e  td valign="top">
+00007a50: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00007a60: 206d 696d 656f 2069 6d70 6f72 7420 4d69   mimeo import Mi
+00007a70: 6d65 6f43 6f6e 6669 6746 6163 746f 7279  meoConfigFactory
+00007a80: 0a0a 636f 6e66 6967 203d 2022 536f 6d65  ..config = "Some
+00007a90: 456e 7469 7479 2d63 6f6e 6669 672e 786d  Entity-config.xm
+00007aa0: 6c22 0a6d 696d 656f 5f63 6f6e 6669 6720  l".mimeo_config 
+00007ab0: 3d20 4d69 6d65 6f43 6f6e 6669 6746 6163  = MimeoConfigFac
+00007ac0: 746f 7279 2e70 6172 7365 2863 6f6e 6669  tory.parse(confi
+00007ad0: 6729 0a60 6060 0a3c 2f74 643e 0a20 203c  g).```.</td>.  <
+00007ae0: 2f74 723e 0a3c 2f74 6162 6c65 3e0a 0a23  /tr>.</table>..#
+00007af0: 2323 2320 5072 6f63 6573 7369 6e67 204d  ### Processing M
+00007b00: 696d 656f 2043 6f6e 6669 6775 7261 7469  imeo Configurati
+00007b10: 6f6e 0a0a 5573 696e 6720 7468 6520 4d69  on..Using the Mi
+00007b20: 6d65 6f20 6173 2061 2070 7974 686f 6e20  meo as a python 
+00007b30: 6c69 6272 6172 7920 796f 7520 6361 6e20  library you can 
+00007b40: 7573 6520 3220 7072 6f63 6573 7369 6e67  use 2 processing
+00007b50: 2061 7070 726f 6163 6865 733a 0a2a 2073   approaches:.* s
+00007b60: 6571 7565 6e74 6961 6c20 7072 6f63 6573  equential proces
+00007b70: 7369 6e67 0a2a 2070 726f 6365 7373 696e  sing.* processin
+00007b80: 6720 696e 2070 6172 616c 6c65 6c20 2875  g in parallel (u
+00007b90: 7365 6420 6279 2064 6566 6175 6c74 2069  sed by default i
+00007ba0: 6e20 4d69 6d65 6f20 434c 4929 0a0a 426f  n Mimeo CLI)..Bo
+00007bb0: 7468 206e 6565 6420 7468 6520 604d 696d  th need the `Mim
+00007bc0: 656f 6772 6170 6860 2063 6c61 7373 2e0a  eograph` class..
+00007bd0: 0a0a 2323 2323 2320 5365 7175 656e 7469  ..##### Sequenti
+00007be0: 616c 2070 726f 6365 7373 696e 670a 0a53  al processing..S
+00007bf0: 6571 7565 6e74 6961 6c20 7072 6f63 6573  equential proces
+00007c00: 7369 6e67 2069 7320 7072 6574 7479 2073  sing is pretty s
+00007c10: 7472 6169 6768 7466 6f72 7761 7264 2061  traightforward a
+00007c20: 6e64 2063 616e 2062 6520 646f 6e65 2077  nd can be done w
+00007c30: 6974 686f 7574 2060 4d69 6d65 6f67 7261  ithout `Mimeogra
+00007c40: 7068 6020 696e 7374 616e 7469 6174 696f  ph` instantiatio
+00007c50: 6e2e 0a0a 2323 2323 2323 2050 726f 6365  n...###### Proce
+00007c60: 7373 696e 670a 0a54 6f20 7369 6d70 6c79  ssing..To simply
+00007c70: 2070 726f 6365 7373 2064 6174 6120 6672   process data fr
+00007c80: 6f6d 2061 204d 696d 656f 2043 6f6e 6669  om a Mimeo Confi
+00007c90: 6775 7261 7469 6f6e 2079 6f75 2063 616e  guration you can
+00007ca0: 2075 7365 2074 6865 2060 4d69 6d65 6f67   use the `Mimeog
+00007cb0: 7261 7068 2e70 726f 6365 7373 2829 6020  raph.process()` 
+00007cc0: 6d65 7468 6f64 3a0a 6060 6070 7974 686f  method:.```pytho
+00007cd0: 6e0a 6672 6f6d 206d 696d 656f 2069 6d70  n.from mimeo imp
+00007ce0: 6f72 7420 4d69 6d65 6f43 6f6e 6669 6746  ort MimeoConfigF
+00007cf0: 6163 746f 7279 2c20 4d69 6d65 6f67 7261  actory, Mimeogra
+00007d00: 7068 0a0a 636f 6e66 6967 5f70 6174 6820  ph..config_path 
+00007d10: 3d20 2265 7861 6d70 6c65 732f 312d 696e  = "examples/1-in
+00007d20: 7472 6f64 7563 7469 6f6e 2f30 312d 6261  troduction/01-ba
+00007d30: 7369 632e 6a73 6f6e 220a 6d69 6d65 6f5f  sic.json".mimeo_
+00007d40: 636f 6e66 6967 203d 204d 696d 656f 436f  config = MimeoCo
+00007d50: 6e66 6967 4661 6374 6f72 792e 7061 7273  nfigFactory.pars
+00007d60: 6528 636f 6e66 6967 5f70 6174 6829 0a4d  e(config_path).M
+00007d70: 696d 656f 6772 6170 682e 7072 6f63 6573  imeograph.proces
+00007d80: 7328 6d69 6d65 6f5f 636f 6e66 6967 290a  s(mimeo_config).
+00007d90: 6060 600a 0a49 7420 7769 6c6c 2067 656e  ```..It will gen
+00007da0: 6572 6174 6520 6461 7461 2061 6e64 2063  erate data and c
+00007db0: 6f6e 7375 6d65 2069 7420 696d 6d65 6469  onsume it immedi
+00007dc0: 6174 656c 792e 0a0a 2323 2323 2323 2047  ately...###### G
+00007dd0: 656e 6572 6174 696e 6720 6f6e 6c79 0a0a  enerating only..
+00007de0: 4966 2079 6f75 2772 6520 676f 696e 6720  If you're going 
+00007df0: 746f 2067 656e 6572 6174 6520 6461 7461  to generate data
+00007e00: 2061 6e64 2075 7365 2069 7420 6173 2061   and use it as a
+00007e10: 2070 7974 686f 6e20 7265 7072 6573 656e   python represen
+00007e20: 7461 7469 6f6e 0a28 6064 6963 7460 2c20  tation.(`dict`, 
+00007e30: 6078 6d6c 2e65 7472 6565 2e45 6c65 6d65  `xml.etree.Eleme
+00007e40: 6e74 5472 6565 2e45 6c65 6d65 6e74 6029  ntTree.Element`)
+00007e50: 202d 2075 7365 2060 4d69 6d65 6f67 7261   - use `Mimeogra
+00007e60: 7068 2e67 656e 6572 6174 6528 2960 206d  ph.generate()` m
+00007e70: 6574 686f 643a 0a60 6060 7079 7468 6f6e  ethod:.```python
+00007e80: 0a66 726f 6d20 6d69 6d65 6f20 696d 706f  .from mimeo impo
+00007e90: 7274 204d 696d 656f 436f 6e66 6967 4661  rt MimeoConfigFa
+00007ea0: 6374 6f72 792c 204d 696d 656f 6772 6170  ctory, Mimeograp
+00007eb0: 680a 0a63 6f6e 6669 675f 7061 7468 203d  h..config_path =
+00007ec0: 2022 6578 616d 706c 6573 2f31 2d69 6e74   "examples/1-int
+00007ed0: 726f 6475 6374 696f 6e2f 3031 2d62 6173  roduction/01-bas
+00007ee0: 6963 2e6a 736f 6e22 0a6d 696d 656f 5f63  ic.json".mimeo_c
+00007ef0: 6f6e 6669 6720 3d20 4d69 6d65 6f43 6f6e  onfig = MimeoCon
+00007f00: 6669 6746 6163 746f 7279 2e70 6172 7365  figFactory.parse
+00007f10: 2863 6f6e 6669 675f 7061 7468 290a 6461  (config_path).da
+00007f20: 7461 203d 204d 696d 656f 6772 6170 682e  ta = Mimeograph.
+00007f30: 6765 6e65 7261 7465 286d 696d 656f 5f63  generate(mimeo_c
+00007f40: 6f6e 6669 6729 0a60 6060 0a0a 2323 2323  onfig).```..####
+00007f50: 2323 2047 656e 6572 6174 696e 6720 616e  ## Generating an
+00007f60: 6420 636f 6e73 756d 696e 6720 696e 2032  d consuming in 2
+00007f70: 2073 7461 6765 730a 0a49 6e20 6361 7365   stages..In case
+00007f80: 2079 6f75 2077 6f75 6c64 206c 696b 6520   you would like 
+00007f90: 746f 2073 6f6d 6568 6f77 206d 6f64 6966  to somehow modif
+00007fa0: 7920 6765 6e65 7261 7465 6420 6461 7461  y generated data
+00007fb0: 2062 6566 6f72 6520 6974 2077 696c 6c20   before it will 
+00007fc0: 6265 2063 6f6e 7375 6d65 642c 0a75 7365  be consumed,.use
+00007fd0: 2060 4d69 6d65 6f67 7261 7068 2e67 656e   `Mimeograph.gen
+00007fe0: 6572 6174 6528 2960 2061 6e64 2060 4d69  erate()` and `Mi
+00007ff0: 6d65 6f67 7261 7068 2e63 6f6e 7375 6d65  meograph.consume
+00008000: 2829 6020 6d65 7468 6f64 732e 0a60 6060  ()` methods..```
+00008010: 7079 7468 6f6e 0a66 726f 6d20 6d69 6d65  python.from mime
+00008020: 6f20 696d 706f 7274 204d 696d 656f 436f  o import MimeoCo
+00008030: 6e66 6967 4661 6374 6f72 792c 204d 696d  nfigFactory, Mim
+00008040: 656f 6772 6170 680a 0a63 6f6e 6669 675f  eograph..config_
+00008050: 7061 7468 203d 2022 6578 616d 706c 6573  path = "examples
+00008060: 2f31 2d69 6e74 726f 6475 6374 696f 6e2f  /1-introduction/
+00008070: 3031 2d62 6173 6963 2e6a 736f 6e22 0a6d  01-basic.json".m
+00008080: 696d 656f 5f63 6f6e 6669 6720 3d20 4d69  imeo_config = Mi
+00008090: 6d65 6f43 6f6e 6669 6746 6163 746f 7279  meoConfigFactory
+000080a0: 2e70 6172 7365 2863 6f6e 6669 675f 7061  .parse(config_pa
+000080b0: 7468 290a 6461 7461 203d 204d 696d 656f  th).data = Mimeo
+000080c0: 6772 6170 682e 6765 6e65 7261 7465 286d  graph.generate(m
+000080d0: 696d 656f 5f63 6f6e 6669 6729 0a23 202e  imeo_config).# .
+000080e0: 2e2e 2079 6f75 7220 6d6f 6469 6669 6361  .. your modifica
+000080f0: 7469 6f6e 7320 2e2e 2e0a 4d69 6d65 6f67  tions ....Mimeog
+00008100: 7261 7068 2e63 6f6e 7375 6d65 286d 696d  raph.consume(mim
+00008110: 656f 5f63 6f6e 6669 672c 2064 6174 6129  eo_config, data)
+00008120: 0a60 6060 0a0a 2323 2323 2320 5072 6f63  .```..##### Proc
+00008130: 6573 7369 6e67 2069 6e20 7061 7261 6c6c  essing in parall
+00008140: 656c 0a0a 5768 656e 2079 6f75 2772 6520  el..When you're 
+00008150: 676f 696e 6720 746f 2070 726f 6365 7373  going to process
+00008160: 2064 6174 6120 2867 656e 6572 6174 6520   data (generate 
+00008170: 616e 6420 636f 6e73 756d 6529 2066 726f  and consume) fro
+00008180: 6d20 7365 7665 7261 6c20 4d69 6d65 6f20  m several Mimeo 
+00008190: 436f 6e66 6967 7572 6174 696f 6e73 0a70  Configurations.p
+000081a0: 726f 6365 7373 696e 6720 696e 2070 6172  rocessing in par
+000081b0: 616c 6c65 6c20 6973 206d 6f72 6520 7065  allel is more pe
+000081c0: 7266 6f72 6d61 6e74 2077 6179 2e20 546f  rformant way. To
+000081d0: 2064 6f20 7468 6174 2c20 796f 7520 6e65   do that, you ne
+000081e0: 6564 2075 7365 2074 6865 2060 4d69 6d65  ed use the `Mime
+000081f0: 6f67 7261 7068 6020 6173 2061 2043 6f6e  ograph` as a Con
+00008200: 7465 7874 204d 616e 6167 6572 0a61 6e64  text Manager.and
+00008210: 2073 7562 6d69 7420 636f 6e66 6967 7320   submit configs 
+00008220: 746f 6765 7468 6572 2077 6974 6820 736f  together with so
+00008230: 6d65 206b 696e 6420 6f66 2069 6465 6e74  me kind of ident
+00008240: 6966 6965 7220 2865 2e67 2e20 636f 6e66  ifier (e.g. conf
+00008250: 6967 2070 6174 6829 2e20 5468 616e 6b73  ig path). Thanks
+00008260: 2074 6f20 7468 6174 2079 6f75 2077 696c   to that you wil
+00008270: 6c20 6b6e 6f77 0a77 6869 6368 2063 6f6e  l know.which con
+00008280: 6669 6720 6861 7320 6661 696c 6564 2028  fig has failed (
+00008290: 6966 2073 6f29 2e0a 0a60 6060 7079 7468  if so)...```pyth
+000082a0: 6f6e 0a66 726f 6d20 6d69 6d65 6f20 696d  on.from mimeo im
+000082b0: 706f 7274 204d 696d 656f 436f 6e66 6967  port MimeoConfig
+000082c0: 4661 6374 6f72 792c 204d 696d 656f 6772  Factory, Mimeogr
+000082d0: 6170 680a 0a63 6f6e 6669 675f 7061 7468  aph..config_path
+000082e0: 7320 3d20 5b0a 2020 2020 2265 7861 6d70  s = [.    "examp
+000082f0: 6c65 732f 312d 696e 7472 6f64 7563 7469  les/1-introducti
+00008300: 6f6e 2f30 312d 6261 7369 632e 6a73 6f6e  on/01-basic.json
+00008310: 222c 0a20 2020 2022 6578 616d 706c 6573  ",.    "examples
+00008320: 2f31 2d69 6e74 726f 6475 6374 696f 6e2f  /1-introduction/
+00008330: 3032 2d63 6f6d 706c 6578 2e6a 736f 6e22  02-complex.json"
+00008340: 2c0a 2020 2020 2265 7861 6d70 6c65 732f  ,.    "examples/
+00008350: 312d 696e 7472 6f64 7563 7469 6f6e 2f30  1-introduction/0
+00008360: 332d 6f75 7470 7574 2d66 6f72 6d61 742d  3-output-format-
+00008370: 786d 6c2e 6a73 6f6e 222c 0a20 2020 2022  xml.json",.    "
+00008380: 6578 616d 706c 6573 2f31 2d69 6e74 726f  examples/1-intro
+00008390: 6475 6374 696f 6e2f 3034 2d6f 7574 7075  duction/04-outpu
+000083a0: 742d 666f 726d 6174 2d6a 736f 6e2e 6a73  t-format-json.js
+000083b0: 6f6e 222c 0a5d 0a77 6974 6820 4d69 6d65  on",.].with Mime
+000083c0: 6f67 7261 7068 2829 2061 7320 6d69 6d65  ograph() as mime
+000083d0: 6f3a 0a20 2020 2066 6f72 2063 6f6e 6669  o:.    for confi
+000083e0: 675f 7061 7468 2069 6e20 636f 6e66 6967  g_path in config
+000083f0: 5f70 6174 6873 3a0a 2020 2020 2020 2020  _paths:.        
+00008400: 6d69 6d65 6f5f 636f 6e66 6967 203d 204d  mimeo_config = M
+00008410: 696d 656f 436f 6e66 6967 4661 6374 6f72  imeoConfigFactor
+00008420: 792e 7061 7273 6528 636f 6e66 6967 5f70  y.parse(config_p
+00008430: 6174 6829 0a20 2020 2020 2020 206d 696d  ath).        mim
+00008440: 656f 5f63 6f6e 6669 672e 6f75 7470 7574  eo_config.output
+00008450: 2e64 6972 6563 7469 6f6e 203d 2022 7374  .direction = "st
+00008460: 646f 7574 220a 2020 2020 2020 2020 6d69  dout".        mi
+00008470: 6d65 6f2e 7375 626d 6974 2828 636f 6e66  meo.submit((conf
+00008480: 6967 5f70 6174 682c 206d 696d 656f 5f63  ig_path, mimeo_c
+00008490: 6f6e 6669 6729 290a 6060 600a 0a23 2320  onfig)).```..## 
+000084a0: 4c69 6365 6e73 650a 0a4d 4954 0a0a 0a23  License..MIT...#
+000084b0: 2320 4175 7468 6f72 730a 0a2d 205b 4054  # Authors..- [@T
+000084c0: 6f6d 6173 7a41 6e69 6f6c 6f77 736b 695d  omaszAniolowski]
+000084d0: 2868 7474 7073 3a2f 2f77 7777 2e67 6974  (https://www.git
+000084e0: 6875 622e 636f 6d2f 546f 6d61 737a 416e  hub.com/TomaszAn
+000084f0: 696f 6c6f 7773 6b69 290a 0a0a 2323 2041  iolowski)...## A
+00008500: 636b 6e6f 776c 6564 6765 6d65 6e74 730a  cknowledgements.
+00008510: 0a20 2d20 5b53 696d 706c 654d 6170 732e  . - [SimpleMaps.
+00008520: 636f 6d5d 2868 7474 7073 3a2f 2f73 696d  com](https://sim
+00008530: 706c 656d 6170 732e 636f 6d2f 6461 7461  plemaps.com/data
+00008540: 2f77 6f72 6c64 2d63 6974 6965 7329 2028  /world-cities) (
+00008550: 4369 7469 6573 2026 2063 6f75 6e74 7269  Cities & countri
+00008560: 6573 2064 6174 6129 0a20 2d20 5b40 6861  es data). - [@ha
+00008570: 646c 6579 2f64 6174 612d 6261 6279 2d6e  dley/data-baby-n
+00008580: 616d 6573 5d28 6874 7470 733a 2f2f 6769  ames](https://gi
+00008590: 7468 7562 2e63 6f6d 2f68 6164 6c65 792f  thub.com/hadley/
+000085a0: 6461 7461 2d62 6162 792d 6e61 6d65 732f  data-baby-names/
+000085b0: 2920 2846 6f72 656e 616d 6573 2064 6174  ) (Forenames dat
+000085c0: 6129 0a20 2d20 5b40 6669 7665 7468 6972  a). - [@fivethir
+000085d0: 7479 6569 6768 2f64 6174 612f 6d6f 7374  tyeigh/data/most
+000085e0: 2d63 6f6d 6d6f 6e2d 6e61 6d65 5d28 6874  -common-name](ht
+000085f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00008600: 2f66 6976 6574 6869 7274 7965 6967 6874  /fivethirtyeight
+00008610: 2f64 6174 612f 7472 6565 2f6d 6173 7465  /data/tree/maste
+00008620: 722f 6d6f 7374 2d63 6f6d 6d6f 6e2d 6e61  r/most-common-na
+00008630: 6d65 2920 2853 7572 6e61 6d65 7320 6461  me) (Surnames da
+00008640: 7461 290a 202d 205b 4064 6174 6173 6574  ta). - [@dataset
+00008650: 732f 6375 7272 656e 6379 2d63 6f64 6573  s/currency-codes
+00008660: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00008670: 2e63 6f6d 2f64 6174 6173 6574 732f 6375  .com/datasets/cu
+00008680: 7272 656e 6379 2d63 6f64 6573 2f29 2028  rrency-codes/) (
+00008690: 4375 7272 656e 6369 6573 2064 6174 6129  Currencies data)
+000086a0: 0a                                       .
```

### Comparing `mimeograph-0.7.0/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-1.0.3/src/mimeograph.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/mimeo/__init__.py
 src/mimeo/__main__.py
+src/mimeo/exc.py
 src/mimeo/mimeo.py
 src/mimeo/tools.py
 src/mimeo/cli/__init__.py
 src/mimeo/cli/exc.py
 src/mimeo/cli/job.py
 src/mimeo/cli/parsers.py
 src/mimeo/config/__init__.py
@@ -34,14 +35,15 @@
 src/mimeo/database/first_names.py
 src/mimeo/database/last_names.py
 src/mimeo/database/mimeo_db.py
 src/mimeo/generators/__init__.py
 src/mimeo/generators/exc.py
 src/mimeo/generators/generator.py
 src/mimeo/generators/generator_factory.py
+src/mimeo/generators/json_generator.py
 src/mimeo/generators/xml_generator.py
 src/mimeo/logging/__init__.py
 src/mimeo/logging/filters.py
 src/mimeo/meta/__init__.py
 src/mimeo/meta/alive.py
 src/mimeo/meta/exc.py
 src/mimeo/resources/__init__.py
```

