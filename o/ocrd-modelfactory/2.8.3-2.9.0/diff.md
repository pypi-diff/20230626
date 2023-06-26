# Comparing `tmp/ocrd_modelfactory-2.8.3.tar.gz` & `tmp/ocrd_modelfactory-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrd_modelfactory-2.8.3.tar", last modified: Mon Jun  8 16:56:36 2020, max compression
+gzip compressed data, was "dist/ocrd_modelfactory-2.9.0.tar", last modified: Tue Jun  9 17:33:33 2020, max compression
```

## Comparing `ocrd_modelfactory-2.8.3.tar` & `ocrd_modelfactory-2.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/
--rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/setup.cfg
--rw-rw-r--   0 kba       (1000) kba       (1000)      799 2020-05-12 11:01:01.000000 ocrd_modelfactory-2.8.3/setup.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      505 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)      116 2020-05-12 11:01:01.000000 ocrd_modelfactory-2.8.3/README.md
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/ocrd_modelfactory.egg-info/
--rw-rw-r--   0 kba       (1000) kba       (1000)      252 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/ocrd_modelfactory.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       42 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/ocrd_modelfactory.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       18 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/ocrd_modelfactory.egg-info/top_level.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)      505 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/ocrd_modelfactory.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/ocrd_modelfactory.egg-info/dependency_links.txt
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:36.000000 ocrd_modelfactory-2.8.3/ocrd_modelfactory/
--rw-rw-r--   0 kba       (1000) kba       (1000)     2672 2020-06-08 11:38:59.000000 ocrd_modelfactory-2.8.3/ocrd_modelfactory/__init__.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:33.000000 ocrd_modelfactory-2.9.0/
+-rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-09 17:33:33.000000 ocrd_modelfactory-2.9.0/setup.cfg
+-rw-rw-r--   0 kba       (1000) kba       (1000)      799 2020-05-12 11:01:01.000000 ocrd_modelfactory-2.9.0/setup.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      505 2020-06-09 17:33:33.000000 ocrd_modelfactory-2.9.0/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)      116 2020-05-12 11:01:01.000000 ocrd_modelfactory-2.9.0/README.md
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:33.000000 ocrd_modelfactory-2.9.0/ocrd_modelfactory.egg-info/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      252 2020-06-09 17:33:32.000000 ocrd_modelfactory-2.9.0/ocrd_modelfactory.egg-info/SOURCES.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       42 2020-06-09 17:33:32.000000 ocrd_modelfactory-2.9.0/ocrd_modelfactory.egg-info/requires.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       18 2020-06-09 17:33:32.000000 ocrd_modelfactory-2.9.0/ocrd_modelfactory.egg-info/top_level.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)      505 2020-06-09 17:33:32.000000 ocrd_modelfactory-2.9.0/ocrd_modelfactory.egg-info/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-09 17:33:32.000000 ocrd_modelfactory-2.9.0/ocrd_modelfactory.egg-info/dependency_links.txt
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:33.000000 ocrd_modelfactory-2.9.0/ocrd_modelfactory/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2672 2020-06-09 17:08:17.000000 ocrd_modelfactory-2.9.0/ocrd_modelfactory/__init__.py
```

### Comparing `ocrd_modelfactory-2.8.3/setup.py` & `ocrd_modelfactory-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ocrd_modelfactory-2.8.3/ocrd_modelfactory/__init__.py` & `ocrd_modelfactory-2.9.0/ocrd_modelfactory/__init__.py`

 * *Files identical despite different names*

