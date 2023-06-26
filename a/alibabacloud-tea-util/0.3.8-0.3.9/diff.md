# Comparing `tmp/alibabacloud_tea_util-0.3.8.tar.gz` & `tmp/alibabacloud_tea_util-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_tea_util-0.3.8.tar", last modified: Wed Nov 16 10:00:06 2022, max compression
+gzip compressed data, was "dist/alibabacloud_tea_util-0.3.9.tar", last modified: Mon Jun 26 10:16:10 2023, max compression
```

## Comparing `alibabacloud_tea_util-0.3.8.tar` & `alibabacloud_tea_util-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/
--rw-r--r--   0 root         (0) root         (0)     1987 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      937 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util/
--rw-r--r--   0 root         (0) root         (0)       23 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12621 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util/client.py
--rw-r--r--   0 root         (0) root         (0)     5536 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1987 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      340 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/alibabacloud_tea_util.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2288 2022-11-16 10:00:06.000000 alibabacloud_tea_util-0.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      937 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13018 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util/client.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      340 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/alibabacloud_tea_util.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-06-26 10:16:10.000000 alibabacloud_tea_util-0.3.9/setup.py
```

### Comparing `alibabacloud_tea_util-0.3.8/PKG-INFO` & `alibabacloud_tea_util-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: alibabacloud_tea_util
-Version: 0.3.8
+Version: 0.3.9
 Summary: The tea-util module of alibabaCloud Python SDK.
 Home-page: https://github.com/aliyun/tea-util/tree/master/python
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tea_util-0.3.8/README.md` & `alibabacloud_tea_util-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tea_util-0.3.8/alibabacloud_tea_util/client.py` & `alibabacloud_tea_util-0.3.9/alibabacloud_tea_util/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,17 @@
     ) -> str:
         """
         Stringify a value by JSON format
         @return: the JSON format string
         """
         if isinstance(val, str):
             return str(val)
-        return json.dumps(val, cls=Client.__ModelEncoder)
+        return json.dumps(
+            val, cls=Client.__ModelEncoder, ensure_ascii=False, separators=(",", ":")
+        )
 
     @staticmethod
     def empty(
         val: str,
     ) -> bool:
         """
         Check the string is empty?
@@ -341,14 +343,26 @@
         @return: the number value
         """
         if not isinstance(value, (int, float)):
             raise ValueError(f'{value} is not a number')
         return value
 
     @staticmethod
+    def assert_as_integer(
+        value: Any,
+    ) -> int:
+        """
+        Assert a value, if it is a integer, return it, otherwise throws
+        @return: the integer value
+        """
+        if not isinstance(value, int):
+            raise ValueError(f'{value} is not a int number')
+        return value
+
+    @staticmethod
     def assert_as_map(
         value: Any,
     ) -> Dict[str, Any]:
         """
         Assert a value, if it is a map, return it, otherwise throws
         @return: the map value
         """
```

### Comparing `alibabacloud_tea_util-0.3.8/alibabacloud_tea_util/models.py` & `alibabacloud_tea_util-0.3.9/alibabacloud_tea_util/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_tea_util-0.3.8/alibabacloud_tea_util.egg-info/PKG-INFO` & `alibabacloud_tea_util-0.3.9/alibabacloud_tea_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: alibabacloud-tea-util
-Version: 0.3.8
+Version: 0.3.9
 Summary: The tea-util module of alibabaCloud Python SDK.
 Home-page: https://github.com/aliyun/tea-util/tree/master/python
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tea_util-0.3.8/setup.py` & `alibabacloud_tea_util-0.3.9/setup.py`

 * *Files identical despite different names*

