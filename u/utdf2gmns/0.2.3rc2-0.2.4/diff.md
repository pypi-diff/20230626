# Comparing `tmp/utdf2gmns-0.2.3rc2.tar.gz` & `tmp/utdf2gmns-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utdf2gmns-0.2.3rc2.tar", last modified: Mon Jun 26 17:38:29 2023, max compression
+gzip compressed data, was "utdf2gmns-0.2.4.tar", last modified: Mon Jun 26 17:41:47 2023, max compression
```

## Comparing `utdf2gmns-0.2.3rc2.tar` & `utdf2gmns-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 17:38:29.048713 utdf2gmns-0.2.3rc2/
--rw-rw-rw-   0        0        0    11558 2022-12-19 22:02:10.000000 utdf2gmns-0.2.3rc2/LICENSE
--rw-rw-rw-   0        0        0     5432 2023-06-26 17:38:29.046717 utdf2gmns-0.2.3rc2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-26 17:38:29.048713 utdf2gmns-0.2.3rc2/setup.cfg
--rw-rw-rw-   0        0        0     1494 2023-06-26 17:37:59.000000 utdf2gmns-0.2.3rc2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:38:28.979713 utdf2gmns-0.2.3rc2/utdf2gmns/
--rw-rw-rw-   0        0        0     1155 2023-06-26 03:03:50.000000 utdf2gmns-0.2.3rc2/utdf2gmns/__init__.py
--rw-rw-rw-   0        0        0     9196 2023-06-26 02:03:52.000000 utdf2gmns-0.2.3rc2/utdf2gmns/__utdf2gmns.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:38:29.034715 utdf2gmns-0.2.3rc2/utdf2gmns/func_lib/
--rw-rw-rw-   0        0        0      277 2023-06-24 00:46:51.000000 utdf2gmns-0.2.3rc2/utdf2gmns/func_lib/__init__.py
--rw-rw-rw-   0        0        0     6379 2023-06-26 02:22:27.000000 utdf2gmns-0.2.3rc2/utdf2gmns/func_lib/geocoding_intersection.py
--rw-rw-rw-   0        0        0     7462 2023-06-26 02:25:19.000000 utdf2gmns-0.2.3rc2/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py
--rw-rw-rw-   0        0        0    11276 2023-06-26 02:07:54.000000 utdf2gmns-0.2.3rc2/utdf2gmns/func_lib/read_utdf.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:38:29.043713 utdf2gmns-0.2.3rc2/utdf2gmns/utils_lib/
--rw-rw-rw-   0        0        0      278 2023-03-07 10:13:11.000000 utdf2gmns-0.2.3rc2/utdf2gmns/utils_lib/__init__.py
--rw-rw-rw-   0        0        0     3356 2023-06-26 02:02:58.000000 utdf2gmns-0.2.3rc2/utdf2gmns/utils_lib/package_settings.py
--rw-rw-rw-   0        0        0     5794 2023-03-14 01:43:28.000000 utdf2gmns-0.2.3rc2/utdf2gmns/utils_lib/utility_lib.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:38:29.022718 utdf2gmns-0.2.3rc2/utdf2gmns.egg-info/
--rw-rw-rw-   0        0        0     5432 2023-06-26 17:38:28.000000 utdf2gmns-0.2.3rc2/utdf2gmns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-06-26 17:38:28.000000 utdf2gmns-0.2.3rc2/utdf2gmns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 17:38:28.000000 utdf2gmns-0.2.3rc2/utdf2gmns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-26 17:38:28.000000 utdf2gmns-0.2.3rc2/utdf2gmns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 17:38:28.000000 utdf2gmns-0.2.3rc2/utdf2gmns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 17:41:47.091031 utdf2gmns-0.2.4/
+-rw-rw-rw-   0        0        0    11558 2022-12-19 22:02:10.000000 utdf2gmns-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     5429 2023-06-26 17:41:47.089032 utdf2gmns-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-26 17:41:47.091031 utdf2gmns-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1489 2023-06-26 17:40:33.000000 utdf2gmns-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:41:47.039031 utdf2gmns-0.2.4/utdf2gmns/
+-rw-rw-rw-   0        0        0     1155 2023-06-26 17:40:57.000000 utdf2gmns-0.2.4/utdf2gmns/__init__.py
+-rw-rw-rw-   0        0        0     9196 2023-06-26 02:03:52.000000 utdf2gmns-0.2.4/utdf2gmns/__utdf2gmns.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:41:47.078030 utdf2gmns-0.2.4/utdf2gmns/func_lib/
+-rw-rw-rw-   0        0        0      277 2023-06-24 00:46:51.000000 utdf2gmns-0.2.4/utdf2gmns/func_lib/__init__.py
+-rw-rw-rw-   0        0        0     6379 2023-06-26 02:22:27.000000 utdf2gmns-0.2.4/utdf2gmns/func_lib/geocoding_intersection.py
+-rw-rw-rw-   0        0        0     7462 2023-06-26 02:25:19.000000 utdf2gmns-0.2.4/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py
+-rw-rw-rw-   0        0        0    11276 2023-06-26 02:07:54.000000 utdf2gmns-0.2.4/utdf2gmns/func_lib/read_utdf.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:41:47.086029 utdf2gmns-0.2.4/utdf2gmns/utils_lib/
+-rw-rw-rw-   0        0        0      278 2023-03-07 10:13:11.000000 utdf2gmns-0.2.4/utdf2gmns/utils_lib/__init__.py
+-rw-rw-rw-   0        0        0     3356 2023-06-26 02:02:58.000000 utdf2gmns-0.2.4/utdf2gmns/utils_lib/package_settings.py
+-rw-rw-rw-   0        0        0     5794 2023-03-14 01:43:28.000000 utdf2gmns-0.2.4/utdf2gmns/utils_lib/utility_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:41:47.066029 utdf2gmns-0.2.4/utdf2gmns.egg-info/
+-rw-rw-rw-   0        0        0     5429 2023-06-26 17:41:46.000000 utdf2gmns-0.2.4/utdf2gmns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-06-26 17:41:46.000000 utdf2gmns-0.2.4/utdf2gmns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 17:41:46.000000 utdf2gmns-0.2.4/utdf2gmns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-26 17:41:46.000000 utdf2gmns-0.2.4/utdf2gmns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 17:41:46.000000 utdf2gmns-0.2.4/utdf2gmns.egg-info/top_level.txt
```

### Comparing `utdf2gmns-0.2.3rc2/LICENSE` & `utdf2gmns-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `utdf2gmns-0.2.3rc2/PKG-INFO` & `utdf2gmns-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utdf2gmns
-Version: 0.2.3rc2
+Version: 0.2.4
 Summary: This open-source package is a tool to convert utdf file to GMNS format.
 Home-page: https://github.com/asu-trans-ai-lab/utdf2gmns
 Author: Xiangyong Luo, Dr.Xuesong (Simon) Zhou
 Author-email: luoxiangyong01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `utdf2gmns-0.2.3rc2/setup.py` & `utdf2gmns-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in f.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="utdf2gmns",  # Replace with your own username
