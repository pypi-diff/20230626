# Comparing `tmp/dcentrapi-0.2.7.tar.gz` & `tmp/dcentrapi-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.7.tar", last modified: Mon Jun 26 11:29:44 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.8.tar", last modified: Mon Jun 26 11:41:12 2023, max compression
```

## Comparing `dcentrapi-0.2.7.tar` & `dcentrapi-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 11:29:44.664819 dcentrapi-0.2.7/
--rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.2.7/LICENSE.rst
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 11:29:44.664679 dcentrapi-0.2.7/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.2.7/README.md
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 11:29:44.663535 dcentrapi-0.2.7/dcentrapi/
--rw-r--r--   0 oded       (502) staff       (20)      829 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/Base.py
--rw-r--r--   0 oded       (502) staff       (20)      332 2023-06-26 08:03:23.000000 dcentrapi-0.2.7/dcentrapi/__init__.py
--rw-r--r--   0 oded       (502) staff       (20)      195 2023-06-26 08:04:49.000000 dcentrapi-0.2.7/dcentrapi/common.py
--rw-r--r--   0 oded       (502) staff       (20)     8714 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/eventPolling.py
--rw-r--r--   0 oded       (502) staff       (20)      491 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/gasMonitor.py
--rw-r--r--   0 oded       (502) staff       (20)      527 2023-06-26 06:53:05.000000 dcentrapi-0.2.7/dcentrapi/hackMitigation.py
--rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.2.7/dcentrapi/merkleTree.py
--rw-r--r--   0 oded       (502) staff       (20)     3059 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/rpcAggregation.py
--rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.2.7/dcentrapi/test.py
--rw-r--r--   0 oded       (502) staff       (20)      804 2023-06-26 05:46:25.000000 dcentrapi-0.2.7/dcentrapi/web3Index.py
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 11:29:44.664489 dcentrapi-0.2.7/dcentrapi.egg-info/
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)      425 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 oded       (502) staff       (20)        1 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 oded       (502) staff       (20)        9 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 oded       (502) staff       (20)       10 2023-06-26 11:29:44.000000 dcentrapi-0.2.7/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 oded       (502) staff       (20)       38 2023-06-26 11:29:44.664864 dcentrapi-0.2.7/setup.cfg
--rw-r--r--   0 oded       (502) staff       (20)     1167 2022-12-21 09:08:31.000000 dcentrapi-0.2.7/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 11:41:12.333450 dcentrapi-0.2.8/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.2.8/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 11:41:12.333316 dcentrapi-0.2.8/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.2.8/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 11:41:12.332435 dcentrapi-0.2.8/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      829 2023-06-26 05:46:25.000000 dcentrapi-0.2.8/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      332 2023-06-26 08:03:23.000000 dcentrapi-0.2.8/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)      195 2023-06-26 11:41:10.000000 dcentrapi-0.2.8/dcentrapi/common.py
+-rw-r--r--   0 oded       (502) staff       (20)     8714 2023-06-26 05:46:25.000000 dcentrapi-0.2.8/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      491 2023-06-26 05:46:25.000000 dcentrapi-0.2.8/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)      525 2023-06-26 11:39:51.000000 dcentrapi-0.2.8/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.2.8/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)     3059 2023-06-26 05:46:25.000000 dcentrapi-0.2.8/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.2.8/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)      804 2023-06-26 05:46:25.000000 dcentrapi-0.2.8/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 11:41:12.333113 dcentrapi-0.2.8/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 11:41:12.000000 dcentrapi-0.2.8/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      425 2023-06-26 11:41:12.000000 dcentrapi-0.2.8/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-06-26 11:41:12.000000 dcentrapi-0.2.8/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-06-26 11:41:12.000000 dcentrapi-0.2.8/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-06-26 11:41:12.000000 dcentrapi-0.2.8/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-06-26 11:41:12.333489 dcentrapi-0.2.8/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1167 2022-12-21 09:08:31.000000 dcentrapi-0.2.8/setup.py
```

### Comparing `dcentrapi-0.2.7/LICENSE.rst` & `dcentrapi-0.2.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.7/PKG-INFO` & `dcentrapi-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.7
+Version: 0.2.8
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.2.7/README.md` & `dcentrapi-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.7/dcentrapi/Base.py` & `dcentrapi-0.2.8/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.7/dcentrapi/eventPolling.py` & `dcentrapi-0.2.8/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.7/dcentrapi/hackMitigation.py` & `dcentrapi-0.2.8/dcentrapi/hackMitigation.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 class HackMitigation(Base):
 
     def are_addresses_blacklisted(self, addresses: [str]):
         url = self.url + "generic_freeze_signal/are_addresses_blacklisted"
         data = {
             "addresses": addresses,
         }
-        response = requests.get(url, params=data, headers=self.headers)
+        response = requests.get(url, json=data, headers=self.headers)
         try:
             return response.json()
         except Exception as e:
             return DapiError(response=response, exception=e)
```

### Comparing `dcentrapi-0.2.7/dcentrapi/merkleTree.py` & `dcentrapi-0.2.8/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.7/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.8/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.7/dcentrapi/test.py` & `dcentrapi-0.2.8/dcentrapi/test.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.7/dcentrapi/web3Index.py` & `dcentrapi-0.2.8/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.7/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.8/dcentrapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.7
+Version: 0.2.8
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.2.7/setup.py` & `dcentrapi-0.2.8/setup.py`

 * *Files identical despite different names*

