# Comparing `tmp/LbAPCommon-0.9.8.tar.gz` & `tmp/LbAPCommon-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbAPCommon-0.9.8.tar", last modified: Thu Jun 22 18:56:21 2023, max compression
+gzip compressed data, was "LbAPCommon-0.9.9.tar", last modified: Thu Jun 22 19:21:10 2023, max compression
```

## Comparing `LbAPCommon-0.9.8.tar` & `LbAPCommon-0.9.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.328000 LbAPCommon-0.9.8/
--rw-r--r--   0 root         (0) root         (0)     2039 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1562 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1144 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    32472 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-22 18:56:21.328000 LbAPCommon-0.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      856 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/README.md
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/environment.yaml
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-22 18:56:21.328000 LbAPCommon-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2536 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.312000 LbAPCommon-0.9.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.316000 LbAPCommon-0.9.8/src/LbAPCommon/
--rw-r--r--   0 root         (0) root         (0)     2108 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5011 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/cern_sso.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.320000 LbAPCommon-0.9.8/src/LbAPCommon/checks/
--rw-r--r--   0 root         (0) root         (0)     4881 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/checks/common.py
--rw-r--r--   0 root         (0) root         (0)     7357 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/checks/num_entries.py
--rw-r--r--   0 root         (0) root         (0)    39009 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/checks/range.py
--rw-r--r--   0 root         (0) root         (0)    20997 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/checks/utils.py
--rw-r--r--   0 root         (0) root         (0)     9381 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/checks/validations.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/config.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/hacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.320000 LbAPCommon-0.9.8/src/LbAPCommon/linting/
--rw-r--r--   0 root         (0) root         (0)      999 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/linting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6047 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/linting/bk_paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.320000 LbAPCommon-0.9.8/src/LbAPCommon/options_parsing/
--rw-r--r--   0 root         (0) root         (0)     3046 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/options_parsing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py
--rw-r--r--   0 root         (0) root         (0)    26782 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/parsing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.320000 LbAPCommon-0.9.8/src/LbAPCommon/validators/
--rw-r--r--   0 root         (0) root         (0)     4451 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/validators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/validators/bookkeeping_xml.py
--rw-r--r--   0 root         (0) root         (0)     3697 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/validators/counters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.320000 LbAPCommon-0.9.8/src/LbAPCommon/validators/logs/
--rw-r--r--   0 root         (0) root         (0)     4105 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/validators/logs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.320000 LbAPCommon-0.9.8/src/LbAPCommon/validators/logs/data/
--rw-r--r--   0 root         (0) root         (0)     3535 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/src/LbAPCommon/validators/logs/data/known_messages.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.316000 LbAPCommon-0.9.8/src/LbAPCommon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-22 18:56:21.000000 LbAPCommon-0.9.8/src/LbAPCommon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1824 2023-06-22 18:56:21.000000 LbAPCommon-0.9.8/src/LbAPCommon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:56:21.000000 LbAPCommon-0.9.8/src/LbAPCommon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:56:21.000000 LbAPCommon-0.9.8/src/LbAPCommon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      155 2023-06-22 18:56:21.000000 LbAPCommon-0.9.8/src/LbAPCommon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-22 18:56:21.000000 LbAPCommon-0.9.8/src/LbAPCommon.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.320000 LbAPCommon-0.9.8/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.320000 LbAPCommon-0.9.8/tests/checks/
--rw-r--r--   0 root         (0) root         (0)   471631 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/checks/example_tuple_with_lumi.root
--rw-r--r--   0 root         (0) root         (0)    47368 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/checks/test_advanced.py
--rw-r--r--   0 root         (0) root         (0)    64427 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/checks/test_simple.py
--rw-r--r--   0 root         (0) root         (0)    90340 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/checks/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.324000 LbAPCommon-0.9.8/tests/example-logs/
--rw-r--r--   0 root         (0) root         (0)   516613 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/example-logs/error-failed-to-read-file.log
--rw-r--r--   0 root         (0) root         (0)   344567 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/example-logs/error-illegal-instruction.log
--rw-r--r--   0 root         (0) root         (0)     3373 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/example-logs/error-missing-shared-library.log
--rw-r--r--   0 root         (0) root         (0)     2723 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/example-logs/error-platform-unsupported.log
--rw-r--r--   0 root         (0) root         (0)   584650 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/example-logs/error-related-info-missing.log
--rw-r--r--   0 root         (0) root         (0)   135940 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/example-logs/good-DaVinci_00110296_00000038_1.log
--rw-r--r--   0 root         (0) root         (0)   139869 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/example-logs/good-DaVinci_00110296_00000194_1.log
--rw-r--r--   0 root         (0) root         (0)   751141 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/example-logs/good-Gauss_00104988_00000011_1.log
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.324000 LbAPCommon-0.9.8/tests/linting/
--rw-r--r--   0 root         (0) root         (0)     1839 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/linting/test_bk_paths.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/linting/test_processing_pass.py
--rw-r--r--   0 root         (0) root         (0)    40668 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/test_good_parsing.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/test_hacks.py
--rw-r--r--   0 root         (0) root         (0)     3540 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/test_log_parsing.py
--rw-r--r--   0 root         (0) root         (0)     3764 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/test_log_splitting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:56:21.328000 LbAPCommon-0.9.8/tests/test_performance/
--rw-r--r--   0 root         (0) root         (0)    44540 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/test_performance/example1.yaml
--rw-r--r--   0 root         (0) root         (0)     1113 2023-06-22 18:56:05.000000 LbAPCommon-0.9.8/tests/test_performance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.632000 LbAPCommon-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-22 19:21:10.632000 LbAPCommon-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      856 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/environment.yaml
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-22 19:21:10.636000 LbAPCommon-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.620000 LbAPCommon-0.9.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.624000 LbAPCommon-0.9.9/src/LbAPCommon/
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/cern_sso.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.624000 LbAPCommon-0.9.9/src/LbAPCommon/checks/
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/checks/common.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/checks/num_entries.py
+-rw-r--r--   0 root         (0) root         (0)    39009 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/checks/range.py
+-rw-r--r--   0 root         (0) root         (0)    20997 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/checks/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9381 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/checks/validations.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/config.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/hacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.628000 LbAPCommon-0.9.9/src/LbAPCommon/linting/
+-rw-r--r--   0 root         (0) root         (0)      999 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/linting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6047 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/linting/bk_paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.628000 LbAPCommon-0.9.9/src/LbAPCommon/options_parsing/
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/options_parsing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py
+-rw-r--r--   0 root         (0) root         (0)    26782 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/parsing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.628000 LbAPCommon-0.9.9/src/LbAPCommon/validators/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/validators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/validators/bookkeeping_xml.py
+-rw-r--r--   0 root         (0) root         (0)     3700 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/validators/counters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.628000 LbAPCommon-0.9.9/src/LbAPCommon/validators/logs/
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/validators/logs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.628000 LbAPCommon-0.9.9/src/LbAPCommon/validators/logs/data/
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/src/LbAPCommon/validators/logs/data/known_messages.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.624000 LbAPCommon-0.9.9/src/LbAPCommon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-22 19:21:10.000000 LbAPCommon-0.9.9/src/LbAPCommon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-06-22 19:21:10.000000 LbAPCommon-0.9.9/src/LbAPCommon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 19:21:10.000000 LbAPCommon-0.9.9/src/LbAPCommon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 19:21:10.000000 LbAPCommon-0.9.9/src/LbAPCommon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-22 19:21:10.000000 LbAPCommon-0.9.9/src/LbAPCommon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-22 19:21:10.000000 LbAPCommon-0.9.9/src/LbAPCommon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.628000 LbAPCommon-0.9.9/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.628000 LbAPCommon-0.9.9/tests/checks/
+-rw-r--r--   0 root         (0) root         (0)   471631 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/checks/example_tuple_with_lumi.root
+-rw-r--r--   0 root         (0) root         (0)    47368 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/checks/test_advanced.py
+-rw-r--r--   0 root         (0) root         (0)    64427 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/checks/test_simple.py
+-rw-r--r--   0 root         (0) root         (0)    90340 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/checks/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.632000 LbAPCommon-0.9.9/tests/example-logs/
+-rw-r--r--   0 root         (0) root         (0)   516613 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/example-logs/error-failed-to-read-file.log
+-rw-r--r--   0 root         (0) root         (0)   344567 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/example-logs/error-illegal-instruction.log
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/example-logs/error-missing-shared-library.log
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/example-logs/error-platform-unsupported.log
+-rw-r--r--   0 root         (0) root         (0)   584650 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/example-logs/error-related-info-missing.log
+-rw-r--r--   0 root         (0) root         (0)   135940 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/example-logs/good-DaVinci_00110296_00000038_1.log
+-rw-r--r--   0 root         (0) root         (0)   139869 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/example-logs/good-DaVinci_00110296_00000194_1.log
+-rw-r--r--   0 root         (0) root         (0)   751141 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/example-logs/good-Gauss_00104988_00000011_1.log
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.632000 LbAPCommon-0.9.9/tests/linting/
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/linting/test_bk_paths.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/linting/test_processing_pass.py
+-rw-r--r--   0 root         (0) root         (0)    40668 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/test_good_parsing.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/test_hacks.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/test_log_parsing.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/test_log_splitting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:21:10.632000 LbAPCommon-0.9.9/tests/test_performance/
+-rw-r--r--   0 root         (0) root         (0)    44540 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/test_performance/example1.yaml
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-22 19:20:53.000000 LbAPCommon-0.9.9/tests/test_performance.py
```

### Comparing `LbAPCommon-0.9.8/.gitignore` & `LbAPCommon-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/.gitlab-ci.yml` & `LbAPCommon-0.9.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/.pre-commit-config.yaml` & `LbAPCommon-0.9.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/LICENSE` & `LbAPCommon-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/PKG-INFO` & `LbAPCommon-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPCommon
-Version: 0.9.8
+Version: 0.9.9
 Summary: Common utilities used by LHCb DPA WP2 related software
 Home-page: https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Keywords: LHCb HEP CERN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LbAPCommon-0.9.8/README.md` & `LbAPCommon-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/setup.py` & `LbAPCommon-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/__init__.py` & `LbAPCommon-0.9.9/src/LbAPCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/cern_sso.py` & `LbAPCommon-0.9.9/src/LbAPCommon/cern_sso.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/checks/__init__.py` & `LbAPCommon-0.9.9/src/LbAPCommon/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/checks/common.py` & `LbAPCommon-0.9.9/src/LbAPCommon/checks/common.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/checks/num_entries.py` & `LbAPCommon-0.9.9/src/LbAPCommon/checks/num_entries.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/checks/range.py` & `LbAPCommon-0.9.9/src/LbAPCommon/checks/range.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/checks/utils.py` & `LbAPCommon-0.9.9/src/LbAPCommon/checks/utils.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/checks/validations.py` & `LbAPCommon-0.9.9/src/LbAPCommon/checks/validations.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/config.py` & `LbAPCommon-0.9.9/src/LbAPCommon/config.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/hacks.py` & `LbAPCommon-0.9.9/src/LbAPCommon/hacks.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/linting/__init__.py` & `LbAPCommon-0.9.9/src/LbAPCommon/linting/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/linting/bk_paths.py` & `LbAPCommon-0.9.9/src/LbAPCommon/linting/bk_paths.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/options_parsing/__init__.py` & `LbAPCommon-0.9.9/src/LbAPCommon/options_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py` & `LbAPCommon-0.9.9/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/parsing.py` & `LbAPCommon-0.9.9/src/LbAPCommon/parsing.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/validators/__init__.py` & `LbAPCommon-0.9.9/src/LbAPCommon/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/validators/bookkeeping_xml.py` & `LbAPCommon-0.9.9/src/LbAPCommon/validators/bookkeeping_xml.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/validators/counters.py` & `LbAPCommon-0.9.9/src/LbAPCommon/validators/counters.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  |    Counter                                      |     #     |    sum     | mean/eff^* | rms/err^*  |     min     |     max     |
 #  |*"#accept"                                       |      1093 |       1093 |(  100.000 +- 0.0914913)%|   -------   |   -------   |
 #  | "Created resolved pi0"                          |     99028 |      99028 |     1.0000 |     0.0000 |      1.0000 |      1.0000 |
 #  | "Created resolved pi0->(ee)(ee)"                |      9283 |       9283 |     1.0000 |     0.0000 |      1.0000 |      1.0000 |
 #  | "Created resolved pi0->g(ee)"                   |     39806 |      39806 |     1.0000 |     0.0000 |      1.0000 |      1.0000 |
 #  | "Created resolved pi0->gg"                      |     49939 |      49939 |     1.0000 |     0.0000 |      1.0000 |      1.0000 |
 
