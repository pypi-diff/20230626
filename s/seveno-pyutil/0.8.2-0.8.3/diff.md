# Comparing `tmp/seveno-pyutil-0.8.2.tar.gz` & `tmp/seveno-pyutil-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seveno-pyutil-0.8.2.tar", last modified: Wed Jun  7 13:58:55 2023, max compression
+gzip compressed data, was "seveno-pyutil-0.8.3.tar", last modified: Mon Jun 26 06:11:35 2023, max compression
```

## Comparing `seveno-pyutil-0.8.2.tar` & `seveno-pyutil-0.8.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      307 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/.bumpversion.cfg
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-07 13:58:04.000000 seveno-pyutil-0.8.2/.readthedocs.yml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3582 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/CHANGELOG.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1072 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/LICENSE
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      332 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2129 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1128 2022-10-28 12:44:39.000000 seveno-pyutil-0.8.2/README.md
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.983728 seveno-pyutil-0.8.2/docs/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3582 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/docs/CHANGELOG.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      613 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/Makefile
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.983728 seveno-pyutil-0.8.2/docs/_static/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/_static/.gitkeep
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.983728 seveno-pyutil-0.8.2/docs/_templates/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/_templates/.gitkeep
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1349 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/docs/api.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1686 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/docs/conf.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5575 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.2/docs/examples_and_usage.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      197 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.2/docs/index.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       48 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/license.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      811 2018-03-28 12:00:39.000000 seveno-pyutil-0.8.2/docs/make.bat
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2677 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/setup.cfg
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       69 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/setup.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.979728 seveno-pyutil-0.8.2/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.987728 seveno-pyutil-0.8.2/src/seveno_pyutil/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      883 2023-06-07 13:58:12.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      631 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/benchmarking_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1322 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/collections_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5876 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/datetime_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7235 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/error_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2796 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/file_utilities.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.987728 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      235 2023-06-07 13:24:07.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2971 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/pretty_formatter.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    15725 2023-06-07 13:58:04.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/sql_filter.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     1713 2023-02-24 09:53:12.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1318 2023-02-24 10:32:16.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2906 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/metaprogramming_helpers.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      533 2017-10-23 09:03:29.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/os_utilities.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      503 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.2/src/seveno_pyutil/string_utilities.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.987728 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2129 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1454 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-07 07:47:35.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      368 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       14 2023-06-07 13:58:55.000000 seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/top_level.txt
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/tests/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       91 2017-09-26 08:22:57.000000 seveno-pyutil-0.8.2/tests/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      263 2018-03-29 15:58:00.000000 seveno-pyutil-0.8.2/tests/benchmarking_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      886 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/collections_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      129 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/conftest.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5585 2022-09-02 15:06:06.000000 seveno-pyutil-0.8.2/tests/datetime_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3042 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/error_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      472 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/file_utilities_spec.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-07 13:58:55.991728 seveno-pyutil-0.8.2/tests/fixtures/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       50 2017-09-26 08:24:03.000000 seveno-pyutil-0.8.2/tests/fixtures/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      743 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/metaprograming_helpers_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      529 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/string_utilities_spec.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      202 2022-01-30 09:43:49.000000 seveno-pyutil-0.8.2/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/examples_and_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.317964 seveno-pyutil-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/src/seveno_pyutil/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/benchmarking_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/collections_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/datetime_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/error_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/pretty_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/sql_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/metaprogramming_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/os_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/string_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/benchmarking_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/collections_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/datetime_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/error_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/file_utilities_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/metaprograming_helpers_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/string_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/test_helpers.py
```

### Comparing `seveno-pyutil-0.8.2/CHANGELOG.md` & `seveno-pyutil-0.8.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.8.3 (2023-06-26)
+
+- build: added GitHub action for publishing releases to PyPi
+
 ## 0.8.2 (2023-06-07)
 
 - feat: prettier format for multiline SQL in SQLFilter
 
 ## 0.8.1 (2023-06-07)
 
 - feat: SQLFiler can now sometimes print real SQL instead of query string + params
