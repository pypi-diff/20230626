# Comparing `tmp/UTDF2GMNS-0.2.2.tar.gz` & `tmp/utdf2gmns-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UTDF2GMNS-0.2.2.tar", last modified: Mon Jun 26 02:43:39 2023, max compression
+gzip compressed data, was "utdf2gmns-0.2.3.tar", last modified: Mon Jun 26 03:04:33 2023, max compression
```

## Comparing `UTDF2GMNS-0.2.2.tar` & `utdf2gmns-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 02:43:39.039786 UTDF2GMNS-0.2.2/
--rw-rw-rw-   0        0        0    11558 2022-12-19 22:02:10.000000 UTDF2GMNS-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4336 2023-06-26 02:43:39.039786 UTDF2GMNS-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3813 2023-06-26 02:41:31.000000 UTDF2GMNS-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 02:43:39.012617 UTDF2GMNS-0.2.2/UTDF2GMNS.egg-info/
--rw-rw-rw-   0        0        0     4336 2023-06-26 02:43:38.000000 UTDF2GMNS-0.2.2/UTDF2GMNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-26 02:43:38.000000 UTDF2GMNS-0.2.2/UTDF2GMNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 02:43:38.000000 UTDF2GMNS-0.2.2/UTDF2GMNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-26 02:43:38.000000 UTDF2GMNS-0.2.2/UTDF2GMNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 02:43:38.000000 UTDF2GMNS-0.2.2/UTDF2GMNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 02:43:39.039786 UTDF2GMNS-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1489 2023-06-26 02:42:29.000000 UTDF2GMNS-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:43:39.017607 UTDF2GMNS-0.2.2/utdf2gmns/
--rw-rw-rw-   0        0        0     1155 2023-06-26 02:42:18.000000 UTDF2GMNS-0.2.2/utdf2gmns/__init__.py
--rw-rw-rw-   0        0        0     9196 2023-06-26 02:03:52.000000 UTDF2GMNS-0.2.2/utdf2gmns/__utdf2gmns.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:43:39.030750 UTDF2GMNS-0.2.2/utdf2gmns/func_lib/
--rw-rw-rw-   0        0        0      277 2023-06-24 00:46:51.000000 UTDF2GMNS-0.2.2/utdf2gmns/func_lib/__init__.py
--rw-rw-rw-   0        0        0     6379 2023-06-26 02:22:27.000000 UTDF2GMNS-0.2.2/utdf2gmns/func_lib/geocoding_intersection.py
--rw-rw-rw-   0        0        0     7462 2023-06-26 02:25:19.000000 UTDF2GMNS-0.2.2/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py
--rw-rw-rw-   0        0        0    11276 2023-06-26 02:07:54.000000 UTDF2GMNS-0.2.2/utdf2gmns/func_lib/read_utdf.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:43:39.038539 UTDF2GMNS-0.2.2/utdf2gmns/utils_lib/
--rw-rw-rw-   0        0        0      278 2023-03-07 10:13:11.000000 UTDF2GMNS-0.2.2/utdf2gmns/utils_lib/__init__.py
--rw-rw-rw-   0        0        0     3356 2023-06-26 02:02:58.000000 UTDF2GMNS-0.2.2/utdf2gmns/utils_lib/package_settings.py
--rw-rw-rw-   0        0        0     5794 2023-03-14 01:43:28.000000 UTDF2GMNS-0.2.2/utdf2gmns/utils_lib/utility_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:04:33.980224 utdf2gmns-0.2.3/
+-rw-rw-rw-   0        0        0    11558 2022-12-19 22:02:10.000000 utdf2gmns-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     4341 2023-06-26 03:04:33.978224 utdf2gmns-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-26 03:04:33.980224 utdf2gmns-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1489 2023-06-26 03:03:36.000000 utdf2gmns-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:04:33.918113 utdf2gmns-0.2.3/utdf2gmns/
+-rw-rw-rw-   0        0        0     1155 2023-06-26 03:03:50.000000 utdf2gmns-0.2.3/utdf2gmns/__init__.py
+-rw-rw-rw-   0        0        0     9196 2023-06-26 02:03:52.000000 utdf2gmns-0.2.3/utdf2gmns/__utdf2gmns.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:04:33.967223 utdf2gmns-0.2.3/utdf2gmns/func_lib/
+-rw-rw-rw-   0        0        0      277 2023-06-24 00:46:51.000000 utdf2gmns-0.2.3/utdf2gmns/func_lib/__init__.py
+-rw-rw-rw-   0        0        0     6379 2023-06-26 02:22:27.000000 utdf2gmns-0.2.3/utdf2gmns/func_lib/geocoding_intersection.py
+-rw-rw-rw-   0        0        0     7462 2023-06-26 02:25:19.000000 utdf2gmns-0.2.3/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py
+-rw-rw-rw-   0        0        0    11276 2023-06-26 02:07:54.000000 utdf2gmns-0.2.3/utdf2gmns/func_lib/read_utdf.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:04:33.973663 utdf2gmns-0.2.3/utdf2gmns/utils_lib/
+-rw-rw-rw-   0        0        0      278 2023-03-07 10:13:11.000000 utdf2gmns-0.2.3/utdf2gmns/utils_lib/__init__.py
+-rw-rw-rw-   0        0        0     3356 2023-06-26 02:02:58.000000 utdf2gmns-0.2.3/utdf2gmns/utils_lib/package_settings.py
+-rw-rw-rw-   0        0        0     5794 2023-03-14 01:43:28.000000 utdf2gmns-0.2.3/utdf2gmns/utils_lib/utility_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:04:33.954869 utdf2gmns-0.2.3/utdf2gmns.egg-info/
+-rw-rw-rw-   0        0        0     4341 2023-06-26 03:04:33.000000 utdf2gmns-0.2.3/utdf2gmns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-06-26 03:04:33.000000 utdf2gmns-0.2.3/utdf2gmns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 03:04:33.000000 utdf2gmns-0.2.3/utdf2gmns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-26 03:04:33.000000 utdf2gmns-0.2.3/utdf2gmns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 03:04:33.000000 utdf2gmns-0.2.3/utdf2gmns.egg-info/top_level.txt
```

### Comparing `UTDF2GMNS-0.2.2/LICENSE` & `utdf2gmns-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.2/PKG-INFO` & `utdf2gmns-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
-Name: UTDF2GMNS
-Version: 0.2.2
+Name: utdf2gmns
+Version: 0.2.3
 Summary: This open-source package is a tool to convert utdf file to GMNS format.
 Home-page: https://github.com/asu-trans-ai-lab/utdf2gmns
 Author: Xiangyong Luo, Dr.Xuesong (Simon) Zhou
 Author-email: luoxiangyong01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## utdf2gmns: Introduction
