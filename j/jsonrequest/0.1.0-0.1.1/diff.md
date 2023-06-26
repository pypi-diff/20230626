# Comparing `tmp/jsonrequest-0.1.0.tar.gz` & `tmp/jsonrequest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrequest-0.1.0.tar", last modified: Mon Jun 26 06:00:10 2023, max compression
+gzip compressed data, was "jsonrequest-0.1.1.tar", last modified: Mon Jun 26 06:12:21 2023, max compression
```

## Comparing `jsonrequest-0.1.0.tar` & `jsonrequest-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:00:10.739331 jsonrequest-0.1.0/
--rw-r--r--   0 JustinRWong   (502) staff       (20)    11357 2023-06-26 05:51:37.000000 jsonrequest-0.1.0/LICENSE
--rw-r--r--   0 JustinRWong   (502) staff       (20)      276 2023-06-26 06:00:10.739221 jsonrequest-0.1.0/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)      106 2023-06-26 05:51:37.000000 jsonrequest-0.1.0/README.md
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:00:10.739063 jsonrequest-0.1.0/jsonrequest.egg-info/
--rw-r--r--   0 JustinRWong   (502) staff       (20)      276 2023-06-26 06:00:10.000000 jsonrequest-0.1.0/jsonrequest.egg-info/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)      200 2023-06-26 06:00:10.000000 jsonrequest-0.1.0/jsonrequest.egg-info/SOURCES.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:00:10.000000 jsonrequest-0.1.0/jsonrequest.egg-info/dependency_links.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 06:00:10.000000 jsonrequest-0.1.0/jsonrequest.egg-info/requires.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:00:10.000000 jsonrequest-0.1.0/jsonrequest.egg-info/top_level.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 06:00:10.739386 jsonrequest-0.1.0/setup.cfg
--rw-r--r--   0 JustinRWong   (502) staff       (20)      350 2023-06-26 05:59:49.000000 jsonrequest-0.1.0/setup.py
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:12:21.596464 jsonrequest-0.1.1/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)    11357 2023-06-26 05:51:37.000000 jsonrequest-0.1.1/LICENSE
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      939 2023-06-26 06:12:21.596336 jsonrequest-0.1.1/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      630 2023-06-26 06:10:47.000000 jsonrequest-0.1.1/README.md
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:12:21.596176 jsonrequest-0.1.1/jsonrequest.egg-info/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      939 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      200 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/SOURCES.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/dependency_links.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/requires.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/top_level.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 06:12:21.596509 jsonrequest-0.1.1/setup.cfg
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      527 2023-06-26 06:10:05.000000 jsonrequest-0.1.1/setup.py
```

### Comparing `jsonrequest-0.1.0/LICENSE` & `jsonrequest-0.1.1/LICENSE`

 * *Files identical despite different names*

