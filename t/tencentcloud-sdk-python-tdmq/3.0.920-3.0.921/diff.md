# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.920.tar", last modified: Thu Jun 22 00:36:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.921.tar", last modified: Mon Jun 26 00:34:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.920.tar` & `tencentcloud-sdk-python-tdmq-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   405597 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   110163 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-22 00:36:32.000000 tencentcloud-sdk-python-tdmq-3.0.920/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   405597 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   110163 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-26 00:34:07.000000 tencentcloud-sdk-python-tdmq-3.0.921/setup.py
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.920'
+__version__ = '3.0.921'
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1722,15 +1722,15 @@
 class CreateCmqQueueRequest(AbstractModel):
     """CreateCmqQueue请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param QueueName: 队列名字，在单个地域同一帐号下唯一。队列名称是一个不超过 64 个字符的字符串，必须以字母为首字符，剩余部分可以包含字母、数字和横划线(-)。
+        :param QueueName: 队列名字，在单个地域同一账号下唯一。队列名称是一个不超过 64 个字符的字符串，必须以字母为首字符，剩余部分可以包含字母、数字和横划线(-)。
         :type QueueName: str
         :param MaxMsgHeapNum: 最大堆积消息数。取值范围在公测期间为 1,000,000 - 10,000,000，正式上线后范围可达到 1000,000-1000,000,000。默认取值在公测期间为 10,000,000，正式上线后为 100,000,000。
         :type MaxMsgHeapNum: int
         :param PollingWaitSeconds: 消息接收长轮询等待时间。取值范围 0-30 秒，默认值 0。
         :type PollingWaitSeconds: int
         :param VisibilityTimeout: 消息可见性超时。取值范围 1-43200 秒（即12小时内），默认值 30。
         :type VisibilityTimeout: int
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.920/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.921/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.920/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.921/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.920/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.921/setup.py`

 * *Files identical despite different names*

