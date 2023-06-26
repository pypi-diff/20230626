# Comparing `tmp/zcc-helper-3.1.tar.gz` & `tmp/zcc-helper-3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcc-helper-3.1.tar", last modified: Mon Jun 26 06:42:06 2023, max compression
+gzip compressed data, was "zcc-helper-3.1rc1.tar", last modified: Sun Jun 25 05:21:52 2023, max compression
```

## Comparing `zcc-helper-3.1.tar` & `zcc-helper-3.1rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-26 06:42:06.667386 zcc-helper-3.1/
--rw-r--r--   0 mark       (501) staff       (20)    10150 2023-06-26 06:42:06.667176 zcc-helper-3.1/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     9867 2022-06-20 04:14:44.000000 zcc-helper-3.1/README.md
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-26 06:42:06.667442 zcc-helper-3.1/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.1/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-26 06:42:06.665450 zcc-helper-3.1/zcc/
--rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.1/zcc/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.1/zcc/__main__.py
--rw-r--r--   0 mark       (501) staff       (20)      244 2023-06-26 06:42:01.000000 zcc-helper-3.1/zcc/constants.py
--rw-r--r--   0 mark       (501) staff       (20)    17770 2023-06-25 05:17:16.000000 zcc-helper-3.1/zcc/controller.py
--rw-r--r--   0 mark       (501) staff       (20)      417 2023-06-25 05:04:27.000000 zcc-helper-3.1/zcc/description.py
--rw-r--r--   0 mark       (501) staff       (20)     9773 2023-06-25 04:59:02.000000 zcc-helper-3.1/zcc/device.py
--rw-r--r--   0 mark       (501) staff       (20)     4430 2023-06-25 05:05:22.000000 zcc-helper-3.1/zcc/discovery.py
--rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.1/zcc/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     3732 2022-06-18 00:10:40.000000 zcc-helper-3.1/zcc/protocol.py
--rw-r--r--   0 mark       (501) staff       (20)     6372 2022-06-18 00:10:40.000000 zcc-helper-3.1/zcc/socket.py
--rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.1/zcc/trace.py
--rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.1/zcc/watchdog.py
--rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.1/zcc.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-26 06:42:06.666849 zcc-helper-3.1/zcc_helper.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)    10150 2023-06-26 06:42:06.000000 zcc-helper-3.1/zcc_helper.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      351 2023-06-26 06:42:06.000000 zcc-helper-3.1/zcc_helper.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-26 06:42:06.000000 zcc-helper-3.1/zcc_helper.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        4 2023-06-26 06:42:06.000000 zcc-helper-3.1/zcc_helper.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 05:21:52.802554 zcc-helper-3.1rc1/
+-rw-r--r--   0 mark       (501) staff       (20)    10153 2023-06-25 05:21:52.802220 zcc-helper-3.1rc1/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     9867 2022-06-20 04:14:44.000000 zcc-helper-3.1rc1/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-25 05:21:52.802625 zcc-helper-3.1rc1/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.1rc1/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 05:21:52.798601 zcc-helper-3.1rc1/zcc/
+-rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.1rc1/zcc/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.1rc1/zcc/__main__.py
+-rw-r--r--   0 mark       (501) staff       (20)      247 2023-06-25 05:21:32.000000 zcc-helper-3.1rc1/zcc/constants.py
+-rw-r--r--   0 mark       (501) staff       (20)    17770 2023-06-25 05:17:16.000000 zcc-helper-3.1rc1/zcc/controller.py
+-rw-r--r--   0 mark       (501) staff       (20)      417 2023-06-25 05:04:27.000000 zcc-helper-3.1rc1/zcc/description.py
+-rw-r--r--   0 mark       (501) staff       (20)     9773 2023-06-25 04:59:02.000000 zcc-helper-3.1rc1/zcc/device.py
+-rw-r--r--   0 mark       (501) staff       (20)     4430 2023-06-25 05:05:22.000000 zcc-helper-3.1rc1/zcc/discovery.py
+-rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.1rc1/zcc/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     3732 2022-06-18 00:10:40.000000 zcc-helper-3.1rc1/zcc/protocol.py
+-rw-r--r--   0 mark       (501) staff       (20)     6372 2022-06-18 00:10:40.000000 zcc-helper-3.1rc1/zcc/socket.py
+-rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.1rc1/zcc/trace.py
+-rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.1rc1/zcc/watchdog.py
+-rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.1rc1/zcc.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 05:21:52.801369 zcc-helper-3.1rc1/zcc_helper.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)    10153 2023-06-25 05:21:52.000000 zcc-helper-3.1rc1/zcc_helper.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      351 2023-06-25 05:21:52.000000 zcc-helper-3.1rc1/zcc_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-25 05:21:52.000000 zcc-helper-3.1rc1/zcc_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        4 2023-06-25 05:21:52.000000 zcc-helper-3.1rc1/zcc_helper.egg-info/top_level.txt
```

### Comparing `zcc-helper-3.1/PKG-INFO` & `zcc-helper-3.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.1
+Version: 3.1rc1
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `zcc-helper-3.1/README.md` & `zcc-helper-3.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/setup.py` & `zcc-helper-3.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/zcc/__main__.py` & `zcc-helper-3.1rc1/zcc/__main__.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/zcc/controller.py` & `zcc-helper-3.1rc1/zcc/controller.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/zcc/device.py` & `zcc-helper-3.1rc1/zcc/device.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/zcc/discovery.py` & `zcc-helper-3.1rc1/zcc/discovery.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/zcc/protocol.py` & `zcc-helper-3.1rc1/zcc/protocol.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/zcc/socket.py` & `zcc-helper-3.1rc1/zcc/socket.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/zcc/trace.py` & `zcc-helper-3.1rc1/zcc/trace.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/zcc/watchdog.py` & `zcc-helper-3.1rc1/zcc/watchdog.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.1/zcc_helper.egg-info/PKG-INFO` & `zcc-helper-3.1rc1/zcc_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.1
+Version: 3.1rc1
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

