# Comparing `tmp/zocalo-0.9.0.tar.gz` & `tmp/zocalo-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zocalo-0.9.0.tar", last modified: Wed Aug 18 08:56:40 2021, max compression
+gzip compressed data, was "zocalo-0.9.1.tar", last modified: Thu Sep 30 09:36:40 2021, max compression
```

## Comparing `zocalo-0.9.0.tar` & `zocalo-0.9.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.680057 zocalo-0.9.0/
--rw-r--r--   0 vsts      (1001) docker     (121)      137 2021-08-18 08:56:34.000000 zocalo-0.9.0/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     3483 2021-08-18 08:56:34.000000 zocalo-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     2150 2021-08-18 08:56:34.000000 zocalo-0.9.0/HISTORY.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1481 2021-08-18 08:56:34.000000 zocalo-0.9.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      262 2021-08-18 08:56:34.000000 zocalo-0.9.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     7820 2021-08-18 08:56:40.680057 zocalo-0.9.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)    10940 2021-08-18 08:56:34.000000 zocalo-0.9.0/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.676057 zocalo-0.9.0/docs/
--rw-r--r--   0 vsts      (1001) docker     (121)      607 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/Makefile
--rw-r--r--   0 vsts      (1001) docker     (121)       28 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/authors.rst
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4832 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (121)       33 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/contributing.rst
--rw-r--r--   0 vsts      (1001) docker     (121)       28 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/history.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      310 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1174 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/installation.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      768 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/make.bat
--rw-r--r--   0 vsts      (1001) docker     (121)       27 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/readme.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     5303 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/siteconfig.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1095 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/workflows.rst
--rw-r--r--   0 vsts      (1001) docker     (121)   110339 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/zocalo_graphic.jpg
--rw-r--r--   0 vsts      (1001) docker     (121)    66503 2021-08-18 08:56:34.000000 zocalo-0.9.0/docs/zocalo_queues.jpg
--rw-r--r--   0 vsts      (1001) docker     (121)      130 2021-08-18 08:56:34.000000 zocalo-0.9.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     2220 2021-08-18 08:56:40.680057 zocalo-0.9.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)      700 2021-08-18 08:56:34.000000 zocalo-0.9.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.672057 zocalo-0.9.0/src/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.676057 zocalo-0.9.0/src/zocalo/
--rw-r--r--   0 vsts      (1001) docker     (121)     2212 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.676057 zocalo-0.9.0/src/zocalo/cli/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7710 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/cli/go.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5343 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/cli/wrap.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.680057 zocalo-0.9.0/src/zocalo/configuration/
--rw-r--r--   0 vsts      (1001) docker     (121)    16593 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/configuration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1146 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/configuration/argparse.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1824 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/configuration/plugin_graylog.py
--rw-r--r--   0 vsts      (1001) docker     (121)      421 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/configuration/plugin_jmx.py
--rw-r--r--   0 vsts      (1001) docker     (121)      421 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/configuration/plugin_rabbitmqapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)      188 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/configuration/plugin_storage.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.680057 zocalo-0.9.0/src/zocalo/service/
--rw-r--r--   0 vsts      (1001) docker     (121)     4378 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/service/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10138 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/service/schlockmeister.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.680057 zocalo-0.9.0/src/zocalo/util/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3385 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/util/jmxstats.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2820 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/util/symlink.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3571 2021-08-18 08:56:34.000000 zocalo-0.9.0/src/zocalo/wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.676057 zocalo-0.9.0/src/zocalo.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     7820 2021-08-18 08:56:40.000000 zocalo-0.9.0/src/zocalo.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1330 2021-08-18 08:56:40.000000 zocalo-0.9.0/src/zocalo.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-08-18 08:56:40.000000 zocalo-0.9.0/src/zocalo.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      658 2021-08-18 08:56:40.000000 zocalo-0.9.0/src/zocalo.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-08-18 08:56:40.000000 zocalo-0.9.0/src/zocalo.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       57 2021-08-18 08:56:40.000000 zocalo-0.9.0/src/zocalo.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        7 2021-08-18 08:56:40.000000 zocalo-0.9.0/src/zocalo.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.680057 zocalo-0.9.0/tests/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.680057 zocalo-0.9.0/tests/configuration/
--rw-r--r--   0 vsts      (1001) docker     (121)    10488 2021-08-18 08:56:34.000000 zocalo-0.9.0/tests/configuration/test_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1383 2021-08-18 08:56:34.000000 zocalo-0.9.0/tests/configuration/test_plugin_graylog.py
--rw-r--r--   0 vsts      (1001) docker     (121)      917 2021-08-18 08:56:34.000000 zocalo-0.9.0/tests/configuration/test_plugin_jmx.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1372 2021-08-18 08:56:34.000000 zocalo-0.9.0/tests/configuration/test_plugin_storage.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1801 2021-08-18 08:56:34.000000 zocalo-0.9.0/tests/test_graylog.py
--rw-r--r--   0 vsts      (1001) docker     (121)      568 2021-08-18 08:56:34.000000 zocalo-0.9.0/tests/test_zocalo.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-08-18 08:56:40.680057 zocalo-0.9.0/tests/util/
--rw-r--r--   0 vsts      (1001) docker     (121)     1817 2021-08-18 08:56:34.000000 zocalo-0.9.0/tests/util/test_symlink.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.075576 zocalo-0.9.1/
+-rw-r--r--   0 vsts      (1001) docker     (121)      137 2021-09-30 09:36:30.000000 zocalo-0.9.1/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     3483 2021-09-30 09:36:30.000000 zocalo-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     2150 2021-09-30 09:36:30.000000 zocalo-0.9.1/HISTORY.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1481 2021-09-30 09:36:30.000000 zocalo-0.9.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      262 2021-09-30 09:36:30.000000 zocalo-0.9.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     7023 2021-09-30 09:36:40.075576 zocalo-0.9.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)    10940 2021-09-30 09:36:30.000000 zocalo-0.9.1/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.071575 zocalo-0.9.1/docs/
+-rw-r--r--   0 vsts      (1001) docker     (121)      607 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (121)       28 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/authors.rst
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     4832 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       33 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/contributing.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)       28 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/history.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)      310 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1174 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/installation.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)      768 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/make.bat
+-rw-r--r--   0 vsts      (1001) docker     (121)       27 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/readme.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     5303 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/siteconfig.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1095 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/workflows.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)   110339 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/zocalo_graphic.jpg
+-rw-r--r--   0 vsts      (1001) docker     (121)    66503 2021-09-30 09:36:30.000000 zocalo-0.9.1/docs/zocalo_queues.jpg
+-rw-r--r--   0 vsts      (1001) docker     (121)      130 2021-09-30 09:36:30.000000 zocalo-0.9.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2220 2021-09-30 09:36:40.075576 zocalo-0.9.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      700 2021-09-30 09:36:30.000000 zocalo-0.9.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.063575 zocalo-0.9.1/src/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.071575 zocalo-0.9.1/src/zocalo/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2212 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.071575 zocalo-0.9.1/src/zocalo/cli/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7710 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/cli/go.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5343 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/cli/wrap.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.075576 zocalo-0.9.1/src/zocalo/configuration/
+-rw-r--r--   0 vsts      (1001) docker     (121)    16663 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/configuration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1146 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/configuration/argparse.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1824 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/configuration/plugin_graylog.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      421 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/configuration/plugin_jmx.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      421 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/configuration/plugin_rabbitmqapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      188 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/configuration/plugin_storage.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.075576 zocalo-0.9.1/src/zocalo/service/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4439 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/service/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10138 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/service/schlockmeister.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.075576 zocalo-0.9.1/src/zocalo/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3386 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/util/jmxstats.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2820 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/util/symlink.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3571 2021-09-30 09:36:30.000000 zocalo-0.9.1/src/zocalo/wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.071575 zocalo-0.9.1/src/zocalo.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7023 2021-09-30 09:36:39.000000 zocalo-0.9.1/src/zocalo.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1330 2021-09-30 09:36:40.000000 zocalo-0.9.1/src/zocalo.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-09-30 09:36:39.000000 zocalo-0.9.1/src/zocalo.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      658 2021-09-30 09:36:39.000000 zocalo-0.9.1/src/zocalo.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-09-30 09:36:39.000000 zocalo-0.9.1/src/zocalo.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)       57 2021-09-30 09:36:39.000000 zocalo-0.9.1/src/zocalo.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        7 2021-09-30 09:36:39.000000 zocalo-0.9.1/src/zocalo.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.075576 zocalo-0.9.1/tests/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.075576 zocalo-0.9.1/tests/configuration/
+-rw-r--r--   0 vsts      (1001) docker     (121)    10870 2021-09-30 09:36:30.000000 zocalo-0.9.1/tests/configuration/test_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1383 2021-09-30 09:36:30.000000 zocalo-0.9.1/tests/configuration/test_plugin_graylog.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      917 2021-09-30 09:36:30.000000 zocalo-0.9.1/tests/configuration/test_plugin_jmx.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1372 2021-09-30 09:36:30.000000 zocalo-0.9.1/tests/configuration/test_plugin_storage.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1801 2021-09-30 09:36:30.000000 zocalo-0.9.1/tests/test_graylog.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      568 2021-09-30 09:36:30.000000 zocalo-0.9.1/tests/test_zocalo.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-09-30 09:36:40.075576 zocalo-0.9.1/tests/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1817 2021-09-30 09:36:30.000000 zocalo-0.9.1/tests/util/test_symlink.py
```

### Comparing `zocalo-0.9.0/CONTRIBUTING.rst` & `zocalo-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/HISTORY.rst` & `zocalo-0.9.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/LICENSE` & `zocalo-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/PKG-INFO` & `zocalo-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,126 +1,129 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: zocalo
-Version: 0.9.0
+Version: 0.9.1
 Summary: Infrastructure components for automated data processing at Diamond Light Source
 Home-page: UNKNOWN
 Author: Diamond Light Source - Scientific Software et al.
 Author-email: scientificsoftware@diamond.ac.uk
 License: BSD
 Project-URL: Download, https://github.com/DiamondLightSource/python-zocalo/releases
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-zocalo
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-zocalo
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-zocalo/issues
-Description: ======
-        Zocalo
-        ======
-        
-        
-        .. image:: https://img.shields.io/pypi/v/zocalo.svg
-                :target: https://pypi.python.org/pypi/zocalo
-                :alt: PyPI release
-        
-        .. image:: https://img.shields.io/conda/vn/conda-forge/zocalo.svg
-                :target: https://anaconda.org/conda-forge/zocalo
-                :alt: Conda version
-        
-        .. image:: https://dev.azure.com/zocalo/python-zocalo/_apis/build/status/DiamondLightSource.python-zocalo?branchName=main
-                :target: https://dev.azure.com/zocalo/python-zocalo/_build/latest?definitionId=2&branchName=main
-                :alt: Build status
-        
-        .. image:: https://img.shields.io/lgtm/grade/python/g/DiamondLightSource/python-zocalo.svg?logo=lgtm&logoWidth=18
-                :target: https://lgtm.com/projects/g/DiamondLightSource/python-zocalo/context:python
-                :alt: Language grade: Python
-        
-        .. image:: https://img.shields.io/lgtm/alerts/g/DiamondLightSource/python-zocalo.svg?logo=lgtm&logoWidth=18
-                :target: https://lgtm.com/projects/g/DiamondLightSource/python-zocalo/alerts/
-                :alt: Total alerts
-        
-        .. image:: https://readthedocs.org/projects/zocalo/badge/?version=latest
-                :target: https://zocalo.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation status
-        
-        .. image:: https://img.shields.io/pypi/pyversions/zocalo.svg
-                :target: https://pypi.org/project/zocalo/
-                :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-                :target: https://github.com/ambv/black
-                :alt: Code style: black
-        
-        .. image:: https://img.shields.io/pypi/l/zocalo.svg
-                :target: https://pypi.python.org/pypi/zocalo
-                :alt: BSD license
-        
-        ..
-        
-                |
-                | `M. Gerstel, A. Ashton, R.J. Gildea, K. Levik, and G. Winter, "Data Analysis Infrastructure for Diamond Light Source Macromolecular & Chemical Crystallography and Beyond", in Proc. ICALEPCS'19, New York, NY, USA, Oct. 2019, pp. 1031-1035. <https://doi.org/10.18429/JACoW-ICALEPCS2019-WEMPR001>`_ |DOI|
-        
-                .. |DOI| image:: https://img.shields.io/badge/DOI-10.18429/JACoW--ICALEPCS2019--WEMPR001-blue.svg
-                        :target: https://doi.org/10.18429/JACoW-ICALEPCS2019-WEMPR001
-                        :alt: Primary Reference DOI
-        
-        |
-        
-        Zocalo is an automated data processing system designed at Diamond Light Source. This repository contains infrastructure components for Zocalo.
-        
-        The idea of Zocalo is a simple one - to build a messaging framework, where text-based messages are sent between parts of the system to coordinate data analysis. In the wider scope of things this also covers things like archiving, but generally it is handling everything that happens after data aquisition.
-        
-        Zocalo as a wider whole is made up of two repositories (plus some private internal repositories when deployed at Diamond):
-        
-        * `DiamondLightSource/python-zocalo <https://github.com/DiamondLightSource/python-zocalo>`_ - Infrastructure components for automated data processing, developed by Diamond Light Source. The package is available through `PyPi <https://pypi.org/project/zocalo/>`__ and `conda-forge <https://anaconda.org/conda-forge/zocalo>`__.
-        * `DiamondLightSource/python-workflows <https://github.com/DiamondLightSource/python-workflows/>`_ - Zocalo is built on the workflows package. It shouldn't be necessary to interact too much with this package, as the details are abstracted by Zocalo. workflows controls the logic of how services connect to each other and what a service is, and actually send the messages to a message broker. Currently this is an ActiveMQ_ broker (via STOMP_) but support for a RabbitMQ_ broker (via pika_) is being added. This is also available on `PyPi <https://pypi.org/project/workflows/>`__ and `conda-forge <https://anaconda.org/conda-forge/workflows>`__.
-        
-        As mentioned, Zocalo is currently built on top of ActiveMQ. ActiveMQ is an apache project that provides a `message broker <https://en.wikipedia.org/wiki/Message_broker>`_ server, acting as a central dispatch that allows various services to communicate. Messages are plaintext, but from the Zocalo point of view it's passing aroung python objects (json dictionaries). Every message sent has a destination to help the message broker route. Messages may either be sent to a specific queue or broadcast to multiple queues. These queues are subscribed to by the services that run in Zocalo. In developing with Zocalo, you may have to interact with ActiveMQ or RabbitMQ, but it is unlikely that you will have to configure it.
-        
-        Zocalo allows for the monitoring of jobs executing ``python-workflows`` services or recipe wrappers. The ``python-workflows`` package contains most of the infrastructure required for the jobs themselves and more detailed documentation of its components can be found in the ``python-workflows`` `GitHub repository <https://github.com/DiamondLightSource/python-workflows/>`_ and `the Zocalo documentation <https://zocalo.readthedocs.io>`_. 
-        
-        .. _ActiveMQ: http://activemq.apache.org/
-        .. _STOMP: https://stomp.github.io/
-        .. _RabbitMQ: https://www.rabbitmq.com/
-        .. _pika: https://github.com/pika/pika
-        
-        
-        =======
-        History
-        =======
-        
-        0.9.0 (2021-08-18)
-        ------------------
-        * Removed --live/--test command line arguments, use -e/--environment instead
-        * zocalo.go, zocalo.service, zocalo.wrap accept -t/--transport command line
-          options, and the default can be set via the site configuration.
-        
-        0.8.1 (2021-07-08)
-        ------------------
-        * Keep wrapper status threads alive through transport disconnection events
-        
-        0.8.0 (2021-05-18)
-        ------------------
-        * Support for Zocalo configuration files
-        
-        0.7.4 (2021-03-17)
-        ------------------
-        * Documentation improvements
-        
-        0.7.3 (2021-01-19)
-        ------------------
-        * Ignore error when logserver hostname can't be looked up immediately
-        
-        0.7.2 (2021-01-18)
-        ------------------
-        * Add a symbolic link handling library function
-        * Cache the logserver hostname by default
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+License-File: LICENSE
+
+======
+Zocalo
+======
+
+
+.. image:: https://img.shields.io/pypi/v/zocalo.svg
+        :target: https://pypi.python.org/pypi/zocalo
+        :alt: PyPI release
+
+.. image:: https://img.shields.io/conda/vn/conda-forge/zocalo.svg
+        :target: https://anaconda.org/conda-forge/zocalo
+        :alt: Conda version
+
+.. image:: https://dev.azure.com/zocalo/python-zocalo/_apis/build/status/DiamondLightSource.python-zocalo?branchName=main
+        :target: https://dev.azure.com/zocalo/python-zocalo/_build/latest?definitionId=2&branchName=main
+        :alt: Build status
+
+.. image:: https://img.shields.io/lgtm/grade/python/g/DiamondLightSource/python-zocalo.svg?logo=lgtm&logoWidth=18
+        :target: https://lgtm.com/projects/g/DiamondLightSource/python-zocalo/context:python
+        :alt: Language grade: Python
+
+.. image:: https://img.shields.io/lgtm/alerts/g/DiamondLightSource/python-zocalo.svg?logo=lgtm&logoWidth=18
+        :target: https://lgtm.com/projects/g/DiamondLightSource/python-zocalo/alerts/
+        :alt: Total alerts
+
+.. image:: https://readthedocs.org/projects/zocalo/badge/?version=latest
+        :target: https://zocalo.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation status
+
+.. image:: https://img.shields.io/pypi/pyversions/zocalo.svg
+        :target: https://pypi.org/project/zocalo/
+        :alt: Supported Python versions
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+        :target: https://github.com/ambv/black
+        :alt: Code style: black
+
+.. image:: https://img.shields.io/pypi/l/zocalo.svg
+        :target: https://pypi.python.org/pypi/zocalo
+        :alt: BSD license
+
+..
+
+        |
+        | `M. Gerstel, A. Ashton, R.J. Gildea, K. Levik, and G. Winter, "Data Analysis Infrastructure for Diamond Light Source Macromolecular & Chemical Crystallography and Beyond", in Proc. ICALEPCS'19, New York, NY, USA, Oct. 2019, pp. 1031-1035. <https://doi.org/10.18429/JACoW-ICALEPCS2019-WEMPR001>`_ |DOI|
+
+        .. |DOI| image:: https://img.shields.io/badge/DOI-10.18429/JACoW--ICALEPCS2019--WEMPR001-blue.svg
+                :target: https://doi.org/10.18429/JACoW-ICALEPCS2019-WEMPR001
+                :alt: Primary Reference DOI
+
+|
+
+Zocalo is an automated data processing system designed at Diamond Light Source. This repository contains infrastructure components for Zocalo.
+
+The idea of Zocalo is a simple one - to build a messaging framework, where text-based messages are sent between parts of the system to coordinate data analysis. In the wider scope of things this also covers things like archiving, but generally it is handling everything that happens after data aquisition.
+
+Zocalo as a wider whole is made up of two repositories (plus some private internal repositories when deployed at Diamond):
+
+* `DiamondLightSource/python-zocalo <https://github.com/DiamondLightSource/python-zocalo>`_ - Infrastructure components for automated data processing, developed by Diamond Light Source. The package is available through `PyPi <https://pypi.org/project/zocalo/>`__ and `conda-forge <https://anaconda.org/conda-forge/zocalo>`__.
+* `DiamondLightSource/python-workflows <https://github.com/DiamondLightSource/python-workflows/>`_ - Zocalo is built on the workflows package. It shouldn't be necessary to interact too much with this package, as the details are abstracted by Zocalo. workflows controls the logic of how services connect to each other and what a service is, and actually send the messages to a message broker. Currently this is an ActiveMQ_ broker (via STOMP_) but support for a RabbitMQ_ broker (via pika_) is being added. This is also available on `PyPi <https://pypi.org/project/workflows/>`__ and `conda-forge <https://anaconda.org/conda-forge/workflows>`__.
+
+As mentioned, Zocalo is currently built on top of ActiveMQ. ActiveMQ is an apache project that provides a `message broker <https://en.wikipedia.org/wiki/Message_broker>`_ server, acting as a central dispatch that allows various services to communicate. Messages are plaintext, but from the Zocalo point of view it's passing aroung python objects (json dictionaries). Every message sent has a destination to help the message broker route. Messages may either be sent to a specific queue or broadcast to multiple queues. These queues are subscribed to by the services that run in Zocalo. In developing with Zocalo, you may have to interact with ActiveMQ or RabbitMQ, but it is unlikely that you will have to configure it.
+
+Zocalo allows for the monitoring of jobs executing ``python-workflows`` services or recipe wrappers. The ``python-workflows`` package contains most of the infrastructure required for the jobs themselves and more detailed documentation of its components can be found in the ``python-workflows`` `GitHub repository <https://github.com/DiamondLightSource/python-workflows/>`_ and `the Zocalo documentation <https://zocalo.readthedocs.io>`_. 
+
+.. _ActiveMQ: http://activemq.apache.org/
+.. _STOMP: https://stomp.github.io/
+.. _RabbitMQ: https://www.rabbitmq.com/
+.. _pika: https://github.com/pika/pika
+
+
+=======
+History
+=======
+
+0.9.0 (2021-08-18)
+------------------
+* Removed --live/--test command line arguments, use -e/--environment instead
+* zocalo.go, zocalo.service, zocalo.wrap accept -t/--transport command line
+  options, and the default can be set via the site configuration.
+
+0.8.1 (2021-07-08)
+------------------
+* Keep wrapper status threads alive through transport disconnection events
+
+0.8.0 (2021-05-18)
+------------------
+* Support for Zocalo configuration files
+
+0.7.4 (2021-03-17)
+------------------
+* Documentation improvements
+
+0.7.3 (2021-01-19)
+------------------
+* Ignore error when logserver hostname can't be looked up immediately
+
+0.7.2 (2021-01-18)
+------------------
+* Add a symbolic link handling library function
+* Cache the logserver hostname by default
+
+
```

### Comparing `zocalo-0.9.0/README.rst` & `zocalo-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/docs/Makefile` & `zocalo-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/docs/conf.py` & `zocalo-0.9.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 author = "Scientific Software"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = "0.9.0"
+version = "0.9.1"
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `zocalo-0.9.0/docs/installation.rst` & `zocalo-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/docs/make.bat` & `zocalo-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/docs/siteconfig.rst` & `zocalo-0.9.1/docs/siteconfig.rst`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/docs/workflows.rst` & `zocalo-0.9.1/docs/workflows.rst`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/docs/zocalo_graphic.jpg` & `zocalo-0.9.1/docs/zocalo_graphic.jpg`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/docs/zocalo_queues.jpg` & `zocalo-0.9.1/docs/zocalo_queues.jpg`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/setup.cfg` & `zocalo-0.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zocalo
-version = 0.9.0
+version = 0.9.1
 description = Infrastructure components for automated data processing at Diamond Light Source
 author = Diamond Light Source - Scientific Software et al.
 author_email = scientificsoftware@diamond.ac.uk
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
```

