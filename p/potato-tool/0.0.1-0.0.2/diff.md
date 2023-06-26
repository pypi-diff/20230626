# Comparing `tmp/potato_tool-0.0.1.tar.gz` & `tmp/potato_tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potato_tool-0.0.1.tar", last modified: Sun Jun 25 07:41:46 2023, max compression
+gzip compressed data, was "potato_tool-0.0.2.tar", last modified: Mon Jun 26 05:11:49 2023, max compression
```

## Comparing `potato_tool-0.0.1.tar` & `potato_tool-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-25 07:41:46.209740 potato_tool-0.0.1/
--rw-r--r--   0 a          (501) staff       (20)     1997 2023-06-25 07:41:46.209477 potato_tool-0.0.1/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)     1715 2023-06-25 07:41:39.000000 potato_tool-0.0.1/README.md
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-25 07:41:46.206827 potato_tool-0.0.1/potato_tool/
--rw-r--r--   0 a          (501) staff       (20)       30 2023-06-25 07:18:35.000000 potato_tool-0.0.1/potato_tool/__init__.py
--rwxr-xr-x   0 a          (501) staff       (20)     4921 2023-06-25 07:36:21.000000 potato_tool-0.0.1/potato_tool/font.py
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-25 07:41:46.209036 potato_tool-0.0.1/potato_tool.egg-info/
--rw-r--r--   0 a          (501) staff       (20)     1997 2023-06-25 07:41:46.000000 potato_tool-0.0.1/potato_tool.egg-info/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)      274 2023-06-25 07:41:46.000000 potato_tool-0.0.1/potato_tool.egg-info/SOURCES.txt
--rw-r--r--   0 a          (501) staff       (20)        1 2023-06-25 07:41:46.000000 potato_tool-0.0.1/potato_tool.egg-info/dependency_links.txt
--rw-r--r--   0 a          (501) staff       (20)      477 2023-06-25 07:41:46.000000 potato_tool-0.0.1/potato_tool.egg-info/entry_points.txt
--rw-r--r--   0 a          (501) staff       (20)       17 2023-06-25 07:41:46.000000 potato_tool-0.0.1/potato_tool.egg-info/requires.txt
--rw-r--r--   0 a          (501) staff       (20)       12 2023-06-25 07:41:46.000000 potato_tool-0.0.1/potato_tool.egg-info/top_level.txt
--rw-r--r--   0 a          (501) staff       (20)       38 2023-06-25 07:41:46.209850 potato_tool-0.0.1/setup.cfg
--rw-r--r--   0 a          (501) staff       (20)     1310 2023-06-25 07:30:03.000000 potato_tool-0.0.1/setup.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 05:11:49.134826 potato_tool-0.0.2/
+-rw-r--r--   0 a          (501) staff       (20)     3395 2023-06-26 05:11:49.134560 potato_tool-0.0.2/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)     3113 2023-06-26 05:07:26.000000 potato_tool-0.0.2/README.md
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 05:11:49.131227 potato_tool-0.0.2/potato_tool/
+-rw-r--r--   0 a          (501) staff       (20)       30 2023-06-25 07:18:35.000000 potato_tool-0.0.2/potato_tool/__init__.py
+-rwxr-xr-x   0 a          (501) staff       (20)     8636 2023-06-26 05:10:25.000000 potato_tool-0.0.2/potato_tool/font.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 05:11:49.134100 potato_tool-0.0.2/potato_tool.egg-info/
+-rw-r--r--   0 a          (501) staff       (20)     3395 2023-06-26 05:11:49.000000 potato_tool-0.0.2/potato_tool.egg-info/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)      274 2023-06-26 05:11:49.000000 potato_tool-0.0.2/potato_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 05:11:49.000000 potato_tool-0.0.2/potato_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 a          (501) staff       (20)      950 2023-06-26 05:11:49.000000 potato_tool-0.0.2/potato_tool.egg-info/entry_points.txt
+-rw-r--r--   0 a          (501) staff       (20)       25 2023-06-26 05:11:49.000000 potato_tool-0.0.2/potato_tool.egg-info/requires.txt
+-rw-r--r--   0 a          (501) staff       (20)       12 2023-06-26 05:11:49.000000 potato_tool-0.0.2/potato_tool.egg-info/top_level.txt
+-rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 05:11:49.134935 potato_tool-0.0.2/setup.cfg
+-rw-r--r--   0 a          (501) staff       (20)     2024 2023-06-26 05:10:09.000000 potato_tool-0.0.2/setup.py
```

