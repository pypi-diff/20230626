# Comparing `tmp/msgram-1.1.2.tar.gz` & `tmp/msgram-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-1.1.2.tar", last modified: Wed Jun 14 13:20:24 2023, max compression
+gzip compressed data, was "msgram-1.2.1.tar", last modified: Mon Jun 26 20:35:49 2023, max compression
```

## Comparing `msgram-1.1.2.tar` & `msgram-1.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.919718 msgram-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-06-14 13:20:04.000000 msgram-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-06-14 13:20:24.919718 msgram-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-14 13:20:04.000000 msgram-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.915718 msgram-1.1.2/msgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-06-14 13:20:24.000000 msgram-1.1.2/msgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-14 13:20:24.000000 msgram-1.1.2/msgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:20:24.000000 msgram-1.1.2/msgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-14 13:20:24.000000 msgram-1.1.2/msgram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-14 13:20:24.000000 msgram-1.1.2/msgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-14 13:20:24.000000 msgram-1.1.2/msgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-14 13:20:04.000000 msgram-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:20:24.919718 msgram-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.915718 msgram-1.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:04.000000 msgram-1.1.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.915718 msgram-1.1.2/src/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.915718 msgram-1.1.2/src/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/commands/cmd_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/commands/cmd_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/commands/cmd_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.919718 msgram-1.1.2/src/cli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.919718 msgram-1.1.2/src/cli/jsonReader/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/jsonReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/jsonReader/jsonReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.919718 msgram-1.1.2/src/cli/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/resources/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/resources/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/resources/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/resources/sqc.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/resources/subcharacteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-14 13:20:04.000000 msgram-1.1.2/src/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.919718 msgram-1.1.2/src/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:04.000000 msgram-1.1.2/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-14 13:20:04.000000 msgram-1.1.2/src/config/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-14 13:20:04.000000 msgram-1.1.2/src/config/setup_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.919718 msgram-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.919718 msgram-1.1.2/tests/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/system/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/system/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/system/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.919718 msgram-1.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:20:24.919718 msgram-1.1.2/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/data/file_reader_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/test_characteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/test_jsonReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/test_sqc.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-14 13:20:04.000000 msgram-1.1.2/tests/unit/test_subcharacteristic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.434786 msgram-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-06-26 20:35:17.000000 msgram-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-06-26 20:35:49.434786 msgram-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-26 20:35:17.000000 msgram-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/msgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-26 20:35:17.000000 msgram-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:35:49.434786 msgram-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/commands/cmd_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/commands/cmd_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/commands/cmd_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/cli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/cli/jsonReader/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/jsonReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/jsonReader/jsonReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.430786 msgram-1.2.1/src/cli/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/subcharacteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/tsqmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.430786 msgram-1.2.1/src/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-26 20:35:17.000000 msgram-1.2.1/src/config/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-26 20:35:17.000000 msgram-1.2.1/src/config/setup_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.430786 msgram-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.430786 msgram-1.2.1/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/system/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/system/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/system/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.434786 msgram-1.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.434786 msgram-1.2.1/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/data/file_reader_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_jsonReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_subcharacteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_tsqmi.py
```

### Comparing `msgram-1.1.2/LICENSE` & `msgram-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-1.1.2/PKG-INFO` & `msgram-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram
-Version: 1.1.2
+Version: 1.2.1
 Summary: The msgram CLI is a command-line interface to use MeasureSoftGram software
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-1.1.2/README.md` & `msgram-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `msgram-1.1.2/msgram.egg-info/PKG-INFO` & `msgram-1.2.1/msgram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram
-Version: 1.1.2
+Version: 1.2.1
 Summary: The msgram CLI is a command-line interface to use MeasureSoftGram software
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-1.1.2/msgram.egg-info/SOURCES.txt` & `msgram-1.2.1/msgram.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 src/cli/exceptions/exceptions.py
 src/cli/jsonReader/__init__.py
 src/cli/jsonReader/jsonReader.py
 src/cli/resources/__init__.py
 src/cli/resources/characteristic.py
 src/cli/resources/measure.py
 src/cli/resources/metrics.py
-src/cli/resources/sqc.py
 src/cli/resources/subcharacteristic.py
+src/cli/resources/tsqmi.py
 src/config/__init__.py
 src/config/settings.py
 src/config/setup_log.py
 tests/__init__.py
 tests/system/__init__.py
 tests/system/test_extract.py
 tests/system/test_help.py
@@ -37,10 +37,10 @@
 tests/unit/__init__.py
 tests/unit/test_calculate.py
 tests/unit/test_characteristic.py
 tests/unit/test_extract.py
 tests/unit/test_init.py
 tests/unit/test_jsonReader.py
 tests/unit/test_measures.py
-tests/unit/test_sqc.py
 tests/unit/test_subcharacteristic.py
+tests/unit/test_tsqmi.py
 tests/unit/data/file_reader_response.py
```

### Comparing `msgram-1.1.2/pyproject.toml` & `msgram-1.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram"
-version = "1.1.2"
+version = "1.2.1"
 description = "The msgram CLI is a command-line interface to use MeasureSoftGram software"
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
@@ -23,20 +23,21 @@
 requires-python = ">=3.8"
 dependencies = [
         "requests==2.28.1",
         "pytz",
         "typing~=3.7.4.3",
         "tabulate==0.8.10",
         "termcolor==1.1.0",
-        "pandas~=1.4.4",
+        "pandas~=2.0.0",
         "setuptools~=60.2.0",
         "python-dotenv",
         "rich",
         "validators==0.20.0",
-        "msgram-core==1.2.1",
+        "msgram-core==1.3.1",
+        "msgram-parser==0.0.7"
     ]
 
 [project.scripts]
 msgram = "src.cli.cli:main"
 
 [tool.mypy]
 strict = true
```

### Comparing `msgram-1.1.2/src/cli/cli.py` & `msgram-1.2.1/src/cli/cli.py`

 * *Files identical despite different names*

### Comparing `msgram-1.1.2/src/cli/commands/cmd_calculate.py` & `msgram-1.2.1/src/cli/commands/cmd_calculate.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from rich.prompt import Prompt
 from rich.tree import Tree
 from staticfiles import DEFAULT_PRE_CONFIG as pre_config
 
 from src.cli.jsonReader import open_json_file, read_mult_files
 from src.cli.resources.characteristic import calculate_characteristics
 from src.cli.resources.measure import calculate_measures