### Comparing `zocalo-0.9.0/setup.py` & `zocalo-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/src/zocalo/__init__.py` & `zocalo-0.9.1/src/zocalo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import socket
 import warnings
 
 import graypy.handler
 
 __author__ = "Markus Gerstel"
 __email__ = "scientificsoftware@diamond.ac.uk"
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 logging.getLogger("zocalo").addHandler(logging.NullHandler())
 
 
 class ConfigurationError(Exception):
     pass
```

### Comparing `zocalo-0.9.0/src/zocalo/cli/go.py` & `zocalo-0.9.1/src/zocalo/cli/go.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/src/zocalo/cli/wrap.py` & `zocalo-0.9.1/src/zocalo/cli/wrap.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/src/zocalo/configuration/__init__.py` & `zocalo-0.9.1/src/zocalo/configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                 dest="environment",
                 metavar="ENV",
                 action="append",
                 default=[],
                 type="choice",
                 choices=sorted(self._environments),
                 help="Enable site-specific settings. Choices are: "
-                + ", ".join(sorted(self._environments)),
+                + ", ".join(sorted(set(self._environments) - {"default"})),
             )
 
     if typing.TYPE_CHECKING:
         # The configuration object will offer access to plugin objects as attributes.
         # Type checking tools will not be able to determine the type of attributes,
         # however we need to tell type checkers that accessing statically undefined
         # attributes is allowed. We do this by setting a return type on __getattr__,
