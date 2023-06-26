# Comparing `tmp/walt-vpn-8.0.tar.gz` & `tmp/walt-vpn-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "walt-vpn-8.0.tar", last modified: Fri Jun 23 07:38:09 2023, max compression
+gzip compressed data, was "walt-vpn-8.1.tar", last modified: Mon Jun 26 14:05:16 2023, max compression
```

## Comparing `walt-vpn-8.0.tar` & `walt-vpn-8.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:09.908673 walt-vpn-8.0/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 15:19:09.000000 walt-vpn-8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      241 2023-06-23 07:38:09.908673 walt-vpn-8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-06-21 15:19:09.000000 walt-vpn-8.0/README.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-23 07:38:09.908673 walt-vpn-8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1286 2023-06-23 07:37:56.000000 walt-vpn-8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:09.908673 walt-vpn-8.0/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:09.908673 walt-vpn-8.0/walt/vpn/
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      392 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/authtool.py
--rwxr-xr-x   0 root         (0) root         (0)     6664 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/client.py
--rwxr-xr-x   0 root         (0) root         (0)       41 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/const.py
--rwxr-xr-x   0 root         (0) root         (0)      796 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:09.908673 walt-vpn-8.0/walt/vpn/ext/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/ext/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      458 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/ext/build.py
--rw-r--r--   0 root         (0) root         (0)    11428 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/ext/loops.c
--rwxr-xr-x   0 root         (0) root         (0)     2619 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:09.908673 walt-vpn-8.0/walt/vpn/setup/
--rwxr-xr-x   0 root         (0) root         (0)     1998 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/setup/S51waltvpnclient
--rwxr-xr-x   0 root         (0) root         (0)     1113 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1458 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/setup/user.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/setup/walt-vpn-server.service
--rw-r--r--   0 root         (0) root         (0)      120 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/setup/walt-vpn-server.socket
--rwxr-xr-x   0 root         (0) root         (0)     1670 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/ssh.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-06-21 15:19:09.000000 walt-vpn-8.0/walt/vpn/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:09.908673 walt-vpn-8.0/walt_vpn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      241 2023-06-23 07:38:09.000000 walt-vpn-8.0/walt_vpn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-23 07:38:09.000000 walt-vpn-8.0/walt_vpn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:09.000000 walt-vpn-8.0/walt_vpn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-23 07:38:09.000000 walt-vpn-8.0/walt_vpn.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-23 07:38:09.000000 walt-vpn-8.0/walt_vpn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:09.000000 walt-vpn-8.0/walt_vpn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:16.191971 walt-vpn-8.1/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 15:19:09.000000 walt-vpn-8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      241 2023-06-26 14:05:16.191971 walt-vpn-8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-06-21 15:19:09.000000 walt-vpn-8.1/README.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-26 14:05:16.191971 walt-vpn-8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-06-26 14:05:03.000000 walt-vpn-8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:16.191971 walt-vpn-8.1/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:16.191971 walt-vpn-8.1/walt/vpn/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      392 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/authtool.py
+-rwxr-xr-x   0 root         (0) root         (0)     6664 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/client.py
+-rwxr-xr-x   0 root         (0) root         (0)       41 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/const.py
+-rwxr-xr-x   0 root         (0) root         (0)      796 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:16.191971 walt-vpn-8.1/walt/vpn/ext/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/ext/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      458 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/ext/build.py
+-rw-r--r--   0 root         (0) root         (0)    11428 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/ext/loops.c
+-rwxr-xr-x   0 root         (0) root         (0)     2619 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:16.191971 walt-vpn-8.1/walt/vpn/setup/
+-rwxr-xr-x   0 root         (0) root         (0)     1998 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/setup/S51waltvpnclient
+-rwxr-xr-x   0 root         (0) root         (0)     1113 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/setup/user.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/setup/walt-vpn-server.service
+-rw-r--r--   0 root         (0) root         (0)      120 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/setup/walt-vpn-server.socket
+-rwxr-xr-x   0 root         (0) root         (0)     1670 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-06-21 15:19:09.000000 walt-vpn-8.1/walt/vpn/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:16.191971 walt-vpn-8.1/walt_vpn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-06-26 14:05:16.000000 walt-vpn-8.1/walt_vpn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-26 14:05:16.000000 walt-vpn-8.1/walt_vpn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:05:16.000000 walt-vpn-8.1/walt_vpn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-26 14:05:16.000000 walt-vpn-8.1/walt_vpn.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-26 14:05:16.000000 walt-vpn-8.1/walt_vpn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 14:05:16.000000 walt-vpn-8.1/walt_vpn.egg-info/top_level.txt
```

### Comparing `walt-vpn-8.0/setup.py` & `walt-vpn-8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from setuptools import find_packages, setup
 
 if sys.version_info[0] == 2:
     sys.exit("Sorry, Python 2 is no longer supported.")
 
 setup_info = {
     "name": "walt-vpn",
-    "version": "8.0",
-    "install_requires": ["walt-common==8.0", "python-daemon<3", "cffi>=1.0.0"],
+    "version": "8.1",
+    "install_requires": ["walt-common==8.1", "python-daemon<3", "cffi>=1.0.0"],
     "author": "WalT developers",
     "author_email": "walt-contact@univ-grenoble-alpes.fr",
     "keywords": "WalT testbed",
     "license": "3-Clause BSD",
     "url": "https://walt-project.liglab.fr",
     "cffi_modules": ["walt/vpn/ext/build.py:ffibuilder"],
     "description": "WalT VPN components.",
```

### Comparing `walt-vpn-8.0/walt/vpn/client.py` & `walt-vpn-8.1/walt/vpn/client.py`

 * *Files identical despite different names*

### Comparing `walt-vpn-8.0/walt/vpn/endpoint.py` & `walt-vpn-8.1/walt/vpn/endpoint.py`

 * *Files identical despite different names*

### Comparing `walt-vpn-8.0/walt/vpn/ext/loops.c` & `walt-vpn-8.1/walt/vpn/ext/loops.c`

 * *Files identical despite different names*

### Comparing `walt-vpn-8.0/walt/vpn/server.py` & `walt-vpn-8.1/walt/vpn/server.py`

 * *Files identical despite different names*

### Comparing `walt-vpn-8.0/walt/vpn/setup/S51waltvpnclient` & `walt-vpn-8.1/walt/vpn/setup/S51waltvpnclient`

 * *Files identical despite different names*

### Comparing `walt-vpn-8.0/walt/vpn/setup/__init__.py` & `walt-vpn-8.1/walt/vpn/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `walt-vpn-8.0/walt/vpn/setup/user.py` & `walt-vpn-8.1/walt/vpn/setup/user.py`

 * *Files identical despite different names*

### Comparing `walt-vpn-8.0/walt/vpn/ssh.py` & `walt-vpn-8.1/walt/vpn/ssh.py`

 * *Files identical despite different names*

### Comparing `walt-vpn-8.0/walt/vpn/tools.py` & `walt-vpn-8.1/walt/vpn/tools.py`

 * *Files identical despite different names*

### Comparing `walt-vpn-8.0/walt_vpn.egg-info/SOURCES.txt` & `walt-vpn-8.1/walt_vpn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

