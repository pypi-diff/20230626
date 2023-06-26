# Comparing `tmp/Hanalytics_python_package-0.2.tar.gz` & `tmp/Hanalytics_python_package-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hanalytics_python_package-0.2.tar", last modified: Fri Jun 23 18:34:43 2023, max compression
+gzip compressed data, was "Hanalytics_python_package-0.3.tar", last modified: Mon Jun 26 10:12:00 2023, max compression
```

## Comparing `Hanalytics_python_package-0.2.tar` & `Hanalytics_python_package-0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-23 18:34:43.887825 Hanalytics_python_package-0.2/
-drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-23 18:34:43.884679 Hanalytics_python_package-0.2/Hanalytics_python_package.egg-info/
--rw-r--r--   0 gasyd      (502) staff       (20)      211 2023-06-23 18:34:43.000000 Hanalytics_python_package-0.2/Hanalytics_python_package.egg-info/PKG-INFO
--rw-r--r--   0 gasyd      (502) staff       (20)      617 2023-06-23 18:34:43.000000 Hanalytics_python_package-0.2/Hanalytics_python_package.egg-info/SOURCES.txt
--rw-r--r--   0 gasyd      (502) staff       (20)        1 2023-06-23 18:34:43.000000 Hanalytics_python_package-0.2/Hanalytics_python_package.egg-info/dependency_links.txt
--rw-r--r--   0 gasyd      (502) staff       (20)       93 2023-06-23 18:34:43.000000 Hanalytics_python_package-0.2/Hanalytics_python_package.egg-info/requires.txt
--rw-r--r--   0 gasyd      (502) staff       (20)       92 2023-06-23 18:34:43.000000 Hanalytics_python_package-0.2/Hanalytics_python_package.egg-info/top_level.txt
--rw-r--r--   0 gasyd      (502) staff       (20)      211 2023-06-23 18:34:43.887581 Hanalytics_python_package-0.2/PKG-INFO
--rw-r--r--   0 gasyd      (502) staff       (20)       20 2023-06-13 13:01:13.000000 Hanalytics_python_package-0.2/README.md
-drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-23 18:34:43.883295 Hanalytics_python_package-0.2/hanalytics/
-drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-23 18:34:43.885231 Hanalytics_python_package-0.2/hanalytics/hanalytics_ga4/
--rw-r--r--   0 gasyd      (502) staff       (20)        0 2023-06-23 17:43:16.000000 Hanalytics_python_package-0.2/hanalytics/hanalytics_ga4/__init__.py
--rw-r--r--   0 gasyd      (502) staff       (20)     1224 2023-06-23 17:43:22.000000 Hanalytics_python_package-0.2/hanalytics/hanalytics_ga4/connectga4.py
--rw-r--r--   0 gasyd      (502) staff       (20)     9001 2023-06-23 17:43:27.000000 Hanalytics_python_package-0.2/hanalytics/hanalytics_ga4/tools.py
-drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-23 18:34:43.885526 Hanalytics_python_package-0.2/hanalytics/hanalytics_keywords_generator/
--rw-r--r--   0 gasyd      (502) staff       (20)     6780 2023-06-23 17:27:05.000000 Hanalytics_python_package-0.2/hanalytics/hanalytics_keywords_generator/googleAds_keywords.py
-drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-23 18:34:43.887171 Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/
--rw-r--r--   0 gasyd      (502) staff       (20)        0 2023-06-23 09:16:04.000000 Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/__init__.py
--rw-r--r--   0 gasyd      (502) staff       (20)     1728 2023-06-23 18:02:50.000000 Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/connect.py
--rw-r--r--   0 gasyd      (502) staff       (20)     2862 2023-06-23 11:06:42.000000 Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/customs.py
--rw-r--r--   0 gasyd      (502) staff       (20)    25386 2023-06-23 17:43:06.000000 Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/query.py
--rw-r--r--   0 gasyd      (502) staff       (20)     9694 2023-06-23 17:43:12.000000 Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/reports.py
--rw-r--r--   0 gasyd      (502) staff       (20)       38 2023-06-23 18:34:43.887890 Hanalytics_python_package-0.2/setup.cfg
--rw-r--r--   0 gasyd      (502) staff       (20)      439 2023-06-23 18:34:38.000000 Hanalytics_python_package-0.2/setup.py
+drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-26 10:12:00.090194 Hanalytics_python_package-0.3/
+drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-26 10:12:00.087250 Hanalytics_python_package-0.3/Hanalytics_python_package.egg-info/
+-rw-r--r--   0 gasyd      (502) staff       (20)      211 2023-06-26 10:12:00.000000 Hanalytics_python_package-0.3/Hanalytics_python_package.egg-info/PKG-INFO
+-rw-r--r--   0 gasyd      (502) staff       (20)      617 2023-06-26 10:12:00.000000 Hanalytics_python_package-0.3/Hanalytics_python_package.egg-info/SOURCES.txt
+-rw-r--r--   0 gasyd      (502) staff       (20)        1 2023-06-26 10:12:00.000000 Hanalytics_python_package-0.3/Hanalytics_python_package.egg-info/dependency_links.txt
+-rw-r--r--   0 gasyd      (502) staff       (20)      101 2023-06-26 10:12:00.000000 Hanalytics_python_package-0.3/Hanalytics_python_package.egg-info/requires.txt
+-rw-r--r--   0 gasyd      (502) staff       (20)       92 2023-06-26 10:12:00.000000 Hanalytics_python_package-0.3/Hanalytics_python_package.egg-info/top_level.txt
+-rw-r--r--   0 gasyd      (502) staff       (20)      211 2023-06-26 10:12:00.090028 Hanalytics_python_package-0.3/PKG-INFO
+-rw-r--r--   0 gasyd      (502) staff       (20)       20 2023-06-13 13:01:13.000000 Hanalytics_python_package-0.3/README.md
+drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-26 10:12:00.085911 Hanalytics_python_package-0.3/hanalytics/
+drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-26 10:12:00.087795 Hanalytics_python_package-0.3/hanalytics/hanalytics_ga4/
+-rw-r--r--   0 gasyd      (502) staff       (20)        0 2023-06-23 17:43:16.000000 Hanalytics_python_package-0.3/hanalytics/hanalytics_ga4/__init__.py
+-rw-r--r--   0 gasyd      (502) staff       (20)     1224 2023-06-23 17:43:22.000000 Hanalytics_python_package-0.3/hanalytics/hanalytics_ga4/connectga4.py
+-rw-r--r--   0 gasyd      (502) staff       (20)     9001 2023-06-23 17:43:27.000000 Hanalytics_python_package-0.3/hanalytics/hanalytics_ga4/tools.py
+drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-26 10:12:00.088097 Hanalytics_python_package-0.3/hanalytics/hanalytics_keywords_generator/
+-rw-r--r--   0 gasyd      (502) staff       (20)     6780 2023-06-23 17:27:05.000000 Hanalytics_python_package-0.3/hanalytics/hanalytics_keywords_generator/googleAds_keywords.py
+drwxr-xr-x   0 gasyd      (502) staff       (20)        0 2023-06-26 10:12:00.089619 Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/
+-rw-r--r--   0 gasyd      (502) staff       (20)        0 2023-06-23 09:16:04.000000 Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/__init__.py
+-rw-r--r--   0 gasyd      (502) staff       (20)     1728 2023-06-23 18:02:50.000000 Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/connect.py
+-rw-r--r--   0 gasyd      (502) staff       (20)     2862 2023-06-23 11:06:42.000000 Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/customs.py
+-rw-r--r--   0 gasyd      (502) staff       (20)    25386 2023-06-23 17:43:06.000000 Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/query.py
+-rw-r--r--   0 gasyd      (502) staff       (20)     9694 2023-06-23 17:43:12.000000 Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/reports.py
+-rw-r--r--   0 gasyd      (502) staff       (20)       38 2023-06-26 10:12:00.090239 Hanalytics_python_package-0.3/setup.cfg
+-rw-r--r--   0 gasyd      (502) staff       (20)      447 2023-06-26 10:10:10.000000 Hanalytics_python_package-0.3/setup.py
```

### Comparing `Hanalytics_python_package-0.2/Hanalytics_python_package.egg-info/SOURCES.txt` & `Hanalytics_python_package-0.3/Hanalytics_python_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Hanalytics_python_package-0.2/hanalytics/hanalytics_ga4/connectga4.py` & `Hanalytics_python_package-0.3/hanalytics/hanalytics_ga4/connectga4.py`

 * *Files identical despite different names*

### Comparing `Hanalytics_python_package-0.2/hanalytics/hanalytics_ga4/tools.py` & `Hanalytics_python_package-0.3/hanalytics/hanalytics_ga4/tools.py`

 * *Files identical despite different names*

### Comparing `Hanalytics_python_package-0.2/hanalytics/hanalytics_keywords_generator/googleAds_keywords.py` & `Hanalytics_python_package-0.3/hanalytics/hanalytics_keywords_generator/googleAds_keywords.py`

 * *Files identical despite different names*

### Comparing `Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/connect.py` & `Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/connect.py`

 * *Files identical despite different names*

### Comparing `Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/customs.py` & `Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/customs.py`

 * *Files identical despite different names*

### Comparing `Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/query.py` & `Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/query.py`

 * *Files identical despite different names*

### Comparing `Hanalytics_python_package-0.2/hanalytics/hanalytics_ua/reports.py` & `Hanalytics_python_package-0.3/hanalytics/hanalytics_ua/reports.py`

 * *Files identical despite different names*

