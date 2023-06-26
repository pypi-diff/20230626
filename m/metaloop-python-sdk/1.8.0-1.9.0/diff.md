# Comparing `tmp/metaloop-python-sdk-1.8.0.tar.gz` & `tmp/metaloop-python-sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaloop-python-sdk-1.8.0.tar", last modified: Thu Dec  8 06:53:21 2022, max compression
+gzip compressed data, was "metaloop-python-sdk-1.9.0.tar", last modified: Fri Dec  9 09:43:56 2022, max compression
```

## Comparing `metaloop-python-sdk-1.8.0.tar` & `metaloop-python-sdk-1.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 06:53:21.007799 metaloop-python-sdk-1.8.0/
--rw-r--r--   0 root         (0) root         (0)     3933 2022-12-08 06:53:21.007799 metaloop-python-sdk-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2256 2022-12-05 04:45:49.000000 metaloop-python-sdk-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 06:53:20.999799 metaloop-python-sdk-1.8.0/metaloop/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2022-12-08 06:53:20.000000 metaloop-python-sdk-1.8.0/metaloop/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 06:53:20.999799 metaloop-python-sdk-1.8.0/metaloop/client/
--rw-rw-rw-   0 root         (0) root         (0)      211 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12095 2022-12-01 04:59:04.000000 metaloop-python-sdk-1.8.0/metaloop/client/cloud_storage.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2022-12-01 04:59:04.000000 metaloop-python-sdk-1.8.0/metaloop/client/download_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     9565 2022-12-08 05:45:48.000000 metaloop-python-sdk-1.8.0/metaloop/client/mds.py
--rw-rw-rw-   0 root         (0) root         (0)     6547 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/client/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    11096 2022-12-07 06:57:06.000000 metaloop-python-sdk-1.8.0/metaloop/client/x_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 06:53:20.999799 metaloop-python-sdk-1.8.0/metaloop/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       88 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22951 2022-12-05 04:45:49.000000 metaloop-python-sdk-1.8.0/metaloop/dataset/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 06:53:21.003799 metaloop-python-sdk-1.8.0/metaloop/examples/
--rw-rw-rw-   0 root         (0) root         (0)       94 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2022-12-07 06:57:06.000000 metaloop-python-sdk-1.8.0/metaloop/examples/call_model_convert.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/examples/dataset_manage.py
--rw-rw-rw-   0 root         (0) root         (0)      640 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/examples/export_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1005 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/examples/import_data.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/examples/import_data_cos.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2022-12-05 04:45:49.000000 metaloop-python-sdk-1.8.0/metaloop/examples/iter_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/examples/s3_file_download.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2022-12-01 04:59:04.000000 metaloop-python-sdk-1.8.0/metaloop/examples/task_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     9565 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 06:53:21.003799 metaloop-python-sdk-1.8.0/metaloop/utils/
--rw-rw-rw-   0 root         (0) root         (0)      357 2022-11-02 13:08:17.000000 metaloop-python-sdk-1.8.0/metaloop/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3188 2022-11-02 13:08:17.000000 metaloop-python-sdk-1.8.0/metaloop/utils/file_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     8125 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/utils/log.py
--rw-rw-rw-   0 root         (0) root         (0)     7519 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.8.0/metaloop/utils/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2022-12-05 04:45:49.000000 metaloop-python-sdk-1.8.0/metaloop/utils/video.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 06:53:21.007799 metaloop-python-sdk-1.8.0/metaloop_python_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3933 2022-12-08 06:53:20.000000 metaloop-python-sdk-1.8.0/metaloop_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2022-12-08 06:53:20.000000 metaloop-python-sdk-1.8.0/metaloop_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-08 06:53:20.000000 metaloop-python-sdk-1.8.0/metaloop_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2022-12-08 06:53:20.000000 metaloop-python-sdk-1.8.0/metaloop_python_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-12-08 06:53:20.000000 metaloop-python-sdk-1.8.0/metaloop_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-08 06:53:21.007799 metaloop-python-sdk-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1460 2022-12-08 06:53:20.000000 metaloop-python-sdk-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 09:43:56.269277 metaloop-python-sdk-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)     4008 2022-12-09 09:43:56.269277 metaloop-python-sdk-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2323 2022-12-09 09:43:38.000000 metaloop-python-sdk-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 09:43:56.265277 metaloop-python-sdk-1.9.0/metaloop/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2022-12-09 09:43:55.000000 metaloop-python-sdk-1.9.0/metaloop/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 09:43:56.265277 metaloop-python-sdk-1.9.0/metaloop/client/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12095 2022-12-01 04:59:04.000000 metaloop-python-sdk-1.9.0/metaloop/client/cloud_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2022-12-01 04:59:04.000000 metaloop-python-sdk-1.9.0/metaloop/client/download_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9565 2022-12-08 05:45:48.000000 metaloop-python-sdk-1.9.0/metaloop/client/mds.py
+-rw-rw-rw-   0 root         (0) root         (0)     6547 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/client/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    11096 2022-12-07 06:57:06.000000 metaloop-python-sdk-1.9.0/metaloop/client/x_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 09:43:56.265277 metaloop-python-sdk-1.9.0/metaloop/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22951 2022-12-05 04:45:49.000000 metaloop-python-sdk-1.9.0/metaloop/dataset/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 09:43:56.269277 metaloop-python-sdk-1.9.0/metaloop/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2022-12-07 06:57:06.000000 metaloop-python-sdk-1.9.0/metaloop/examples/call_model_convert.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/examples/dataset_manage.py
+-rw-rw-rw-   0 root         (0) root         (0)      640 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/examples/export_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/examples/import_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/examples/import_data_cos.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2022-12-05 04:45:49.000000 metaloop-python-sdk-1.9.0/metaloop/examples/iter_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/examples/s3_file_download.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2022-12-01 04:59:04.000000 metaloop-python-sdk-1.9.0/metaloop/examples/task_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     9565 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 09:43:56.269277 metaloop-python-sdk-1.9.0/metaloop/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2022-11-02 13:08:17.000000 metaloop-python-sdk-1.9.0/metaloop/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3188 2022-11-02 13:08:17.000000 metaloop-python-sdk-1.9.0/metaloop/utils/file_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     8125 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/utils/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     7519 2022-10-31 07:06:42.000000 metaloop-python-sdk-1.9.0/metaloop/utils/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2022-12-05 04:45:49.000000 metaloop-python-sdk-1.9.0/metaloop/utils/video.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 09:43:56.269277 metaloop-python-sdk-1.9.0/metaloop_python_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4008 2022-12-09 09:43:56.000000 metaloop-python-sdk-1.9.0/metaloop_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2022-12-09 09:43:56.000000 metaloop-python-sdk-1.9.0/metaloop_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-09 09:43:56.000000 metaloop-python-sdk-1.9.0/metaloop_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2022-12-09 09:43:56.000000 metaloop-python-sdk-1.9.0/metaloop_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-12-09 09:43:56.000000 metaloop-python-sdk-1.9.0/metaloop_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-09 09:43:56.269277 metaloop-python-sdk-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2022-12-09 09:43:55.000000 metaloop-python-sdk-1.9.0/setup.py
```

### Comparing `metaloop-python-sdk-1.8.0/PKG-INFO` & `metaloop-python-sdk-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaloop-python-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Deepglint Metaloop Python SDK
 Home-page: http://data.deepglint.com/
 Author: yuma
 Author-email: yuma@deepglint.com
 License: Apache License 2.0
 Project-URL: Documentation, https://gitlab.deepglint.com/metaloop/metaloop-python-sdk
 Project-URL: Source, https://gitlab.deepglint.com/metaloop/metaloop-python-sdk
