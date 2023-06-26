# Comparing `tmp/RLS Task-0.1dev.tar.gz` & `tmp/RLS Task-0.11dev.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RLS Task-0.1dev.tar", last modified: Mon Jun 26 08:25:26 2023, max compression
+gzip compressed data, was "RLS Task-0.11dev.tar", last modified: Mon Jun 26 08:44:11 2023, max compression
```

## Comparing `RLS Task-0.1dev.tar` & `RLS Task-0.11dev.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:25:26.604653 RLS Task-0.1dev/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 08:25:26.604653 RLS Task-0.1dev/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:25:26.604653 RLS Task-0.1dev/RLS/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-26 08:25:08.072518 RLS Task-0.1dev/RLS/TaskGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-26 08:25:08.072518 RLS Task-0.1dev/RLS/TaskMain.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-26 08:25:08.072518 RLS Task-0.1dev/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:44:11.400016 RLS Task-0.11dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-26 08:44:11.400016 RLS Task-0.11dev/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:44:11.400016 RLS Task-0.11dev/RLS/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-26 08:43:53.283357 RLS Task-0.11dev/RLS/TaskGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-26 08:43:53.283357 RLS Task-0.11dev/RLS/TaskMain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 08:43:53.283357 RLS Task-0.11dev/setup.py
```

### Comparing `RLS Task-0.1dev/RLS/TaskGUI.py` & `RLS Task-0.11dev/RLS/TaskGUI.py`

 * *Files identical despite different names*

### Comparing `RLS Task-0.1dev/RLS/TaskMain.py` & `RLS Task-0.11dev/RLS/TaskMain.py`

 * *Files identical despite different names*

