# Comparing `tmp/fastexception-0.1.1.tar.gz` & `tmp/fastexception-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastexception-0.1.1.tar", last modified: Mon Jun 26 05:55:17 2023, max compression
+gzip compressed data, was "fastexception-0.1.2.tar", last modified: Mon Jun 26 06:44:51 2023, max compression
```

## Comparing `fastexception-0.1.1.tar` & `fastexception-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 05:55:17.230054 fastexception-0.1.1/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      262 2023-06-26 05:55:17.230054 fastexception-0.1.1/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1174 2023-06-25 19:34:30.000000 fastexception-0.1.1/README.rst
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 05:55:17.230054 fastexception-0.1.1/fastexception.egg-info/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      262 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      213 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/SOURCES.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/dependency_links.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/requires.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/top_level.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      107 2023-06-26 05:55:17.230054 fastexception-0.1.1/setup.cfg
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      367 2023-06-25 18:28:15.000000 fastexception-0.1.1/setup.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 06:44:51.380868 fastexception-0.1.2/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1274 2023-06-26 06:44:51.380868 fastexception-0.1.2/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1174 2023-06-25 19:34:30.000000 fastexception-0.1.2/README.rst
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 06:44:51.380868 fastexception-0.1.2/fastexception.egg-info/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1274 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      213 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/SOURCES.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/dependency_links.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/requires.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/top_level.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      107 2023-06-26 06:44:51.380868 fastexception-0.1.2/setup.cfg
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      581 2023-06-26 06:44:37.000000 fastexception-0.1.2/setup.py
```

### Comparing `fastexception-0.1.1/README.rst` & `fastexception-0.1.2/README.rst`

 * *Files identical despite different names*

