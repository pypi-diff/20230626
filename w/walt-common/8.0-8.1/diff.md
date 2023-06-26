# Comparing `tmp/walt-common-8.0.tar.gz` & `tmp/walt-common-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "walt-common-8.0.tar", last modified: Fri Jun 23 07:38:01 2023, max compression
+gzip compressed data, was "walt-common-8.1.tar", last modified: Mon Jun 26 14:05:07 2023, max compression
```

## Comparing `walt-common-8.0.tar` & `walt-common-8.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-23 07:38:01.264801 walt-common-8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      144 2022-03-29 14:58:03.000000 walt-common-8.0/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:01.264801 walt-common-8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-23 07:37:56.000000 walt-common-8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.260801 walt-common-8.0/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-common-8.0/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt/common/
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/api.py
--rwxr-xr-x   0 root         (0) root         (0)    11877 2023-06-22 13:09:04.000000 walt-common-8.0/walt/common/apilink.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/busybox_init.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/config.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt/common/crypto/
--rw-r--r--   0 root         (0) root         (0)      833 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/crypto/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30717 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/crypto/blowfish.py
--rwxr-xr-x   0 root         (0) root         (0)     2289 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/crypto/dh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt/common/devices/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-common-8.0/walt/common/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/devices/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt/common/devices/switches/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/devices/switches/__init__.py
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/devices/switches/netgear.py
--rwxr-xr-x   0 root         (0) root         (0)    10436 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/evloop.py
--rw-r--r--   0 root         (0) root         (0)     9360 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/fakeipxe.py
--rwxr-xr-x   0 root         (0) root         (0)     2996 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/fifo.py
--rw-r--r--   0 root         (0) root         (0)     6734 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/formatting.py
--rwxr-xr-x   0 root         (0) root         (0)      960 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/io.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/logs.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/netsetup.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/reusable.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/service.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/settings.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/setup.py
--rw-r--r--   0 root         (0) root         (0)     5348 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/systemd.py
--rw-r--r--   0 root         (0) root         (0)     4096 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/tcp.py
--rwxr-xr-x   0 root         (0) root         (0)     3976 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/term.py
--rw-r--r--   0 root         (0) root         (0)     8286 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/tools.py
--rwxr-xr-x   0 root         (0) root         (0)      967 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/tty.py
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/udp.py
--rw-r--r--   0 root         (0) root         (0)     2629 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/unix.py
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-23 07:37:56.000000 walt-common-8.0/walt/common/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:07.496100 walt-common-8.1/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-26 14:05:07.496100 walt-common-8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      144 2022-03-29 14:58:03.000000 walt-common-8.1/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 14:05:07.496100 walt-common-8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-26 14:05:03.000000 walt-common-8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:07.492100 walt-common-8.1/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-common-8.1/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:07.496100 walt-common-8.1/walt/common/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/api.py
+-rwxr-xr-x   0 root         (0) root         (0)    11877 2023-06-22 13:09:04.000000 walt-common-8.1/walt/common/apilink.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/busybox_init.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:07.496100 walt-common-8.1/walt/common/crypto/
+-rw-r--r--   0 root         (0) root         (0)      833 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30717 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/crypto/blowfish.py
+-rwxr-xr-x   0 root         (0) root         (0)     2289 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/crypto/dh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:07.496100 walt-common-8.1/walt/common/devices/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-common-8.1/walt/common/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/devices/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:07.496100 walt-common-8.1/walt/common/devices/switches/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/devices/switches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/devices/switches/netgear.py
+-rwxr-xr-x   0 root         (0) root         (0)    10436 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/evloop.py
+-rw-r--r--   0 root         (0) root         (0)     9360 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/fakeipxe.py
+-rwxr-xr-x   0 root         (0) root         (0)     2996 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/fifo.py
+-rw-r--r--   0 root         (0) root         (0)     6734 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/formatting.py
+-rwxr-xr-x   0 root         (0) root         (0)      960 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/io.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/logs.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/netsetup.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/reusable.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/service.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/settings.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/setup.py
+-rw-r--r--   0 root         (0) root         (0)     5348 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/systemd.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/tcp.py
+-rwxr-xr-x   0 root         (0) root         (0)     3976 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/term.py
+-rw-r--r--   0 root         (0) root         (0)     8286 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/tools.py
+-rwxr-xr-x   0 root         (0) root         (0)      967 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/tty.py
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/udp.py
+-rw-r--r--   0 root         (0) root         (0)     2629 2023-06-21 15:19:09.000000 walt-common-8.1/walt/common/unix.py
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 14:05:03.000000 walt-common-8.1/walt/common/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:07.496100 walt-common-8.1/walt_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-26 14:05:07.000000 walt-common-8.1/walt_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-26 14:05:07.000000 walt-common-8.1/walt_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:05:07.000000 walt-common-8.1/walt_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-26 14:05:07.000000 walt-common-8.1/walt_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 14:05:07.000000 walt-common-8.1/walt_common.egg-info/top_level.txt
```

### Comparing `walt-common-8.0/setup.py` & `walt-common-8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 if sys.version_info[0] == 2:
     sys.exit("Sorry, Python 2 is no longer supported.")
 
 setup_info = {
     "name": "walt-common",
-    "version": "8.0",
+    "version": "8.1",
     "install_requires": [
         "plumbum>=1.7.2",
         "requests>=2.21.0",
         "python-dateutil>=2.8.1",
         "pyyaml>=5.3.1",
     ],
     "author": "WalT developers",
```

### Comparing `walt-common-8.0/walt/common/api.py` & `walt-common-8.1/walt/common/api.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/apilink.py` & `walt-common-8.1/walt/common/apilink.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/busybox_init.py` & `walt-common-8.1/walt/common/busybox_init.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/config.py` & `walt-common-8.1/walt/common/config.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/constants.py` & `walt-common-8.1/walt/common/constants.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/crypto/__init__.py` & `walt-common-8.1/walt/common/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/crypto/blowfish.py` & `walt-common-8.1/walt/common/crypto/blowfish.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/crypto/dh.py` & `walt-common-8.1/walt/common/crypto/dh.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/devices/registry.py` & `walt-common-8.1/walt/common/devices/registry.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/evloop.py` & `walt-common-8.1/walt/common/evloop.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/fakeipxe.py` & `walt-common-8.1/walt/common/fakeipxe.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/fifo.py` & `walt-common-8.1/walt/common/fifo.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/formatting.py` & `walt-common-8.1/walt/common/formatting.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/io.py` & `walt-common-8.1/walt/common/io.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/logs.py` & `walt-common-8.1/walt/common/logs.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/netsetup.py` & `walt-common-8.1/walt/common/netsetup.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/reusable.py` & `walt-common-8.1/walt/common/reusable.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/service.py` & `walt-common-8.1/walt/common/service.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/settings.py` & `walt-common-8.1/walt/common/settings.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/setup.py` & `walt-common-8.1/walt/common/setup.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/systemd.py` & `walt-common-8.1/walt/common/systemd.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/tcp.py` & `walt-common-8.1/walt/common/tcp.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/term.py` & `walt-common-8.1/walt/common/term.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/tools.py` & `walt-common-8.1/walt/common/tools.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/tty.py` & `walt-common-8.1/walt/common/tty.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt/common/unix.py` & `walt-common-8.1/walt/common/unix.py`

 * *Files identical despite different names*

### Comparing `walt-common-8.0/walt_common.egg-info/SOURCES.txt` & `walt-common-8.1/walt_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

