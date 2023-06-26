# Comparing `tmp/autobean-0.2.0.tar.gz` & `tmp/autobean-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobean-0.2.0.tar", last modified: Sat May 13 12:44:42 2023, max compression
+gzip compressed data, was "autobean-0.2.1.tar", last modified: Mon Jun 26 10:16:01 2023, max compression
```

## Comparing `autobean-0.2.0.tar` & `autobean-0.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.354304 autobean-0.2.0/
--rw-r--r--   0 seiarotg   (501) staff       (20)    18092 2019-09-03 05:14:19.000000 autobean-0.2.0/LICENSE
--rw-r--r--   0 seiarotg   (501) staff       (20)     2311 2023-05-13 12:44:42.353918 autobean-0.2.0/PKG-INFO
--rw-r--r--   0 seiarotg   (501) staff       (20)     1701 2023-05-13 12:32:14.000000 autobean-0.2.0/README.md
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.334193 autobean-0.2.0/autobean/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2021-01-02 21:42:25.000000 autobean-0.2.0/autobean/__init__.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.337187 autobean-0.2.0/autobean/include/
--rw-r--r--   0 seiarotg   (501) staff       (20)       88 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/include/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     1028 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/include/plugin.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.337991 autobean-0.2.0/autobean/include/tests/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-09-05 14:56:04.000000 autobean-0.2.0/autobean/include/tests/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      869 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/include/tests/test_runner.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.339407 autobean-0.2.0/autobean/narration/
--rw-r--r--   0 seiarotg   (501) staff       (20)       69 2019-09-01 11:30:46.000000 autobean-0.2.0/autobean/narration/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      464 2022-06-11 14:47:44.000000 autobean-0.2.0/autobean/narration/comments.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     1458 2022-06-11 14:47:44.000000 autobean-0.2.0/autobean/narration/plugin.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.340221 autobean-0.2.0/autobean/narration/tests/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-09-01 14:17:47.000000 autobean-0.2.0/autobean/narration/tests/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      195 2022-06-11 14:47:44.000000 autobean-0.2.0/autobean/narration/tests/test_runner.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.344420 autobean-0.2.0/autobean/share/
--rw-r--r--   0 seiarotg   (501) staff       (20)       59 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/share/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     3340 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/share/include.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      826 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/share/include_context.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     8890 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/share/link_accounts.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     9345 2023-01-29 01:59:08.000000 autobean-0.2.0/autobean/share/plugin.py
--rw-r--r--   0 seiarotg   (501) staff       (20)    10792 2023-01-29 03:37:02.000000 autobean-0.2.0/autobean/share/policy_lib.py
--rw-r--r--   0 seiarotg   (501) staff       (20)    23168 2023-01-29 03:38:18.000000 autobean-0.2.0/autobean/share/policy_lib_test.py
--rw-r--r--   0 seiarotg   (501) staff       (20)    21459 2023-01-29 01:59:21.000000 autobean-0.2.0/autobean/share/split_account.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.345327 autobean-0.2.0/autobean/share/tests/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-08-10 06:00:31.000000 autobean-0.2.0/autobean/share/tests/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      358 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/share/tests/test_runner.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      125 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/share/viewpoint_lib.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.346379 autobean-0.2.0/autobean/sorted/
--rw-r--r--   0 seiarotg   (501) staff       (20)       66 2021-01-01 19:45:48.000000 autobean-0.2.0/autobean/sorted/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     3836 2022-12-19 14:01:53.000000 autobean-0.2.0/autobean/sorted/plugin.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.347817 autobean-0.2.0/autobean/stock_split/
--rw-r--r--   0 seiarotg   (501) staff       (20)       58 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/stock_split/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     3057 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/stock_split/plugin.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     4040 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/stock_split/plugin_test.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.348733 autobean-0.2.0/autobean/truelayer/
--rw-r--r--   0 seiarotg   (501) staff       (20)       49 2020-12-29 22:03:00.000000 autobean-0.2.0/autobean/truelayer/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)    17780 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/truelayer/importer.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.351622 autobean-0.2.0/autobean/utils/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-08-10 06:00:31.000000 autobean-0.2.0/autobean/utils/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      953 2022-06-11 14:47:44.000000 autobean-0.2.0/autobean/utils/compare.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     5637 2023-01-02 23:04:05.000000 autobean-0.2.0/autobean/utils/deduplicate.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     1124 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/utils/error_lib.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     7686 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/utils/plugin_lib.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     9373 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/utils/plugin_test_utils.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.352534 autobean-0.2.0/autobean/xcheck/
--rw-r--r--   0 seiarotg   (501) staff       (20)       93 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/xcheck/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)     4205 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/xcheck/plugin.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.353361 autobean-0.2.0/autobean/xcheck/tests/
--rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-08-10 06:00:31.000000 autobean-0.2.0/autobean/xcheck/tests/__init__.py
--rw-r--r--   0 seiarotg   (501) staff       (20)      868 2023-01-29 01:35:33.000000 autobean-0.2.0/autobean/xcheck/tests/test_runner.py
-drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-05-13 12:44:42.336339 autobean-0.2.0/autobean.egg-info/
--rw-r--r--   0 seiarotg   (501) staff       (20)     2311 2023-05-13 12:44:42.000000 autobean-0.2.0/autobean.egg-info/PKG-INFO
--rw-r--r--   0 seiarotg   (501) staff       (20)     1360 2023-05-13 12:44:42.000000 autobean-0.2.0/autobean.egg-info/SOURCES.txt
--rw-r--r--   0 seiarotg   (501) staff       (20)        1 2023-05-13 12:44:42.000000 autobean-0.2.0/autobean.egg-info/dependency_links.txt
--rw-r--r--   0 seiarotg   (501) staff       (20)       47 2023-05-13 12:44:42.000000 autobean-0.2.0/autobean.egg-info/requires.txt
--rw-r--r--   0 seiarotg   (501) staff       (20)        9 2023-05-13 12:44:42.000000 autobean-0.2.0/autobean.egg-info/top_level.txt
--rw-r--r--   0 seiarotg   (501) staff       (20)       38 2023-05-13 12:44:42.354410 autobean-0.2.0/setup.cfg
--rw-r--r--   0 seiarotg   (501) staff       (20)      959 2023-05-13 12:31:37.000000 autobean-0.2.0/setup.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.132926 autobean-0.2.1/
+-rw-r--r--   0 seiarotg   (501) staff       (20)    18092 2019-09-03 05:14:19.000000 autobean-0.2.1/LICENSE
+-rw-r--r--   0 seiarotg   (501) staff       (20)     2311 2023-06-26 10:16:01.132270 autobean-0.2.1/PKG-INFO
+-rw-r--r--   0 seiarotg   (501) staff       (20)     1701 2023-05-13 12:32:14.000000 autobean-0.2.1/README.md
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.085144 autobean-0.2.1/autobean/
+-rw-r--r--   0 seiarotg   (501) staff       (20)        0 2021-01-02 21:42:25.000000 autobean-0.2.1/autobean/__init__.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.090978 autobean-0.2.1/autobean/include/
+-rw-r--r--   0 seiarotg   (501) staff       (20)       88 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/include/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     1028 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/include/plugin.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.092545 autobean-0.2.1/autobean/include/tests/
+-rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-09-05 14:56:04.000000 autobean-0.2.1/autobean/include/tests/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)      869 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/include/tests/test_runner.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.096265 autobean-0.2.1/autobean/narration/
+-rw-r--r--   0 seiarotg   (501) staff       (20)       69 2019-09-01 11:30:46.000000 autobean-0.2.1/autobean/narration/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)      464 2022-06-11 14:47:44.000000 autobean-0.2.1/autobean/narration/comments.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     1458 2022-06-11 14:47:44.000000 autobean-0.2.1/autobean/narration/plugin.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.097639 autobean-0.2.1/autobean/narration/tests/
+-rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-09-01 14:17:47.000000 autobean-0.2.1/autobean/narration/tests/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)      195 2022-06-11 14:47:44.000000 autobean-0.2.1/autobean/narration/tests/test_runner.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.109920 autobean-0.2.1/autobean/share/
+-rw-r--r--   0 seiarotg   (501) staff       (20)       59 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     3512 2023-06-26 10:08:53.000000 autobean-0.2.1/autobean/share/include.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)      826 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/include_context.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     8890 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/link_accounts.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     9345 2023-01-29 01:59:08.000000 autobean-0.2.1/autobean/share/plugin.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)    10792 2023-01-29 03:37:02.000000 autobean-0.2.1/autobean/share/policy_lib.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)    23168 2023-01-29 03:38:18.000000 autobean-0.2.1/autobean/share/policy_lib_test.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)    21459 2023-01-29 01:59:21.000000 autobean-0.2.1/autobean/share/split_account.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.111709 autobean-0.2.1/autobean/share/tests/
+-rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-08-10 06:00:31.000000 autobean-0.2.1/autobean/share/tests/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)      358 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/tests/test_runner.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)      125 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/share/viewpoint_lib.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.113824 autobean-0.2.1/autobean/sorted/
+-rw-r--r--   0 seiarotg   (501) staff       (20)       66 2021-01-01 19:45:48.000000 autobean-0.2.1/autobean/sorted/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     3836 2022-12-19 14:01:53.000000 autobean-0.2.1/autobean/sorted/plugin.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.117613 autobean-0.2.1/autobean/stock_split/
+-rw-r--r--   0 seiarotg   (501) staff       (20)       58 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/stock_split/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     3057 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/stock_split/plugin.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     4040 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/stock_split/plugin_test.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.119105 autobean-0.2.1/autobean/truelayer/
+-rw-r--r--   0 seiarotg   (501) staff       (20)       49 2020-12-29 22:03:00.000000 autobean-0.2.1/autobean/truelayer/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)    17776 2023-05-13 12:50:56.000000 autobean-0.2.1/autobean/truelayer/importer.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.125065 autobean-0.2.1/autobean/utils/
+-rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-08-10 06:00:31.000000 autobean-0.2.1/autobean/utils/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)      953 2022-06-11 14:47:44.000000 autobean-0.2.1/autobean/utils/compare.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     5637 2023-01-02 23:04:05.000000 autobean-0.2.1/autobean/utils/deduplicate.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     1124 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/utils/error_lib.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     7686 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/utils/plugin_lib.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     9373 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/utils/plugin_test_utils.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.128287 autobean-0.2.1/autobean/xcheck/
+-rw-r--r--   0 seiarotg   (501) staff       (20)       93 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/xcheck/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)     4205 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/xcheck/plugin.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.131100 autobean-0.2.1/autobean/xcheck/tests/
+-rw-r--r--   0 seiarotg   (501) staff       (20)        0 2019-08-10 06:00:31.000000 autobean-0.2.1/autobean/xcheck/tests/__init__.py
+-rw-r--r--   0 seiarotg   (501) staff       (20)      868 2023-01-29 01:35:33.000000 autobean-0.2.1/autobean/xcheck/tests/test_runner.py
+drwxr-xr-x   0 seiarotg   (501) staff       (20)        0 2023-06-26 10:16:01.088417 autobean-0.2.1/autobean.egg-info/
+-rw-r--r--   0 seiarotg   (501) staff       (20)     2311 2023-06-26 10:16:00.000000 autobean-0.2.1/autobean.egg-info/PKG-INFO
+-rw-r--r--   0 seiarotg   (501) staff       (20)     1360 2023-06-26 10:16:01.000000 autobean-0.2.1/autobean.egg-info/SOURCES.txt
+-rw-r--r--   0 seiarotg   (501) staff       (20)        1 2023-06-26 10:16:00.000000 autobean-0.2.1/autobean.egg-info/dependency_links.txt
+-rw-r--r--   0 seiarotg   (501) staff       (20)       42 2023-06-26 10:16:00.000000 autobean-0.2.1/autobean.egg-info/requires.txt
+-rw-r--r--   0 seiarotg   (501) staff       (20)        9 2023-06-26 10:16:00.000000 autobean-0.2.1/autobean.egg-info/top_level.txt
+-rw-r--r--   0 seiarotg   (501) staff       (20)       38 2023-06-26 10:16:01.133059 autobean-0.2.1/setup.cfg
+-rw-r--r--   0 seiarotg   (501) staff       (20)      959 2023-06-26 10:11:25.000000 autobean-0.2.1/setup.py
```

### Comparing `autobean-0.2.0/LICENSE` & `autobean-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/PKG-INFO` & `autobean-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobean
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of plugins and scripts that help automating bookkeeping with beancount
 Home-page: https://github.com/SEIAROTg/autobean
 Author: SEIAROTg
 Author-email: seiarotg@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `autobean-0.2.0/README.md` & `autobean-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/include/plugin.py` & `autobean-0.2.1/autobean/include/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/include/tests/test_runner.py` & `autobean-0.2.1/autobean/include/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/narration/plugin.py` & `autobean-0.2.1/autobean/narration/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/share/include.py` & `autobean-0.2.1/autobean/share/include.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         self._includes.update(options['include'])
         self._entries_by_file[path] = entries
         return ()
 
     @plugin_lib.handle_custom('autobean.share.link', 'path to an included ledger, an account in it, path to another included ledger, and an account in it')
     def handle_link(self, entry: Custom, path: str, account: plugin_lib.Account, complement_path: str, complement_account: plugin_lib.Account) -> Iterable[Directive]:
         self._check_enabled(entry)
+        path = os.path.join(os.path.dirname(entry.meta['filename']), path)
+        complement_path = os.path.join(os.path.dirname(entry.meta['filename']), complement_path)
         self._links.append(link_accounts.Link(
             path=path,
             account=account,
             complement_path=complement_path,
             complement_account=complement_account,
             custom=entry,
         ))
```