+## utdf2gmns
+
+## Introduction
 
 This open-source package is a tool to convert utdf file to GMNS format.
 
 ## Required Data Input Files:
 
 * [X] UTDF.csv
 * [X] node.csv (GMNS format)
```

### Comparing `UTDF2GMNS-0.2.2/README.md` & `utdf2gmns-0.2.3/utdf2gmns.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,24 @@
-## utdf2gmns: Introduction
+Metadata-Version: 2.1
+Name: utdf2gmns
+Version: 0.2.3
+Summary: This open-source package is a tool to convert utdf file to GMNS format.
+Home-page: https://github.com/asu-trans-ai-lab/utdf2gmns
+Author: Xiangyong Luo, Dr.Xuesong (Simon) Zhou
+Author-email: luoxiangyong01@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## utdf2gmns
+
+## Introduction
 
 This open-source package is a tool to convert utdf file to GMNS format.
 
 ## Required Data Input Files:
 
 * [X] UTDF.csv
 * [X] node.csv (GMNS format)
```

### Comparing `UTDF2GMNS-0.2.2/setup.py` & `utdf2gmns-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # Contact Info: luoxiangyong01@gmail.com
 # Author/Copyright: Mr. Xiangyong Luo
 ##############################################################
 
 
 import setuptools
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open("Readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 try:
     # if have requirements.txt file inside the folder
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in f.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
-    name="UTDF2GMNS",  # Replace with your own username
-    version="0.2.2",
+    name="utdf2gmns",  # Replace with your own username
+    version="0.2.3",
     author="Xiangyong Luo, Dr.Xuesong (Simon) Zhou",
     author_email="luoxiangyong01@gmail.com",
     description="This open-source package is a tool to convert utdf file to GMNS format.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/asu-trans-ai-lab/utdf2gmns",
```

### Comparing `UTDF2GMNS-0.2.2/utdf2gmns/__init__.py` & `utdf2gmns-0.2.3/utdf2gmns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
            'match_intersection_node',
            'match_movement_and_intersection_node',
            'match_movement_utdf_lane',
            'match_movement_utdf_phase_timeplans',
            'package_settings'
            ]
 
-print("UTDF2GMNS Version: ", "0.2.2")
+print("UTDF2GMNS Version: ", "0.2.3")
```

### Comparing `UTDF2GMNS-0.2.2/utdf2gmns/__utdf2gmns.py` & `utdf2gmns-0.2.3/utdf2gmns/__utdf2gmns.py`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.2/utdf2gmns/func_lib/geocoding_intersection.py` & `utdf2gmns-0.2.3/utdf2gmns/func_lib/geocoding_intersection.py`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.2/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py` & `utdf2gmns-0.2.3/utdf2gmns/func_lib/match_node_intersection_movement_utdf.py`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.2/utdf2gmns/func_lib/read_utdf.py` & `utdf2gmns-0.2.3/utdf2gmns/func_lib/read_utdf.py`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.2/utdf2gmns/utils_lib/package_settings.py` & `utdf2gmns-0.2.3/utdf2gmns/utils_lib/package_settings.py`

 * *Files identical despite different names*

### Comparing `UTDF2GMNS-0.2.2/utdf2gmns/utils_lib/utility_lib.py` & `utdf2gmns-0.2.3/utdf2gmns/utils_lib/utility_lib.py`

 * *Files identical despite different names*

