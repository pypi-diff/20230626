# Comparing `tmp/dcentrapi-0.2.6.tar.gz` & `tmp/dcentrapi-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.6.tar", last modified: Mon Jun 26 07:56:13 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.7.tar", last modified: Mon Jun 26 11:29:44 2023, max compression
```

## Comparing `dcentrapi-0.2.6.tar` & `dcentrapi-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 07:56:13.505123 dcentrapi-0.2.6/
--rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.2.6/LICENSE.rst
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 07:56:13.504991 dcentrapi-0.2.6/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.2.6/README.md
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 07:56:13.504110 dcentrapi-0.2.6/dcentrapi/
--rw-r--r--   0 oded       (502) staff       (20)      829 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/Base.py
--rw-r--r--   0 oded       (502) staff       (20)      280 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/__init__.py
--rw-r--r--   0 oded       (502) staff       (20)      195 2023-06-26 06:53:05.000000 dcentrapi-0.2.6/dcentrapi/common.py
--rw-r--r--   0 oded       (502) staff       (20)     8714 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/eventPolling.py
--rw-r--r--   0 oded       (502) staff       (20)      491 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/gasMonitor.py
--rw-r--r--   0 oded       (502) staff       (20)      527 2023-06-26 06:53:05.000000 dcentrapi-0.2.6/dcentrapi/hackMitigation.py
--rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.2.6/dcentrapi/merkleTree.py
--rw-r--r--   0 oded       (502) staff       (20)     3059 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/rpcAggregation.py
--rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.2.6/dcentrapi/test.py
--rw-r--r--   0 oded       (502) staff       (20)      804 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/web3Index.py
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 07:56:13.504809 dcentrapi-0.2.6/dcentrapi.egg-info/
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)      425 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 oded       (502) staff       (20)        1 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 oded       (502) staff       (20)        9 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 oded       (502) staff       (20)       10 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 oded       (502) staff       (20)       38 2023-06-26 07:56:13.505161 dcentrapi-0.2.6/setup.cfg
--rw-r--r--   0 oded       (502) staff       (20)     1167 2022-12-21 09:08:31.000000 dcentrapi-0.2.6/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 11:29:44.664819 dcentrapi-0.2.7/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.2.7/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 11:29:44.664679 dcentrapi-0.2.7/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.2.7/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 11:29:44.663535 dcentrapi-0.2.7/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      829 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      332 2023-06-26 08:03:23.000000 dcentrapi-0.2.7/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)      195 2023-06-26 08:04:49.000000 dcentrapi-0.2.7/dcentrapi/common.py
+-rw-r--r--   0 oded       (502) staff       (20)     8714 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      491 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)      527 2023-06-26 06:53:05.000000 dcentrapi-0.2.7/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.2.7/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)     3059 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.2.7/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)      804 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 11:29:44.664489 dcentrapi-0.2.7/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      425 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-06-26 11:29:44.664864 dcentrapi-0.2.7/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1167 2022-12-21 09:08:31.000000 dcentrapi-0.2.7/setup.py
```

### Comparing `dcentrapi-0.2.6/LICENSE.rst` & `dcentrapi-0.2.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.6/PKG-INFO` & `dcentrapi-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.6
+Version: 0.2.7
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.2.6/README.md` & `dcentrapi-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.6/dcentrapi/Base.py` & `dcentrapi-0.2.7/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.6/dcentrapi/eventPolling.py` & `dcentrapi-0.2.7/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.6/dcentrapi/hackMitigation.py` & `dcentrapi-0.2.7/dcentrapi/hackMitigation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.6/dcentrapi/merkleTree.py` & `dcentrapi-0.2.7/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.6/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.7/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.6/dcentrapi/test.py` & `dcentrapi-0.2.7/dcentrapi/test.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.6/dcentrapi/web3Index.py` & `dcentrapi-0.2.7/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.6/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.7/dcentrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.6
+Version: 0.2.7
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.2.6/setup.py` & `dcentrapi-0.2.7/setup.py`

 * *Files identical despite different names*