### Comparing `autobean-0.2.0/autobean/share/include_context.py` & `autobean-0.2.1/autobean/share/include_context.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/share/link_accounts.py` & `autobean-0.2.1/autobean/share/link_accounts.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/share/plugin.py` & `autobean-0.2.1/autobean/share/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/share/policy_lib.py` & `autobean-0.2.1/autobean/share/policy_lib.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/share/policy_lib_test.py` & `autobean-0.2.1/autobean/share/policy_lib_test.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/share/split_account.py` & `autobean-0.2.1/autobean/share/split_account.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/sorted/plugin.py` & `autobean-0.2.1/autobean/sorted/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/stock_split/plugin.py` & `autobean-0.2.1/autobean/stock_split/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/stock_split/plugin_test.py` & `autobean-0.2.1/autobean/stock_split/plugin_test.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/truelayer/importer.py` & `autobean-0.2.1/autobean/truelayer/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,15 +401,15 @@
         state = secrets.token_urlsafe(16)
         code = None
         auth_link = None
 
         class HttpHandler(http.server.BaseHTTPRequestHandler):
             def do_POST(self) -> None:
                 logging.info('OAuth response received.')
-                length = int(self.headers.get('Content-Length'))
+                length = int(self.headers['Content-Length'])
                 body = self.rfile.read(length).decode('utf-8')
                 data = dict(urllib.parse.parse_qsl(body))
                 received_state = data.get('state')
                 received_code = data.get('code')
 
                 if received_code and received_state == state:
                     nonlocal code
