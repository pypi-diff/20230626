# Comparing `tmp/waivek-0.1.3.tar.gz` & `tmp/waivek-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waivek-0.1.3.tar", last modified: Mon Jun 26 17:01:35 2023, max compression
+gzip compressed data, was "waivek-0.1.4.tar", last modified: Mon Jun 26 17:14:25 2023, max compression
```

## Comparing `waivek-0.1.3.tar` & `waivek-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 17:01:35.235937 waivek-0.1.3/
--rw-rw-rw-   0        0        0      141 2023-06-26 17:01:35.235937 waivek-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-26 17:01:35.235937 waivek-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1087 2023-06-26 17:01:23.000000 waivek-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:01:35.204686 waivek-0.1.3/waivek/
--rw-rw-rw-   0        0        0      377 2023-06-26 13:32:15.000000 waivek-0.1.3/waivek/__init__.py
--rw-rw-rw-   0        0        0     5601 2023-06-26 13:00:33.000000 waivek-0.1.3/waivek/color.py
--rw-rw-rw-   0        0        0    17147 2023-06-26 13:00:47.000000 waivek-0.1.3/waivek/common.py
--rw-rw-rw-   0        0        0    18804 2023-06-26 13:00:50.000000 waivek-0.1.3/waivek/db.py
--rw-rw-rw-   0        0        0    25668 2023-06-26 13:01:04.000000 waivek-0.1.3/waivek/error.py
--rw-rw-rw-   0        0        0     4725 2023-06-26 13:01:06.000000 waivek-0.1.3/waivek/frame.py
--rw-rw-rw-   0        0        0     9044 2023-06-26 13:01:10.000000 waivek-0.1.3/waivek/get.py
--rw-rw-rw-   0        0        0    28068 2023-06-26 13:01:20.000000 waivek-0.1.3/waivek/ic.py
--rw-rw-rw-   0        0        0     6272 2023-06-26 13:01:23.000000 waivek-0.1.3/waivek/print_utils.py
--rw-rw-rw-   0        0        0     1883 2022-09-26 11:19:33.000000 waivek-0.1.3/waivek/reltools.py
--rw-rw-rw-   0        0        0     4431 2023-06-26 16:58:35.000000 waivek-0.1.3/waivek/reqs.py
--rw-rw-rw-   0        0        0     1191 2023-06-26 13:01:34.000000 waivek-0.1.3/waivek/tdd.py
--rw-rw-rw-   0        0        0      395 2023-06-26 13:01:40.000000 waivek-0.1.3/waivek/template.py
--rw-rw-rw-   0        0        0    21659 2023-06-26 13:01:55.000000 waivek-0.1.3/waivek/test.py
--rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1.3/waivek/timer.py
--rw-rw-rw-   0        0        0     5908 2023-06-26 13:02:00.000000 waivek-0.1.3/waivek/trace.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:01:35.235937 waivek-0.1.3/waivek.egg-info/
--rw-rw-rw-   0        0        0      141 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 17:14:25.381242 waivek-0.1.4/
+-rw-rw-rw-   0        0        0      996 2023-06-26 17:14:25.381242 waivek-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2023-06-26 17:13:33.000000 waivek-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 17:14:25.381242 waivek-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1207 2023-06-26 17:14:14.000000 waivek-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:14:25.349557 waivek-0.1.4/waivek/
+-rw-rw-rw-   0        0        0      377 2023-06-26 17:09:35.000000 waivek-0.1.4/waivek/__init__.py
+-rw-rw-rw-   0        0        0     5601 2023-06-26 13:00:33.000000 waivek-0.1.4/waivek/color.py
+-rw-rw-rw-   0        0        0    17147 2023-06-26 13:00:47.000000 waivek-0.1.4/waivek/common.py
+-rw-rw-rw-   0        0        0    18804 2023-06-26 13:00:50.000000 waivek-0.1.4/waivek/db.py
+-rw-rw-rw-   0        0        0    25668 2023-06-26 13:01:04.000000 waivek-0.1.4/waivek/error.py
+-rw-rw-rw-   0        0        0     4725 2023-06-26 13:01:06.000000 waivek-0.1.4/waivek/frame.py
+-rw-rw-rw-   0        0        0     9044 2023-06-26 13:01:10.000000 waivek-0.1.4/waivek/get.py
+-rw-rw-rw-   0        0        0    28068 2023-06-26 13:01:20.000000 waivek-0.1.4/waivek/ic.py
+-rw-rw-rw-   0        0        0     6272 2023-06-26 13:01:23.000000 waivek-0.1.4/waivek/print_utils.py
+-rw-rw-rw-   0        0        0     1883 2022-09-26 11:19:33.000000 waivek-0.1.4/waivek/reltools.py
+-rw-rw-rw-   0        0        0     4431 2023-06-26 16:58:35.000000 waivek-0.1.4/waivek/reqs.py
+-rw-rw-rw-   0        0        0     1191 2023-06-26 13:01:34.000000 waivek-0.1.4/waivek/tdd.py
+-rw-rw-rw-   0        0        0      395 2023-06-26 13:01:40.000000 waivek-0.1.4/waivek/template.py
+-rw-rw-rw-   0        0        0    21659 2023-06-26 13:01:55.000000 waivek-0.1.4/waivek/test.py
+-rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1.4/waivek/timer.py
+-rw-rw-rw-   0        0        0     5908 2023-06-26 13:02:00.000000 waivek-0.1.4/waivek/trace.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:14:25.381242 waivek-0.1.4/waivek.egg-info/
+-rw-rw-rw-   0        0        0      996 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 17:14:25.000000 waivek-0.1.4/waivek.egg-info/top_level.txt
```

### Comparing `waivek-0.1.3/waivek/color.py` & `waivek-0.1.4/waivek/color.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/common.py` & `waivek-0.1.4/waivek/common.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/db.py` & `waivek-0.1.4/waivek/db.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/error.py` & `waivek-0.1.4/waivek/error.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/frame.py` & `waivek-0.1.4/waivek/frame.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/get.py` & `waivek-0.1.4/waivek/get.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/ic.py` & `waivek-0.1.4/waivek/ic.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/print_utils.py` & `waivek-0.1.4/waivek/print_utils.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/reltools.py` & `waivek-0.1.4/waivek/reltools.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/reqs.py` & `waivek-0.1.4/waivek/reqs.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/tdd.py` & `waivek-0.1.4/waivek/tdd.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/test.py` & `waivek-0.1.4/waivek/test.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/timer.py` & `waivek-0.1.4/waivek/timer.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.3/waivek/trace.py` & `waivek-0.1.4/waivek/trace.py`

 * *Files identical despite different names*

