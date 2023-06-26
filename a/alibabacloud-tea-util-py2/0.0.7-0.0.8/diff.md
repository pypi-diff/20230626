# Comparing `tmp/alibabacloud_tea_util_py2-0.0.7.tar.gz` & `tmp/alibabacloud_tea_util_py2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_tea_util_py2-0.0.7.tar", last modified: Wed Nov 16 10:00:10 2022, max compression
+gzip compressed data, was "dist/alibabacloud_tea_util_py2-0.0.8.tar", last modified: Mon Jun 26 10:16:14 2023, max compression
```

## Comparing `alibabacloud_tea_util_py2-0.0.7.tar` & `alibabacloud_tea_util_py2-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     1826 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      943 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util/
--rw-r--r--   0 root         (0) root         (0)       23 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10239 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util/client.py
--rw-r--r--   0 root         (0) root         (0)     5526 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1826 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      360 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2197 2022-11-16 10:00:10.000000 alibabacloud_tea_util_py2-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      943 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10629 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/client.py
+-rw-r--r--   0 root         (0) root         (0)     5526 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      360 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-06-26 10:16:14.000000 alibabacloud_tea_util_py2-0.0.8/setup.py
```

### Comparing `alibabacloud_tea_util_py2-0.0.7/PKG-INFO` & `alibabacloud_tea_util_py2-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud_tea_util_py2
-Version: 0.0.7
+Version: 0.0.8
 Summary: The tea-util module of alibabaCloud Python2 SDK.
 Home-page: https://github.com/aliyun/tea-util/tree/master/python2
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tea_util_py2-0.0.7/README.md` & `alibabacloud_tea_util_py2-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util/client.py` & `alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,16 +156,17 @@
     def to_jsonstring(val):
         """
         Stringify a value by JSON format
         @return: the JSON format string
         """
         if isinstance(val, str):
             return str(val)
-        return json.dumps(val, cls=Client._ModelEncoder)
-
+        return json.dumps(
+            val, cls=Client._ModelEncoder, ensure_ascii=False, separators=(",", ":")
+        )
     @staticmethod
     def empty(val):
         """
         Check the string is empty?
         @return: if string is null or zero length, return true
         """
         return not val
@@ -255,14 +256,24 @@
         @return: the number value
         """
         if not isinstance(value, TeaConverter.number):
             raise ValueError('%s is not a number' % TeaConverter.to_str(value))
         return value
 
     @staticmethod
+    def assert_as_integer(value):
+        """
+        Assert a value, if it is a number, return it, otherwise throws
+        @return: the number value
+        """
+        if not isinstance(value, int):
+            raise ValueError('%s is not a int number' % TeaConverter.to_str(value))
+        return value
+
+    @staticmethod
     def assert_as_map(value):
         """
         Assert a value, if it is a map, return it, otherwise throws
         @return: the map value
         """
         if not isinstance(value, dict):
             raise ValueError('%s is not a dict' % TeaConverter.to_str(value))
```

### Comparing `alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util/models.py` & `alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_tea_util_py2-0.0.7/alibabacloud_tea_util_py2.egg-info/PKG-INFO` & `alibabacloud_tea_util_py2-0.0.8/alibabacloud_tea_util_py2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud-tea-util-py2
-Version: 0.0.7
+Version: 0.0.8
 Summary: The tea-util module of alibabaCloud Python2 SDK.
 Home-page: https://github.com/aliyun/tea-util/tree/master/python2
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tea_util_py2-0.0.7/setup.py` & `alibabacloud_tea_util_py2-0.0.8/setup.py`

 * *Files identical despite different names*

