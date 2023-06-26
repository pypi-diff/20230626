# Comparing `tmp/walt-node-8.0.tar.gz` & `tmp/walt-node-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "walt-node-8.0.tar", last modified: Fri Jun 23 07:38:19 2023, max compression
+gzip compressed data, was "walt-node-8.1.tar", last modified: Mon Jun 26 14:05:25 2023, max compression
```

## Comparing `walt-node-8.0.tar` & `walt-node-8.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:19.048537 walt-node-8.0/
--rw-r--r--   0 root         (0) root         (0)       34 2022-03-29 14:58:03.000000 walt-node-8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      264 2023-06-23 07:38:19.048537 walt-node-8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      124 2022-03-29 14:58:03.000000 walt-node-8.0/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:19.048537 walt-node-8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1066 2023-06-23 07:37:56.000000 walt-node-8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:19.048537 walt-node-8.0/sh/
--rwxr-xr-x   0 root         (0) root         (0)     2517 2022-03-29 14:58:03.000000 walt-node-8.0/sh/walt-log-monitor
--rwxr-xr-x   0 root         (0) root         (0)      109 2022-03-29 14:58:03.000000 walt-node-8.0/sh/walt-monitor
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:19.048537 walt-node-8.0/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-node-8.0/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:19.048537 walt-node-8.0/walt/node/
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/__init__.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/const.py
--rwxr-xr-x   0 root         (0) root         (0)     3483 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/ipxekexec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:19.048537 walt-node-8.0/walt/node/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-node-8.0/walt/node/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/logs/cache.py
--rwxr-xr-x   0 root         (0) root         (0)      266 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/logs/daemon.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/logs/flow.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/logs/listener.py
--rwxr-xr-x   0 root         (0) root         (0)     4225 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/logs/monitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:19.048537 walt-node-8.0/walt/node/serial/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-node-8.0/walt/node/serial/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4540 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/serial/autolog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:19.048537 walt-node-8.0/walt/node/setup/
--rw-r--r--   0 root         (0) root         (0)      339 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-21 15:19:09.000000 walt-node-8.0/walt/node/setup/walt-logs.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:19.048537 walt-node-8.0/walt_node.egg-info/
--rw-r--r--   0 root         (0) root         (0)      264 2023-06-23 07:38:19.000000 walt-node-8.0/walt_node.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      619 2023-06-23 07:38:19.000000 walt-node-8.0/walt_node.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:19.000000 walt-node-8.0/walt_node.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      201 2023-06-23 07:38:19.000000 walt-node-8.0/walt_node.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-23 07:38:19.000000 walt-node-8.0/walt_node.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:19.000000 walt-node-8.0/walt_node.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:25.515833 walt-node-8.1/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-03-29 14:58:03.000000 walt-node-8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      264 2023-06-26 14:05:25.515833 walt-node-8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      124 2022-03-29 14:58:03.000000 walt-node-8.1/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 14:05:25.515833 walt-node-8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-06-26 14:05:03.000000 walt-node-8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:25.515833 walt-node-8.1/sh/
+-rwxr-xr-x   0 root         (0) root         (0)     2517 2022-03-29 14:58:03.000000 walt-node-8.1/sh/walt-log-monitor
+-rwxr-xr-x   0 root         (0) root         (0)      109 2022-03-29 14:58:03.000000 walt-node-8.1/sh/walt-monitor
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:25.515833 walt-node-8.1/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-node-8.1/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:25.515833 walt-node-8.1/walt/node/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/const.py
+-rwxr-xr-x   0 root         (0) root         (0)     3483 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/ipxekexec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:25.515833 walt-node-8.1/walt/node/logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-node-8.1/walt/node/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/logs/cache.py
+-rwxr-xr-x   0 root         (0) root         (0)      266 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/logs/daemon.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/logs/flow.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/logs/listener.py
+-rwxr-xr-x   0 root         (0) root         (0)     4225 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/logs/monitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:25.515833 walt-node-8.1/walt/node/serial/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-node-8.1/walt/node/serial/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4540 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/serial/autolog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:25.515833 walt-node-8.1/walt/node/setup/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-21 15:19:09.000000 walt-node-8.1/walt/node/setup/walt-logs.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:25.515833 walt-node-8.1/walt_node.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-06-26 14:05:25.000000 walt-node-8.1/walt_node.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-26 14:05:25.000000 walt-node-8.1/walt_node.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:05:25.000000 walt-node-8.1/walt_node.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      201 2023-06-26 14:05:25.000000 walt-node-8.1/walt_node.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-26 14:05:25.000000 walt-node-8.1/walt_node.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 14:05:25.000000 walt-node-8.1/walt_node.egg-info/top_level.txt
```

### Comparing `walt-node-8.0/setup.py` & `walt-node-8.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from setuptools import find_packages, setup
 
 if sys.version_info[0] == 2:
     sys.exit("Sorry, Python 2 is no longer supported.")
 
 setup_info = {
     "name": "walt-node",
-    "version": "8.0",
-    "install_requires": ["walt-common==8.0"],
+    "version": "8.1",
+    "install_requires": ["walt-common==8.1"],
     "author": "WalT developers",
     "author_email": "walt-contact@univ-grenoble-alpes.fr",
     "keywords": "WalT testbed",
     "license": "3-Clause BSD",
     "url": "https://walt-project.liglab.fr",
     "description": "WalT optional software embedded in images.",
     "entry_points": {
```

### Comparing `walt-node-8.0/sh/walt-log-monitor` & `walt-node-8.1/sh/walt-log-monitor`

 * *Files identical despite different names*

### Comparing `walt-node-8.0/walt/node/ipxekexec.py` & `walt-node-8.1/walt/node/ipxekexec.py`

 * *Files identical despite different names*

### Comparing `walt-node-8.0/walt/node/logs/cache.py` & `walt-node-8.1/walt/node/logs/cache.py`

 * *Files identical despite different names*

### Comparing `walt-node-8.0/walt/node/logs/flow.py` & `walt-node-8.1/walt/node/logs/flow.py`

 * *Files identical despite different names*

### Comparing `walt-node-8.0/walt/node/logs/listener.py` & `walt-node-8.1/walt/node/logs/listener.py`

 * *Files identical despite different names*

### Comparing `walt-node-8.0/walt/node/logs/monitor.py` & `walt-node-8.1/walt/node/logs/monitor.py`

 * *Files identical despite different names*

### Comparing `walt-node-8.0/walt/node/serial/autolog.py` & `walt-node-8.1/walt/node/serial/autolog.py`

 * *Files identical despite different names*

### Comparing `walt-node-8.0/walt_node.egg-info/SOURCES.txt` & `walt-node-8.1/walt_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

