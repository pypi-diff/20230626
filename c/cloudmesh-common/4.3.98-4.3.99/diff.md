# Comparing `tmp/cloudmesh-common-4.3.98.tar.gz` & `tmp/cloudmesh-common-4.3.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmesh-common-4.3.98.tar", last modified: Fri Mar 11 03:47:23 2022, max compression
+gzip compressed data, was "cloudmesh-common-4.3.99.tar", last modified: Tue Mar 15 22:41:25 2022, max compression
```

## Comparing `cloudmesh-common-4.3.98.tar` & `cloudmesh-common-4.3.99.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-11 03:47:23.440991 cloudmesh-common-4.3.98/
--rw-rw-r--   0 green     (1000) green     (1000)      318 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/AUTHORS
--rw-rw-r--   0 green     (1000) green     (1000)     1265 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/CHANGELOG.md
--rw-rw-r--   0 green     (1000) green     (1000)      842 2022-02-22 00:45:59.000000 cloudmesh-common-4.3.98/LICENSE
--rw-rw-r--   0 green     (1000) green     (1000)      232 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/MANIFEST.in
--rw-rw-r--   0 green     (1000) green     (1000)     7213 2022-03-11 03:47:23.440991 cloudmesh-common-4.3.98/PKG-INFO
--rw-rw-r--   0 green     (1000) green     (1000)     5550 2022-03-07 22:55:07.000000 cloudmesh-common-4.3.98/README.md
--rw-rw-r--   0 green     (1000) green     (1000)        6 2022-03-11 03:47:06.000000 cloudmesh-common-4.3.98/VERSION
--rw-rw-r--   0 green     (1000) green     (1000)        0 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/__init__.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-11 03:47:23.440991 cloudmesh-common-4.3.98/cloudmesh/
--rw-rw-r--   0 green     (1000) green     (1000)      363 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/__init__.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-11 03:47:23.440991 cloudmesh-common-4.3.98/cloudmesh/common/
--rw-rw-r--   0 green     (1000) green     (1000)     3439 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/Benchmark.py
--rw-rw-r--   0 green     (1000) green     (1000)     3198 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/DateTime.py
--rw-rw-r--   0 green     (1000) green     (1000)     2482 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/DictList.py
--rw-rw-r--   0 green     (1000) green     (1000)     9585 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/FlatDict.py
--rw-rw-r--   0 green     (1000) green     (1000)    13187 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/Host.py
--rw-rw-r--   0 green     (1000) green     (1000)      959 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/Inspector.py
--rwxrwxr-x   0 green     (1000) green     (1000)     3994 2022-01-19 15:27:34.000000 cloudmesh-common-4.3.98/cloudmesh/common/JobMultiHostScript.py
--rw-rw-r--   0 green     (1000) green     (1000)     5358 2022-01-19 15:27:34.000000 cloudmesh-common-4.3.98/cloudmesh/common/JobScript.py
--rw-rw-r--   0 green     (1000) green     (1000)     8968 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/JobSet.py
--rw-rw-r--   0 green     (1000) green     (1000)    16677 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/Printer.py
--rwxrwxr-x   0 green     (1000) green     (1000)    41163 2022-03-11 03:46:32.000000 cloudmesh-common-4.3.98/cloudmesh/common/Shell.py
--rw-rw-r--   0 green     (1000) green     (1000)    18123 2022-03-10 23:17:09.000000 cloudmesh-common-4.3.98/cloudmesh/common/StopWatch.py
--rw-rw-r--   0 green     (1000) green     (1000)     5825 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/TableParser.py
--rw-rw-r--   0 green     (1000) green     (1000)    11616 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/Tabulate.py
--rw-rw-r--   0 green     (1000) green     (1000)      649 2022-03-11 03:47:06.000000 cloudmesh-common-4.3.98/cloudmesh/common/__init__.py
--rw-rw-r--   0 green     (1000) green     (1000)       19 2022-03-11 03:47:06.000000 cloudmesh-common-4.3.98/cloudmesh/common/__version__.py
--rw-rw-r--   0 green     (1000) green     (1000)     9019 2022-02-22 15:46:38.000000 cloudmesh-common-4.3.98/cloudmesh/common/console.py
--rw-rw-r--   0 green     (1000) green     (1000)     2768 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/debug.py
--rw-rw-r--   0 green     (1000) green     (1000)     3418 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/default.py
--rw-rw-r--   0 green     (1000) green     (1000)     2540 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/deprecated.py
--rw-rw-r--   0 green     (1000) green     (1000)      468 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/dotdict.py
--rw-rw-r--   0 green     (1000) green     (1000)     1946 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/error.py
--rw-rw-r--   0 green     (1000) green     (1000)     2170 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/location.py
--rw-rw-r--   0 green     (1000) green     (1000)     2213 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/logger.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-11 03:47:23.440991 cloudmesh-common-4.3.98/cloudmesh/common/notebook/
--rw-rw-r--   0 green     (1000) green     (1000)      340 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/notebook/__init__.py
--rw-rw-r--   0 green     (1000) green     (1000)     4646 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/parameter.py
--rw-rw-r--   0 green     (1000) green     (1000)    52798 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/prettytable.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-11 03:47:23.440991 cloudmesh-common-4.3.98/cloudmesh/common/run/
--rw-rw-r--   0 green     (1000) green     (1000)        0 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/run/__init__.py
--rw-rw-r--   0 green     (1000) green     (1000)      846 2022-02-14 16:23:38.000000 cloudmesh-common-4.3.98/cloudmesh/common/run/background.py
--rw-rw-r--   0 green     (1000) green     (1000)      327 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/run/file.py
--rw-rw-r--   0 green     (1000) green     (1000)      271 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/run/subprocess.py
--rw-rw-r--   0 green     (1000) green     (1000)      403 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/security.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-11 03:47:23.440991 cloudmesh-common-4.3.98/cloudmesh/common/ssh/
--rw-rw-r--   0 green     (1000) green     (1000)       21 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/ssh/__init__.py
--rw-rw-r--   0 green     (1000) green     (1000)     2535 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/ssh/authorized_keys.py
--rw-rw-r--   0 green     (1000) green     (1000)     1615 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/ssh/encrypt.py
--rw-rw-r--   0 green     (1000) green     (1000)     6397 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/ssh/ssh_config.py
--rw-rw-r--   0 green     (1000) green     (1000)     2073 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/strdb.py
--rw-rw-r--   0 green     (1000) green     (1000)     3111 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/sudo.py
--rw-rw-r--   0 green     (1000) green     (1000)     4031 2022-03-05 11:20:41.000000 cloudmesh-common-4.3.98/cloudmesh/common/systeminfo.py
--rw-rw-r--   0 green     (1000) green     (1000)      608 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/todo.py
--rw-rw-r--   0 green     (1000) green     (1000)    14816 2022-03-11 02:54:20.000000 cloudmesh-common-4.3.98/cloudmesh/common/util.py
--rw-rw-r--   0 green     (1000) green     (1000)     1984 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/variables.py
--rw-rw-r--   0 green     (1000) green     (1000)     2538 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/cloudmesh/common/wifi.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-11 03:47:23.440991 cloudmesh-common-4.3.98/cloudmesh_common.egg-info/
--rw-rw-r--   0 green     (1000) green     (1000)     7213 2022-03-11 03:47:23.000000 cloudmesh-common-4.3.98/cloudmesh_common.egg-info/PKG-INFO
--rw-rw-r--   0 green     (1000) green     (1000)     1721 2022-03-11 03:47:23.000000 cloudmesh-common-4.3.98/cloudmesh_common.egg-info/SOURCES.txt
--rw-rw-r--   0 green     (1000) green     (1000)        1 2022-03-11 03:47:23.000000 cloudmesh-common-4.3.98/cloudmesh_common.egg-info/dependency_links.txt
--rw-rw-r--   0 green     (1000) green     (1000)       10 2022-03-11 03:47:23.000000 cloudmesh-common-4.3.98/cloudmesh_common.egg-info/namespace_packages.txt
--rw-rw-r--   0 green     (1000) green     (1000)        1 2022-03-11 03:47:23.000000 cloudmesh-common-4.3.98/cloudmesh_common.egg-info/not-zip-safe
--rw-rw-r--   0 green     (1000) green     (1000)      111 2022-03-11 03:47:23.000000 cloudmesh-common-4.3.98/cloudmesh_common.egg-info/requires.txt
--rw-rw-r--   0 green     (1000) green     (1000)       10 2022-03-11 03:47:23.000000 cloudmesh-common-4.3.98/cloudmesh_common.egg-info/top_level.txt
--rw-rw-r--   0 green     (1000) green     (1000)       75 2022-01-31 00:34:22.000000 cloudmesh-common-4.3.98/requirements-dev.txt
--rw-rw-r--   0 green     (1000) green     (1000)      210 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/requirements.txt
--rw-rw-r--   0 green     (1000) green     (1000)       67 2022-03-11 03:47:23.440991 cloudmesh-common-4.3.98/setup.cfg
--rw-rw-r--   0 green     (1000) green     (1000)     3941 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.98/setup.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-15 22:41:25.861112 cloudmesh-common-4.3.99/
+-rw-rw-r--   0 green     (1000) green     (1000)      318 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/AUTHORS
+-rw-rw-r--   0 green     (1000) green     (1000)     1265 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/CHANGELOG.md
+-rw-rw-r--   0 green     (1000) green     (1000)      842 2022-02-22 00:45:59.000000 cloudmesh-common-4.3.99/LICENSE
+-rw-rw-r--   0 green     (1000) green     (1000)      232 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/MANIFEST.in
+-rw-rw-r--   0 green     (1000) green     (1000)     7213 2022-03-15 22:41:25.861112 cloudmesh-common-4.3.99/PKG-INFO
+-rw-rw-r--   0 green     (1000) green     (1000)     5550 2022-03-07 22:55:07.000000 cloudmesh-common-4.3.99/README.md
+-rw-rw-r--   0 green     (1000) green     (1000)        6 2022-03-15 22:41:13.000000 cloudmesh-common-4.3.99/VERSION
+-rw-rw-r--   0 green     (1000) green     (1000)        0 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/__init__.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-15 22:41:25.857112 cloudmesh-common-4.3.99/cloudmesh/
+-rw-rw-r--   0 green     (1000) green     (1000)      363 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/__init__.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-15 22:41:25.857112 cloudmesh-common-4.3.99/cloudmesh/common/
+-rw-rw-r--   0 green     (1000) green     (1000)     3439 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/Benchmark.py
+-rw-rw-r--   0 green     (1000) green     (1000)     3198 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/DateTime.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2482 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/DictList.py
+-rw-rw-r--   0 green     (1000) green     (1000)     9585 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/FlatDict.py
+-rw-rw-r--   0 green     (1000) green     (1000)    13187 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/Host.py
+-rw-rw-r--   0 green     (1000) green     (1000)      959 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/Inspector.py
+-rwxrwxr-x   0 green     (1000) green     (1000)     3994 2022-01-19 15:27:34.000000 cloudmesh-common-4.3.99/cloudmesh/common/JobMultiHostScript.py
+-rw-rw-r--   0 green     (1000) green     (1000)     5358 2022-01-19 15:27:34.000000 cloudmesh-common-4.3.99/cloudmesh/common/JobScript.py
+-rw-rw-r--   0 green     (1000) green     (1000)     8968 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/JobSet.py
+-rw-rw-r--   0 green     (1000) green     (1000)    16677 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/Printer.py
+-rwxrwxr-x   0 green     (1000) green     (1000)    41163 2022-03-11 03:46:32.000000 cloudmesh-common-4.3.99/cloudmesh/common/Shell.py
+-rw-rw-r--   0 green     (1000) green     (1000)    20465 2022-03-15 22:39:30.000000 cloudmesh-common-4.3.99/cloudmesh/common/StopWatch.py
+-rw-rw-r--   0 green     (1000) green     (1000)     5825 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/TableParser.py
+-rw-rw-r--   0 green     (1000) green     (1000)    11616 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/Tabulate.py
+-rw-rw-r--   0 green     (1000) green     (1000)      649 2022-03-15 22:41:13.000000 cloudmesh-common-4.3.99/cloudmesh/common/__init__.py
+-rw-rw-r--   0 green     (1000) green     (1000)       19 2022-03-15 22:41:13.000000 cloudmesh-common-4.3.99/cloudmesh/common/__version__.py
+-rw-rw-r--   0 green     (1000) green     (1000)     9019 2022-02-22 15:46:38.000000 cloudmesh-common-4.3.99/cloudmesh/common/console.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2768 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/debug.py
+-rw-rw-r--   0 green     (1000) green     (1000)     3418 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/default.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2540 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/deprecated.py
+-rw-rw-r--   0 green     (1000) green     (1000)      468 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/dotdict.py
+-rw-rw-r--   0 green     (1000) green     (1000)     1946 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/error.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2170 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/location.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2213 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/logger.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-15 22:41:25.857112 cloudmesh-common-4.3.99/cloudmesh/common/notebook/
+-rw-rw-r--   0 green     (1000) green     (1000)      340 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/notebook/__init__.py
+-rw-rw-r--   0 green     (1000) green     (1000)     4646 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/parameter.py
+-rw-rw-r--   0 green     (1000) green     (1000)    52798 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/prettytable.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-15 22:41:25.857112 cloudmesh-common-4.3.99/cloudmesh/common/run/
+-rw-rw-r--   0 green     (1000) green     (1000)        0 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/run/__init__.py
+-rw-rw-r--   0 green     (1000) green     (1000)      846 2022-02-14 16:23:38.000000 cloudmesh-common-4.3.99/cloudmesh/common/run/background.py
+-rw-rw-r--   0 green     (1000) green     (1000)      327 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/run/file.py
+-rw-rw-r--   0 green     (1000) green     (1000)      271 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/run/subprocess.py
+-rw-rw-r--   0 green     (1000) green     (1000)      403 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/security.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-15 22:41:25.857112 cloudmesh-common-4.3.99/cloudmesh/common/ssh/
+-rw-rw-r--   0 green     (1000) green     (1000)       21 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/ssh/__init__.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2535 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/ssh/authorized_keys.py
+-rw-rw-r--   0 green     (1000) green     (1000)     1615 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/ssh/encrypt.py
+-rw-rw-r--   0 green     (1000) green     (1000)     6397 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/ssh/ssh_config.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2073 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/strdb.py
+-rw-rw-r--   0 green     (1000) green     (1000)     3111 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/sudo.py
+-rw-rw-r--   0 green     (1000) green     (1000)     4031 2022-03-05 11:20:41.000000 cloudmesh-common-4.3.99/cloudmesh/common/systeminfo.py
+-rw-rw-r--   0 green     (1000) green     (1000)      608 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/todo.py
+-rw-rw-r--   0 green     (1000) green     (1000)    14816 2022-03-11 02:54:20.000000 cloudmesh-common-4.3.99/cloudmesh/common/util.py
+-rw-rw-r--   0 green     (1000) green     (1000)     1984 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/variables.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2538 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/cloudmesh/common/wifi.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-15 22:41:25.861112 cloudmesh-common-4.3.99/cloudmesh_common.egg-info/
+-rw-rw-r--   0 green     (1000) green     (1000)     7213 2022-03-15 22:41:25.000000 cloudmesh-common-4.3.99/cloudmesh_common.egg-info/PKG-INFO
+-rw-rw-r--   0 green     (1000) green     (1000)     1721 2022-03-15 22:41:25.000000 cloudmesh-common-4.3.99/cloudmesh_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 green     (1000) green     (1000)        1 2022-03-15 22:41:25.000000 cloudmesh-common-4.3.99/cloudmesh_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       10 2022-03-15 22:41:25.000000 cloudmesh-common-4.3.99/cloudmesh_common.egg-info/namespace_packages.txt
+-rw-rw-r--   0 green     (1000) green     (1000)        1 2022-03-15 22:41:25.000000 cloudmesh-common-4.3.99/cloudmesh_common.egg-info/not-zip-safe
+-rw-rw-r--   0 green     (1000) green     (1000)      111 2022-03-15 22:41:25.000000 cloudmesh-common-4.3.99/cloudmesh_common.egg-info/requires.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       10 2022-03-15 22:41:25.000000 cloudmesh-common-4.3.99/cloudmesh_common.egg-info/top_level.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       75 2022-01-31 00:34:22.000000 cloudmesh-common-4.3.99/requirements-dev.txt
+-rw-rw-r--   0 green     (1000) green     (1000)      210 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/requirements.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       67 2022-03-15 22:41:25.861112 cloudmesh-common-4.3.99/setup.cfg
+-rw-rw-r--   0 green     (1000) green     (1000)     3941 2022-01-18 14:59:44.000000 cloudmesh-common-4.3.99/setup.py
```

### Comparing `cloudmesh-common-4.3.98/CHANGELOG.md` & `cloudmesh-common-4.3.99/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/LICENSE` & `cloudmesh-common-4.3.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/PKG-INFO` & `cloudmesh-common-4.3.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-common
-Version: 4.3.98
+Version: 4.3.99
 Summary: A set of useful APIs for cloudmesh
 Home-page: https://github.com/cloudmesh/cloudmesh-common
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cloudmesh-common-4.3.98/README.md` & `cloudmesh-common-4.3.99/README.md`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/Benchmark.py` & `cloudmesh-common-4.3.99/cloudmesh/common/Benchmark.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/DateTime.py` & `cloudmesh-common-4.3.99/cloudmesh/common/DateTime.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/DictList.py` & `cloudmesh-common-4.3.99/cloudmesh/common/DictList.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/FlatDict.py` & `cloudmesh-common-4.3.99/cloudmesh/common/FlatDict.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/Host.py` & `cloudmesh-common-4.3.99/cloudmesh/common/Host.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/Inspector.py` & `cloudmesh-common-4.3.99/cloudmesh/common/Inspector.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/JobMultiHostScript.py` & `cloudmesh-common-4.3.99/cloudmesh/common/JobMultiHostScript.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/JobScript.py` & `cloudmesh-common-4.3.99/cloudmesh/common/JobScript.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/JobSet.py` & `cloudmesh-common-4.3.99/cloudmesh/common/JobSet.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/Printer.py` & `cloudmesh-common-4.3.99/cloudmesh/common/Printer.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/Shell.py` & `cloudmesh-common-4.3.99/cloudmesh/common/Shell.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/StopWatch.py` & `cloudmesh-common-4.3.99/cloudmesh/common/StopWatch.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,21 +17,63 @@
     time.sleep(0.1)
     StopWatch.stop(t)
 
 pprint(StopWatch.get_benchmark(user=user, node=node))
 
 StopWatch.benchmark(user=user, node=node)
 
+## Context Block
+
+StoWatch alos comes with a context block allowing to use the convenient with statement. However thi sis only recommended
+when the block is small as it is easy to lose the indentation in larger code. You can also certainly split the code up in
+functions so it is easier managable.
+
+Here is a simple example on how to use the with statement, showing that is can be used for streams and files.
+The mode tetermins if the file will be recreated, or if it will be appanded on. In addition there is the ability to
+write metadata into the record with a dict that can optionally be passed along.
+
+    from cloudmesh.common.StopWatch import StopWatchBlock
+    from cloudmesh.common.StopWatch import StopWatch
+    from cloudmesh.common.util import readfile
+    import time
+
+    data = {"variable": "value"}
+
+    with StopWatchBlock("total"):
+        time.sleep(1.0)
+
+    with StopWatchBlock("dict", data=data):
+        time.sleep(1.0)
+        data["step"] = 1
+
+    with StopWatchBlock("file", data=data, log="a.log", mode="w"):
+        time.sleep(1.0)
+        data["step"] = 2
+
+    with StopWatchBlock("append", data=data, log="a.log", mode="a"):
+        time.sleep(1.0)
+        data["step"] = 3
+
+    content = readfile ("a.log")
+    print (79*"=")
+    print (content.strip())
+    print (79*"=")
+
+    StopWatch.benchmark(sysinfo=False, user="gregor", node="computer", attributes="short")
+
 """
 import os
 import time
+import datetime
 from pprint import pprint
+import sys
 
 from cloudmesh.common.Tabulate import Printer
 from cloudmesh.common.systeminfo import systeminfo as cm_systeminfo
+from time import perf_counter
 
 
 def rename(newname):
     """
     decorator to rename a function
     :param newname: function name
     :type newname: str
@@ -59,15 +101,14 @@
     def wrapper(*args, **kwargs):
         StopWatch.start(func.__name__)
         func(*args, **kwargs)
         StopWatch.stop(func.__name__)
 
     return wrapper
 
-
 class StopWatch(object):
     """
     A class to measure times between events.
     """
     debug = False
     verbose = True
     # Timer start dict
@@ -606,7 +647,38 @@
             entry = [entry[i] for i in index_attributes]
             label_tags = entry[0].split(label_split_char)
             entry = entry + label_tags
             data.append(entry)
 
         return {"headers": headers,
                 "data": data}
+
+
+
+class StopWatchBlock:
+
+    def __init__(self, name, data=None, log=sys.stdout, mode="w"):
+        self.name = name
+        self.data = data
+        self.log = log
+        self.is_file = False
+        self.start = datetime.datetime.now()
+        if type(log) == str:
+            self.is_file = True
+            self.log = open(log, mode)
+
+
+    def __enter__(self):
+        StopWatch.start(self.name)
+        return StopWatch.get(self.name)
+
+    def __exit__(self, type, value, traceback):
+        self.stop = datetime.datetime.now()
+        StopWatch.stop(self.name)
+        entry = StopWatch.get(self.name)
+        if self.data:
+            print (f"# {self.name}, {entry}, {self.start}, {self.stop}, {self.data}", file=self.log)
+        else:
+            print (f"# {self.name}, {entry}, {self.start}, {self.stop}", file=self.log)
+        if self.is_file:
+            self.log.close()
+
```

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/TableParser.py` & `cloudmesh-common-4.3.99/cloudmesh/common/TableParser.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/Tabulate.py` & `cloudmesh-common-4.3.99/cloudmesh/common/Tabulate.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/__init__.py` & `cloudmesh-common-4.3.99/cloudmesh/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from cloudmesh.common.console import Console
 from cloudmesh.common.Shell import Shell
 from cloudmesh.common.debug import VERBOSE
 from cloudmesh.common.dotdict import dotdict
 from cloudmesh.common.FlatDict import FlatDict
 from cloudmesh.common.variables import Variables
 
