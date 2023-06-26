# Comparing `tmp/alibabacloud_btripopen20220520_py2-1.1.5.tar.gz` & `tmp/alibabacloud_btripopen20220520_py2-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.5.tar", last modified: Fri Jun 16 07:44:51 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.6.tar", last modified: Mon Jun 26 02:21:11 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520_py2-1.1.5.tar` & `alibabacloud_btripopen20220520_py2-1.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/
--rw-r--r--   0 root         (0) root         (0)     3417 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223404 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  2006169 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2933 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223404 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  2006565 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/setup.py
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.5/ChangeLog.md` & `alibabacloud_btripopen20220520_py2-1.1.6/ChangeLog.md`

 * *Files 0% similar despite different names*

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

### Comparing `alibabacloud_btripopen20220520_py2-1.1.5/LICENSE` & `alibabacloud_btripopen20220520_py2-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.5/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520_py2
-Version: 1.1.5
+Version: 1.1.6
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.5/README-CN.md` & `alibabacloud_btripopen20220520_py2-1.1.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.5/README.md` & `alibabacloud_btripopen20220520_py2-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -29634,37 +29634,47 @@
         m = m or dict()
         if m.get('dis_order_id') is not None:
             self.dis_order_id = m.get('dis_order_id')
         return self
 
 
 class HotelOrderCancelResponseBodyModule(TeaModel):
-    def __init__(self, cancel_success=None, forfeit_fee=None):
+    def __init__(self, cancel_success=None, code=None, desc=None, forfeit_fee=None):
         self.cancel_success = cancel_success  # type: bool
+        self.code = code  # type: str
+        self.desc = desc  # type: str
         self.forfeit_fee = forfeit_fee  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(HotelOrderCancelResponseBodyModule, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, message=None, module=None, request_id=None, success=None, trace_id=None):
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520-py2
-Version: 1.1.5
+Version: 1.1.6
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.5/setup.py` & `alibabacloud_btripopen20220520_py2-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520_py2.
 
-Created on 16/06/2023
+Created on 26/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python2"
```