```

### Comparing `autobean-0.2.0/autobean/utils/compare.py` & `autobean-0.2.1/autobean/utils/compare.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/utils/deduplicate.py` & `autobean-0.2.1/autobean/utils/deduplicate.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/utils/error_lib.py` & `autobean-0.2.1/autobean/utils/error_lib.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/utils/plugin_lib.py` & `autobean-0.2.1/autobean/utils/plugin_lib.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/utils/plugin_test_utils.py` & `autobean-0.2.1/autobean/utils/plugin_test_utils.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/xcheck/plugin.py` & `autobean-0.2.1/autobean/xcheck/plugin.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean/xcheck/tests/test_runner.py` & `autobean-0.2.1/autobean/xcheck/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/autobean.egg-info/PKG-INFO` & `autobean-0.2.1/autobean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobean
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of plugins and scripts that help automating bookkeeping with beancount
 Home-page: https://github.com/SEIAROTg/autobean
 Author: SEIAROTg
 Author-email: seiarotg@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `autobean-0.2.0/autobean.egg-info/SOURCES.txt` & `autobean-0.2.1/autobean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autobean-0.2.0/setup.py` & `autobean-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt', 'r') as f:
     requirements = list(filter(None, f.read().split('\n')))
 
 setuptools.setup(
     name='autobean',
-    version='0.2.0',
+    version='0.2.1',
     author='SEIAROTg',
     author_email='seiarotg@gmail.com',
     description='A collection of plugins and scripts that help automating bookkeeping with beancount',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/SEIAROTg/autobean',
     packages=setuptools.find_packages(),
```