@@ -25,38 +25,39 @@
         ## Documentation
         
         More information can be found on the [examples](https://gitlab.deepglint.com/metaloop/metaloop-python-sdk/-/tree/dev/metaloop/examples)
         
         ## Usage
         生成API Token
         ```
-          在登录平台后，在浏览器中访问 http://192.168.100.71:30301/api/v1/api_token 即可获取本用户的token
+          在登录平台后，点击页面右上角的用户名，在个人信息页面中，即可获取本用户的API Token
           正式环境将http://192.168.100.71:30301 替换为 http://data.deepglint.com
         ```
         操作数据集
         ```python
         import time
         
         from metaloop.client import MDS
         
         
         if __name__ == '__main__':
-            # 192.168.100.71 is test server
-            mds_client = MDS("0c02ca70e142b75a75ca4118ce33dbb0", "http://192.168.100.71:30301")
+            # use MDS("0c02ca70e142b75a75ca4118ce33dbb0", "http://192.168.100.71:30301") when connecting test-server
+            mds_client = MDS("0c02ca70e142b75a75ca4118ce33dbb0")
         
             date_time = time.strftime("%Y%m%d%H%M%S", time.localtime())
             dataset_name = f"test_dataset_{date_time}"
         
             # create new dataset
             dataset = mds_client.create_dataset(
                 dataset_name,
                 "image",
                 ["screw"],
                 comment="this is a test dataset for mds"
             )
+            # print dataset info
             dataset.summary()
             
             # get existed dataset
             dataset = mds_client.get_dataset(dataset_name)
             dataset.summary()
         
             # create version
```

### Comparing `metaloop-python-sdk-1.8.0/README.md` & `metaloop-python-sdk-1.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,38 +15,39 @@
 ## Documentation
 
 More information can be found on the [examples](https://gitlab.deepglint.com/metaloop/metaloop-python-sdk/-/tree/dev/metaloop/examples)
 
 ## Usage
 生成API Token
 ```
-  在登录平台后，在浏览器中访问 http://192.168.100.71:30301/api/v1/api_token 即可获取本用户的token
+  在登录平台后，点击页面右上角的用户名，在个人信息页面中，即可获取本用户的API Token
   正式环境将http://192.168.100.71:30301 替换为 http://data.deepglint.com
 ```
 操作数据集
 ```python
 import time
 
 from metaloop.client import MDS
 
 
 if __name__ == '__main__':
-    # 192.168.100.71 is test server
-    mds_client = MDS("0c02ca70e142b75a75ca4118ce33dbb0", "http://192.168.100.71:30301")
+    # use MDS("0c02ca70e142b75a75ca4118ce33dbb0", "http://192.168.100.71:30301") when connecting test-server
+    mds_client = MDS("0c02ca70e142b75a75ca4118ce33dbb0")
 
     date_time = time.strftime("%Y%m%d%H%M%S", time.localtime())
     dataset_name = f"test_dataset_{date_time}"
 
     # create new dataset
     dataset = mds_client.create_dataset(
         dataset_name,
         "image",
         ["screw"],
         comment="this is a test dataset for mds"
     )
+    # print dataset info
     dataset.summary()
     
     # get existed dataset
     dataset = mds_client.get_dataset(dataset_name)
     dataset.summary()
 
     # create version
```

### Comparing `metaloop-python-sdk-1.8.0/metaloop/client/cloud_storage.py` & `metaloop-python-sdk-1.9.0/metaloop/client/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/client/download_helper.py` & `metaloop-python-sdk-1.9.0/metaloop/client/download_helper.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/client/mds.py` & `metaloop-python-sdk-1.9.0/metaloop/client/mds.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/client/requests.py` & `metaloop-python-sdk-1.9.0/metaloop/client/requests.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/client/x_api.py` & `metaloop-python-sdk-1.9.0/metaloop/client/x_api.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/dataset/dataset.py` & `metaloop-python-sdk-1.9.0/metaloop/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/examples/call_model_convert.py` & `metaloop-python-sdk-1.9.0/metaloop/examples/call_model_convert.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/examples/dataset_manage.py` & `metaloop-python-sdk-1.9.0/metaloop/examples/dataset_manage.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/examples/export_data.py` & `metaloop-python-sdk-1.9.0/metaloop/examples/export_data.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/examples/import_data.py` & `metaloop-python-sdk-1.9.0/metaloop/examples/import_data.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/examples/iter_data.py` & `metaloop-python-sdk-1.9.0/metaloop/examples/iter_data.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/examples/s3_file_download.py` & `metaloop-python-sdk-1.9.0/metaloop/examples/s3_file_download.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/exception.py` & `metaloop-python-sdk-1.9.0/metaloop/exception.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/utils/file_helper.py` & `metaloop-python-sdk-1.9.0/metaloop/utils/file_helper.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/utils/log.py` & `metaloop-python-sdk-1.9.0/metaloop/utils/log.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/utils/requests.py` & `metaloop-python-sdk-1.9.0/metaloop/utils/requests.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop/utils/video.py` & `metaloop-python-sdk-1.9.0/metaloop/utils/video.py`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/metaloop_python_sdk.egg-info/PKG-INFO` & `metaloop-python-sdk-1.9.0/metaloop_python_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaloop-python-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Deepglint Metaloop Python SDK
 Home-page: http://data.deepglint.com/
 Author: yuma
 Author-email: yuma@deepglint.com
 License: Apache License 2.0
 Project-URL: Documentation, https://gitlab.deepglint.com/metaloop/metaloop-python-sdk
 Project-URL: Source, https://gitlab.deepglint.com/metaloop/metaloop-python-sdk
@@ -25,38 +25,39 @@
         ## Documentation
         
         More information can be found on the [examples](https://gitlab.deepglint.com/metaloop/metaloop-python-sdk/-/tree/dev/metaloop/examples)
         
         ## Usage
         生成API Token
         ```
-          在登录平台后，在浏览器中访问 http://192.168.100.71:30301/api/v1/api_token 即可获取本用户的token
+          在登录平台后，点击页面右上角的用户名，在个人信息页面中，即可获取本用户的API Token
           正式环境将http://192.168.100.71:30301 替换为 http://data.deepglint.com
         ```
         操作数据集
         ```python
         import time
         
         from metaloop.client import MDS
         
         
         if __name__ == '__main__':
-            # 192.168.100.71 is test server
-            mds_client = MDS("0c02ca70e142b75a75ca4118ce33dbb0", "http://192.168.100.71:30301")
+            # use MDS("0c02ca70e142b75a75ca4118ce33dbb0", "http://192.168.100.71:30301") when connecting test-server
+            mds_client = MDS("0c02ca70e142b75a75ca4118ce33dbb0")
         
             date_time = time.strftime("%Y%m%d%H%M%S", time.localtime())
             dataset_name = f"test_dataset_{date_time}"
         
             # create new dataset
             dataset = mds_client.create_dataset(
                 dataset_name,
                 "image",
                 ["screw"],
                 comment="this is a test dataset for mds"
             )
+            # print dataset info
             dataset.summary()
             
             # get existed dataset
             dataset = mds_client.get_dataset(dataset_name)
             dataset.summary()
         
             # create version
```

### Comparing `metaloop-python-sdk-1.8.0/metaloop_python_sdk.egg-info/SOURCES.txt` & `metaloop-python-sdk-1.9.0/metaloop_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaloop-python-sdk-1.8.0/setup.py` & `metaloop-python-sdk-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     's3transfer >= 0.5.2',
     'boto3 >= 1.16.25',
     'botocore >= 1.24.40',
 ]
 
 setup(
     name='metaloop-python-sdk',
-    version='1.8.0',
+    version='1.9.0',
     packages=find_packages(exclude=['tests*']),
     url='http://data.deepglint.com/',
     license='Apache License 2.0',
     author='yuma',
     author_email='yuma@deepglint.com',
     description='Deepglint Metaloop Python SDK',
     long_description_content_type='text/markdown',
```

