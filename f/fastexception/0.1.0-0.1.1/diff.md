# Comparing `tmp/fastexception-0.1.0.tar.gz` & `tmp/fastexception-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastexception-0.1.0.tar", last modified: Sun Jun 25 14:45:23 2023, max compression
+gzip compressed data, was "fastexception-0.1.1.tar", last modified: Mon Jun 26 05:55:17 2023, max compression
```

## Comparing `fastexception-0.1.0.tar` & `fastexception-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-25 14:45:23.504134 fastexception-0.1.0/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      391 2023-06-25 14:45:23.504134 fastexception-0.1.0/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-25 13:08:34.000000 fastexception-0.1.0/README.md
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-25 14:45:23.504134 fastexception-0.1.0/fastexception.egg-info/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      391 2023-06-25 14:45:23.000000 fastexception-0.1.0/fastexception.egg-info/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      202 2023-06-25 14:45:23.000000 fastexception-0.1.0/fastexception.egg-info/SOURCES.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-25 14:45:23.000000 fastexception-0.1.0/fastexception.egg-info/dependency_links.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-25 14:45:23.000000 fastexception-0.1.0/fastexception.egg-info/requires.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-25 14:45:23.000000 fastexception-0.1.0/fastexception.egg-info/top_level.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-06-25 14:45:23.504134 fastexception-0.1.0/setup.cfg
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      503 2023-06-25 14:44:49.000000 fastexception-0.1.0/setup.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 05:55:17.230054 fastexception-0.1.1/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      262 2023-06-26 05:55:17.230054 fastexception-0.1.1/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1174 2023-06-25 19:34:30.000000 fastexception-0.1.1/README.rst
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 05:55:17.230054 fastexception-0.1.1/fastexception.egg-info/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      262 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      213 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/SOURCES.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/dependency_links.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/requires.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 05:55:17.000000 fastexception-0.1.1/fastexception.egg-info/top_level.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      107 2023-06-26 05:55:17.230054 fastexception-0.1.1/setup.cfg
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      367 2023-06-25 18:28:15.000000 fastexception-0.1.1/setup.py
```