```

### Comparing `seveno-pyutil-0.8.2/LICENSE` & `seveno-pyutil-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/PKG-INFO` & `seveno-pyutil-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.2
+Version: 0.8.3
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
@@ -27,15 +27,15 @@
 
 # Overview
 
 [![PyPI Status](https://badge.fury.io/py/seveno-pyutil.svg)](https://badge.fury.io/py/seveno-pyutil)
 [![license](https://img.shields.io/pypi/l/seveno_pyutil.svg)](https://opensource.org/licenses/MIT)
 [![tests](https://github.com/tadams42/seveno_pyutil/actions/workflows/tests.yaml/badge.svg?branch=development)](https://github.com/tadams42/seveno_pyutil/actions/workflows/tests.yaml)
 [![codecov](https://codecov.io/gh/tadams42/seveno_pyutil/branch/development/graph/badge.svg?token=9WIWK7B3XX)](https://codecov.io/gh/tadams42/seveno_pyutil)
-[![Documentation Status](https://readthedocs.org/projects/seveno_pyutil/badge/?version=latest)](http://seveno_pyutil.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/seveno-pyutil/badge/?version=latest)](http://seveno-pyutil.readthedocs.io/en/latest/?badge=latest)
 [![python_versions](https://img.shields.io/pypi/pyversions/seveno_pyutil.svg)](https://pypi.org/project/seveno_pyutil/)
 
 Various unsorted Python utilities. [Examples of usage](https://seveno-pyutil.readthedocs.io/en/latest/examples_and_usage.html)
 
 ## Installation
 
 ~~~sh
@@ -49,9 +49,9 @@
 ~~~
 
 ## Development mode
 
 Install with extra dev packages
 
 ~~~sh
-pip install -e .[dev]
+pip install -e .[dev,tests]
 ~~~
```

### Comparing `seveno-pyutil-0.8.2/README.md` & `seveno-pyutil-0.8.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Overview
 
 [![PyPI Status](https://badge.fury.io/py/seveno-pyutil.svg)](https://badge.fury.io/py/seveno-pyutil)
 [![license](https://img.shields.io/pypi/l/seveno_pyutil.svg)](https://opensource.org/licenses/MIT)
 [![tests](https://github.com/tadams42/seveno_pyutil/actions/workflows/tests.yaml/badge.svg?branch=development)](https://github.com/tadams42/seveno_pyutil/actions/workflows/tests.yaml)
 [![codecov](https://codecov.io/gh/tadams42/seveno_pyutil/branch/development/graph/badge.svg?token=9WIWK7B3XX)](https://codecov.io/gh/tadams42/seveno_pyutil)
-[![Documentation Status](https://readthedocs.org/projects/seveno_pyutil/badge/?version=latest)](http://seveno_pyutil.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/seveno-pyutil/badge/?version=latest)](http://seveno-pyutil.readthedocs.io/en/latest/?badge=latest)
 [![python_versions](https://img.shields.io/pypi/pyversions/seveno_pyutil.svg)](https://pypi.org/project/seveno_pyutil/)
 
 Various unsorted Python utilities. [Examples of usage](https://seveno-pyutil.readthedocs.io/en/latest/examples_and_usage.html)
 
 ## Installation
 
 ~~~sh
@@ -22,9 +22,9 @@
 ~~~
 
 ## Development mode
 
 Install with extra dev packages
 
 ~~~sh
-pip install -e .[dev]
+pip install -e .[dev,tests]
 ~~~
```

### Comparing `seveno-pyutil-0.8.2/docs/CHANGELOG.md` & `seveno-pyutil-0.8.3/docs/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.8.3 (2023-06-26)
+
+- build: added GitHub action for publishing releases to PyPi
+
 ## 0.8.2 (2023-06-07)
 
 - feat: prettier format for multiline SQL in SQLFilter
 
 ## 0.8.1 (2023-06-07)
 
 - feat: SQLFiler can now sometimes print real SQL instead of query string + params
```

### Comparing `seveno-pyutil-0.8.2/docs/Makefile` & `seveno-pyutil-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/docs/api.rst` & `seveno-pyutil-0.8.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/docs/conf.py` & `seveno-pyutil-0.8.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 
 author = "tadams42"
 project = "seveno-pyutil"
 copyright = (
     ", ".join(str(y) for y in range(2017, datetime.now().year + 1)) + ", " + author
 )
-release = "0.8.2"
+release = "0.8.3"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
```

### Comparing `seveno-pyutil-0.8.2/docs/examples_and_usage.rst` & `seveno-pyutil-0.8.3/docs/examples_and_usage.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/docs/make.bat` & `seveno-pyutil-0.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/pyproject.toml` & `seveno-pyutil-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "seveno-pyutil"
-version = "0.8.2"
+version = "0.8.3"
 description = "Various unsorted Python utilities"
 readme = "README.md"
+requires-python = ">=3.10"
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3 :: Only",
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries :: Python Modules",
 ]
+keywords = ["utilities"]
+license = { text = "MIT" }
+authors = [{ name = "Tomislav Adamic", email = "tomislav.adamic@gmail.com" }]
+
 dependencies = [
 	"colorlog",
 	"holidays",
 	"marshmallow>=3",
 	"pretty-traceback",
 	"pygments",
 	"python-dateutil>=2.6.0",
 	"sqlparse",
 	"tzlocal",
 ]
-keywords = ["utilities"]
-license = { text = "MIT" }
-requires-python = ">=3.10"
-authors = [{ name = "Tomislav Adamic", email = "tomislav.adamic@gmail.com" }]
 
 
 [project.urls]
 Source = "https://github.com/tadams42/seveno_pyutil"
 Documentation = "https://seveno-pyutil.readthedocs.io/en/latest/"
```

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/__init__.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.2"
+__version__ = "0.8.3"
 
 import logging
 
 from .benchmarking_utilities import Stopwatch
 from .collections_utilities import in_batches
 from .datetime_utilities import ensure_tzinfo, iter_year_month
 from .error_utilities import ExceptionsAsErrors, add_error_to
```

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/benchmarking_utilities.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/benchmarking_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/collections_utilities.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/collections_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/datetime_utilities.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/datetime_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/error_utilities.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/error_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/file_utilities.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/file_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/pretty_formatter.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/pretty_formatter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/sql_filter.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/sql_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,24 @@
                     import flask
                     from seveno_pyutil import FlaskSQLStats, SQLFilter
 
                     SQLFilter.register_sqlalchemy_logging_events(
                         "may_app_sql_logger", 100
                     )
 
-                    db.session.execute("select * from books")
+                    app = flask.Flask()
+
+                    @app.before_request
+                    def log_current_request():
+                        FlaskSQLStats.open()
+
+                        @flask.after_this_request
+                        def log_current_response(response):
+                            FlaskSQLStats.close()
+                            return response
         """
 
         from sqlalchemy import event
         from sqlalchemy.engine import Engine
 
         connection_enricher = ConnectionEnricher(logger, duration_threshold_ms)
```

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/logging_utilities/utilities.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/metaprogramming_helpers.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/metaprogramming_helpers.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil/os_utilities.py` & `seveno-pyutil-0.8.3/src/seveno_pyutil/os_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/PKG-INFO` & `seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.2
+Version: 0.8.3
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
@@ -27,15 +27,15 @@
 
 # Overview
 
 [![PyPI Status](https://badge.fury.io/py/seveno-pyutil.svg)](https://badge.fury.io/py/seveno-pyutil)
 [![license](https://img.shields.io/pypi/l/seveno_pyutil.svg)](https://opensource.org/licenses/MIT)
 [![tests](https://github.com/tadams42/seveno_pyutil/actions/workflows/tests.yaml/badge.svg?branch=development)](https://github.com/tadams42/seveno_pyutil/actions/workflows/tests.yaml)
 [![codecov](https://codecov.io/gh/tadams42/seveno_pyutil/branch/development/graph/badge.svg?token=9WIWK7B3XX)](https://codecov.io/gh/tadams42/seveno_pyutil)
-[![Documentation Status](https://readthedocs.org/projects/seveno_pyutil/badge/?version=latest)](http://seveno_pyutil.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/seveno-pyutil/badge/?version=latest)](http://seveno-pyutil.readthedocs.io/en/latest/?badge=latest)
 [![python_versions](https://img.shields.io/pypi/pyversions/seveno_pyutil.svg)](https://pypi.org/project/seveno_pyutil/)
 
 Various unsorted Python utilities. [Examples of usage](https://seveno-pyutil.readthedocs.io/en/latest/examples_and_usage.html)
 
 ## Installation
 
 ~~~sh
@@ -49,9 +49,9 @@
 ~~~
 
 ## Development mode
 
 Install with extra dev packages
 
 ~~~sh
-pip install -e .[dev]
+pip install -e .[dev,tests]
 ~~~
```

### Comparing `seveno-pyutil-0.8.2/src/seveno_pyutil.egg-info/SOURCES.txt` & `seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/tests/collections_utilities_spec.py` & `seveno-pyutil-0.8.3/tests/collections_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/tests/datetime_utilities_spec.py` & `seveno-pyutil-0.8.3/tests/datetime_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/tests/error_utilities_spec.py` & `seveno-pyutil-0.8.3/tests/error_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/tests/metaprograming_helpers_spec.py` & `seveno-pyutil-0.8.3/tests/metaprograming_helpers_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.2/tests/string_utilities_spec.py` & `seveno-pyutil-0.8.3/tests/string_utilities_spec.py`

 * *Files identical despite different names*