@@ -365,15 +365,17 @@
         raise TypeError(
             "Either a configuration string or a configuration file must be specified"
         )
 
     # Resolve all lazy file references relative to the specified context parameter
     for plugin in parsed:
         if isinstance(parsed[plugin], str):
-            parsed[plugin] = context.joinpath(parsed[plugin]).resolve()
+            parsed[plugin] = (
+                context / pathlib.Path(parsed[plugin]).expanduser()
+            ).resolve()
 
     # Recursively identify and merge external files (DFS)
     if parsed.get("include"):
         for include_file in parsed["include"]:
             try:
                 file_reference = context.joinpath(include_file).resolve()
                 include = _read_configuration_yaml(file_reference.read_text())
```

### Comparing `zocalo-0.9.0/src/zocalo/configuration/argparse.py` & `zocalo-0.9.1/src/zocalo/configuration/argparse.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/src/zocalo/configuration/plugin_graylog.py` & `zocalo-0.9.1/src/zocalo/configuration/plugin_graylog.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/src/zocalo/service/__init__.py` & `zocalo-0.9.1/src/zocalo/service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         self.log.debug("Launching %r", sys.argv)
 
     def on_parsing(self, options, args):
         if options.verbose:
             self.console.setLevel(logging.DEBUG)
         if options.debug:
             self.console.setLevel(logging.DEBUG)
