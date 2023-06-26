# Comparing `tmp/walt-virtual-8.0.tar.gz` & `tmp/walt-virtual-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "walt-virtual-8.0.tar", last modified: Fri Jun 23 07:38:05 2023, max compression
+gzip compressed data, was "walt-virtual-8.1.tar", last modified: Mon Jun 26 14:05:11 2023, max compression
```

## Comparing `walt-virtual-8.0.tar` & `walt-virtual-8.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.324741 walt-virtual-8.0/
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-21 15:19:09.000000 walt-virtual-8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-23 07:38:05.324741 walt-virtual-8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      139 2022-03-29 14:58:03.000000 walt-virtual-8.0/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:05.324741 walt-virtual-8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      893 2023-06-23 07:37:56.000000 walt-virtual-8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/sh/
--rwxr-xr-x   0 root         (0) root         (0)       66 2023-06-21 15:19:09.000000 walt-virtual-8.0/sh/walt-vnode-ifdown
--rwxr-xr-x   0 root         (0) root         (0)      174 2023-06-21 15:19:09.000000 walt-virtual-8.0/sh/walt-vnode-ifup
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/walt/virtual/
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/walt/virtual/node/
--rwxr-xr-x   0 root         (0) root         (0)       58 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    16206 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/node.py
--rw-r--r--   0 root         (0) root         (0)     3359 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/udhcpc.py
--rwxr-xr-x   0 root         (0) root         (0)      889 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/walt-vnode-ifdown
--rwxr-xr-x   0 root         (0) root         (0)     2016 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/node/walt-vnode-ifup
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.320741 walt-virtual-8.0/walt/virtual/setup/
--rwxr-xr-x   0 root         (0) root         (0)     2215 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/setup/S52waltvirtualnode
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/setup/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      434 2023-06-21 15:19:09.000000 walt-virtual-8.0/walt/virtual/setup/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:05.324741 walt-virtual-8.0/walt_virtual.egg-info/
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      581 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:05.000000 walt-virtual-8.0/walt_virtual.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:11.584040 walt-virtual-8.1/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-21 15:19:09.000000 walt-virtual-8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-26 14:05:11.584040 walt-virtual-8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      139 2022-03-29 14:58:03.000000 walt-virtual-8.1/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 14:05:11.584040 walt-virtual-8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      893 2023-06-26 14:05:03.000000 walt-virtual-8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:11.584040 walt-virtual-8.1/sh/
+-rwxr-xr-x   0 root         (0) root         (0)       66 2023-06-21 15:19:09.000000 walt-virtual-8.1/sh/walt-vnode-ifdown
+-rwxr-xr-x   0 root         (0) root         (0)      174 2023-06-21 15:19:09.000000 walt-virtual-8.1/sh/walt-vnode-ifup
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:11.584040 walt-virtual-8.1/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:11.584040 walt-virtual-8.1/walt/virtual/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/virtual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:11.584040 walt-virtual-8.1/walt/virtual/node/
+-rwxr-xr-x   0 root         (0) root         (0)       58 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/virtual/node/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16206 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/virtual/node/node.py
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/virtual/node/udhcpc.py
+-rwxr-xr-x   0 root         (0) root         (0)      889 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/virtual/node/walt-vnode-ifdown
+-rwxr-xr-x   0 root         (0) root         (0)     2016 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/virtual/node/walt-vnode-ifup
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:11.584040 walt-virtual-8.1/walt/virtual/setup/
+-rwxr-xr-x   0 root         (0) root         (0)     2215 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/virtual/setup/S52waltvirtualnode
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/virtual/setup/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      434 2023-06-21 15:19:09.000000 walt-virtual-8.1/walt/virtual/setup/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:11.584040 walt-virtual-8.1/walt_virtual.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-26 14:05:11.000000 walt-virtual-8.1/walt_virtual.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      581 2023-06-26 14:05:11.000000 walt-virtual-8.1/walt_virtual.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:05:11.000000 walt-virtual-8.1/walt_virtual.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-26 14:05:11.000000 walt-virtual-8.1/walt_virtual.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-26 14:05:11.000000 walt-virtual-8.1/walt_virtual.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 14:05:11.000000 walt-virtual-8.1/walt_virtual.egg-info/top_level.txt
```

### Comparing `walt-virtual-8.0/setup.py` & `walt-virtual-8.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from setuptools import find_packages, setup
 
 if sys.version_info[0] == 2:
     sys.exit("Sorry, Python 2 is no longer supported.")
 
 setup_info = {
     "name": "walt-virtual",
-    "version": "8.0",
-    "install_requires": ["walt-common==8.0"],
+    "version": "8.1",
+    "install_requires": ["walt-common==8.1"],
     "author": "WalT developers",
     "author_email": "walt-contact@univ-grenoble-alpes.fr",
     "keywords": "WalT testbed",
     "license": "3-Clause BSD",
     "url": "https://walt-project.liglab.fr",
     "description": "WalT components related to virtualization.",
     "entry_points": {
```

### Comparing `walt-virtual-8.0/walt/virtual/node/node.py` & `walt-virtual-8.1/walt/virtual/node/node.py`

 * *Files identical despite different names*

### Comparing `walt-virtual-8.0/walt/virtual/node/udhcpc.py` & `walt-virtual-8.1/walt/virtual/node/udhcpc.py`

 * *Files identical despite different names*

### Comparing `walt-virtual-8.0/walt/virtual/node/walt-vnode-ifdown` & `walt-virtual-8.1/walt/virtual/node/walt-vnode-ifdown`

 * *Files identical despite different names*

### Comparing `walt-virtual-8.0/walt/virtual/node/walt-vnode-ifup` & `walt-virtual-8.1/walt/virtual/node/walt-vnode-ifup`

 * *Files identical despite different names*

### Comparing `walt-virtual-8.0/walt/virtual/setup/S52waltvirtualnode` & `walt-virtual-8.1/walt/virtual/setup/S52waltvirtualnode`

 * *Files identical despite different names*

### Comparing `walt-virtual-8.0/walt_virtual.egg-info/SOURCES.txt` & `walt-virtual-8.1/walt_virtual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

