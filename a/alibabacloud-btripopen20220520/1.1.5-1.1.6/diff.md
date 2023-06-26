# Comparing `tmp/alibabacloud_btripopen20220520-1.1.5.tar.gz` & `tmp/alibabacloud_btripopen20220520-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.5.tar", last modified: Fri Jun 16 07:45:17 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.6.tar", last modified: Mon Jun 26 02:21:41 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520-1.1.5.tar` & `alibabacloud_btripopen20220520-1.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/
--rw-r--r--   0 root         (0) root         (0)     3543 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   525626 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  1984083 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2023-06-16 07:45:17.000000 alibabacloud_btripopen20220520-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)     3580 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   525626 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  1984483 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/setup.py
```

### Comparing `alibabacloud_btripopen20220520-1.1.5/ChangeLog.md` & `alibabacloud_btripopen20220520-1.1.6/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-16 Version: 1.1.5
+- Update.
+
 2023-06-15 Version: 1.1.4
 - Update.
 
 2023-06-12 Version: 1.1.3
 - Update.
 
 2023-06-09 Version: 1.1.2
```

### Comparing `alibabacloud_btripopen20220520-1.1.5/LICENSE` & `alibabacloud_btripopen20220520-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.5/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520
-Version: 1.1.5
+Version: 1.1.6
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.5/README-CN.md` & `alibabacloud_btripopen20220520-1.1.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.5/README.md` & `alibabacloud_btripopen20220520-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -33757,38 +33757,50 @@
         return self
 
 
 class HotelOrderCancelResponseBodyModule(TeaModel):
     def __init__(
         self,
         cancel_success: bool = None,
+        code: str = None,
+        desc: str = None,
         forfeit_fee: int = None,
     ):
         self.cancel_success = cancel_success
+        self.code = code
+        self.desc = desc
         self.forfeit_fee = forfeit_fee
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.cancel_success is not None:
             result['cancel_success'] = self.cancel_success
+        if self.code is not None:
+            result['code'] = self.code
+        if self.desc is not None:
+            result['desc'] = self.desc
         if self.forfeit_fee is not None:
             result['forfeit_fee'] = self.forfeit_fee
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('cancel_success') is not None:
             self.cancel_success = m.get('cancel_success')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('desc') is not None:
+            self.desc = m.get('desc')
         if m.get('forfeit_fee') is not None:
             self.forfeit_fee = m.get('forfeit_fee')
         return self
 
 
 class HotelOrderCancelResponseBody(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_btripopen20220520-1.1.5/alibabacloud_btripopen20220520.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520
-Version: 1.1.5
+Version: 1.1.6
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.5/setup.py` & `alibabacloud_btripopen20220520-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520.
 
-Created on 16/06/2023
+Created on 26/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python"
```