-from src.cli.resources.sqc import calculate_sqc
+from src.cli.resources.tsqmi import calculate_tsqmi
 from src.cli.resources.subcharacteristic import calculate_subcharacteristics
 from src.cli.utils import print_error, print_info, print_panel, print_rule, print_table
 from src.cli.exceptions import exceptions
 from src.config.settings import DEFAULT_CONFIG_PATH, FILE_CONFIG
 
 logger = logging.getLogger("msgram")
 
@@ -53,17 +53,21 @@
     if not isfile:
         for file, file_name in read_mult_files(extracted_path, "msgram"):
             result = calculate_all(file, file_name, config)
             data_calculated.append(result)
             success = True
     else:
         try:
-            data_calculated = calculate_all(open_json_file(extracted_path), extracted_path.name, config)
+            data_calculated = calculate_all(
+                open_json_file(extracted_path), extracted_path.name, config
+            )
             success = True
-            output_format = Prompt.ask("\n\n[black]Display as:", choices=["tabular", "tree", "raw"])
+            output_format = Prompt.ask(
+                "\n\n[black]Display as:", choices=["tabular", "tree", "raw"]
+            )
         except exceptions.MeasureSoftGramCLIException as e:
             print(f"[red]Error calculating {extracted_path}: {e}\n")
 
     if success:
         print_info("\n[#A9A9A9]All calculations performed[/] successfully!")
 
     show_results(output_format, data_calculated, config_path)
@@ -83,88 +87,92 @@
         config, data_measures["measures"]
     )
 
     data_characteristics, _ = calculate_characteristics(
         config, data_subcharacteristics["subcharacteristics"]
     )
 
-    data_sqc, _ = calculate_sqc(config, data_characteristics["characteristics"])
+    data_tsqmi, _ = calculate_tsqmi(config, data_characteristics["characteristics"])
 
     version = re.search(r"\d{1,2}-\d{1,2}-\d{4}-\d{1,2}-\d{1,2}", file_name)[0]
     repository = file_name.split(version)[0][:-1]
 
     return {
         "repository": [{"key": "repository", "value": repository}],
         "version": [{"key": "version", "value": version}],
         "measures": data_measures["measures"],
         "subcharacteristics": data_subcharacteristics["subcharacteristics"],
         "characteristics": data_characteristics["characteristics"],
-        "sqc": data_sqc["sqc"],
+        "tsqmi": data_tsqmi["tsqmi"],
     }
 
 
 def show_results(output_format, data_calculated, config_path):
     if output_format == "tabular":
         show_tabulate(data_calculated)
 
     elif output_format == "raw":
         print(data_calculated)
 
     elif output_format == "tree":
         show_tree(data_calculated)
 
     elif len(data_calculated) == 0:
-        print_info(f"[yellow]WARNING: No extracted file readed so no {output_format} was generated!")
+        print_info(
+            f"[yellow]WARNING: No extracted file readed so no {output_format} was generated!"
+        )
 
     elif output_format == "csv":
         print_info("Exporting CSV...")
         export_csv(data_calculated, config_path)
 
     elif output_format == "json":
         print_info("Exporting JSON...")
         export_json(data_calculated, config_path)
 
 
 def show_tabulate(data_calculated):
-    sqc = data_calculated["sqc"][0]
+    tsqmi = data_calculated["tsqmi"][0]
     characteristics = {c["key"]: c["value"] for c in data_calculated["characteristics"]}
-    subcharacteristics = {sc["key"]: sc["value"] for sc in data_calculated["subcharacteristics"]}
+    subcharacteristics = {
+        sc["key"]: sc["value"] for sc in data_calculated["subcharacteristics"]
+    }
     measures = {m["key"]: m["value"] for m in data_calculated["measures"]}
 
     print_table(measures, "measures", "measures")
     print_table(subcharacteristics, "subcharacteristics", "subcharacteristics")
     print_table(characteristics, "characteristics", "characteristics")
-    print_table(sqc, "sqc", "sqc")
+    print_table(tsqmi, "tsqmi", "tsqmi")
 
 
 def get_obj_by_element(object_list: list, element_key: str, element_to_find):
     return next((obj for obj in object_list if obj[element_key] == element_to_find), {})
 
 
 def show_tree(data_calculated):
-    sqc = data_calculated["sqc"][0]
+    tsqmi = data_calculated["tsqmi"][0]
     characteristics = data_calculated["characteristics"]
     subcharacteristics = data_calculated["subcharacteristics"]
     measures = data_calculated["measures"]
 
     print("Overview - tree:\n\n")
-    sqc_tree = Tree(f"[green]{sqc['key']}: {sqc['value']}")
+    tsqmi_tree = Tree(f"[green]{tsqmi['key']}: {tsqmi['value']}")
 
     for char_c, char in zip(pre_config["characteristics"], characteristics):
-        char_tree = sqc_tree.add(f"[red]{char['key']}: {char['value']}")
+        char_tree = tsqmi_tree.add(f"[red]{char['key']}: {char['value']}")
 
         for subchar_c in char_c["subcharacteristics"]:
             subchar = get_obj_by_element(subcharacteristics, "key", subchar_c["key"])
             sub_char_tree = char_tree.add(f"[blue]{subchar['key']} {subchar['value']}")
 
             for measure_c in subchar_c["measures"]:
                 measure = get_obj_by_element(measures, "key", measure_c["key"])
                 sub_char_tree.add(f"[yellow]{measure['key']} {measure['value']}")
 
