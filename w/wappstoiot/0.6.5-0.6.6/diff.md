# Comparing `tmp/wappstoiot-0.6.5.tar.gz` & `tmp/wappstoiot-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wappstoiot-0.6.5.tar", last modified: Tue Feb 28 13:19:50 2023, max compression
+gzip compressed data, was "wappstoiot-0.6.6.tar", last modified: Mon Jun 26 11:15:27 2023, max compression
```

## Comparing `wappstoiot-0.6.5.tar` & `wappstoiot-0.6.6.tar`

### file list

```diff
@@ -1,45 +1,69 @@
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-02-28 13:19:50.064149 wappstoiot-0.6.5/
--rw-r--r--   0 bach      (1000) bach      (1000)     5021 2023-02-28 13:17:32.000000 wappstoiot-0.6.5/CHANGELOG.md
--rw-rw-r--   0 bach      (1000) bach      (1000)     1064 2022-03-14 08:11:46.000000 wappstoiot-0.6.5/LICENSE
--rw-rw-r--   0 bach      (1000) bach      (1000)       38 2022-03-14 08:11:46.000000 wappstoiot-0.6.5/MANIFEST.in
--rw-r--r--   0 bach      (1000) bach      (1000)     8252 2023-02-28 13:19:50.064149 wappstoiot-0.6.5/PKG-INFO
--rw-r--r--   0 bach      (1000) bach      (1000)     2800 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/README.md
--rw-r--r--   0 bach      (1000) bach      (1000)       38 2023-02-28 13:19:50.064149 wappstoiot-0.6.5/setup.cfg
--rw-rw-r--   0 bach      (1000) bach      (1000)     2286 2022-07-12 12:41:58.000000 wappstoiot-0.6.5/setup.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-02-28 13:19:50.053149 wappstoiot-0.6.5/test/
--rw-r--r--   0 bach      (1000) bach      (1000)     3151 2023-02-28 09:18:04.000000 wappstoiot-0.6.5/test/test_real_world.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-02-28 13:19:50.054149 wappstoiot-0.6.5/wappstoiot/
--rw-r--r--   0 bach      (1000) bach      (1000)    10998 2023-02-28 13:17:32.000000 wappstoiot-0.6.5/wappstoiot/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)     8035 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/wappstoiot/__main__.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-02-28 13:19:50.057149 wappstoiot-0.6.5/wappstoiot/connections/
--rw-rw-r--   0 bach      (1000) bach      (1000)        0 2022-03-14 08:11:45.000000 wappstoiot-0.6.5/wappstoiot/connections/__init__.py
--rw-rw-r--   0 bach      (1000) bach      (1000)     2469 2022-03-14 08:11:45.000000 wappstoiot-0.6.5/wappstoiot/connections/protocol.py
--rw-r--r--   0 bach      (1000) bach      (1000)     9934 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/wappstoiot/connections/sslsocket.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-02-28 13:19:50.059149 wappstoiot-0.6.5/wappstoiot/modules/
--rw-rw-r--   0 bach      (1000) bach      (1000)        0 2022-03-14 08:11:45.000000 wappstoiot-0.6.5/wappstoiot/modules/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)    15727 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/wappstoiot/modules/device.py
--rw-r--r--   0 bach      (1000) bach      (1000)    10719 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/wappstoiot/modules/network.py
--rw-r--r--   0 bach      (1000) bach      (1000)    19243 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/wappstoiot/modules/template.py
--rw-r--r--   0 bach      (1000) bach      (1000)    27776 2023-02-28 12:46:35.000000 wappstoiot-0.6.5/wappstoiot/modules/value.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-02-28 13:19:50.060149 wappstoiot-0.6.5/wappstoiot/schema/
--rw-rw-r--   0 bach      (1000) bach      (1000)        0 2022-03-14 08:11:45.000000 wappstoiot-0.6.5/wappstoiot/schema/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)    12612 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/wappstoiot/schema/base_schema.py
--rw-rw-r--   0 bach      (1000) bach      (1000)     5598 2022-05-05 14:14:25.000000 wappstoiot-0.6.5/wappstoiot/schema/iot_schema.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-02-28 13:19:50.061149 wappstoiot-0.6.5/wappstoiot/service/
--rw-rw-r--   0 bach      (1000) bach      (1000)        0 2022-03-14 08:11:45.000000 wappstoiot-0.6.5/wappstoiot/service/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)    22423 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/wappstoiot/service/iot_api.py
--rw-rw-r--   0 bach      (1000) bach      (1000)     4180 2022-03-14 08:11:45.000000 wappstoiot-0.6.5/wappstoiot/service/template.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-02-28 13:19:50.063149 wappstoiot-0.6.5/wappstoiot/utils/
--rw-r--r--   0 bach      (1000) bach      (1000)      646 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/wappstoiot/utils/Timestamp.py
--rw-rw-r--   0 bach      (1000) bach      (1000)        0 2022-03-14 08:11:45.000000 wappstoiot-0.6.5/wappstoiot/utils/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)      325 2023-02-27 15:18:27.000000 wappstoiot-0.6.5/wappstoiot/utils/certificateread.py
--rw-rw-r--   0 bach      (1000) bach      (1000)      382 2022-03-14 08:11:45.000000 wappstoiot-0.6.5/wappstoiot/utils/name_check.py
--rw-rw-r--   0 bach      (1000) bach      (1000)     2607 2022-07-12 12:41:58.000000 wappstoiot-0.6.5/wappstoiot/utils/observer.py
--rw-rw-r--   0 bach      (1000) bach      (1000)     2497 2022-07-12 12:41:58.000000 wappstoiot-0.6.5/wappstoiot/utils/offline_storage.py
--rw-rw-r--   0 bach      (1000) bach      (1000)     6497 2022-03-14 08:11:45.000000 wappstoiot-0.6.5/wappstoiot/utils/tracer.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-02-28 13:19:50.056149 wappstoiot-0.6.5/wappstoiot.egg-info/
--rw-r--r--   0 bach      (1000) bach      (1000)     8252 2023-02-28 13:19:48.000000 wappstoiot-0.6.5/wappstoiot.egg-info/PKG-INFO
--rw-r--r--   0 bach      (1000) bach      (1000)      950 2023-02-28 13:19:49.000000 wappstoiot-0.6.5/wappstoiot.egg-info/SOURCES.txt
--rw-r--r--   0 bach      (1000) bach      (1000)        1 2023-02-28 13:19:48.000000 wappstoiot-0.6.5/wappstoiot.egg-info/dependency_links.txt
--rw-r--r--   0 bach      (1000) bach      (1000)       51 2023-02-28 13:19:49.000000 wappstoiot-0.6.5/wappstoiot.egg-info/requires.txt
--rw-r--r--   0 bach      (1000) bach      (1000)       11 2023-02-28 13:19:49.000000 wappstoiot-0.6.5/wappstoiot.egg-info/top_level.txt
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.235953 wappstoiot-0.6.6/
+-rw-r--r--   0 bach      (1000) bach      (1000)     5336 2023-06-22 10:08:45.000000 wappstoiot-0.6.6/CHANGELOG.md
+-rw-rw-r--   0 bach      (1000) bach      (1000)     1064 2022-03-14 08:11:46.000000 wappstoiot-0.6.6/LICENSE
+-rw-r--r--   0 bach      (1000) bach      (1000)      115 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/MANIFEST.in
+-rw-r--r--   0 bach      (1000) bach      (1000)     8895 2023-06-26 11:15:27.234953 wappstoiot-0.6.6/PKG-INFO
+-rw-r--r--   0 bach      (1000) bach      (1000)     3128 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/README.md
+-rw-r--r--   0 bach      (1000) bach      (1000)       38 2023-06-26 11:15:27.235953 wappstoiot-0.6.6/setup.cfg
+-rw-r--r--   0 bach      (1000) bach      (1000)     2368 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/setup.py
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.214953 wappstoiot-0.6.6/test/
+-rw-r--r--   0 bach      (1000) bach      (1000)     3159 2023-06-22 10:08:45.000000 wappstoiot-0.6.6/test/test_real_world.py
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.216953 wappstoiot-0.6.6/wappstoiot/
+-rw-r--r--   0 bach      (1000) bach      (1000)    11300 2023-06-22 10:08:45.000000 wappstoiot-0.6.6/wappstoiot/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1080 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     8363 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/__main__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      503 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/__main__.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.220953 wappstoiot-0.6.6/wappstoiot/connections/
+-rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/connections/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/connections/__init__.pyi
+-rw-rw-r--   0 bach      (1000) bach      (1000)     2469 2022-03-14 08:11:45.000000 wappstoiot-0.6.6/wappstoiot/connections/protocol.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      756 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/connections/protocol.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     9934 2023-02-27 15:18:27.000000 wappstoiot-0.6.6/wappstoiot/connections/sslsocket.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      938 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/connections/sslsocket.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.224953 wappstoiot-0.6.6/wappstoiot/modules/
+-rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    16057 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/modules/device.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3496 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/device.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    10785 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/modules/network.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1695 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/network.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    19243 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/modules/template.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1964 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/template.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    28153 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/modules/value.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3569 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/value.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)       62 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/py.typed
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.226953 wappstoiot-0.6.6/wappstoiot/schema/
+-rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/schema/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/schema/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    12612 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/schema/base_schema.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     8211 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/schema/base_schema.pyi
+-rw-rw-r--   0 bach      (1000) bach      (1000)     5598 2022-05-05 14:14:25.000000 wappstoiot-0.6.6/wappstoiot/schema/iot_schema.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1620 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/schema/iot_schema.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.229953 wappstoiot-0.6.6/wappstoiot/service/
+-rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/service/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/service/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    22423 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/service/iot_api.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3438 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/service/iot_api.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     4180 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/service/template.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     2604 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/service/template.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.233953 wappstoiot-0.6.6/wappstoiot/utils/
+-rw-r--r--   0 bach      (1000) bach      (1000)      646 2023-02-27 15:18:27.000000 wappstoiot-0.6.6/wappstoiot/utils/Timestamp.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      107 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/Timestamp.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)      426 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/utils/certificateread.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      122 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/certificateread.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)      691 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/name_check.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      142 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/name_check.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     2704 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/utils/observer.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      403 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/observer.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     2497 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/utils/offline_storage.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      665 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/offline_storage.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     6497 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/utils/tracer.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1304 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/tracer.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.218953 wappstoiot-0.6.6/wappstoiot.egg-info/
+-rw-r--r--   0 bach      (1000) bach      (1000)     8895 2023-06-26 11:15:26.000000 wappstoiot-0.6.6/wappstoiot.egg-info/PKG-INFO
+-rw-r--r--   0 bach      (1000) bach      (1000)     1699 2023-06-26 11:15:27.000000 wappstoiot-0.6.6/wappstoiot.egg-info/SOURCES.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)        1 2023-06-26 11:15:26.000000 wappstoiot-0.6.6/wappstoiot.egg-info/dependency_links.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)       51 2023-06-26 11:15:26.000000 wappstoiot-0.6.6/wappstoiot.egg-info/requires.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)       11 2023-06-26 11:15:26.000000 wappstoiot-0.6.6/wappstoiot.egg-info/top_level.txt
```

### Comparing `wappstoiot-0.6.5/CHANGELOG.md` & `wappstoiot-0.6.6/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+v0.6.6 (Jun 22 2023)
+===============================================================================
+## Added
+ * Code Stub.
+
+## Changed
+ * Now inform which characters are illegal in the given name.
+
+## Fixed
+ * The `getReportTimestamp` & `getControlTimestamp` now ensures the return is `None` or of type datetime.
+
 v0.6.5 (Feb 28 2023)
 ===============================================================================
 ## Fixed
  * Report & Control now generate a timestamp in UTC time.
 
 v0.6.4 (Feb 27 2023)
 ===============================================================================
