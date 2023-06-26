# Comparing `tmp/yplib-1.8.0.tar.gz` & `tmp/yplib-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.8.0.tar", last modified: Mon Jun 26 00:53:03 2023, max compression
+gzip compressed data, was "dist\yplib-1.8.1.tar", last modified: Mon Jun 26 01:19:49 2023, max compression
```

## Comparing `yplib-1.8.0.tar` & `yplib-1.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 00:53:03.347092 yplib-1.8.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.8.0/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-26 00:53:03.346594 yplib-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.8.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 00:53:03.347092 yplib-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-26 00:52:56.000000 yplib-1.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 00:53:03.343153 yplib-1.8.0/yplib/
--rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.8.0/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 00:52:47.000000 yplib-1.8.0/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.8.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.8.0/yplib/db.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.8.0/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.8.0/yplib/http_util.py
--rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.8.0/yplib/index.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.8.0/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-26 00:53:03.346082 yplib-1.8.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-26 00:53:03.000000 yplib-1.8.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-26 00:53:03.000000 yplib-1.8.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 00:53:03.000000 yplib-1.8.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-26 00:53:03.000000 yplib-1.8.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 01:19:49.812380 yplib-1.8.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-26 01:19:49.811880 yplib-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.8.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 01:19:49.812380 yplib-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-26 01:19:38.000000 yplib-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 01:19:49.808881 yplib-1.8.1/yplib/
+-rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.8.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:19:30.000000 yplib-1.8.1/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.8.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.8.1/yplib/db.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.8.1/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.8.1/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.8.1/yplib/index.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.8.1/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-26 01:19:49.811381 yplib-1.8.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-26 01:19:49.000000 yplib-1.8.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-26 01:19:49.000000 yplib-1.8.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 01:19:49.000000 yplib-1.8.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-26 01:19:49.000000 yplib-1.8.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.8.0/LICENSE` & `yplib-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.8.0/setup.py` & `yplib-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.8.0",
+  version="1.8.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.8.0/yplib/chart.py` & `yplib-1.8.1/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.0/yplib/chart_html.py` & `yplib-1.8.1/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.0/yplib/db.py` & `yplib-1.8.1/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.0/yplib/file.py` & `yplib-1.8.1/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.0/yplib/http_util.py` & `yplib-1.8.1/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.0/yplib/index.py` & `yplib-1.8.1/yplib/index.py`

 * *Files identical despite different names*

