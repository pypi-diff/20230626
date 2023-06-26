# Comparing `tmp/waivek-0.1.tar.gz` & `tmp/waivek-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waivek-0.1.tar", last modified: Mon Jun 26 11:18:38 2023, max compression
+gzip compressed data, was "waivek-0.1.1.tar", last modified: Mon Jun 26 12:31:44 2023, max compression
```

## Comparing `waivek-0.1.tar` & `waivek-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 11:18:38.734633 waivek-0.1/
--rw-rw-rw-   0        0        0      139 2023-06-26 11:18:38.734633 waivek-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-26 11:18:38.734633 waivek-0.1/setup.cfg
--rw-rw-rw-   0        0        0      545 2023-06-26 11:14:55.000000 waivek-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 11:18:38.687262 waivek-0.1/waivek/
--rw-rw-rw-   0        0        0      377 2023-06-26 09:58:41.000000 waivek-0.1/waivek/__init__.py
--rw-rw-rw-   0        0        0     5600 2023-06-26 09:48:41.000000 waivek-0.1/waivek/color.py
--rw-rw-rw-   0        0        0    17139 2023-06-26 09:56:36.000000 waivek-0.1/waivek/common.py
--rw-rw-rw-   0        0        0    18800 2022-11-05 22:58:49.000000 waivek-0.1/waivek/db.py
--rw-rw-rw-   0        0        0    25650 2023-05-30 00:32:44.000000 waivek-0.1/waivek/error.py
--rw-rw-rw-   0        0        0     4721 2023-06-25 06:52:08.000000 waivek-0.1/waivek/frame.py
--rw-rw-rw-   0        0        0     9039 2023-06-23 02:40:29.000000 waivek-0.1/waivek/get.py
--rw-rw-rw-   0        0        0    28060 2023-06-26 04:17:30.000000 waivek-0.1/waivek/ic.py
--rw-rw-rw-   0        0        0     6271 2023-06-26 09:57:54.000000 waivek-0.1/waivek/print_utils.py
--rw-rw-rw-   0        0        0     1883 2022-09-26 11:19:33.000000 waivek-0.1/waivek/reltools.py
--rw-rw-rw-   0        0        0     4112 2023-06-26 06:51:05.000000 waivek-0.1/waivek/reqs.py
--rw-rw-rw-   0        0        0     1189 2023-06-24 22:48:50.000000 waivek-0.1/waivek/tdd.py
--rw-rw-rw-   0        0        0      391 2023-06-24 22:15:02.000000 waivek-0.1/waivek/template.py
--rw-rw-rw-   0        0        0    21646 2023-06-25 08:39:39.000000 waivek-0.1/waivek/test.py
--rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1/waivek/timer.py
--rw-rw-rw-   0        0        0     5903 2022-10-10 07:32:48.000000 waivek-0.1/waivek/trace.py
-drwxrwxrwx   0        0        0        0 2023-06-26 11:18:38.719003 waivek-0.1/waivek.egg-info/
--rw-rw-rw-   0        0        0      139 2023-06-26 11:18:38.000000 waivek-0.1/waivek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-06-26 11:18:38.000000 waivek-0.1/waivek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 11:18:38.000000 waivek-0.1/waivek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-06-26 11:18:38.000000 waivek-0.1/waivek.egg-info/requires.txt
--rw-rw-rw-   0        0        0       75 2023-06-26 11:18:38.000000 waivek-0.1/waivek.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:44.553997 waivek-0.1.1/
+-rw-rw-rw-   0        0        0      141 2023-06-26 12:31:44.550989 waivek-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-26 12:31:44.554997 waivek-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-26 12:31:26.000000 waivek-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:44.535335 waivek-0.1.1/waivek/
+-rw-rw-rw-   0        0        0      367 2023-06-26 12:26:02.000000 waivek-0.1.1/waivek/__init__.py
+-rw-rw-rw-   0        0        0     5600 2023-06-26 09:48:41.000000 waivek-0.1.1/waivek/color.py
+-rw-rw-rw-   0        0        0    17139 2023-06-26 09:56:36.000000 waivek-0.1.1/waivek/common.py
+-rw-rw-rw-   0        0        0    18800 2022-11-05 22:58:49.000000 waivek-0.1.1/waivek/db.py
+-rw-rw-rw-   0        0        0    25650 2023-05-30 00:32:44.000000 waivek-0.1.1/waivek/error.py
+-rw-rw-rw-   0        0        0     4721 2023-06-25 06:52:08.000000 waivek-0.1.1/waivek/frame.py
+-rw-rw-rw-   0        0        0     9039 2023-06-23 02:40:29.000000 waivek-0.1.1/waivek/get.py
+-rw-rw-rw-   0        0        0    28060 2023-06-26 04:17:30.000000 waivek-0.1.1/waivek/ic.py
+-rw-rw-rw-   0        0        0     6271 2023-06-26 09:57:54.000000 waivek-0.1.1/waivek/print_utils.py
+-rw-rw-rw-   0        0        0     1883 2022-09-26 11:19:33.000000 waivek-0.1.1/waivek/reltools.py
+-rw-rw-rw-   0        0        0     4112 2023-06-26 06:51:05.000000 waivek-0.1.1/waivek/reqs.py
+-rw-rw-rw-   0        0        0     1189 2023-06-24 22:48:50.000000 waivek-0.1.1/waivek/tdd.py
+-rw-rw-rw-   0        0        0      391 2023-06-24 22:15:02.000000 waivek-0.1.1/waivek/template.py
+-rw-rw-rw-   0        0        0    21646 2023-06-25 08:39:39.000000 waivek-0.1.1/waivek/test.py
+-rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1.1/waivek/timer.py
+-rw-rw-rw-   0        0        0     5903 2022-10-10 07:32:48.000000 waivek-0.1.1/waivek/trace.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:44.550346 waivek-0.1.1/waivek.egg-info/
+-rw-rw-rw-   0        0        0      141 2023-06-26 12:31:44.000000 waivek-0.1.1/waivek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-06-26 12:31:44.000000 waivek-0.1.1/waivek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 12:31:44.000000 waivek-0.1.1/waivek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-06-26 12:31:44.000000 waivek-0.1.1/waivek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       75 2023-06-26 12:31:44.000000 waivek-0.1.1/waivek.egg-info/top_level.txt
```

### Comparing `waivek-0.1/setup.py` & `waivek-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://www.python.org/dev/peps/pep-0508/#environment-markers
 from setuptools import setup
 setup(
         name='waivek',
-        version='0.1',
+        version='0.1.1',
         packages=['waivek'],
         py_modules = ['color', 'common', 'db', 'error', 'frame', 'get', 'ic', 'print_utils', 'reltools', 'timer', 'trace'],
         install_requires = [
             'aiohttp==3.8.1',
             'executing==0.8.2',
             'python_dateutil==2.8.2',
             'timeago==1.0.14',
```

### Comparing `waivek-0.1/waivek/color.py` & `waivek-0.1.1/waivek/color.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/common.py` & `waivek-0.1.1/waivek/common.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/db.py` & `waivek-0.1.1/waivek/db.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/error.py` & `waivek-0.1.1/waivek/error.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/frame.py` & `waivek-0.1.1/waivek/frame.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/get.py` & `waivek-0.1.1/waivek/get.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/ic.py` & `waivek-0.1.1/waivek/ic.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/print_utils.py` & `waivek-0.1.1/waivek/print_utils.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/reltools.py` & `waivek-0.1.1/waivek/reltools.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/reqs.py` & `waivek-0.1.1/waivek/reqs.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/tdd.py` & `waivek-0.1.1/waivek/tdd.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/test.py` & `waivek-0.1.1/waivek/test.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/timer.py` & `waivek-0.1.1/waivek/timer.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1/waivek/trace.py` & `waivek-0.1.1/waivek/trace.py`

 * *Files identical despite different names*