```

### Comparing `wappstoiot-0.6.5/LICENSE` & `wappstoiot-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/PKG-INFO` & `wappstoiot-0.6.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: wappstoiot
-Version: 0.6.5
+Version: 0.6.6
 Summary: Simple Wappsto Python user-interface to Wappsto IoT
 Home-page: https://github.com/Wappsto/python-wappsto-iot
 Author: Seluxit A/S
 Author-email: support@seluxit.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Wappsto IoT
 ===============================================================================
 
-[![Build Status](https://travis-ci.com/Wappsto/python-wappsto-iot.svg?branch=master)](https://travis-ci.com/Wappsto/python-wappsto-iot)
-[![Coverage Status](https://coveralls.io/repos/github/Wappsto/python-wappsto-iot/badge.svg?branch=master)](https://coveralls.io/github/Wappsto/python-wappsto-iot?branch=master)
+[![python](https://img.shields.io/badge/Python-3.6%203.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
+[![Test Status](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/test.yml/badge.svg)](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/test.yml)
+[![Lint Status](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/lint.yml/badge.svg)](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/lint.yml)
+[![Coverage](https://codecov.io/github/wappsto/python-wappsto-iot/branch/main/graph/badge.svg)](https://codecov.io/github/wappsto/python-wappsto-iot)
 
 The wappstoiot module provide a simple python interface to [wappsto.com](https://wappsto.com/) for easy prototyping.
 
 
 ## Prerequisites
 
 A [wappsto.com](https://wappsto.com/) Account, that the unit can connect to.
@@ -57,15 +59,15 @@
 
 
 Working examples of usage can be found in the [example folder](./example).
 
 The needed certificates can be downloaded with: `python -m wappstoiot --path echo`
 Where path is the path to the config-folder, given in the following code example.
 
-There is also a Wapp avaliable called: [IoT Certificate Manager](https://wappsto.com/store/wapp=iot_certificate_manager) on wappsto,
+There is also a Wapp avaliable called: [IoT Certificate Manager](https://wappsto.com/store/application/iot_certificate_manager) on wappsto,
 that given you a GUI to do the same and more.
 
 ### Echo example
 
 The following explains the example code found in [echo.py](./example/echo.py).
 
 
@@ -119,14 +121,25 @@
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details.
 
 
 
+v0.6.6 (Jun 22 2023)
+===============================================================================
+## Added
+ * Code Stub.
+
+## Changed
+ * Now inform which characters are illegal in the given name.
+
+## Fixed
+ * The `getReportTimestamp` & `getControlTimestamp` now ensures the return is `None` or of type datetime.
+
 v0.6.5 (Feb 28 2023)
 ===============================================================================
 ## Fixed
  * Report & Control now generate a timestamp in UTC time.
 
 v0.6.4 (Feb 27 2023)
 ===============================================================================
```

### Comparing `wappstoiot-0.6.5/README.md` & `wappstoiot-0.6.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Wappsto IoT
 ===============================================================================
 
-[![Build Status](https://travis-ci.com/Wappsto/python-wappsto-iot.svg?branch=master)](https://travis-ci.com/Wappsto/python-wappsto-iot)
-[![Coverage Status](https://coveralls.io/repos/github/Wappsto/python-wappsto-iot/badge.svg?branch=master)](https://coveralls.io/github/Wappsto/python-wappsto-iot?branch=master)
+[![python](https://img.shields.io/badge/Python-3.6%203.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
+[![Test Status](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/test.yml/badge.svg)](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/test.yml)
+[![Lint Status](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/lint.yml/badge.svg)](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/lint.yml)
+[![Coverage](https://codecov.io/github/wappsto/python-wappsto-iot/branch/main/graph/badge.svg)](https://codecov.io/github/wappsto/python-wappsto-iot)
 
 The wappstoiot module provide a simple python interface to [wappsto.com](https://wappsto.com/) for easy prototyping.
 
 
 ## Prerequisites
 
 A [wappsto.com](https://wappsto.com/) Account, that the unit can connect to.
@@ -43,15 +45,15 @@
 
 
 Working examples of usage can be found in the [example folder](./example).
 
 The needed certificates can be downloaded with: `python -m wappstoiot --path echo`
 Where path is the path to the config-folder, given in the following code example.
 
-There is also a Wapp avaliable called: [IoT Certificate Manager](https://wappsto.com/store/wapp=iot_certificate_manager) on wappsto,
+There is also a Wapp avaliable called: [IoT Certificate Manager](https://wappsto.com/store/application/iot_certificate_manager) on wappsto,
 that given you a GUI to do the same and more.
 
 ### Echo example
 
 The following explains the example code found in [echo.py](./example/echo.py).
```

### Comparing `wappstoiot-0.6.5/setup.py` & `wappstoiot-0.6.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,17 @@
         "Operating System :: OS Independent"
     ],
     packages=find_packages(),
     # tests_require=[
     #     'pytest',
     #     'tox'
     # ],
+    package_data={
+        'wappstoiot': ["py.typed", "*.pyi", "**/*.pyi"]
+    },
     install_requires=[
         'slxjsonrpc>=0.8.1',
         'pydantic>=1.6.1',
         'requests>=2.25.1'
     ],
     # entry_points={  # TODO: fix __main__.py to be optional.
     #     "console_scripts": "wappstoiot=wappstoiot:__main__"
```

### Comparing `wappstoiot-0.6.5/test/test_real_world.py` & `wappstoiot-0.6.6/test/test_real_world.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import uuid
 import wappstoiot
 
 from typing import Optional
 
 from utils import file_utils
 
-from wappstoiot.__main__ import start_session
-from wappstoiot.__main__ import create_network
-from wappstoiot.__main__ import claim_network
-from wappstoiot.__main__ import create_certificaties_files
+from wappstoiot.__main__ import _start_session
+from wappstoiot.__main__ import _create_network
+from wappstoiot.__main__ import _claim_network
+from wappstoiot.__main__ import _create_certificaties_files
 
 
 def pytest_generate_tests(metafunc):
     """Attach the cmd-line args to a test-class that needs them."""
     token = metafunc.config.getoption("token")
     if token and hasattr(metafunc.cls, 'token'):
         metafunc.cls.token = token
@@ -31,37 +31,37 @@
         username: Optional[str] = None,
         password: Optional[str] = None,
         token: Optional[str] = None,
     ):
         """Generate the needed certificates for a 'real' world test."""
         base_url: str = "qa.wappsto.com"
         if not token:
-            session = start_session(
+            session = _start_session(
                 base_url=base_url,
                 username=username,
                 password=password,
             )
         else:
             session = token
 
-        creator = create_network(
+        creator = _create_network(
             session=session,
             base_url=base_url,
             dry_run=False
         )
-        claim_network(
+        _claim_network(
             session=session,
             base_url=base_url,
             network_uuid=creator.get('network', {}).get('id'),
             dry_run=False
         )
 
         self.temp.mkdir(exist_ok=True)
 
-        create_certificaties_files(self.temp, creator, dry_run=False)
+        _create_certificaties_files(self.temp, creator, dry_run=False)
 
 
 class TestWithOutMocking(BaseTestClassWithCertificateFiles):
 
     token: Optional[uuid.UUID] = None
 
     @classmethod
```

### Comparing `wappstoiot-0.6.5/wappstoiot/__init__.py` & `wappstoiot-0.6.6/wappstoiot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 from .utils import observer
 from .utils import name_check
 
 # #############################################################################
 #                             __init__ Setup Stuff
 # #############################################################################
 
-__version__ = "v0.6.5"
+__version__ = "v0.6.6"
 __auther__ = "Seluxit A/S"
 
 __all__ = [
     'Network',
     'Device',
     'Value',
     'onStatusChange',
@@ -89,15 +89,14 @@
     StatusID: Union[service.StatusID, connection.StatusID],
     callback: Callable[[Union[service.StatusID, connection.StatusID], Any], None]
 ):
     """
     Configure an action when the Status have changed.
 
     def callback(StatusID: StatusID, newStatus: Any):
-
     """
     observer.subscribe(
         event_name=StatusID,
         callback=callback
     )
 
 
@@ -194,17 +193,15 @@
 #         kwargs = {"username": login[0], "password": login[1]}
 #     else:
 #         raise ValueError("No login was found.")
 #     __the_connection = RestAPI(**kwargs, url=configs.end_point)
 
 
 def _certificate_check(path) -> Dict[str, Path]:
-    """
-    Check if the right certificates are at the given path.
-    """
+    """Check if the right certificates are at the given path."""
     certi_path = {
         "ca": "ca.crt",
         "crt": "client.crt",
         "key": "client.key",
     }
     r_paths: Dict[str, Path] = {}
     for k, f in certi_path.items():
@@ -292,20 +289,28 @@
 #                             Create Stuff
 # #############################################################################
 
 def createNetwork(
     name: str,
     description: str = "",
 ) -> Network:
+    """
+    Create a new Wappsto Network.
+
+    A Wappsto Network is references to the main grouping, of which multiple
+    device are connected.
+    """
     global __config_folder
     global __the_connection
 
-    if not name_check.legal_name(name):
+    illegal_chars: str = name_check.illegal_characters(name)
+
+    if illegal_chars:
         raise ValueError(
-            "Given name contain a ilegal character."
+            f"Given name contain a illegal character: {illegal_chars}"
             f"May only contain: {name_check.wappsto_letters}"
         )
 
     if not __the_connection:
         config()
 
     if not __config_folder:
@@ -325,23 +330,25 @@
 
 # -------------------------------------------------------------------------
 #   Connection methods
 # -------------------------------------------------------------------------
 
 
 def connect():
+    """NOT Implemented yet."""
     pass
 
 
 def disconnect():
+    """NOT Implemented yet."""
     pass
 
 
 def close():
-    """."""
+    """Close down the connection to wappsto."""
     atexit.unregister(close)
     __ping_pong_thread_killed.set()
     __offline_storage_thread_killed.set()
     # atexit._run_exitfuncs()
     global __connection_closed
     global __the_connection
```

### Comparing `wappstoiot-0.6.5/wappstoiot/__main__.py` & `wappstoiot-0.6.6/wappstoiot/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""
+A helper script to generate the needed certificates for wappsto.
+
+Certificates are use for the Wappsto IoT library to identify itself on
+the wappsto platform, through a secure connection.
+"""
 import argparse
 import getpass
 import json
 import pathlib
 import sys
 import uuid
 
@@ -49,15 +55,15 @@
         err = data.text
     else:
         err = err.get('message', f"Unknown Error: http error: {data.status_code}")
     print(f"\t{err}")
     exit(-2)
 
 
-def start_session(base_url, username, password):
+def _start_session(base_url, username, password):
     session_json = {
         "username": username,
         "password": password,
         "remember_me": False
     }
 
     url = f"https://{base_url}/services/session"
@@ -77,15 +83,15 @@
     rjson = json.loads(rdata.text)
 
     print(rjson)
 
     return rjson["meta"]["id"]
 
 
-def create_network(
+def _create_network(
     session,
     base_url,
     # network_uuid=None,
     product=None,
     test_mode=False,
     reset_manufacturer=False,
     dry_run=False
@@ -124,15 +130,15 @@
         print("\nDry-run: Fake Certificates created!")
 
     print(f"\nCertificate generated for new network:\t{rjson['network']['id']}")
 
     return rjson
 
 
-def claim_network(session, base_url, network_uuid, dry_run=False):
+def _claim_network(session, base_url, network_uuid, dry_run=False):
     url = f"https://{base_url}/services/2.0/network/{network_uuid}"
 
     headers = {
         "Content-type": "application/json",
         "X-session": str(session)
     }
 
@@ -158,15 +164,15 @@
         }
         print("\nFake Claiming the Network.")
 
     print(f"\nNetwork: {network_uuid} have been claimed.")
     return rjson
 
 
-def get_network(session, base_url, network_uuid):
+def _get_network(session, base_url, network_uuid):
     url = f"https://{base_url}/services/2.1/creator?this_network.id={network_uuid}"
     headers = {
         "Content-type": "application/json",
         "X-session": str(session)
     }
 
     rdata = requests.get(
@@ -200,15 +206,15 @@
     rjson = json.loads(rdata.text)
 
     print(f"\nCertificate retrieved for network:\t{rjson['network']['id']}")
 
     return rjson
 
 
-def create_certificaties_files(location, creator, dry_run):
+def _create_certificaties_files(location, creator, dry_run):
     creator["ca"], creator["certificate"], creator["private_key"]
 
     if not dry_run:
         location.mkdir(exist_ok=True)
         try:
             with open(location / "ca.crt", "w") as file:
                 file.write(creator["ca"])
@@ -223,14 +229,19 @@
             exit(-3)
     else:
         print("\nDry-run: Fake Save done!")
     print(f"\nLocation of generated certificates:\t{location.absolute()}")
 
 
 def main():
+    """
+    Main logic of the program.
+
+    Parses the terminal argument, and execute the thereby given commands.
+    """
     global debug
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--dry_run",
         action='store_true',
         help="Run the Script, without making the files & folders.",
@@ -267,43 +278,43 @@
     args = parser.parse_args(sys.argv[1:])
 
     debug = args.debug if args.debug else False
 
     base_url = wappstoUrl[args.env]
 
     if not args.token:
-        session = start_session(
+        session = _start_session(
             base_url=base_url,
             username=input("Wappsto Username: "),
             password=getpass.getpass(prompt="Wappsto Password: "),
         )
     else:
         session = args.token
     if not args.recreate:
-        creator = create_network(
+        creator = _create_network(
             session=session,
             base_url=base_url,
             dry_run=args.dry_run
         )
-        claim_network(
+        _claim_network(
             session=session,
             base_url=base_url,
             network_uuid=creator.get('network', {}).get('id'),
             dry_run=args.dry_run
         )
     else:
-        creator = get_network(
+        creator = _get_network(
             session=session,
             base_url=base_url,
             network_uuid=args.recreate,
         )
 
     args.path.mkdir(exist_ok=True)
 
-    create_certificaties_files(args.path, creator, args.dry_run)
+    _create_certificaties_files(args.path, creator, args.dry_run)
 
     print("\nEnjoy...")
     exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `wappstoiot-0.6.5/wappstoiot/connections/protocol.py` & `wappstoiot-0.6.6/wappstoiot/connections/protocol.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot/connections/sslsocket.py` & `wappstoiot-0.6.6/wappstoiot/connections/sslsocket.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot/modules/device.py` & `wappstoiot-0.6.6/wappstoiot/modules/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -345,17 +345,19 @@
         mapping: Optional[Dict[str, str]] = None,
         meaningful_zero: Optional[bool] = None,
         ordered_mapping: Optional[bool] = None,
     ) -> Value:
         kwargs = locals()
         kwargs.pop('self')
 
-        if not name_check.legal_name(name):
+        illegal_chars: str = name_check.illegal_characters(name)
+
+        if illegal_chars:
             raise ValueError(
-                "Given name contain a ilegal character."
+                f"Given name contain a illegal character: {illegal_chars}"
                 f"May only contain: {name_check.wappsto_letters}"
             )
 
         value_uuid = self.connection.get_value_where(
             device_uuid=self.uuid,
             name=name
         )
@@ -381,17 +383,19 @@
         description: Optional[str] = None,
         period: Optional[int] = None,  # in Sec
         delta: Optional[Union[int, float]] = None,
     ) -> Value:
         kwargs = locals()
         kwargs.pop('self')
 
-        if not name_check.legal_name(name):
+        illegal_chars: str = name_check.illegal_characters(name)
+
+        if illegal_chars:
             raise ValueError(
-                "Given name contain a ilegal character."
+                f"Given name contain a illegal character: {illegal_chars}"
                 f"May only contain: {name_check.wappsto_letters}"
             )
 
         value_uuid = self.connection.get_value_where(
             device_uuid=self.uuid,
             name=name
         )
@@ -417,17 +421,19 @@
         description: Optional[str] = None,
         period: Optional[int] = None,  # in Sec
         delta: Optional[Union[int, float]] = None,
     ) -> Value:
         kwargs = locals()
         kwargs.pop('self')
 
-        if not name_check.legal_name(name):
+        illegal_chars: str = name_check.illegal_characters(name)
+
+        if illegal_chars:
             raise ValueError(
-                "Given name contain a ilegal character."
+                f"Given name contain a illegal character: {illegal_chars}"
                 f"May only contain: {name_check.wappsto_letters}"
             )
 
         value_uuid = self.connection.get_value_where(
             device_uuid=self.uuid,
             name=name
         )
@@ -453,17 +459,19 @@
         description: Optional[str] = None,
         period: Optional[int] = None,  # in Sec
         delta: Optional[Union[int, float]] = None,
     ) -> Value:
         kwargs = locals()
         kwargs.pop('self')
 
-        if not name_check.legal_name(name):
+        illegal_chars: str = name_check.illegal_characters(name)
+
+        if illegal_chars:
             raise ValueError(
-                "Given name contain a ilegal character."
+                f"Given name contain a illegal character: {illegal_chars}"
                 f"May only contain: {name_check.wappsto_letters}"
             )
 
         value_uuid = self.connection.get_value_where(
             device_uuid=self.uuid,
             name=name
         )
@@ -492,17 +500,19 @@
 
         If a value_type have been set, that means that the parameters like:
         name, permission, min, max, step, encoding & unit have been set
         for you, to be the right settings for the given type. But you can
         still change it, if you choose sow.
         """
 
-        if not name_check.legal_name(name):
+        illegal_chars: str = name_check.illegal_characters(name)
+
+        if illegal_chars:
             raise ValueError(
-                "Given name contain a ilegal character."
+                f"Given name contain a illegal character: {illegal_chars}"
                 f"May only contain: {name_check.wappsto_letters}"
             )
 
         value_uuid = self.connection.get_value_where(
             device_uuid=self.uuid,
             name=name
         )
```

### Comparing `wappstoiot-0.6.5/wappstoiot/modules/network.py` & `wappstoiot-0.6.6/wappstoiot/modules/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,17 +304,19 @@
 
         This could be a button that is connected to this unit,
         or in the case of this unit is a gateway, it could be a remote unit.
         """
         kwargs = locals()
         kwargs.pop('self')
 
-        if not name_check.legal_name(name):
+        illegal_chars: str = name_check.illegal_characters(name)
+
+        if illegal_chars:
             raise ValueError(
-                "Given name contain a ilegal character."
+                f"Given name contain a illegal character: {illegal_chars}"
                 f"May only contain: {name_check.wappsto_letters}"
             )
 
         device_uuid = self.connection.get_device_where(
             network_uuid=self.uuid,
             name=name
         )
```

### Comparing `wappstoiot-0.6.5/wappstoiot/modules/template.py` & `wappstoiot-0.6.6/wappstoiot/modules/template.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot/modules/value.py` & `wappstoiot-0.6.6/wappstoiot/modules/value.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,18 @@
     def getControlTimestamp(self) -> Optional[datetime]:
         """
         Returns the timestamp for when last Control value was updated.
 
         The returned timestamp will be the last time Control value was updated,
         unless there isn't one, then it will return None.
         """
-        return self.control_state.timestamp
+        if isinstance(self.control_state.timestamp, datetime):
+            return self.control_state.timestamp
+        if isinstance(self.control_state.timestamp, str):
+            return str_to_datetime(self.control_state.timestamp)
 
     def getReportData(self) -> Optional[Union[float, str]]:
         """
         Returns the last Report value.
 
         The returned value will be the last Report value.
         unless there isn't one, then it will return None.
@@ -222,15 +225,18 @@
     def getReportTimestamp(self) -> Optional[datetime]:
         """
         Returns the timestamp for when last Report value was updated.
 
         The returned timestamp will be the last time Control value was updated,
         unless there isn't one, then it will return None.
         """
-        return self.report_state.timestamp
+        if isinstance(self.report_state.timestamp, datetime):
+            return self.report_state.timestamp
+        if isinstance(self.report_state.timestamp, str):
+            return str_to_datetime(self.report_state.timestamp)
 
     @property
     def name(self) -> str:
         """Returns the name of the value."""
         return self.element.name
 
     @property
```

### Comparing `wappstoiot-0.6.5/wappstoiot/schema/base_schema.py` & `wappstoiot-0.6.6/wappstoiot/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot/schema/iot_schema.py` & `wappstoiot-0.6.6/wappstoiot/schema/iot_schema.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot/service/iot_api.py` & `wappstoiot-0.6.6/wappstoiot/service/iot_api.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot/service/template.py` & `wappstoiot-0.6.6/wappstoiot/service/template.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot/utils/Timestamp.py` & `wappstoiot-0.6.6/wappstoiot/utils/Timestamp.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot/utils/observer.py` & `wappstoiot-0.6.6/wappstoiot/utils/observer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Contain the Observer functionality.
+
+The Observer Pattern, is as design pattern, that 
+"""
 import logging
 import threading
 
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Callable
@@ -21,19 +26,19 @@
 
 def subscribe(event_name: str, callback: Callable[[str, Any], None]) -> None:
     """
     Subscribe to the event with given event name.
 
     Note: If lambda was used to subscribe with, it need to be the same
     instance that is used to unsubscribe with. So if it is needed to
-    unsubscibe, save the instance.
+    unsubscribe, save the instance.
 
     Args:
         event_name: The Unique name for the wanted event.
-        callback: The function that need triggeret on the given event.
+        callback: The function that need triggered on the given event.
             The function will be called with the 'event_name', and 'data',
             that the event generate.
     """
     obs_log.debug(f"New Subscriber: {event_name}, {callback}")
     if event_name not in subscriber:
         subscriber[event_name] = default_subscriber.copy()
     subscriber[event_name].append(callback)
@@ -61,20 +66,20 @@
     Unsubscribe from given event name.
 
     Note: if lambda was used to subscribe with, it need to be the same
     instance that is used to unsubscribe with.
 
     Args:
         event_name: The Unique name for the wanted event.
-        callback: The function that need triggeret on the given event.
+        callback: The function that need triggered on the given event.
             The function will be called with the 'event_name', and 'data',
             that the event generate.
 
     Returns:
-        True, is the function was removed from the subcriber list.
+        True, is the function was removed from the subscriber list.
         False, if it could not be, as in could not find it.
     """
     obs_log.debug(f"Unsubscribing: {event_name}, {callback}")
 
     try:
         # NOTE: Faster then testing if callback is in the list, when it is (60%+).
         subscriber.get(event_name, []).remove(callback)
```

### Comparing `wappstoiot-0.6.5/wappstoiot/utils/offline_storage.py` & `wappstoiot-0.6.6/wappstoiot/utils/offline_storage.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot/utils/tracer.py` & `wappstoiot-0.6.6/wappstoiot/utils/tracer.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.5/wappstoiot.egg-info/PKG-INFO` & `wappstoiot-0.6.6/wappstoiot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: wappstoiot
-Version: 0.6.5
+Version: 0.6.6
 Summary: Simple Wappsto Python user-interface to Wappsto IoT
 Home-page: https://github.com/Wappsto/python-wappsto-iot
 Author: Seluxit A/S
 Author-email: support@seluxit.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Wappsto IoT
 ===============================================================================
 
-[![Build Status](https://travis-ci.com/Wappsto/python-wappsto-iot.svg?branch=master)](https://travis-ci.com/Wappsto/python-wappsto-iot)
-[![Coverage Status](https://coveralls.io/repos/github/Wappsto/python-wappsto-iot/badge.svg?branch=master)](https://coveralls.io/github/Wappsto/python-wappsto-iot?branch=master)
+[![python](https://img.shields.io/badge/Python-3.6%203.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
+[![Test Status](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/test.yml/badge.svg)](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/test.yml)
+[![Lint Status](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/lint.yml/badge.svg)](https://github.com/Wappsto/python-wappsto-iot/actions/workflows/lint.yml)
+[![Coverage](https://codecov.io/github/wappsto/python-wappsto-iot/branch/main/graph/badge.svg)](https://codecov.io/github/wappsto/python-wappsto-iot)
 
 The wappstoiot module provide a simple python interface to [wappsto.com](https://wappsto.com/) for easy prototyping.
 
 
 ## Prerequisites
 
 A [wappsto.com](https://wappsto.com/) Account, that the unit can connect to.
@@ -57,15 +59,15 @@
 
 
 Working examples of usage can be found in the [example folder](./example).
 
 The needed certificates can be downloaded with: `python -m wappstoiot --path echo`
 Where path is the path to the config-folder, given in the following code example.
 
-There is also a Wapp avaliable called: [IoT Certificate Manager](https://wappsto.com/store/wapp=iot_certificate_manager) on wappsto,
+There is also a Wapp avaliable called: [IoT Certificate Manager](https://wappsto.com/store/application/iot_certificate_manager) on wappsto,
 that given you a GUI to do the same and more.
 
 ### Echo example
 
 The following explains the example code found in [echo.py](./example/echo.py).
 
 
@@ -119,14 +121,25 @@
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details.
 
 
 
+v0.6.6 (Jun 22 2023)
+===============================================================================
+## Added
+ * Code Stub.
+
+## Changed
+ * Now inform which characters are illegal in the given name.
+
+## Fixed
+ * The `getReportTimestamp` & `getControlTimestamp` now ensures the return is `None` or of type datetime.
+
 v0.6.5 (Feb 28 2023)
 ===============================================================================
 ## Fixed
  * Report & Control now generate a timestamp in UTC time.
 
 v0.6.4 (Feb 27 2023)
 ===============================================================================
```

### Comparing `wappstoiot-0.6.5/wappstoiot.egg-info/SOURCES.txt` & `wappstoiot-0.6.6/wappstoiot.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,58 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 test/test_real_world.py
 wappstoiot/__init__.py
+wappstoiot/__init__.pyi
 wappstoiot/__main__.py
+wappstoiot/__main__.pyi
+wappstoiot/py.typed
 wappstoiot.egg-info/PKG-INFO
 wappstoiot.egg-info/SOURCES.txt
 wappstoiot.egg-info/dependency_links.txt
 wappstoiot.egg-info/requires.txt
 wappstoiot.egg-info/top_level.txt
 wappstoiot/connections/__init__.py
+wappstoiot/connections/__init__.pyi
 wappstoiot/connections/protocol.py
+wappstoiot/connections/protocol.pyi
 wappstoiot/connections/sslsocket.py
+wappstoiot/connections/sslsocket.pyi
 wappstoiot/modules/__init__.py
+wappstoiot/modules/__init__.pyi
 wappstoiot/modules/device.py
+wappstoiot/modules/device.pyi
 wappstoiot/modules/network.py
+wappstoiot/modules/network.pyi
 wappstoiot/modules/template.py
+wappstoiot/modules/template.pyi
 wappstoiot/modules/value.py
+wappstoiot/modules/value.pyi
 wappstoiot/schema/__init__.py
+wappstoiot/schema/__init__.pyi
 wappstoiot/schema/base_schema.py
+wappstoiot/schema/base_schema.pyi
 wappstoiot/schema/iot_schema.py
+wappstoiot/schema/iot_schema.pyi
 wappstoiot/service/__init__.py
+wappstoiot/service/__init__.pyi
 wappstoiot/service/iot_api.py
+wappstoiot/service/iot_api.pyi
 wappstoiot/service/template.py
+wappstoiot/service/template.pyi
 wappstoiot/utils/Timestamp.py
+wappstoiot/utils/Timestamp.pyi
 wappstoiot/utils/__init__.py
+wappstoiot/utils/__init__.pyi
 wappstoiot/utils/certificateread.py
+wappstoiot/utils/certificateread.pyi
 wappstoiot/utils/name_check.py
+wappstoiot/utils/name_check.pyi
 wappstoiot/utils/observer.py
+wappstoiot/utils/observer.pyi
 wappstoiot/utils/offline_storage.py
-wappstoiot/utils/tracer.py
+wappstoiot/utils/offline_storage.pyi
+wappstoiot/utils/tracer.py
+wappstoiot/utils/tracer.pyi
```