+            logging.getLogger("pika").setLevel(logging.INFO)
             logging.getLogger("stomp.py").setLevel(logging.DEBUG)
             logging.getLogger("workflows").setLevel(logging.DEBUG)
         self.options = options
 
     def before_frontend_construction(self, kwargs):
         kwargs["verbose_service"] = True
         kwargs["environment"] = kwargs.get("environment", {})
```

### Comparing `zocalo-0.9.0/src/zocalo/service/schlockmeister.py` & `zocalo-0.9.1/src/zocalo/service/schlockmeister.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/src/zocalo/util/jmxstats.py` & `zocalo-0.9.1/src/zocalo/util/jmxstats.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     from a running JVM."""
 
     def __init__(self, zc: zocalo.configuration.Configuration):
         if not zc.jmx:
             raise zocalo.ConfigurationError(
                 "There are no JMX credentials configured in your environment"
             )
-        self.url = f"http://{zc.jmx['host']}:{zc.jmx['port']}/{zc.jmx['baseurl']}/read/"
+        self.url = f"http://{zc.jmx['host']}:{zc.jmx['port']}/{zc.jmx['base_url']}/read/"
         self._authstring = b"Basic " + base64.b64encode(
             zc.jmx["username"].encode("utf-8")
             + b":"
             + zc.jmx["password"].encode("utf-8")
         )
 
     def __getattribute__(self, attribute):
```

### Comparing `zocalo-0.9.0/src/zocalo/util/symlink.py` & `zocalo-0.9.1/src/zocalo/util/symlink.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/src/zocalo/wrapper.py` & `zocalo-0.9.1/src/zocalo/wrapper.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/src/zocalo.egg-info/PKG-INFO` & `zocalo-0.9.1/src/zocalo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,126 +1,129 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: zocalo
-Version: 0.9.0
+Version: 0.9.1
 Summary: Infrastructure components for automated data processing at Diamond Light Source
 Home-page: UNKNOWN
 Author: Diamond Light Source - Scientific Software et al.
 Author-email: scientificsoftware@diamond.ac.uk
 License: BSD
 Project-URL: Download, https://github.com/DiamondLightSource/python-zocalo/releases
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-zocalo
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-zocalo
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-zocalo/issues
-Description: ======
-        Zocalo
-        ======
-        
-        
-        .. image:: https://img.shields.io/pypi/v/zocalo.svg
-                :target: https://pypi.python.org/pypi/zocalo
-                :alt: PyPI release
-        
-        .. image:: https://img.shields.io/conda/vn/conda-forge/zocalo.svg
-                :target: https://anaconda.org/conda-forge/zocalo
-                :alt: Conda version
-        
-        .. image:: https://dev.azure.com/zocalo/python-zocalo/_apis/build/status/DiamondLightSource.python-zocalo?branchName=main
-                :target: https://dev.azure.com/zocalo/python-zocalo/_build/latest?definitionId=2&branchName=main
-                :alt: Build status
-        
-        .. image:: https://img.shields.io/lgtm/grade/python/g/DiamondLightSource/python-zocalo.svg?logo=lgtm&logoWidth=18
-                :target: https://lgtm.com/projects/g/DiamondLightSource/python-zocalo/context:python
-                :alt: Language grade: Python
-        
-        .. image:: https://img.shields.io/lgtm/alerts/g/DiamondLightSource/python-zocalo.svg?logo=lgtm&logoWidth=18
-                :target: https://lgtm.com/projects/g/DiamondLightSource/python-zocalo/alerts/
-                :alt: Total alerts
-        
-        .. image:: https://readthedocs.org/projects/zocalo/badge/?version=latest
-                :target: https://zocalo.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation status
-        
-        .. image:: https://img.shields.io/pypi/pyversions/zocalo.svg
-                :target: https://pypi.org/project/zocalo/
-                :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-                :target: https://github.com/ambv/black
-                :alt: Code style: black
-        
-        .. image:: https://img.shields.io/pypi/l/zocalo.svg
-                :target: https://pypi.python.org/pypi/zocalo
-                :alt: BSD license
-        
-        ..
-        
-                |
-                | `M. Gerstel, A. Ashton, R.J. Gildea, K. Levik, and G. Winter, "Data Analysis Infrastructure for Diamond Light Source Macromolecular & Chemical Crystallography and Beyond", in Proc. ICALEPCS'19, New York, NY, USA, Oct. 2019, pp. 1031-1035. <https://doi.org/10.18429/JACoW-ICALEPCS2019-WEMPR001>`_ |DOI|
-        
-                .. |DOI| image:: https://img.shields.io/badge/DOI-10.18429/JACoW--ICALEPCS2019--WEMPR001-blue.svg
-                        :target: https://doi.org/10.18429/JACoW-ICALEPCS2019-WEMPR001
-                        :alt: Primary Reference DOI
-        
-        |
-        
-        Zocalo is an automated data processing system designed at Diamond Light Source. This repository contains infrastructure components for Zocalo.
-        
-        The idea of Zocalo is a simple one - to build a messaging framework, where text-based messages are sent between parts of the system to coordinate data analysis. In the wider scope of things this also covers things like archiving, but generally it is handling everything that happens after data aquisition.
-        
-        Zocalo as a wider whole is made up of two repositories (plus some private internal repositories when deployed at Diamond):
-        
-        * `DiamondLightSource/python-zocalo <https://github.com/DiamondLightSource/python-zocalo>`_ - Infrastructure components for automated data processing, developed by Diamond Light Source. The package is available through `PyPi <https://pypi.org/project/zocalo/>`__ and `conda-forge <https://anaconda.org/conda-forge/zocalo>`__.
-        * `DiamondLightSource/python-workflows <https://github.com/DiamondLightSource/python-workflows/>`_ - Zocalo is built on the workflows package. It shouldn't be necessary to interact too much with this package, as the details are abstracted by Zocalo. workflows controls the logic of how services connect to each other and what a service is, and actually send the messages to a message broker. Currently this is an ActiveMQ_ broker (via STOMP_) but support for a RabbitMQ_ broker (via pika_) is being added. This is also available on `PyPi <https://pypi.org/project/workflows/>`__ and `conda-forge <https://anaconda.org/conda-forge/workflows>`__.
-        
-        As mentioned, Zocalo is currently built on top of ActiveMQ. ActiveMQ is an apache project that provides a `message broker <https://en.wikipedia.org/wiki/Message_broker>`_ server, acting as a central dispatch that allows various services to communicate. Messages are plaintext, but from the Zocalo point of view it's passing aroung python objects (json dictionaries). Every message sent has a destination to help the message broker route. Messages may either be sent to a specific queue or broadcast to multiple queues. These queues are subscribed to by the services that run in Zocalo. In developing with Zocalo, you may have to interact with ActiveMQ or RabbitMQ, but it is unlikely that you will have to configure it.
-        
-        Zocalo allows for the monitoring of jobs executing ``python-workflows`` services or recipe wrappers. The ``python-workflows`` package contains most of the infrastructure required for the jobs themselves and more detailed documentation of its components can be found in the ``python-workflows`` `GitHub repository <https://github.com/DiamondLightSource/python-workflows/>`_ and `the Zocalo documentation <https://zocalo.readthedocs.io>`_. 
-        
-        .. _ActiveMQ: http://activemq.apache.org/
-        .. _STOMP: https://stomp.github.io/
-        .. _RabbitMQ: https://www.rabbitmq.com/
-        .. _pika: https://github.com/pika/pika
-        
-        
-        =======
-        History
-        =======
-        
-        0.9.0 (2021-08-18)
-        ------------------
-        * Removed --live/--test command line arguments, use -e/--environment instead
-        * zocalo.go, zocalo.service, zocalo.wrap accept -t/--transport command line
-          options, and the default can be set via the site configuration.
-        
-        0.8.1 (2021-07-08)
-        ------------------
-        * Keep wrapper status threads alive through transport disconnection events
-        
-        0.8.0 (2021-05-18)
-        ------------------
-        * Support for Zocalo configuration files
-        
-        0.7.4 (2021-03-17)
-        ------------------
-        * Documentation improvements
-        
-        0.7.3 (2021-01-19)
-        ------------------
-        * Ignore error when logserver hostname can't be looked up immediately
-        
-        0.7.2 (2021-01-18)
-        ------------------
-        * Add a symbolic link handling library function
-        * Cache the logserver hostname by default
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+License-File: LICENSE
+
+======
+Zocalo
+======
+
+
+.. image:: https://img.shields.io/pypi/v/zocalo.svg
+        :target: https://pypi.python.org/pypi/zocalo
+        :alt: PyPI release
+
+.. image:: https://img.shields.io/conda/vn/conda-forge/zocalo.svg
+        :target: https://anaconda.org/conda-forge/zocalo
+        :alt: Conda version
+
+.. image:: https://dev.azure.com/zocalo/python-zocalo/_apis/build/status/DiamondLightSource.python-zocalo?branchName=main
+        :target: https://dev.azure.com/zocalo/python-zocalo/_build/latest?definitionId=2&branchName=main
+        :alt: Build status
+
+.. image:: https://img.shields.io/lgtm/grade/python/g/DiamondLightSource/python-zocalo.svg?logo=lgtm&logoWidth=18
+        :target: https://lgtm.com/projects/g/DiamondLightSource/python-zocalo/context:python
+        :alt: Language grade: Python
+
+.. image:: https://img.shields.io/lgtm/alerts/g/DiamondLightSource/python-zocalo.svg?logo=lgtm&logoWidth=18
+        :target: https://lgtm.com/projects/g/DiamondLightSource/python-zocalo/alerts/
+        :alt: Total alerts
+
+.. image:: https://readthedocs.org/projects/zocalo/badge/?version=latest
+        :target: https://zocalo.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation status
+
+.. image:: https://img.shields.io/pypi/pyversions/zocalo.svg
+        :target: https://pypi.org/project/zocalo/
+        :alt: Supported Python versions
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+        :target: https://github.com/ambv/black
+        :alt: Code style: black
+
+.. image:: https://img.shields.io/pypi/l/zocalo.svg
+        :target: https://pypi.python.org/pypi/zocalo
+        :alt: BSD license
+
+..
+
+        |
+        | `M. Gerstel, A. Ashton, R.J. Gildea, K. Levik, and G. Winter, "Data Analysis Infrastructure for Diamond Light Source Macromolecular & Chemical Crystallography and Beyond", in Proc. ICALEPCS'19, New York, NY, USA, Oct. 2019, pp. 1031-1035. <https://doi.org/10.18429/JACoW-ICALEPCS2019-WEMPR001>`_ |DOI|
+
+        .. |DOI| image:: https://img.shields.io/badge/DOI-10.18429/JACoW--ICALEPCS2019--WEMPR001-blue.svg
+                :target: https://doi.org/10.18429/JACoW-ICALEPCS2019-WEMPR001
+                :alt: Primary Reference DOI
+
+|
+
+Zocalo is an automated data processing system designed at Diamond Light Source. This repository contains infrastructure components for Zocalo.
+
+The idea of Zocalo is a simple one - to build a messaging framework, where text-based messages are sent between parts of the system to coordinate data analysis. In the wider scope of things this also covers things like archiving, but generally it is handling everything that happens after data aquisition.
+
+Zocalo as a wider whole is made up of two repositories (plus some private internal repositories when deployed at Diamond):
+
+* `DiamondLightSource/python-zocalo <https://github.com/DiamondLightSource/python-zocalo>`_ - Infrastructure components for automated data processing, developed by Diamond Light Source. The package is available through `PyPi <https://pypi.org/project/zocalo/>`__ and `conda-forge <https://anaconda.org/conda-forge/zocalo>`__.
+* `DiamondLightSource/python-workflows <https://github.com/DiamondLightSource/python-workflows/>`_ - Zocalo is built on the workflows package. It shouldn't be necessary to interact too much with this package, as the details are abstracted by Zocalo. workflows controls the logic of how services connect to each other and what a service is, and actually send the messages to a message broker. Currently this is an ActiveMQ_ broker (via STOMP_) but support for a RabbitMQ_ broker (via pika_) is being added. This is also available on `PyPi <https://pypi.org/project/workflows/>`__ and `conda-forge <https://anaconda.org/conda-forge/workflows>`__.
+
+As mentioned, Zocalo is currently built on top of ActiveMQ. ActiveMQ is an apache project that provides a `message broker <https://en.wikipedia.org/wiki/Message_broker>`_ server, acting as a central dispatch that allows various services to communicate. Messages are plaintext, but from the Zocalo point of view it's passing aroung python objects (json dictionaries). Every message sent has a destination to help the message broker route. Messages may either be sent to a specific queue or broadcast to multiple queues. These queues are subscribed to by the services that run in Zocalo. In developing with Zocalo, you may have to interact with ActiveMQ or RabbitMQ, but it is unlikely that you will have to configure it.
+
+Zocalo allows for the monitoring of jobs executing ``python-workflows`` services or recipe wrappers. The ``python-workflows`` package contains most of the infrastructure required for the jobs themselves and more detailed documentation of its components can be found in the ``python-workflows`` `GitHub repository <https://github.com/DiamondLightSource/python-workflows/>`_ and `the Zocalo documentation <https://zocalo.readthedocs.io>`_. 
+
+.. _ActiveMQ: http://activemq.apache.org/
+.. _STOMP: https://stomp.github.io/
+.. _RabbitMQ: https://www.rabbitmq.com/
+.. _pika: https://github.com/pika/pika
+
+
+=======
+History
+=======
+
+0.9.0 (2021-08-18)
+------------------
+* Removed --live/--test command line arguments, use -e/--environment instead
+* zocalo.go, zocalo.service, zocalo.wrap accept -t/--transport command line
+  options, and the default can be set via the site configuration.
+
+0.8.1 (2021-07-08)
+------------------
+* Keep wrapper status threads alive through transport disconnection events
+
+0.8.0 (2021-05-18)
+------------------
+* Support for Zocalo configuration files
+
+0.7.4 (2021-03-17)
+------------------
+* Documentation improvements
+
+0.7.3 (2021-01-19)
+------------------
+* Ignore error when logserver hostname can't be looked up immediately
+
+0.7.2 (2021-01-18)
+------------------
+* Add a symbolic link handling library function
+* Cache the logserver hostname by default
+
+
```

### Comparing `zocalo-0.9.0/src/zocalo.egg-info/SOURCES.txt` & `zocalo-0.9.1/src/zocalo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/src/zocalo.egg-info/entry_points.txt` & `zocalo-0.9.1/src/zocalo.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/tests/configuration/test_configuration.py` & `zocalo-0.9.1/tests/configuration/test_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import pathlib
 from unittest import mock
 
 import pytest
 
 import zocalo.configuration
 
 sample_configuration = """