-RE_COUNTER_ROW = r"(^\s\|[\s\*]\"(?P<name>.*?)\"\s*\|(?P<count>[0-9\.\%\(\)\+\-\se]+)\|(?P<sum>[0-9\.\%\(\)\+\-\se]+)\|(?P<meaneff>[0-9\.\%\(\)\+\- e]+)\|(?P<rmserr>[0-9\.\%\(\)\+\-\se]+)\|(?P<min>[0-9\.\%\(\)\+\-\-\se]+)\|((?P<max>[0-9\.\%\(\)\+\- e]+)\||)$\n)"
+RE_COUNTER_ROW = r"(^\s\|[\s\*]\"(?P<name>.*?)\"\s*\|(?P<count>[0-9\.\%\(\)\+\-\se]+)\|(?P<sum>[0-9\.\%\(\)\+\-\se]+)\|(?P<meaneff>[0-9\.\%\(\)\+\- e]+)\|(?P<rmserr>[0-9\.\%\(\)\+\-\se]+)\|((?P<min>[0-9\.\%\(\)\+\-\-\se]+)\||)((?P<max>[0-9\.\%\(\)\+\- e]+)\||)$\n)"
 # Parses a single counter row of the block e.g.
 #  |*"#accept"                                       |      1093 |       1093 |(  100.000 +- 0.0914913)%|   -------   |   -------   |
 
 RE_FLAGS = re.IGNORECASE | re.MULTILINE
 RE_ROW_PARSER = re.compile(RE_COUNTER_ROW, RE_FLAGS)
 RE_FULL_COUNTER_PARSER = re.compile(RE_COUNTER_BLOCK, RE_FLAGS)
