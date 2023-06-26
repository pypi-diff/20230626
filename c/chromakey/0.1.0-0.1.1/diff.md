# Comparing `tmp/chromakey-0.1.0.tar.gz` & `tmp/chromakey-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromakey-0.1.0.tar", last modified: Mon Jun 26 14:24:31 2023, max compression
+gzip compressed data, was "chromakey-0.1.1.tar", last modified: Mon Jun 26 14:33:41 2023, max compression
```

## Comparing `chromakey-0.1.0.tar` & `chromakey-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 wteoh     (1000) wteoh     (1000)        0 2023-06-26 14:24:31.953028 chromakey-0.1.0/
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)     1068 2023-06-26 14:23:28.000000 chromakey-0.1.0/LICENSE
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)       75 2023-06-26 14:24:31.953028 chromakey-0.1.0/PKG-INFO
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)      293 2023-06-26 14:23:28.000000 chromakey-0.1.0/README.md
-drwxrwxr-x   0 wteoh     (1000) wteoh     (1000)        0 2023-06-26 14:24:31.953028 chromakey-0.1.0/chromakey/
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)        0 2023-06-26 14:23:28.000000 chromakey-0.1.0/chromakey/__init__.py
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)     1333 2023-06-26 14:23:28.000000 chromakey-0.1.0/chromakey/core.py
-drwxrwxr-x   0 wteoh     (1000) wteoh     (1000)        0 2023-06-26 14:24:31.953028 chromakey-0.1.0/chromakey.egg-info/
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)       75 2023-06-26 14:24:31.000000 chromakey-0.1.0/chromakey.egg-info/PKG-INFO
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)      230 2023-06-26 14:24:31.000000 chromakey-0.1.0/chromakey.egg-info/SOURCES.txt
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)        1 2023-06-26 14:24:31.000000 chromakey-0.1.0/chromakey.egg-info/dependency_links.txt
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)       19 2023-06-26 14:24:31.000000 chromakey-0.1.0/chromakey.egg-info/requires.txt
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)       10 2023-06-26 14:24:31.000000 chromakey-0.1.0/chromakey.egg-info/top_level.txt
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)       38 2023-06-26 14:24:31.953028 chromakey-0.1.0/setup.cfg
--rw-rw-r--   0 wteoh     (1000) wteoh     (1000)      178 2023-06-26 14:23:28.000000 chromakey-0.1.0/setup.py
+drwxrwxr-x   0 wteoh     (1000) wteoh     (1000)        0 2023-06-26 14:33:41.786825 chromakey-0.1.1/
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)     1068 2023-06-26 14:23:28.000000 chromakey-0.1.1/LICENSE
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)      528 2023-06-26 14:33:41.786825 chromakey-0.1.1/PKG-INFO
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)      293 2023-06-26 14:23:28.000000 chromakey-0.1.1/README.md
+drwxrwxr-x   0 wteoh     (1000) wteoh     (1000)        0 2023-06-26 14:33:41.782825 chromakey-0.1.1/chromakey/
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)        0 2023-06-26 14:23:28.000000 chromakey-0.1.1/chromakey/__init__.py
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)     1333 2023-06-26 14:23:28.000000 chromakey-0.1.1/chromakey/core.py
+drwxrwxr-x   0 wteoh     (1000) wteoh     (1000)        0 2023-06-26 14:33:41.786825 chromakey-0.1.1/chromakey.egg-info/
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)      528 2023-06-26 14:33:41.000000 chromakey-0.1.1/chromakey.egg-info/PKG-INFO
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)      230 2023-06-26 14:33:41.000000 chromakey-0.1.1/chromakey.egg-info/SOURCES.txt
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)        1 2023-06-26 14:33:41.000000 chromakey-0.1.1/chromakey.egg-info/dependency_links.txt
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)       19 2023-06-26 14:33:41.000000 chromakey-0.1.1/chromakey.egg-info/requires.txt
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)       10 2023-06-26 14:33:41.000000 chromakey-0.1.1/chromakey.egg-info/top_level.txt
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)       38 2023-06-26 14:33:41.786825 chromakey-0.1.1/setup.cfg
+-rw-rw-r--   0 wteoh     (1000) wteoh     (1000)      572 2023-06-26 14:33:07.000000 chromakey-0.1.1/setup.py
```

### Comparing `chromakey-0.1.0/LICENSE` & `chromakey-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chromakey-0.1.0/chromakey/core.py` & `chromakey-0.1.1/chromakey/core.py`

 * *Files identical despite different names*

