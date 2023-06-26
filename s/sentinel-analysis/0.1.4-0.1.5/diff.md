# Comparing `tmp/sentinel_analysis-0.1.4.tar.gz` & `tmp/sentinel_analysis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentinel_analysis-0.1.4.tar", max compression
+gzip compressed data, was "sentinel_analysis-0.1.5.tar", max compression
```

## Comparing `sentinel_analysis-0.1.4.tar` & `sentinel_analysis-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.4/README.md
--rw-r--r--   0        0        0      669 2023-06-25 23:05:18.119775 sentinel_analysis-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.4/sentinel_analysis/__init__.py
--rw-r--r--   0        0        0     3574 2023-06-25 16:10:47.832172 sentinel_analysis-0.1.4/sentinel_analysis/alert.py
--rw-r--r--   0        0        0     8393 2023-06-25 23:03:02.727301 sentinel_analysis-0.1.4/sentinel_analysis/main.py
--rw-r--r--   0        0        0      478 2023-06-25 11:58:27.079353 sentinel_analysis-0.1.4/sentinel_analysis/report.py
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 sentinel_analysis-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-26 11:03:55.971747 sentinel_analysis-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-26 11:03:55.971747 sentinel_analysis-0.1.5/README.md
+-rw-r--r--   0        0        0      669 2023-06-26 11:03:56.039748 sentinel_analysis-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 11:03:56.039748 sentinel_analysis-0.1.5/sentinel_analysis/__init__.py
+-rw-r--r--   0        0        0     3574 2023-06-26 11:03:56.039748 sentinel_analysis-0.1.5/sentinel_analysis/alert.py
+-rw-r--r--   0        0        0     8393 2023-06-26 11:03:56.039748 sentinel_analysis-0.1.5/sentinel_analysis/main.py
+-rw-r--r--   0        0        0      478 2023-06-26 11:03:56.039748 sentinel_analysis-0.1.5/sentinel_analysis/report.py
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 sentinel_analysis-0.1.5/PKG-INFO
```

### Comparing `sentinel_analysis-0.1.4/pyproject.toml` & `sentinel_analysis-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentinel-analysis"
-version = "0.1.4"
+version = "0.1.5"
 description = "This tools allows for a user, by means of specified flags, to process a parquet file containing traffic dumps in search for a set of traffic patterns"
 authors = ["David Araújo <david2araujo5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sentinel_analysis"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `sentinel_analysis-0.1.4/sentinel_analysis/alert.py` & `sentinel_analysis-0.1.5/sentinel_analysis/alert.py`

 * *Files identical despite different names*

### Comparing `sentinel_analysis-0.1.4/sentinel_analysis/main.py` & `sentinel_analysis-0.1.5/sentinel_analysis/main.py`

 * *Files identical despite different names*

### Comparing `sentinel_analysis-0.1.4/PKG-INFO` & `sentinel_analysis-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentinel-analysis
-Version: 0.1.4
+Version: 0.1.5
 Summary: This tools allows for a user, by means of specified flags, to process a parquet file containing traffic dumps in search for a set of traffic patterns
 Author: David Araújo
 Author-email: david2araujo5@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dnspython (>=2.3.0,<3.0.0)
```