@@ -364,7 +365,23 @@
         zocalo.configuration.from_string(
             f"""
             version: 1
             include:
               - {secondary_file}
             """
         )
+
+
+def test_resolve_external_references_into_home_directory():
+    merged = zocalo.configuration._merge_configuration(
+        """
+        version: 1
+        foo: ~/bar.yml
+        """,
+        None,
+        pathlib.Path.cwd(),
+    )
+    assert merged == {
+        "version": 1,
+        "foo": pathlib.Path("~/bar.yml").expanduser(),
+        "environments": {},
+    }
```

### Comparing `zocalo-0.9.0/tests/configuration/test_plugin_graylog.py` & `zocalo-0.9.1/tests/configuration/test_plugin_graylog.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/tests/configuration/test_plugin_jmx.py` & `zocalo-0.9.1/tests/configuration/test_plugin_jmx.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/tests/configuration/test_plugin_storage.py` & `zocalo-0.9.1/tests/configuration/test_plugin_storage.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/tests/test_graylog.py` & `zocalo-0.9.1/tests/test_graylog.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/tests/test_zocalo.py` & `zocalo-0.9.1/tests/test_zocalo.py`

 * *Files identical despite different names*

### Comparing `zocalo-0.9.0/tests/util/test_symlink.py` & `zocalo-0.9.1/tests/util/test_symlink.py`

 * *Files identical despite different names*