```

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/validators/logs/__init__.py` & `LbAPCommon-0.9.9/src/LbAPCommon/validators/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon/validators/logs/data/known_messages.yaml` & `LbAPCommon-0.9.9/src/LbAPCommon/validators/logs/data/known_messages.yaml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon.egg-info/PKG-INFO` & `LbAPCommon-0.9.9/src/LbAPCommon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPCommon
-Version: 0.9.8
+Version: 0.9.9
 Summary: Common utilities used by LHCb DPA WP2 related software
 Home-page: https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Keywords: LHCb HEP CERN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LbAPCommon-0.9.8/src/LbAPCommon.egg-info/SOURCES.txt` & `LbAPCommon-0.9.9/src/LbAPCommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/checks/example_tuple_with_lumi.root` & `LbAPCommon-0.9.9/tests/checks/example_tuple_with_lumi.root`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/checks/test_advanced.py` & `LbAPCommon-0.9.9/tests/checks/test_advanced.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/checks/test_simple.py` & `LbAPCommon-0.9.9/tests/checks/test_simple.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/checks/test_utils.py` & `LbAPCommon-0.9.9/tests/checks/test_utils.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/example-logs/error-failed-to-read-file.log` & `LbAPCommon-0.9.9/tests/example-logs/error-failed-to-read-file.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/example-logs/error-illegal-instruction.log` & `LbAPCommon-0.9.9/tests/example-logs/error-illegal-instruction.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/example-logs/error-missing-shared-library.log` & `LbAPCommon-0.9.9/tests/example-logs/error-missing-shared-library.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/example-logs/error-platform-unsupported.log` & `LbAPCommon-0.9.9/tests/example-logs/error-platform-unsupported.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/example-logs/error-related-info-missing.log` & `LbAPCommon-0.9.9/tests/example-logs/error-related-info-missing.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/example-logs/good-DaVinci_00110296_00000038_1.log` & `LbAPCommon-0.9.9/tests/example-logs/good-DaVinci_00110296_00000038_1.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/example-logs/good-DaVinci_00110296_00000194_1.log` & `LbAPCommon-0.9.9/tests/example-logs/good-DaVinci_00110296_00000194_1.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/example-logs/good-Gauss_00104988_00000011_1.log` & `LbAPCommon-0.9.9/tests/example-logs/good-Gauss_00104988_00000011_1.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/linting/test_bk_paths.py` & `LbAPCommon-0.9.9/tests/linting/test_bk_paths.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/linting/test_processing_pass.py` & `LbAPCommon-0.9.9/tests/linting/test_processing_pass.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/test_good_parsing.py` & `LbAPCommon-0.9.9/tests/test_good_parsing.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/test_hacks.py` & `LbAPCommon-0.9.9/tests/test_hacks.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/test_log_parsing.py` & `LbAPCommon-0.9.9/tests/test_log_parsing.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/test_log_splitting.py` & `LbAPCommon-0.9.9/tests/test_log_splitting.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/test_performance/example1.yaml` & `LbAPCommon-0.9.9/tests/test_performance/example1.yaml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.8/tests/test_performance.py` & `LbAPCommon-0.9.9/tests/test_performance.py`

 * *Files identical despite different names*

