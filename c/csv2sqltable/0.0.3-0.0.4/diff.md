# Comparing `tmp/csv2sqltable-0.0.3.tar.gz` & `tmp/csv2sqltable-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv2sqltable-0.0.3.tar", last modified: Mon Jun 26 07:18:46 2023, max compression
+gzip compressed data, was "csv2sqltable-0.0.4.tar", last modified: Mon Jun 26 07:21:57 2023, max compression
```

## Comparing `csv2sqltable-0.0.3.tar` & `csv2sqltable-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 07:18:46.416400 csv2sqltable-0.0.3/
--rw-rw-rw-   0        0        0       19 2023-03-18 16:27:25.000000 csv2sqltable-0.0.3/License.txt
--rw-rw-rw-   0        0        0       25 2023-03-18 16:27:25.000000 csv2sqltable-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      370 2023-06-26 07:18:46.414398 csv2sqltable-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       90 2023-06-26 07:18:23.000000 csv2sqltable-0.0.3/Readme.txt
--rw-rw-rw-   0        0        0     1017 2023-03-18 16:27:25.000000 csv2sqltable-0.0.3/about.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 07:18:46.393139 csv2sqltable-0.0.3/csv2sqltable/
--rw-rw-rw-   0        0        0       80 2023-06-26 07:15:45.000000 csv2sqltable-0.0.3/csv2sqltable/__init__.py
--rw-rw-rw-   0        0        0      663 2023-06-26 06:51:43.000000 csv2sqltable-0.0.3/csv2sqltable/convert.py
-drwxrwxrwx   0        0        0        0 2023-06-26 07:18:46.412400 csv2sqltable-0.0.3/csv2sqltable.egg-info/
--rw-rw-rw-   0        0        0      370 2023-06-26 07:18:45.000000 csv2sqltable-0.0.3/csv2sqltable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-26 07:18:46.000000 csv2sqltable-0.0.3/csv2sqltable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 07:18:45.000000 csv2sqltable-0.0.3/csv2sqltable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-26 07:18:45.000000 csv2sqltable-0.0.3/csv2sqltable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 07:18:46.416400 csv2sqltable-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      504 2023-06-26 07:18:07.000000 csv2sqltable-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:21:57.186872 csv2sqltable-0.0.4/
+-rw-rw-rw-   0        0        0       19 2023-03-18 16:27:25.000000 csv2sqltable-0.0.4/License.txt
+-rw-rw-rw-   0        0        0       25 2023-03-18 16:27:25.000000 csv2sqltable-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1167 2023-06-26 07:21:57.185873 csv2sqltable-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2023-06-26 07:21:40.000000 csv2sqltable-0.0.4/Readme.txt
+-rw-rw-rw-   0        0        0     1017 2023-03-18 16:27:25.000000 csv2sqltable-0.0.4/about.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 07:21:57.163870 csv2sqltable-0.0.4/csv2sqltable/
+-rw-rw-rw-   0        0        0       80 2023-06-26 07:15:45.000000 csv2sqltable-0.0.4/csv2sqltable/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-06-26 06:51:43.000000 csv2sqltable-0.0.4/csv2sqltable/convert.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:21:57.182870 csv2sqltable-0.0.4/csv2sqltable.egg-info/
+-rw-rw-rw-   0        0        0     1167 2023-06-26 07:21:56.000000 csv2sqltable-0.0.4/csv2sqltable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-26 07:21:56.000000 csv2sqltable-0.0.4/csv2sqltable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 07:21:56.000000 csv2sqltable-0.0.4/csv2sqltable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-26 07:21:56.000000 csv2sqltable-0.0.4/csv2sqltable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 07:21:57.187871 csv2sqltable-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      504 2023-06-26 07:20:36.000000 csv2sqltable-0.0.4/setup.py
```

### Comparing `csv2sqltable-0.0.3/about.txt` & `csv2sqltable-0.0.4/about.txt`

 * *Files identical despite different names*

### Comparing `csv2sqltable-0.0.3/csv2sqltable/convert.py` & `csv2sqltable-0.0.4/csv2sqltable/convert.py`

 * *Files identical despite different names*

