# Comparing `tmp/walt-client-g5k-8.0.tar.gz` & `tmp/walt-client-g5k-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "walt-client-g5k-8.0.tar", last modified: Fri Jun 23 07:38:27 2023, max compression
+gzip compressed data, was "walt-client-g5k-8.1.tar", last modified: Mon Jun 26 14:05:33 2023, max compression
```

## Comparing `walt-client-g5k-8.0.tar` & `walt-client-g5k-8.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      821 2023-06-23 07:37:56.000000 walt-client-g5k-8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/walt/client/
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/walt/client/g5k/
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/__init__.py
--rw-r--r--   0 root         (0) root         (0)      305 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/walt/client/g5k/deploy/
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/deploy/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5660 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/deploy/deploy.py
--rwxr-xr-x   0 root         (0) root         (0)    12645 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/deploy/helper.py
--rwxr-xr-x   0 root         (0) root         (0)     2130 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/deploy/remote-server-conf.py
--rwxr-xr-x   0 root         (0) root         (0)     4207 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/deploy/status.py
--rw-r--r--   0 root         (0) root         (0)     1934 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/myexeco.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/plugin.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/printer.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/reboot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/walt/client/g5k/recipes/
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/recipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/recipes/const.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/recipes/editor.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/recipes/manager.py
--rw-r--r--   0 root         (0) root         (0)     2016 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/recipes/printer.py
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/recipes/tools.py
--rwxr-xr-x   0 root         (0) root         (0)      764 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/release.py
--rw-r--r--   0 root         (0) root         (0)    11205 2023-06-22 13:09:04.000000 walt-client-g5k-8.0/walt/client/g5k/reservation.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/startup.py
--rwxr-xr-x   0 root         (0) root         (0)     5620 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/tools.py
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/types.py
--rwxr-xr-x   0 root         (0) root         (0)     2011 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/g5k/wait.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/walt/client/metadata/
--rw-r--r--   0 root         (0) root         (0)      238 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-21 15:19:09.000000 walt-client-g5k-8.0/walt/client/metadata/g5k.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:27.208416 walt-client-g5k-8.0/walt_client_g5k.egg-info/
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-23 07:38:27.000000 walt-client-g5k-8.0/walt_client_g5k.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1090 2023-06-23 07:38:27.000000 walt-client-g5k-8.0/walt_client_g5k.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:27.000000 walt-client-g5k-8.0/walt_client_g5k.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-23 07:38:27.000000 walt-client-g5k-8.0/walt_client_g5k.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-23 07:38:27.000000 walt-client-g5k-8.0/walt_client_g5k.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:27.000000 walt-client-g5k-8.0/walt_client_g5k.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      821 2023-06-26 14:05:03.000000 walt-client-g5k-8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/walt/client/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/walt/client/g5k/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/walt/client/g5k/deploy/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/deploy/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5660 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/deploy/deploy.py
+-rwxr-xr-x   0 root         (0) root         (0)    12645 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/deploy/helper.py
+-rwxr-xr-x   0 root         (0) root         (0)     2130 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/deploy/remote-server-conf.py
+-rwxr-xr-x   0 root         (0) root         (0)     4207 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/deploy/status.py
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/myexeco.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/printer.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/reboot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/walt/client/g5k/recipes/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/recipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/recipes/const.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/recipes/editor.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/recipes/manager.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/recipes/printer.py
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/recipes/tools.py
+-rwxr-xr-x   0 root         (0) root         (0)      764 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/release.py
+-rw-r--r--   0 root         (0) root         (0)    11205 2023-06-22 13:09:04.000000 walt-client-g5k-8.1/walt/client/g5k/reservation.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/startup.py
+-rwxr-xr-x   0 root         (0) root         (0)     5620 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/tools.py
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/types.py
+-rwxr-xr-x   0 root         (0) root         (0)     2011 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/g5k/wait.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/walt/client/metadata/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-21 15:19:09.000000 walt-client-g5k-8.1/walt/client/metadata/g5k.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:33.843710 walt-client-g5k-8.1/walt_client_g5k.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-26 14:05:33.000000 walt-client-g5k-8.1/walt_client_g5k.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-06-26 14:05:33.000000 walt-client-g5k-8.1/walt_client_g5k.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:05:33.000000 walt-client-g5k-8.1/walt_client_g5k.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-26 14:05:33.000000 walt-client-g5k-8.1/walt_client_g5k.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-26 14:05:33.000000 walt-client-g5k-8.1/walt_client_g5k.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 14:05:33.000000 walt-client-g5k-8.1/walt_client_g5k.egg-info/top_level.txt
```

### Comparing `walt-client-g5k-8.0/setup.py` & `walt-client-g5k-8.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from setuptools import find_packages, setup
 
 if sys.version_info[0] == 2:
     sys.exit("Sorry, Python 2 is no longer supported.")
 
 setup_info = {
     "name": "walt-client-g5k",
-    "version": "8.0",
-    "install_requires": ["execo>=2.6.5", "walt-client==8.0"],
+    "version": "8.1",
+    "install_requires": ["execo>=2.6.5", "walt-client==8.1"],
     "author": "WalT developers",
     "author_email": "walt-contact@univ-grenoble-alpes.fr",
     "keywords": "WalT testbed",
     "license": "3-Clause BSD",
     "url": "https://walt-project.liglab.fr",
     "description": "WalT control tool -- Grid'5000 plugin.",
     "entry_points": {
```

### Comparing `walt-client-g5k-8.0/walt/client/g5k/cli.py` & `walt-client-g5k-8.1/walt/client/g5k/cli.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/deploy/deploy.py` & `walt-client-g5k-8.1/walt/client/g5k/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/deploy/helper.py` & `walt-client-g5k-8.1/walt/client/g5k/deploy/helper.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/deploy/remote-server-conf.py` & `walt-client-g5k-8.1/walt/client/g5k/deploy/remote-server-conf.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/deploy/status.py` & `walt-client-g5k-8.1/walt/client/g5k/deploy/status.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/myexeco.py` & `walt-client-g5k-8.1/walt/client/g5k/myexeco.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/plugin.py` & `walt-client-g5k-8.1/walt/client/g5k/plugin.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/printer.py` & `walt-client-g5k-8.1/walt/client/g5k/printer.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/reboot.py` & `walt-client-g5k-8.1/walt/client/g5k/reboot.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/recipes/editor.py` & `walt-client-g5k-8.1/walt/client/g5k/recipes/editor.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/recipes/manager.py` & `walt-client-g5k-8.1/walt/client/g5k/recipes/manager.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/recipes/printer.py` & `walt-client-g5k-8.1/walt/client/g5k/recipes/printer.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/release.py` & `walt-client-g5k-8.1/walt/client/g5k/release.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/reservation.py` & `walt-client-g5k-8.1/walt/client/g5k/reservation.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/tools.py` & `walt-client-g5k-8.1/walt/client/g5k/tools.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/g5k/wait.py` & `walt-client-g5k-8.1/walt/client/g5k/wait.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt/client/metadata/g5k.py` & `walt-client-g5k-8.1/walt/client/metadata/g5k.py`

 * *Files identical despite different names*

### Comparing `walt-client-g5k-8.0/walt_client_g5k.egg-info/SOURCES.txt` & `walt-client-g5k-8.1/walt_client_g5k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

