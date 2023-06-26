# Comparing `tmp/SFM4300_readout-0.1.tar.gz` & `tmp/SFM4300_readout-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SFM4300_readout-0.1.tar", last modified: Mon Jun 26 09:24:47 2023, max compression
+gzip compressed data, was "SFM4300_readout-0.1.2.tar", last modified: Mon Jun 26 11:29:56 2023, max compression
```

## Comparing `SFM4300_readout-0.1.tar` & `SFM4300_readout-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,15 @@
-drwxrwxr-x   0 oscar     (1002) oscar     (1002)        0 2023-06-26 09:24:47.038289 SFM4300_readout-0.1/
--rw-rw-r--   0 oscar     (1002) oscar     (1002)      604 2023-06-26 09:24:47.038289 SFM4300_readout-0.1/PKG-INFO
--rw-rw-r--   0 oscar     (1002) oscar     (1002)      198 2023-06-26 09:00:47.714698 SFM4300_readout-0.1/README
-drwxrwxr-x   0 oscar     (1002) oscar     (1002)        0 2023-06-26 09:24:47.038289 SFM4300_readout-0.1/SFM4300_readout/
--rw-rw-r--   0 oscar     (1002) oscar     (1002)     1833 2023-06-26 08:47:58.270339 SFM4300_readout-0.1/SFM4300_readout/SensorInterface.py
--rw-rw-r--   0 oscar     (1002) oscar     (1002)       51 2023-06-26 08:58:25.424836 SFM4300_readout-0.1/SFM4300_readout/__init__.py
--rw-rw-r--   0 oscar     (1002) oscar     (1002)       40 2023-06-26 08:56:44.930350 SFM4300_readout-0.1/setup.cfg
--rw-rw-r--   0 oscar     (1002) oscar     (1002)      857 2023-06-26 09:13:03.970376 SFM4300_readout-0.1/setup.py
+drwxrwxr-x   0 oscar     (1002) oscar     (1002)        0 2023-06-26 11:29:56.483703 SFM4300_readout-0.1.2/
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)     1068 2023-06-26 08:09:04.000000 SFM4300_readout-0.1.2/LICENSE
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)      784 2023-06-26 11:29:56.479703 SFM4300_readout-0.1.2/PKG-INFO
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)      198 2023-06-26 09:00:47.000000 SFM4300_readout-0.1.2/README.md
+drwxrwxr-x   0 oscar     (1002) oscar     (1002)        0 2023-06-26 11:29:56.471703 SFM4300_readout-0.1.2/SFM4300_readout/
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)     1833 2023-06-26 08:47:58.000000 SFM4300_readout-0.1.2/SFM4300_readout/SensorInterface.py
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)       51 2023-06-26 08:58:25.000000 SFM4300_readout-0.1.2/SFM4300_readout/__init__.py
+drwxrwxr-x   0 oscar     (1002) oscar     (1002)        0 2023-06-26 11:29:56.479703 SFM4300_readout-0.1.2/SFM4300_readout.egg-info/
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)      784 2023-06-26 11:29:56.000000 SFM4300_readout-0.1.2/SFM4300_readout.egg-info/PKG-INFO
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)      289 2023-06-26 11:29:56.000000 SFM4300_readout-0.1.2/SFM4300_readout.egg-info/SOURCES.txt
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)        1 2023-06-26 11:29:56.000000 SFM4300_readout-0.1.2/SFM4300_readout.egg-info/dependency_links.txt
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)       26 2023-06-26 11:29:56.000000 SFM4300_readout-0.1.2/SFM4300_readout.egg-info/requires.txt
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)       16 2023-06-26 11:29:56.000000 SFM4300_readout-0.1.2/SFM4300_readout.egg-info/top_level.txt
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)      719 2023-06-26 11:29:32.000000 SFM4300_readout-0.1.2/pyproject.toml
+-rw-rw-r--   0 oscar     (1002) oscar     (1002)       38 2023-06-26 11:29:56.483703 SFM4300_readout-0.1.2/setup.cfg
```

### Comparing `SFM4300_readout-0.1/SFM4300_readout/SensorInterface.py` & `SFM4300_readout-0.1.2/SFM4300_readout/SensorInterface.py`

 * *Files identical despite different names*

