# Comparing `tmp/CADPR-0.1.0.tar.gz` & `tmp/CADPR-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CADPR-0.1.0.tar", last modified: Wed Apr  5 22:05:10 2023, max compression
+gzip compressed data, was "CADPR-0.1.1.tar", last modified: Mon Apr 10 16:45:28 2023, max compression
```

## Comparing `CADPR-0.1.0.tar` & `CADPR-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-05 22:05:10.635559 CADPR-0.1.0/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 CADPR-0.1.0/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18045 2023-04-05 22:05:10.635080 CADPR-0.1.0/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 CADPR-0.1.0/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-05 22:05:10.635727 CADPR-0.1.0/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2234 2023-04-05 22:04:27.000000 CADPR-0.1.0/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-05 22:05:10.631425 CADPR-0.1.0/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-05 22:05:10.634263 CADPR-0.1.0/src/CADPR.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18045 2023-04-05 22:05:10.000000 CADPR-0.1.0/src/CADPR.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      401 2023-04-05 22:05:10.000000 CADPR-0.1.0/src/CADPR.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-05 22:05:10.000000 CADPR-0.1.0/src/CADPR.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-05 22:05:10.000000 CADPR-0.1.0/src/CADPR.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      134 2023-04-05 22:05:10.000000 CADPR-0.1.0/src/CADPR.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     9133 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19846 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     8728 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3710 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/_IMPSummaryDashboard.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13952 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6490 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7240 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-05 17:14:16.000000 CADPR-0.1.0/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 16:45:28.874560 CADPR-0.1.1/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 CADPR-0.1.1/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18045 2023-04-10 16:45:28.874052 CADPR-0.1.1/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 CADPR-0.1.1/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-10 16:45:28.874725 CADPR-0.1.1/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2252 2023-04-10 16:41:41.000000 CADPR-0.1.1/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 16:45:28.870559 CADPR-0.1.1/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 16:45:28.873405 CADPR-0.1.1/src/CADPR.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18045 2023-04-10 16:45:28.000000 CADPR-0.1.1/src/CADPR.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      421 2023-04-10 16:45:28.000000 CADPR-0.1.1/src/CADPR.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-10 16:45:28.000000 CADPR-0.1.1/src/CADPR.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-10 16:45:28.000000 CADPR-0.1.1/src/CADPR.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      147 2023-04-10 16:45:28.000000 CADPR-0.1.1/src/CADPR.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19846 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3710 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/_IMPSummaryDashboard.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3205 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13952 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6490 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7240 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-10 16:40:29.000000 CADPR-0.1.1/src/__init__.py
```

### Comparing `CADPR-0.1.0/LICENSE` & `CADPR-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CADPR-0.1.0/PKG-INFO` & `CADPR-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CADPR
-Version: 0.1.0
+Version: 0.1.1
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CADPR-0.1.0/README.md` & `CADPR-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `CADPR-0.1.0/setup.py` & `CADPR-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='CADPR',
-	version='0.1.0',
+	version='0.1.1',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"_IMPSummaryDashboard",
+		"_SearchFiles",
 		"_SnowflakeDependencies",
 		"_SnowflakePull",
 		"NikeQA",
 		"_QA",
 		"_GitHub",
 		"NikeCA"
 	],
```

### Comparing `CADPR-0.1.0/src/CADPR.egg-info/PKG-INFO` & `CADPR-0.1.1/src/CADPR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CADPR
-Version: 0.1.0
+Version: 0.1.1
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CADPR-0.1.0/src/CADPR.egg-info/requires.txt` & `CADPR-0.1.1/src/CADPR.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `CADPR-0.1.0/src/NikeSF.py` & `CADPR-0.1.1/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `CADPR-0.1.0/src/_BuildSearchQuery.py` & `CADPR-0.1.1/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `CADPR-0.1.0/src/_IMPSummaryDashboard.py` & `CADPR-0.1.1/src/_IMPSummaryDashboard.py`

 * *Files identical despite different names*

### Comparing `CADPR-0.1.0/src/_QA.py` & `CADPR-0.1.1/src/_QA.py`

 * *Files identical despite different names*

### Comparing `CADPR-0.1.0/src/_SnowflakeData.py` & `CADPR-0.1.1/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `CADPR-0.1.0/src/_SnowflakeDependencies.py` & `CADPR-0.1.1/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `CADPR-0.1.0/src/_SnowflakePull.py` & `CADPR-0.1.1/src/_SnowflakePull.py`

 * *Files identical despite different names*

