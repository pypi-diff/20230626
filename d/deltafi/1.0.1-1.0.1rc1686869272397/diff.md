# Comparing `tmp/deltafi-1.0.1.tar.gz` & `tmp/deltafi-1.0.1rc1686869272397.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-1.0.1.tar", max compression
+gzip compressed data, was "deltafi-1.0.1rc1686869272397.tar", max compression
```

## Comparing `deltafi-1.0.1.tar` & `deltafi-1.0.1rc1686869272397.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-1.0.1/README.md
--rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-1.0.1/deltafi/__init__.py
--rw-r--r--   0        0        0     7330 2023-06-09 15:16:11.399155 deltafi-1.0.1/deltafi/action.py
--rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-1.0.1/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-1.0.1/deltafi/actiontype.py
--rw-r--r--   0        0        0    11025 2023-06-09 15:16:11.400155 deltafi-1.0.1/deltafi/domain.py
--rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-1.0.1/deltafi/exception.py
--rw-r--r--   0        0        0     6290 2023-06-09 15:16:11.401155 deltafi-1.0.1/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-1.0.1/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-1.0.1/deltafi/metric.py
--rw-r--r--   0        0        0    11666 2023-06-06 18:39:40.022585 deltafi-1.0.1/deltafi/plugin.py
--rw-r--r--   0        0        0    10706 2023-05-22 14:40:08.186270 deltafi-1.0.1/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-1.0.1/deltafi/storage.py
--rw-r--r--   0        0        0     1277 2023-06-26 14:56:42.082903 deltafi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1708 1970-01-01 00:00:00.000000 deltafi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:38:35.784256 deltafi-1.0.1rc1686869272397/README.md
+-rw-r--r--   0        0        0      706 2023-04-10 13:38:35.784256 deltafi-1.0.1rc1686869272397/deltafi/__init__.py
+-rw-r--r--   0        0        0     7330 2023-06-09 15:19:00.338093 deltafi-1.0.1rc1686869272397/deltafi/action.py
+-rw-r--r--   0        0        0     1981 2023-04-10 13:38:35.785256 deltafi-1.0.1rc1686869272397/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      985 2023-05-10 13:16:19.135727 deltafi-1.0.1rc1686869272397/deltafi/actiontype.py
+-rw-r--r--   0        0        0    11025 2023-06-09 15:19:00.339093 deltafi-1.0.1rc1686869272397/deltafi/domain.py
+-rw-r--r--   0        0        0     1149 2023-04-24 18:51:23.516157 deltafi-1.0.1rc1686869272397/deltafi/exception.py
+-rw-r--r--   0        0        0     6290 2023-06-09 15:19:00.339093 deltafi-1.0.1rc1686869272397/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:38:35.786256 deltafi-1.0.1rc1686869272397/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:38:35.786256 deltafi-1.0.1rc1686869272397/deltafi/metric.py
+-rw-r--r--   0        0        0    11666 2023-06-07 15:12:39.537100 deltafi-1.0.1rc1686869272397/deltafi/plugin.py
+-rw-r--r--   0        0        0    10706 2023-05-24 15:03:17.102464 deltafi-1.0.1rc1686869272397/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-17 15:15:04.065396 deltafi-1.0.1rc1686869272397/deltafi/storage.py
+-rw-r--r--   0        0        0     1292 2023-06-15 22:48:03.100551 deltafi-1.0.1rc1686869272397/pyproject.toml
+-rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 deltafi-1.0.1rc1686869272397/PKG-INFO
```

### Comparing `deltafi-1.0.1/deltafi/__init__.py` & `deltafi-1.0.1rc1686869272397/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/action.py` & `deltafi-1.0.1rc1686869272397/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/actioneventqueue.py` & `deltafi-1.0.1rc1686869272397/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/actiontype.py` & `deltafi-1.0.1rc1686869272397/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/domain.py` & `deltafi-1.0.1rc1686869272397/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/exception.py` & `deltafi-1.0.1rc1686869272397/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/input.py` & `deltafi-1.0.1rc1686869272397/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/logger.py` & `deltafi-1.0.1rc1686869272397/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/metric.py` & `deltafi-1.0.1rc1686869272397/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/plugin.py` & `deltafi-1.0.1rc1686869272397/deltafi/plugin.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/result.py` & `deltafi-1.0.1rc1686869272397/deltafi/result.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/deltafi/storage.py` & `deltafi-1.0.1rc1686869272397/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.1/pyproject.toml` & `deltafi-1.0.1rc1686869272397/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "1.0.1"
+version = "1.0.1rc1686869272397"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-1.0.1/PKG-INFO` & `deltafi-1.0.1rc1686869272397/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 1.0.1
+Version: 1.0.1rc1686869272397
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

