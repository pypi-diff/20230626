# Comparing `tmp/roblox-aio.py-1.0.1.tar.gz` & `tmp/roblox-aio.py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-aio.py-1.0.1.tar", last modified: Sun Jun 25 15:29:27 2023, max compression
+gzip compressed data, was "roblox-aio.py-1.0.2.tar", last modified: Sun Jun 25 16:08:34 2023, max compression
```

## Comparing `roblox-aio.py-1.0.1.tar` & `roblox-aio.py-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jess      (1001) users      (100)        0 2023-06-25 15:29:27.636380 roblox-aio.py-1.0.1/
--rw-r--r--   0 jess      (1001) users      (100)      249 2023-06-25 15:29:27.636380 roblox-aio.py-1.0.1/PKG-INFO
--rw-r--r--   0 jess      (1001) users      (100)       75 2023-04-27 15:19:24.000000 roblox-aio.py-1.0.1/README.md
-drwxr-xr-x   0 jess      (1001) users      (100)        0 2023-06-25 15:29:27.636380 roblox-aio.py-1.0.1/roblox_aio/
--rw-r--r--   0 jess      (1001) users      (100)      287 2023-04-27 15:19:24.000000 roblox-aio.py-1.0.1/roblox_aio/__init__.py
--rw-r--r--   0 jess      (1001) users      (100)      777 2023-06-25 15:19:46.000000 roblox-aio.py-1.0.1/roblox_aio/auth.py
--rw-r--r--   0 jess      (1001) users      (100)       74 2023-04-27 15:19:24.000000 roblox-aio.py-1.0.1/roblox_aio/endpoints.py
--rw-r--r--   0 jess      (1001) users      (100)      663 2023-06-25 15:20:11.000000 roblox-aio.py-1.0.1/roblox_aio/user.py
-drwxr-xr-x   0 jess      (1001) users      (100)        0 2023-06-25 15:29:27.636380 roblox-aio.py-1.0.1/roblox_aio.py.egg-info/
--rw-r--r--   0 jess      (1001) users      (100)      249 2023-06-25 15:29:27.000000 roblox-aio.py-1.0.1/roblox_aio.py.egg-info/PKG-INFO
--rw-r--r--   0 jess      (1001) users      (100)      287 2023-06-25 15:29:27.000000 roblox-aio.py-1.0.1/roblox_aio.py.egg-info/SOURCES.txt
--rw-r--r--   0 jess      (1001) users      (100)        1 2023-06-25 15:29:27.000000 roblox-aio.py-1.0.1/roblox_aio.py.egg-info/dependency_links.txt
--rw-r--r--   0 jess      (1001) users      (100)       14 2023-06-25 15:29:27.000000 roblox-aio.py-1.0.1/roblox_aio.py.egg-info/requires.txt
--rw-r--r--   0 jess      (1001) users      (100)       11 2023-06-25 15:29:27.000000 roblox-aio.py-1.0.1/roblox_aio.py.egg-info/top_level.txt
--rw-r--r--   0 jess      (1001) users      (100)       38 2023-06-25 15:29:27.636380 roblox-aio.py-1.0.1/setup.cfg
--rw-r--r--   0 jess      (1001) users      (100)      320 2023-06-25 15:28:53.000000 roblox-aio.py-1.0.1/setup.py
+drwxr-xr-x   0 jess      (1001) users      (100)        0 2023-06-25 16:08:34.631396 roblox-aio.py-1.0.2/
+-rw-r--r--   0 jess      (1001) users      (100)      633 2023-06-25 16:08:34.631396 roblox-aio.py-1.0.2/PKG-INFO
+-rw-r--r--   0 jess      (1001) users      (100)      271 2023-06-25 16:05:57.000000 roblox-aio.py-1.0.2/README.md
+drwxr-xr-x   0 jess      (1001) users      (100)        0 2023-06-25 16:08:34.627396 roblox-aio.py-1.0.2/roblox_aio/
+-rw-r--r--   0 jess      (1001) users      (100)      287 2023-04-27 15:19:24.000000 roblox-aio.py-1.0.2/roblox_aio/__init__.py
+-rw-r--r--   0 jess      (1001) users      (100)      777 2023-06-25 15:19:46.000000 roblox-aio.py-1.0.2/roblox_aio/auth.py
+-rw-r--r--   0 jess      (1001) users      (100)       74 2023-04-27 15:19:24.000000 roblox-aio.py-1.0.2/roblox_aio/endpoints.py
+-rw-r--r--   0 jess      (1001) users      (100)      663 2023-06-25 15:20:11.000000 roblox-aio.py-1.0.2/roblox_aio/user.py
+drwxr-xr-x   0 jess      (1001) users      (100)        0 2023-06-25 16:08:34.627396 roblox-aio.py-1.0.2/roblox_aio.py.egg-info/
+-rw-r--r--   0 jess      (1001) users      (100)      633 2023-06-25 16:08:34.000000 roblox-aio.py-1.0.2/roblox_aio.py.egg-info/PKG-INFO
+-rw-r--r--   0 jess      (1001) users      (100)      287 2023-06-25 16:08:34.000000 roblox-aio.py-1.0.2/roblox_aio.py.egg-info/SOURCES.txt
+-rw-r--r--   0 jess      (1001) users      (100)        1 2023-06-25 16:08:34.000000 roblox-aio.py-1.0.2/roblox_aio.py.egg-info/dependency_links.txt
+-rw-r--r--   0 jess      (1001) users      (100)       20 2023-06-25 16:08:34.000000 roblox-aio.py-1.0.2/roblox_aio.py.egg-info/requires.txt
+-rw-r--r--   0 jess      (1001) users      (100)       11 2023-06-25 16:08:34.000000 roblox-aio.py-1.0.2/roblox_aio.py.egg-info/top_level.txt
+-rw-r--r--   0 jess      (1001) users      (100)       38 2023-06-25 16:08:34.631396 roblox-aio.py-1.0.2/setup.cfg
+-rw-r--r--   0 jess      (1001) users      (100)      506 2023-06-25 16:08:12.000000 roblox-aio.py-1.0.2/setup.py
```

### Comparing `roblox-aio.py-1.0.1/roblox_aio/auth.py` & `roblox-aio.py-1.0.2/roblox_aio/auth.py`

 * *Files identical despite different names*

### Comparing `roblox-aio.py-1.0.1/roblox_aio/user.py` & `roblox-aio.py-1.0.2/roblox_aio/user.py`

 * *Files identical despite different names*