-    version="0.2.3 rc02",
+    version="0.2.4",
     author="Xiangyong Luo, Dr.Xuesong (Simon) Zhou",
     author_email="luoxiangyong01@gmail.com",
     description="This open-source package is a tool to convert utdf file to GMNS format.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/asu-trans-ai-lab/utdf2gmns",
```

### Comparing `utdf2gmns-0.2.3rc2/utdf2gmns/__init__.py` & `utdf2gmns-0.2.4/utdf2gmns/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
            'match_intersection_node',
            'match_movement_and_intersection_node',
            'match_movement_utdf_lane',
            'match_movement_utdf_phase_timeplans',
            'package_settings'
            ]
 
-print("UTDF2GMNS Version: ", "0.2.3")
+print("utdf2gmns version: ", "0.2.4")
```

### Comparing `utdf2gmns-0.2.3rc2/utdf2gmns/__utdf2gmns.py` & `utdf2gmns-0.2.4/utdf2gmns/__utdf2gmns.py`

 * *Files identical despite different names*

### Comparing `utdf2gmns-0.2.3rc2/utdf2gmns/func_lib/geocoding_intersection.py` & `utdf2gmns-0.2.4/utdf2gmns/func_lib/geocoding_intersection.py`

 * *Files identical despite different names*

### Comparing `utdf2gmns-0.2.3rc2/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py` & `utdf2gmns-0.2.4/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py`

 * *Files identical despite different names*

### Comparing `utdf2gmns-0.2.3rc2/utdf2gmns/func_lib/read_utdf.py` & `utdf2gmns-0.2.4/utdf2gmns/func_lib/read_utdf.py`

 * *Files identical despite different names*

### Comparing `utdf2gmns-0.2.3rc2/utdf2gmns/utils_lib/package_settings.py` & `utdf2gmns-0.2.4/utdf2gmns/utils_lib/package_settings.py`

 * *Files identical despite different names*

### Comparing `utdf2gmns-0.2.3rc2/utdf2gmns/utils_lib/utility_lib.py` & `utdf2gmns-0.2.4/utdf2gmns/utils_lib/utility_lib.py`

 * *Files identical despite different names*

### Comparing `utdf2gmns-0.2.3rc2/utdf2gmns.egg-info/PKG-INFO` & `utdf2gmns-0.2.4/utdf2gmns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utdf2gmns
-Version: 0.2.3rc2
+Version: 0.2.4
 Summary: This open-source package is a tool to convert utdf file to GMNS format.
 Home-page: https://github.com/asu-trans-ai-lab/utdf2gmns
 Author: Xiangyong Luo, Dr.Xuesong (Simon) Zhou
 Author-email: luoxiangyong01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