-    print(sqc_tree)
+    print(tsqmi_tree)
 
 
 def export_json(data_calculated: list, file_path: Path = DEFAULT_CONFIG_PATH):
     file_path = file_path.joinpath("calc_msgram.json")
     with open(file_path, "w", encoding="utf-8") as write_file:
         json.dump(
             data_calculated,
```

### Comparing `msgram-1.1.2/src/cli/commands/cmd_extract.py` & `msgram-1.2.1/src/cli/commands/cmd_extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import json
 import logging
 import os
 import re
 import sys
 from time import perf_counter
 
-from parsers.sonarqube import Sonarqube
 from rich import print
 from rich.console import Console
+from genericparser import GenericParser
 
 from src.cli.jsonReader import folder_reader
-from src.cli.utils import make_progress_bar, print_info, print_panel, print_rule, print_warn
+from src.cli.utils import (
+    make_progress_bar,
+    print_info,
+    print_panel,
+    print_rule,
+    print_warn,
+)
 
 logger = logging.getLogger("msgram")
 
 
 def get_infos_from_name(filename: str) -> str:
     """
     filename: str = fga-eps-mds-2022-1-MeasureSoftGram-Service-09-11-2022-16-11-42-develop.json
@@ -49,39 +55,44 @@
         exit(1)
 
     console = Console()
     console.clear()
     print_rule("Extract metrics")
 
     if not os.path.isdir(extracted_path):
-        logger.error(f'FileNotFoundError: extract directory "{extracted_path}" does not exists')
-        print_warn(f"FileNotFoundError: extract directory[blue]'{extracted_path}'[/]does not exists")
+        logger.error(
+            f'FileNotFoundError: extract directory "{extracted_path}" does not exists'
+        )
+        print_warn(
+            f"FileNotFoundError: extract directory[blue]'{extracted_path}'[/]does not exists"
+        )
         sys.exit(1)
 
     logger.debug(f"output_origin: {output_origin}")
     logger.debug(f"data_path: {data_path}")
     logger.debug(f"language_extension: {language_extension}")
 
     files = list(data_path.glob("*.json"))
     valid_files = len(files)
-    parser = Sonarqube() if output_origin == "sonarqube" else None
+    parser = GenericParser()
 
     print_info(f"\n> Extract and save metrics [[blue ]{output_origin}[/]]:")
     with make_progress_bar() as progress_bar:
-
-        task_request = progress_bar.add_task("[#A9A9A9]Extracting files: ", total=len(files))
+        task_request = progress_bar.add_task(
+            "[#A9A9A9]Extracting files: ", total=len(files)
+        )
         progress_bar.advance(task_request)
 
         for component, filename, files_error in folder_reader(data_path, "json"):
             if files_error:
                 progress_bar.update(task_request, advance=files_error)
                 valid_files = valid_files - files_error
 
             name = get_infos_from_name(filename)
-            result = parser.extract_supported_metrics(component)
+            result = parser.parse(input_value=component, type_input=output_origin)
 
             print(f"[dark_green]Reading:[/] [black]{filename}[/]")
             print(f"[dark_green]Save   :[/] [black]{name}[/]\n")
 
             with open(f"{extracted_path}/{name}", "w") as f:
                 f.write(json.dumps(result, indent=4))
```

### Comparing `msgram-1.1.2/src/cli/commands/cmd_init.py` & `msgram-1.2.1/src/cli/commands/cmd_init.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,24 +33,28 @@
         print_info(f"Created dir: {config_path}")
         config_path.mkdir()
 
     replace = True
 
     if file_path.exists():
         print_info(f"MSGram config file [bold red]'{FILE_CONFIG}'[/] exists already!")
-        replace = Confirm.ask(f"> Do you want to replace [bold blue]'{FILE_CONFIG}'[/]?")
+        replace = Confirm.ask(
+            f"> Do you want to replace [bold blue]'{FILE_CONFIG}'[/]?"
+        )
 
     if replace:
         try:
             with file_path.open("w") as f:
                 f.write(json.dumps(DEFAULT_PRE_CONFIG, indent=4))
         except OSError:
             console.line(2)
             print_error("Error opening or writing to file")
-        print_info(f"The file config: '{config_path.name}/msgram.json' was created successfully.")
+        print_info(
+            f"The file config: '{config_path.name}/msgram.json' was created successfully."
+        )
 
     else:
         print_info(f"The file config: '{config_path.name}/msgram.json' not changed...")
 
     print_panel(
         "> [#008080]Run msgram extract -o sonarqube -dp data_path -ep extract_path[/], to extract supported metrics!"
     )
```

### Comparing `msgram-1.1.2/src/cli/exceptions/exceptions.py` & `msgram-1.2.1/src/cli/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `msgram-1.1.2/src/cli/jsonReader/jsonReader.py` & `msgram-1.2.1/src/cli/jsonReader/jsonReader.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,25 @@
 
 
 def read_mult_files(directory: Path, pattern: str):
     for path_file in directory.glob(f"*.{pattern}"):
         try:
             yield open_json_file(path_file), path_file.name
         except exceptions.MeasureSoftGramCLIException:
-            print(f"[red]Error calculating {path_file.name}: Failed to decode the JSON file.\n")
+            print(
+                f"[red]Error calculating {path_file.name}: Failed to decode the JSON file.\n"
+            )
 
 
 def folder_reader(dir_path, pattern):
     num_files_error = 0
     if not list(dir_path.glob(f"*.{pattern}")):
-        raise exceptions.MeasureSoftGramCLIException(f"No files .{pattern} found inside folder.")
+        raise exceptions.MeasureSoftGramCLIException(
+            f"No files .{pattern} found inside folder."
+        )
 
     for path_file in dir_path.glob(f"*.{pattern}"):
         try:
             yield file_reader(path_file), path_file.name, num_files_error
             num_files_error = 0
         except exceptions.MeasureSoftGramCLIException as e:
             print(f"[green]Reading:[/] [black]{path_file.name}[/]")
@@ -67,15 +71,17 @@
             return json.load(file)
 
     except FileNotFoundError:
         raise exceptions.FileNotFound("The file was not found")
     except IsADirectoryError:
         raise exceptions.UnableToOpenFile(f"File {path_file.name} is a directory")
     except json.JSONDecodeError as error:
-        raise exceptions.InvalidMetricsJsonFile(f"Failed to decode the JSON file. {error}")
+        raise exceptions.InvalidMetricsJsonFile(
+            f"Failed to decode the JSON file. {error}"
+        )
 
 
 def get_missing_keys_str(attrs, required_attrs):
     missing_keys = [req_key for req_key in required_attrs if req_key not in attrs]
     return ", ".join(missing_keys)
 
 
@@ -86,32 +92,38 @@
     if len(missing_keys) > 0:
         raise exceptions.InvalidMetricsJsonFile(
             f"Invalid Sonar JSON keys. Missing keys are: {missing_keys}"
         )
 
     base_component = json_data["baseComponent"]
     base_component_attrs = list(base_component.keys())
-    missing_keys = get_missing_keys_str(base_component_attrs, REQUIRED_SONAR_BASE_COMPONENT_KEYS)
+    missing_keys = get_missing_keys_str(
+        base_component_attrs, REQUIRED_SONAR_BASE_COMPONENT_KEYS
+    )
 
     if len(missing_keys) > 0:
         raise exceptions.InvalidMetricsJsonFile(
             f"Invalid Sonar baseComponent keys. Missing keys are: {missing_keys}"
         )
 
     base_component_measures = base_component["measures"]
     base_component_measures_attrs = [bc["metric"] for bc in base_component_measures]
-    missing_keys = get_missing_keys_str(base_component_measures_attrs, REQUIRED_TRK_MEASURES)
+    missing_keys = get_missing_keys_str(
+        base_component_measures_attrs, REQUIRED_TRK_MEASURES
+    )
 
     if len(missing_keys) > 0:
         raise exceptions.InvalidMetricsJsonFile(
             f"Invalid Sonar baseComponent TRK measures. Missing keys are: {missing_keys}"
         )
 
     if len(json_data["components"]) == 0:
-        raise exceptions.InvalidMetricsJsonFile("File with valid schema but no metrics data.")
+        raise exceptions.InvalidMetricsJsonFile(
+            "File with valid schema but no metrics data."
+        )
 
 
 def check_file_extension(file_name):
     if file_name.split(".")[-1] != "json":
         raise exceptions.InvalidMetricsJsonFile("Only JSON files are accepted.")
```

### Comparing `msgram-1.1.2/src/cli/parsers.py` & `msgram-1.2.1/src/cli/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import argparse
 
 from pathlib import Path
 
 from src.cli.commands import command_init, command_extract, command_calculate
 from src.config.settings import (
-    AVAILABLE_IMPORTS, SUPPORTED_FORMATS,
-    DEFAULT_CONFIG_PATH, AVAILABLE_GEN_FORMATS
+    AVAILABLE_IMPORTS,
+    SUPPORTED_FORMATS,
+    DEFAULT_CONFIG_PATH,
+    AVAILABLE_GEN_FORMATS,
 )
 
 
 def create_parser():
     parser = argparse.ArgumentParser(
         prog="msgram",
         description="Command line interface for measuresoftgram",
@@ -75,23 +77,24 @@
         help="The source code language extension",
         default="py",
     )
     parser_extract.set_defaults(func=command_extract)  # function command extract
 
     # =====================================< COMMAND calculate >=====================================
     parser_calculate = subparsers.add_parser(
-        "calculate", help="Calculates all entities",
+        "calculate",
+        help="Calculates all entities",
     )
 
     parser_calculate.add_argument(
         "all",
         type=str,
         nargs="?",
         help=(
-            "Returns the calculated value of the entities: measures, subcharacteristics, characteristics, sqc"
+            "Returns the calculated value of the entities: measures, subcharacteristics, characteristics, tsqmi"
         ),
     )
 
     parser_calculate.add_argument(
         "-ep",
         "--extracted_path",
         type=lambda p: Path(p).absolute(),
```

### Comparing `msgram-1.1.2/src/cli/resources/characteristic.py` & `msgram-1.2.1/src/cli/resources/subcharacteristic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-from src.cli.resources.subcharacteristic import get_subcharacteristic_value
+from src.cli.resources.measure import get_measure_value
 
-from resources import calculate_characteristics as core_calculate
+from resources import calculate_subcharacteristics as core_calculate
 
 
-def get_characteristic_value(chars, sqc):
-    char_calculated = []
-    for char in sqc:
-        char_key = char["key"]
+def get_subcharacteristic_value(subchars, char):
+    subchar_calculated = []
+    for subchar in char:
+        subchar_key = subchar["key"]
 
-        char_calculated.append({
-            "key": char_key,
-            "value": {m['key']: m['value'] for m in chars}[char_key],
-            "weight": char['weight'],
-        })
+        subchar_calculated.append(
+            {
+                "key": subchar_key,
+                "value": {m["key"]: m["value"] for m in subchars}[subchar_key],
+                "weight": subchar["weight"],
+            }
+        )
 
-    return char_calculated
+    return subchar_calculated
 
 
-def calculate_characteristics(config, subchars):
-    characteristics = config['characteristics']
+def calculate_subcharacteristics(config, measures):
+    subchars = [sc["subcharacteristics"] for sc in config["characteristics"]]
     calculate_infos = []
 
-    for char in characteristics:
-        calculate_infos.append({
-            'key': char['key'],
-            'subcharacteristics': get_subcharacteristic_value(subchars, char['subcharacteristics'])
-        })
+    for subchar in subchars:
+        calculate_infos.append(
+            {
+                "key": subchar[0]["key"],
+                "measures": get_measure_value(measures, subchar[0]["measures"]),
+            }
+        )
 
     headers = ["Id", "Name", "Description", "Value", "Created at"]
-    return core_calculate({'characteristics': calculate_infos}), headers
+    return core_calculate({"subcharacteristics": calculate_infos}), headers
```

### Comparing `msgram-1.1.2/src/cli/resources/measure.py` & `msgram-1.2.1/src/cli/resources/measure.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from resources import calculate_measures as core_calculate
-from staticfiles import SONARQUBE_SUPPORTED_MEASURES
+from src.config.settings import SUPPORTED_MEASURES
 
 from src.cli.resources.metrics import get_metric_value
 
 logger = logging.getLogger("msgram")
 
 
 def get_measure_value(measures, subchar):
@@ -19,25 +19,29 @@
                 "weight": measure["weight"],
             }
         )
 
     return measures_calculated
 
 
-def calculate_measures(json_data, config: dict = {
+def calculate_measures(
+    json_data,
+    config: dict = {
         "characteristics": [{"subcharacteristics": [{"measures": [{"key": ""}]}]}]
-}):
+    },
+):
     extracted = get_metric_value(json_data)
 
     calculate_infos = []
-    for measures in SONARQUBE_SUPPORTED_MEASURES:
+    for measures in SUPPORTED_MEASURES:
         calculate_infos.append(
             {
                 "key": list(measures.keys())[0],
                 "parameters": {
-                    metric: extracted[metric] for metric in list(measures.values())[0]["metrics"]
+                    metric: extracted[metric]
+                    for metric in list(measures.values())[0]["metrics"]
                 },
             }
         )
 
     headers = ["Id", "Name", "Description", "Value", "Created at"]
     return core_calculate({"measures": calculate_infos}, config), headers
```

### Comparing `msgram-1.1.2/src/cli/resources/metrics.py` & `msgram-1.2.1/src/cli/resources/metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 def get_metric_value(extracted):
     """
     Função que recupera o valor mais recente da métrica
     """
     # Métricas que o parâmetro é uma lista de valores
     listed_values = [
-        'coverage', 'complexity', 'functions',
-        'comment_lines_density', 'duplicated_lines_density'
+        "coverage",
+        "complexity",
+        "functions",
+        "comment_lines_density",
+        "duplicated_lines_density",
     ]
 
     # Métricas que o parâmetro é extraido do UTS
-    uts_values = ['test_execution_time', 'tests']
+    uts_values = ["test_execution_time", "tests"]
     response_data = {}
 
     # Para todos os arquivos extraidos
     for path_readed in extracted.values():
-        qualifier = path_readed['qualifier']
-        measures = path_readed['measures']
+        qualifier = path_readed["qualifier"]
+        measures = path_readed["measures"]
 
         # Para cada métrica dentro das medidas
         for metric in measures:
-            metric_name = metric['metric']
-            metric_value = metric['value']
+            metric_name = metric["metric"]
+            metric_value = metric["value"]
 
             # Se ela for "agregada", olho apenas arquivos FIL,
             # se não, salvo somente a última.
-            if metric_name in listed_values and qualifier == 'FIL':
+            if metric_name in listed_values and qualifier == "FIL":
                 response_data.setdefault(metric_name, []).append(metric_value)
-            elif metric_name in uts_values and qualifier == 'UTS':
+            elif metric_name in uts_values and qualifier == "UTS":
                 response_data.setdefault(metric_name, []).append(metric_value)
-            elif metric_name not in (listed_values + uts_values) and qualifier == 'TRK':
+            elif metric_name not in (listed_values + uts_values) and qualifier == "TRK":
                 response_data[metric_name] = metric_value
 
     return response_data
```

### Comparing `msgram-1.1.2/src/cli/resources/subcharacteristic.py` & `msgram-1.2.1/src/cli/resources/characteristic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from src.cli.resources.measure import get_measure_value
+from src.cli.resources.subcharacteristic import get_subcharacteristic_value
 
-from resources import calculate_subcharacteristics as core_calculate
+from resources import calculate_characteristics as core_calculate
 
 
-def get_subcharacteristic_value(subchars, char):
-    subchar_calculated = []
-    for subchar in char:
-        subchar_key = subchar["key"]
+def get_characteristic_value(chars, tsqmi):
+    char_calculated = []
+    for char in tsqmi:
+        char_key = char["key"]
 
-        subchar_calculated.append({
-            "key": subchar_key,
-            "value": {m['key']: m['value'] for m in subchars}[subchar_key],
-            "weight": subchar['weight'],
-        })
+        char_calculated.append(
+            {
+                "key": char_key,
+                "value": {m["key"]: m["value"] for m in chars}[char_key],
+                "weight": char["weight"],
+            }
+        )
 
-    return subchar_calculated
+    return char_calculated
 
 
-def calculate_subcharacteristics(config, measures):
-    subchars = [sc['subcharacteristics'] for sc in config['characteristics']]
+def calculate_characteristics(config, subchars):
+    characteristics = config["characteristics"]
     calculate_infos = []
 
-    for subchar in subchars:
-        calculate_infos.append({
-            'key': subchar[0]['key'],
-            'measures': get_measure_value(measures, subchar[0]['measures'])
-        })
+    for char in characteristics:
+        calculate_infos.append(
+            {
+                "key": char["key"],
+                "subcharacteristics": get_subcharacteristic_value(
+                    subchars, char["subcharacteristics"]
+                ),
+            }
+        )
 
     headers = ["Id", "Name", "Description", "Value", "Created at"]
-    return core_calculate({'subcharacteristics': calculate_infos}), headers
+    return core_calculate({"characteristics": calculate_infos}), headers
```

### Comparing `msgram-1.1.2/src/cli/utils.py` & `msgram-1.2.1/src/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 def print_error(text: str):
     """Print a error message."""
     console.print(text, style="red")
 
 
 def print_table(the_dict: dict, table_name: str = "", field: str = ""):
-
     table = Table(
         title=table_name,
         title_style="bold",
         row_styles=["none", "dim"],
         border_style="bright_yellow",
         pad_edge=False,
         box=box.MINIMAL,
```

### Comparing `msgram-1.1.2/src/config/setup_log.py` & `msgram-1.2.1/src/config/setup_log.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     if log_mod == "quiet":
         basic_config("INFO", "WARNING", "w")
     elif log_mod == "verbose":
         basic_config("DEBUG", "DEBUG", "w")
     else:
         basic_config("WARNING", "ERROR", "w")
 
+
 # =================================================================================================
 
 
 def basic_config(console_level_name, file_level_name, file_mode):
-
     console_handler = logging.StreamHandler(sys.stdout)
     console_formatter = logging.Formatter(LOG_FORMATS[console_level_name], datefmt)
     console_handler.setFormatter(console_formatter)
     # console_handler.setLevel(LOG_LEVELS[console_level_name])
 
     # file_handler = logging.FileHandler(file_name, file_mode)
     # file_formatter = logging.Formatter(LOG_FORMATS[file_level_name])
```

### Comparing `msgram-1.1.2/tests/system/test_help.py` & `msgram-1.2.1/tests/system/test_help.py`

 * *Files identical despite different names*

### Comparing `msgram-1.1.2/tests/system/test_init.py` & `msgram-1.2.1/tests/system/test_init.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,24 +13,20 @@
     return out, err, proc.returncode
 
 
 def test_msgram_init_should_execute_sucessfully():
     temp_path = tempfile.mkdtemp()
     dir_path = f"{temp_path}/.msgram"
 
-    _, _, returncode = capture(
-        ["msgram", "init", "-cp", dir_path]
-    )
+    _, _, returncode = capture(["msgram", "init", "-cp", dir_path])
 
     assert returncode == 0
     shutil.rmtree(temp_path)
 
 
 def test_init_should_create_pre_config_in_existent_directory():
     temp_path = tempfile.mkdtemp()
 
-    _, err, returncode = capture(
-        ["msgram", "init", "-cp", temp_path]
-    )
+    _, err, returncode = capture(["msgram", "init", "-cp", temp_path])
 
     assert returncode == 0
     shutil.rmtree(temp_path)
```

### Comparing `msgram-1.1.2/tests/unit/test_calculate.py` & `msgram-1.2.1/tests/unit/test_calculate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,195 +1,229 @@
+import copy
 import os
+import shutil
 import sys
-import copy
-import pytest
 import tempfile
-import shutil
-
 from io import StringIO
 from pathlib import Path
 from unittest.mock import patch
 
-from src.cli.commands.cmd_calculate import command_calculate, calculate_all
+import pytest
+
+from src.cli.commands.cmd_calculate import calculate_all, command_calculate
 from src.cli.jsonReader import open_json_file
 
 CALCULATE_ARGS = {
     "output_format": "csv",
     "config_path": Path(""),
     "extracted_path": Path(""),
 }
 
 
 @pytest.mark.parametrize(
-    "calculate_arg",
-    ['output_format', 'config_path', 'extracted_path']
+    "calculate_arg", ["output_format", "config_path", "extracted_path"]
 )
 def test_calculate_invalid_args(calculate_arg):
     captured_output = StringIO()
     sys.stdout = captured_output
 
     args = copy.deepcopy(CALCULATE_ARGS)
     del args[calculate_arg]
 
     with pytest.raises(SystemExit):
         command_calculate(args)
 
     sys.stdout = sys.__stdout__
-    assert f"KeyError: args['{calculate_arg}'] - non-existent parameters" in captured_output.getvalue()
+    assert (
+        f"KeyError: args['{calculate_arg}'] - non-existent parameters"
+        in captured_output.getvalue()
+    )
 
 
 @pytest.mark.parametrize(
     "output_format,mult_file",
     [
-        ("tabular", False), ("tree", False), ("raw", False),
-        ("csv", True), ("json", True)
-    ]
+        ("tabular", False),
+        ("tree", False),
+        ("raw", False),
+        ("csv", True),
+        ("json", True),
+    ],
 )
 def test_calculate_file(output_format, mult_file):
     config_dirpath = tempfile.mkdtemp()
     extract_dirpath = tempfile.mkdtemp()
 
-    shutil.copy(
-        "tests/unit/data/msgram.json",
-        f"{config_dirpath}/msgram.json"
-    )
+    shutil.copy("tests/unit/data/msgram.json", f"{config_dirpath}/msgram.json")
 
     extracted_file_name = "fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-05-2023-21-40-30-develop-extracted.msgram"
     shutil.copy(
         f"tests/unit/data/{extracted_file_name}",
-        f"{extract_dirpath}/{extracted_file_name}"
+        f"{extract_dirpath}/{extracted_file_name}",
     )
 
     args = {
         "output_format": output_format,
         "config_path": Path(config_dirpath),
         "extracted_path": Path(
             extract_dirpath + (f"/{extracted_file_name}" if not mult_file else "")
         ),
     }
 
     if not mult_file:
-        calculate_patch = patch('builtins.input', return_value=output_format)
+        calculate_patch = patch("builtins.input", return_value=output_format)
         calculate_patch.start()
 
     command_calculate(args)
 
     assert len(os.listdir(config_dirpath)) == 2 if mult_file else 1
     assert len(os.listdir(extract_dirpath)) == 1
 
     shutil.rmtree(config_dirpath)
     shutil.rmtree(extract_dirpath)
 
 
 def test_calculate_all_dict():
     file_name = "fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-05-2023-21-40-30-develop-extracted.msgram"
     json_data = open_json_file(Path(f"tests/unit/data/{file_name}"))
-    config = open_json_file(Path('tests/unit/data/msgram.json'))
+    config = open_json_file(Path("tests/unit/data/msgram.json"))
 
     calculated = calculate_all(json_data, file_name, config)
+    print(calculated)
     assert calculated == {
-        'repository': [{'key': 'repository', 'value': 'fga-eps-mds-2022-2-MeasureSoftGram-CLI'}],
-        'version': [{'key': 'version', 'value': '01-05-2023-21-40'}],
-        'measures': [
-            {'key': 'passed_tests', 'value': 1.0},
-            {'key': 'test_builds', 'value': pytest.approx(0.9999969696180555, 0.00000000000001)},
-            {'key': 'test_coverage', 'value': pytest.approx(0.5153846153846154, 0.00000000000001)},
-            {'key': 'non_complex_file_density', 'value': pytest.approx(0.3789488966318234, 0.00000000000001)},
-            {'key': 'commented_file_density', 'value': pytest.approx(0.029230769230769227, 0.00000000000001)},
-            {'key': 'duplication_absense', 'value': 1.0}
+        "repository": [
+            {"key": "repository", "value": "fga-eps-mds-2022-2-MeasureSoftGram-CLI"}
+        ],
+        "version": [{"key": "version", "value": "01-05-2023-21-40"}],
+        "measures": [
+            {"key": "passed_tests", "value": 1.0},
+            {
+                "key": "test_builds",
+                "value": pytest.approx(0.9996969618055556, 0.00000000000001),
+            },
+            {
+                "key": "test_coverage",
+                "value": pytest.approx(0.4707692307692307, 0.00000000000001),
+            },
+            {
+                "key": "non_complex_file_density",
+                "value": pytest.approx(0.3789488966318234, 0.00000000000001),
+            },
+            {
+                "key": "commented_file_density",
+                "value": pytest.approx(0.029230769230769227, 0.00000000000001),
+            },
+            {"key": "duplication_absense", "value": 1.0},
+        ],
+        "subcharacteristics": [
+            {
+                "key": "testing_status",
+                "value": pytest.approx(0.8543507067377631, 0.00000000000001),
+            },
+            {
+                "key": "modifiability",
+                "value": pytest.approx(0.6276266582884098, 0.00000000000001),
+            },
         ],
-        'subcharacteristics': [
-            {'key': 'testing_status', 'value': pytest.approx(0.8633460569923477, 0.00000000000001)},
-            {'key': 'modifiability', 'value': pytest.approx(0.6276266582884098, 0.00000000000001)}
+        "characteristics": [
+            {
+                "key": "reliability",
+                "value": pytest.approx(0.8543507067377631, 0.00000000000001),
+            },
+            {
+                "key": "maintainability",
+                "value": pytest.approx(0.6276266582884098, 0.00000000000001),
+            },
+        ],
+        "tsqmi": [
+            {
+                "key": "tsqmi",
+                "value": pytest.approx(0.7496100160408716, 0.00000000000001),
+            }
         ],
-        'characteristics': [
-            {'key': 'reliability', 'value': pytest.approx(0.8633460569923477, 0.00000000000001)},
-            {'key': 'maintainability', 'value': pytest.approx(0.6276266582884098, 0.00000000000001)}],
-        'sqc': [{'key': 'sqc', 'value': pytest.approx(0.754745532056504, 0.00000000000001)}]
     }
 
 
 def test_calculate_invalid_config_file():
     captured_output = StringIO()
     sys.stdout = captured_output
 
     config_dirpath = tempfile.mkdtemp()
 
-    shutil.copy(
-        "tests/unit/data/invalid_json.json",
-        f"{config_dirpath}/msgram.json"
-    )
+    shutil.copy("tests/unit/data/invalid_json.json", f"{config_dirpath}/msgram.json")
 
     args = {
-        "output_format": 'csv',
+        "output_format": "csv",
         "config_path": Path(config_dirpath),
         "extracted_path": Path("."),
     }
 
     with pytest.raises(SystemExit):
         command_calculate(args)
 
     sys.stdout = sys.__stdout__
-    assert f"Error reading msgram.json config file in {config_dirpath}" in captured_output.getvalue()
+    assert (
+        f"Error reading msgram.json config file in {config_dirpath}"
+        in captured_output.getvalue()
+    )
 
     shutil.rmtree(config_dirpath)
 
 
 def test_calculate_invalid_extracted_file():
     captured_output = StringIO()
     sys.stdout = captured_output
 
     config_dirpath = tempfile.mkdtemp()
     extract_dirpath = tempfile.mkdtemp()
 
-    shutil.copy(
-        "tests/unit/data/msgram.json",
-        f"{config_dirpath}/msgram.json"
-    )
+    shutil.copy("tests/unit/data/msgram.json", f"{config_dirpath}/msgram.json")
 
     extracted_file_name = "invalid_json.json"
     shutil.copy(
         f"tests/unit/data/{extracted_file_name}",
-        f"{extract_dirpath}/{extracted_file_name}"
+        f"{extract_dirpath}/{extracted_file_name}",
     )
 
     args = {
         "output_format": "csv",
         "config_path": Path(config_dirpath),
-        "extracted_path": Path(
-            extract_dirpath + f"/{extracted_file_name}"),
+        "extracted_path": Path(extract_dirpath + f"/{extracted_file_name}"),
     }
 
     command_calculate(args)
 
     sys.stdout = sys.__stdout__
-    assert f"Error calculating {extract_dirpath}/{extracted_file_name}" in captured_output.getvalue()
+    assert (
+        f"Error calculating {extract_dirpath}/{extracted_file_name}"
+        in captured_output.getvalue()
+    )
     assert "All calculations performed" not in captured_output.getvalue()
 
     shutil.rmtree(config_dirpath)
     shutil.rmtree(extract_dirpath)
 
 
 def test_calculate_warn_zero_calculated_files():
     captured_output = StringIO()
     sys.stdout = captured_output
 
     config_dirpath = tempfile.mkdtemp()
 
-    shutil.copy(
-        "tests/unit/data/msgram.json",
-        f"{config_dirpath}/msgram.json"
-    )
+    shutil.copy("tests/unit/data/msgram.json", f"{config_dirpath}/msgram.json")
 
     args = {
         "output_format": "csv",
         "config_path": Path(config_dirpath),
         "extracted_path": Path("."),
     }
 
     command_calculate(args)
 
     sys.stdout = sys.__stdout__
-    assert "WARNING: No extracted file readed so no csv was generated!" in captured_output.getvalue()
+    assert (
+        "WARNING: No extracted file readed so no csv was generated!"
+        in captured_output.getvalue()
+    )
     assert "All calculations performed" not in captured_output.getvalue()
 
     shutil.rmtree(config_dirpath)
```

### Comparing `msgram-1.1.2/tests/unit/test_extract.py` & `msgram-1.2.1/tests/unit/test_extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 
 from src.cli.commands.cmd_extract import get_infos_from_name, command_extract
 
 EXTRACT_ARGS = {
     "output_origin": "sonarqube",
     "extracted_path": Path(""),
     "data_path": Path(""),
-    "language_extension": "py"
+    "language_extension": "py",
 }
 
 
 def test_get_file_infos():
     file_path = "tests/unit/data/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json"
 
     file_name = get_infos_from_name(file_path)
-    assert "fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop-extracted.msgram" in file_name
+    assert (
+        "fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop-extracted.msgram"
+        in file_name
+    )
 
 
 def test_not_get_file_infos_wrong_name():
     filename = "metrics/wrong-name.json"
 
     with pytest.raises(SystemExit) as e:
         _ = get_infos_from_name(filename)
@@ -34,29 +37,26 @@
     assert e.value.code == 1
 
 
 def test_command_extract_should_succeed():
     config_dirpath = tempfile.mkdtemp()
     extract_dirpath = tempfile.mkdtemp()
 
-    shutil.copy(
-        "tests/unit/data/msgram.json",
-        f"{config_dirpath}/msgram.json"
-    )
+    shutil.copy("tests/unit/data/msgram.json", f"{config_dirpath}/msgram.json")
 
     shutil.copy(
         "tests/unit/data/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json",
-        f"{extract_dirpath}/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json"
+        f"{extract_dirpath}/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json",
     )
 
     args = {
         "output_origin": "sonarqube",
         "extracted_path": Path(config_dirpath),
         "data_path": Path(extract_dirpath),
-        "language_extension": "py"
+        "language_extension": "py",
     }
 
     captured_output = StringIO()
     sys.stdout = captured_output
 
     command_extract(args)
 
@@ -70,35 +70,38 @@
 
     shutil.rmtree(config_dirpath)
     shutil.rmtree(extract_dirpath)
 
 
 @pytest.mark.parametrize(
     "extract_arg",
-    ['output_origin', 'extracted_path', 'data_path', 'language_extension']
+    ["output_origin", "extracted_path", "data_path", "language_extension"],
 )
 def test_extract_invalid_args(extract_arg):
     captured_output = StringIO()
     sys.stdout = captured_output
 
     args = copy.deepcopy(EXTRACT_ARGS)
     del args[extract_arg]
 
     with pytest.raises(SystemExit):
         command_extract(args)
 
     sys.stdout = sys.__stdout__
-    assert f"KeyError: args['{extract_arg}'] - non-existent parameters" in captured_output.getvalue()
+    assert (
+        f"KeyError: args['{extract_arg}'] - non-existent parameters"
+        in captured_output.getvalue()
+    )
 
 
 def test_command_extract_extracted_path_is_not_a_dir():
     captured_output = StringIO()
     sys.stdout = captured_output
 
     args = copy.deepcopy(EXTRACT_ARGS)
-    args['extracted_path'] = Path('inexistent')
+    args["extracted_path"] = Path("inexistent")
 
     with pytest.raises(SystemExit):
         command_extract(args)
 
     sys.stdout = sys.__stdout__
-    assert 'FileNotFoundError: extract directory' in captured_output.getvalue()
+    assert "FileNotFoundError: extract directory" in captured_output.getvalue()
```

### Comparing `msgram-1.1.2/tests/unit/test_init.py` & `msgram-1.2.1/tests/unit/test_init.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,66 +6,67 @@
 
 from io import StringIO
 from pathlib import Path
 from unittest.mock import patch
 
 from src.cli.commands.cmd_init import command_init
 
-INIT_ARGS = {
-    'config_path': '.testmsgram'
-}
+INIT_ARGS = {"config_path": ".testmsgram"}
 
 
-@pytest.mark.parametrize(
-    "init_arg",
-    ['config_path']
-)
+@pytest.mark.parametrize("init_arg", ["config_path"])
 def test_init_invalid_args(init_arg):
     captured_output = StringIO()
     sys.stdout = captured_output
 
     with pytest.raises(SystemExit):
         command_init({})
 
     sys.stdout = sys.__stdout__
-    assert f"KeyError: args['{init_arg}'] - non-existent parameters" in captured_output.getvalue()
+    assert (
+        f"KeyError: args['{init_arg}'] - non-existent parameters"
+        in captured_output.getvalue()
+    )
 
 
 def test_init_config_file():
     temp_path = tempfile.mkdtemp()
     config_path = f'{temp_path}/{INIT_ARGS["config_path"]}'
 
     captured_output = StringIO()
     sys.stdout = captured_output
 
-    command_init({'config_path': Path(config_path)})
+    command_init({"config_path": Path(config_path)})
     sys.stdout = sys.__stdout__
 
     assert len(os.listdir(config_path)) == 1
-    assert os.listdir(config_path)[0] == 'msgram.json'
+    assert os.listdir(config_path)[0] == "msgram.json"
 
-    assert "The file config: '.testmsgram/msgram.json' was created successfully." in captured_output.getvalue()
+    assert (
+        "The file config: '.testmsgram/msgram.json' was created successfully."
+        in captured_output.getvalue()
+    )
 
     shutil.rmtree(temp_path)
 
 
 def test_init_replace_file():
     config_path = tempfile.mkdtemp()
 
     captured_output = StringIO()
     sys.stdout = captured_output
 
-    shutil.copy(
-        "tests/unit/data/msgram.json",
-        f"{config_path}/msgram.json"
-    )
+    shutil.copy("tests/unit/data/msgram.json", f"{config_path}/msgram.json")
 
-    with patch('builtins.input', return_value='n'):
-        command_init({'config_path': Path(config_path)})
+    with patch("builtins.input", return_value="n"):
+        command_init({"config_path": Path(config_path)})
         sys.stdout = sys.__stdout__
 
     assert len(os.listdir(config_path)) == 1
-    assert os.listdir(config_path)[0] == 'msgram.json'
+    assert os.listdir(config_path)[0] == "msgram.json"
 
-    assert f"The file config: '{config_path.split('/')[-1]}/msgram.json' not changed..." in captured_output.getvalue()
+    assert (
+        f"The file config: '{config_path.split('/')[-1]}/msgram.json' not changed..."
+        in captured_output.getvalue()
+    )
 
     shutil.rmtree(config_path)
```

### Comparing `msgram-1.1.2/tests/unit/test_jsonReader.py` & `msgram-1.2.1/tests/unit/test_jsonReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     assert components == EXPECTED_SONAR_JSON_COMPONENTS
 
 
 class TestOpenJsonFile:
     """
     Tests open_json_file function
     """
+
     def test_file_not_found(self):
         """
         Test when the file does not exists
         """
         with pytest.raises(exceptions.FileNotFound) as error:
             jsonReader.open_json_file(Path("tests/utils/sona.json"))
 
@@ -74,15 +75,15 @@
         Test when an error is returned
         """
 
         # with mocker.patch("sys.stdout", new=StringIO()) as fake_out:
         message = jsonReader.validate_metrics_post(status_code)
 
         assert (
-            f'FAIL: The host service server returned a {status_code} error. Trying again'
+            f"FAIL: The host service server returned a {status_code} error. Trying again"
             == message
         )
 
 
 class TestCheckMetricsValues:
     """
     Tests check_metrics_values function
@@ -230,15 +231,15 @@
                     "key": "",
                     "name": "",
                     "qualifier": "",
                     "measures": [
                         {"metric": "test_failures"},
                         {"metric": "test_errors"},
                         {"metric": "files"},
-                        {"metric": "ncloc"}
+                        {"metric": "ncloc"},
                     ],
                 },
                 "components": {},
             },
             "File with valid schema but no metrics data.",
         ),
     ]
@@ -254,30 +255,35 @@
         assert error_msg in str(error.value)
 
 
 def test_read_multiple_files():
     dirpath = tempfile.mkdtemp()
     shutil.copy(
         "tests/unit/data/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json",
-        f"{dirpath}/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json"
+        f"{dirpath}/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json",
     )
 
-    file_names = [file_name for _, file_name in jsonReader.read_mult_files(Path(dirpath), 'json')]
+    file_names = [
+        file_name for _, file_name in jsonReader.read_mult_files(Path(dirpath), "json")
+    ]
     assert len(file_names) == 1
-    assert file_names[0] == "fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json"
+    assert (
+        file_names[0]
+        == "fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json"
+    )
 
     shutil.rmtree(dirpath)
 
 
 def test_validate_empty_folder_pattern():
     dirpath = tempfile.mkdtemp()
     shutil.copy(
         "tests/unit/data/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json",
-        f"{dirpath}/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json"
+        f"{dirpath}/fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-11-2023-21-59-03-develop.json",
     )
 
     with pytest.raises(exceptions.MeasureSoftGramCLIException) as error:
-        list(jsonReader.folder_reader(Path(dirpath), 'empty'))
+        list(jsonReader.folder_reader(Path(dirpath), "empty"))
 
     assert str(error.value) == "No files .empty found inside folder."
 
     shutil.rmtree(dirpath)
```