-version = '4.3.98'
+version = '4.3.99'
```

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/console.py` & `cloudmesh-common-4.3.99/cloudmesh/common/console.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/debug.py` & `cloudmesh-common-4.3.99/cloudmesh/common/debug.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/default.py` & `cloudmesh-common-4.3.99/cloudmesh/common/default.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/deprecated.py` & `cloudmesh-common-4.3.99/cloudmesh/common/deprecated.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/error.py` & `cloudmesh-common-4.3.99/cloudmesh/common/error.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/location.py` & `cloudmesh-common-4.3.99/cloudmesh/common/location.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/logger.py` & `cloudmesh-common-4.3.99/cloudmesh/common/logger.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/parameter.py` & `cloudmesh-common-4.3.99/cloudmesh/common/parameter.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/prettytable.py` & `cloudmesh-common-4.3.99/cloudmesh/common/prettytable.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/run/background.py` & `cloudmesh-common-4.3.99/cloudmesh/common/run/background.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/ssh/authorized_keys.py` & `cloudmesh-common-4.3.99/cloudmesh/common/ssh/authorized_keys.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/ssh/encrypt.py` & `cloudmesh-common-4.3.99/cloudmesh/common/ssh/encrypt.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/ssh/ssh_config.py` & `cloudmesh-common-4.3.99/cloudmesh/common/ssh/ssh_config.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/strdb.py` & `cloudmesh-common-4.3.99/cloudmesh/common/strdb.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/sudo.py` & `cloudmesh-common-4.3.99/cloudmesh/common/sudo.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/systeminfo.py` & `cloudmesh-common-4.3.99/cloudmesh/common/systeminfo.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/todo.py` & `cloudmesh-common-4.3.99/cloudmesh/common/todo.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/util.py` & `cloudmesh-common-4.3.99/cloudmesh/common/util.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/variables.py` & `cloudmesh-common-4.3.99/cloudmesh/common/variables.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh/common/wifi.py` & `cloudmesh-common-4.3.99/cloudmesh/common/wifi.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/cloudmesh_common.egg-info/PKG-INFO` & `cloudmesh-common-4.3.99/cloudmesh_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-common
-Version: 4.3.98
+Version: 4.3.99
 Summary: A set of useful APIs for cloudmesh
 Home-page: https://github.com/cloudmesh/cloudmesh-common
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cloudmesh-common-4.3.98/cloudmesh_common.egg-info/SOURCES.txt` & `cloudmesh-common-4.3.99/cloudmesh_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-common-4.3.98/setup.py` & `cloudmesh-common-4.3.99/setup.py`

 * *Files identical despite different names*

