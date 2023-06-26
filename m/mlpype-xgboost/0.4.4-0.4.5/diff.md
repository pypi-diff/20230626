# Comparing `tmp/mlpype-xgboost-0.4.4.tar.gz` & `tmp/mlpype-xgboost-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-xgboost-0.4.4.tar", last modified: Fri Jun 23 09:48:31 2023, max compression
+gzip compressed data, was "mlpype-xgboost-0.4.5.tar", last modified: Mon Jun 26 20:43:25 2023, max compression
```

## Comparing `mlpype-xgboost-0.4.4.tar` & `mlpype-xgboost-0.4.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:31.412169 mlpype-xgboost-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 09:48:31.412169 mlpype-xgboost-0.4.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:31.412169 mlpype-xgboost-0.4.4/mlpype_xgboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 09:48:31.000000 mlpype-xgboost-0.4.4/mlpype_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-23 09:48:31.000000 mlpype-xgboost-0.4.4/mlpype_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:31.000000 mlpype-xgboost-0.4.4/mlpype_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-23 09:48:31.000000 mlpype-xgboost-0.4.4/mlpype_xgboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:31.000000 mlpype-xgboost-0.4.4/mlpype_xgboost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:48:31.412169 mlpype-xgboost-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-23 09:44:01.000000 mlpype-xgboost-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:43:25.325697 mlpype-xgboost-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 20:43:25.325697 mlpype-xgboost-0.4.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:43:25.325697 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:43:25.000000 mlpype-xgboost-0.4.5/mlpype_xgboost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:43:25.325697 mlpype-xgboost-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-26 20:39:45.000000 mlpype-xgboost-0.4.5/setup.py
```

