# Comparing `tmp/asyncio-oss-1.0.2.tar.gz` & `tmp/asyncio-oss-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio-oss-1.0.2.tar", last modified: Fri Jun 23 18:24:18 2023, max compression
+gzip compressed data, was "asyncio-oss-1.1.0.tar", last modified: Mon Jun 26 18:04:00 2023, max compression
```

## Comparing `asyncio-oss-1.0.2.tar` & `asyncio-oss-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-23 18:24:18.933663 asyncio-oss-1.0.2/
--rw-r--r--   0 longyao    (501) staff       (20)     1064 2023-05-24 15:02:54.000000 asyncio-oss-1.0.2/LICENSE
--rw-r--r--   0 longyao    (501) staff       (20)     2533 2023-06-23 18:24:18.933573 asyncio-oss-1.0.2/PKG-INFO
--rw-r--r--   0 longyao    (501) staff       (20)     2187 2023-06-23 18:21:23.000000 asyncio-oss-1.0.2/README.md
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-23 18:24:18.932575 asyncio-oss-1.0.2/asyncio_oss/
--rw-r--r--   0 longyao    (501) staff       (20)      435 2023-05-29 15:33:32.000000 asyncio-oss-1.0.2/asyncio_oss/__init__.py
--rw-r--r--   0 longyao    (501) staff       (20)   134427 2023-06-05 16:55:09.000000 asyncio-oss-1.0.2/asyncio_oss/api.py
--rw-r--r--   0 longyao    (501) staff       (20)     9063 2023-05-24 15:02:54.000000 asyncio-oss-1.0.2/asyncio_oss/exceptions.py
--rw-r--r--   0 longyao    (501) staff       (20)     6431 2023-06-05 16:55:09.000000 asyncio-oss-1.0.2/asyncio_oss/http.py
--rw-r--r--   0 longyao    (501) staff       (20)    13014 2023-06-23 18:07:43.000000 asyncio-oss-1.0.2/asyncio_oss/iterators.py
--rw-r--r--   0 longyao    (501) staff       (20)    80193 2023-05-24 15:02:54.000000 asyncio-oss-1.0.2/asyncio_oss/models.py
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-23 18:24:18.933421 asyncio-oss-1.0.2/asyncio_oss/test/
--rw-r--r--   0 longyao    (501) staff       (20)      554 2023-05-29 13:59:36.000000 asyncio-oss-1.0.2/asyncio_oss/test/__init__.py
--rw-r--r--   0 longyao    (501) staff       (20)     2550 2023-06-05 16:35:18.000000 asyncio-oss-1.0.2/asyncio_oss/test/object_test.py
--rw-r--r--   0 longyao    (501) staff       (20)      499 2023-06-23 17:51:40.000000 asyncio-oss-1.0.2/asyncio_oss/test/service_test.py
--rw-r--r--   0 longyao    (501) staff       (20)    26065 2023-05-24 15:02:54.000000 asyncio-oss-1.0.2/asyncio_oss/utils.py
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-23 18:24:18.933119 asyncio-oss-1.0.2/asyncio_oss.egg-info/
--rw-r--r--   0 longyao    (501) staff       (20)     2533 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/PKG-INFO
--rw-r--r--   0 longyao    (501) staff       (20)      451 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/SOURCES.txt
--rw-r--r--   0 longyao    (501) staff       (20)        1 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/dependency_links.txt
--rw-r--r--   0 longyao    (501) staff       (20)       13 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/requires.txt
--rw-r--r--   0 longyao    (501) staff       (20)       12 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/top_level.txt
--rw-r--r--   0 longyao    (501) staff       (20)       38 2023-06-23 18:24:18.933698 asyncio-oss-1.0.2/setup.cfg
--rw-r--r--   0 longyao    (501) staff       (20)      679 2023-06-23 18:21:23.000000 asyncio-oss-1.0.2/setup.py
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-26 18:04:00.209848 asyncio-oss-1.1.0/
+-rw-r--r--   0 longyao    (501) staff       (20)     1064 2023-05-24 15:02:54.000000 asyncio-oss-1.1.0/LICENSE
+-rw-r--r--   0 longyao    (501) staff       (20)     2944 2023-06-26 18:04:00.209755 asyncio-oss-1.1.0/PKG-INFO
+-rw-r--r--   0 longyao    (501) staff       (20)     2598 2023-06-26 18:02:55.000000 asyncio-oss-1.1.0/README.md
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-26 18:04:00.208317 asyncio-oss-1.1.0/asyncio_oss/
+-rw-r--r--   0 longyao    (501) staff       (20)      848 2023-06-26 17:53:43.000000 asyncio-oss-1.1.0/asyncio_oss/__init__.py
+-rw-r--r--   0 longyao    (501) staff       (20)   152258 2023-06-26 17:05:09.000000 asyncio-oss-1.1.0/asyncio_oss/api.py
+-rw-r--r--   0 longyao    (501) staff       (20)     9451 2023-06-26 14:59:28.000000 asyncio-oss-1.1.0/asyncio_oss/exceptions.py
+-rw-r--r--   0 longyao    (501) staff       (20)     6699 2023-06-26 17:30:19.000000 asyncio-oss-1.1.0/asyncio_oss/http.py
+-rw-r--r--   0 longyao    (501) staff       (20)    13081 2023-06-26 15:02:39.000000 asyncio-oss-1.1.0/asyncio_oss/iterators.py
+-rw-r--r--   0 longyao    (501) staff       (20)     4729 2023-06-26 17:31:59.000000 asyncio-oss-1.1.0/asyncio_oss/models.py
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-26 18:04:00.209478 asyncio-oss-1.1.0/asyncio_oss/test/
+-rw-r--r--   0 longyao    (501) staff       (20)      554 2023-05-29 13:59:36.000000 asyncio-oss-1.1.0/asyncio_oss/test/__init__.py
+-rw-r--r--   0 longyao    (501) staff       (20)     2550 2023-06-25 15:44:33.000000 asyncio-oss-1.1.0/asyncio_oss/test/object_test.py
+-rw-r--r--   0 longyao    (501) staff       (20)      499 2023-06-23 17:51:40.000000 asyncio-oss-1.1.0/asyncio_oss/test/service_test.py
+-rw-r--r--   0 longyao    (501) staff       (20)     5892 2023-06-26 17:30:19.000000 asyncio-oss-1.1.0/asyncio_oss/utils.py
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-26 18:04:00.208945 asyncio-oss-1.1.0/asyncio_oss.egg-info/
+-rw-r--r--   0 longyao    (501) staff       (20)     2944 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/PKG-INFO
+-rw-r--r--   0 longyao    (501) staff       (20)      451 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/SOURCES.txt
+-rw-r--r--   0 longyao    (501) staff       (20)        1 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/dependency_links.txt
+-rw-r--r--   0 longyao    (501) staff       (20)       13 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/requires.txt
+-rw-r--r--   0 longyao    (501) staff       (20)       12 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/top_level.txt
+-rw-r--r--   0 longyao    (501) staff       (20)       38 2023-06-26 18:04:00.209881 asyncio-oss-1.1.0/setup.cfg
+-rw-r--r--   0 longyao    (501) staff       (20)      679 2023-06-26 18:01:57.000000 asyncio-oss-1.1.0/setup.py
```

### Comparing `asyncio-oss-1.0.2/LICENSE` & `asyncio-oss-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.0.2/PKG-INFO` & `asyncio-oss-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio-oss
-Version: 1.0.2
+Version: 1.1.0
 Summary: An asynchronous python client SDK for OSS(Aliyun Object Storage Service).
 Home-page: https://github.com/Yaocool/async-oss
 Author: Ozzy
 Author-email: ozzycharon@gmail.com
 License: MIT
 Keywords: asyncio-oss,async-oss,oss
 Description-Content-Type: text/markdown
@@ -24,14 +24,16 @@
 $ git clone git@github.com:Yaocool/async-oss.git
 $ python setup.py bdist_wheel
 $ pip install ./dist/asyncio_oss-1.0.0-py3-none-any.whl
 ```
 
 # Example
 ```python
+import logging
+
 import asyncio_oss
 import asyncio
 import oss2
 
 OSS_ENDPOINT = 'https://oss-cn-hangzhou.aliyuncs.com'  # definition in https://help.aliyun.com/document_detail/31837.html
 OSS_KEY = '<Your AccessKeyID>'
 OSS_SECRET = '<Your AccessKeySecret>'
@@ -58,14 +60,17 @@
             print(obj.key)
 
         # Delete Object
         await bucket.delete_object(OBJECT_KEY)
 
 
 if __name__ == '__main__':
+    # open global log
+    log_file_path = "example_logfile.log"
+    asyncio_oss.set_file_logger(log_file_path, 'asyncio_oss', logging.DEBUG)
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
 # ChangeLogs
 * [Jul 29, 2022 - 1.0.0]
   * fix `http.py/do_request` method stream read bug
@@ -74,10 +79,15 @@
 * [May 30, 2023 - 1.0.1]
   * bump version to 1.0.1 for PyPI package description updating
 * [June 24, 2023 - 1.0.2]
   * remove unused fields add params in `asyncio_oss/http.py api.py` files
   * fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug
   * add `list_buckets` test case in `tests/service_test.py` for `Service` class
   * bump version to 1.0.2
+* [June 27, 2023 - 1.1.0]
+  * remove unused objects and methods in `asyncio_oss/models.py` and `asyncio_oss/utils.py` to streamline sdk package
+  * support oss2==2.18.0 newest apis
+  * support global log
+  * bump version to 1.1.0
 
-# Discussions
-Any questions can be raised in Discussions, I will answer them from time to time~
+# Discussions Or Issues
+Any questions can be raised in `Discussions` or `Issues`, I will answer them from time to time.
```

### Comparing `asyncio-oss-1.0.2/README.md` & `asyncio-oss-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 $ git clone git@github.com:Yaocool/async-oss.git
 $ python setup.py bdist_wheel
 $ pip install ./dist/asyncio_oss-1.0.0-py3-none-any.whl
 ```
 
 # Example
 ```python
+import logging
+
 import asyncio_oss
 import asyncio
 import oss2
 
 OSS_ENDPOINT = 'https://oss-cn-hangzhou.aliyuncs.com'  # definition in https://help.aliyun.com/document_detail/31837.html
 OSS_KEY = '<Your AccessKeyID>'
 OSS_SECRET = '<Your AccessKeySecret>'
@@ -46,14 +48,17 @@
             print(obj.key)
 
         # Delete Object
         await bucket.delete_object(OBJECT_KEY)
 
 
 if __name__ == '__main__':
+    # open global log
+    log_file_path = "example_logfile.log"
+    asyncio_oss.set_file_logger(log_file_path, 'asyncio_oss', logging.DEBUG)
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
 # ChangeLogs
 * [Jul 29, 2022 - 1.0.0]
   * fix `http.py/do_request` method stream read bug
@@ -62,10 +67,15 @@
 * [May 30, 2023 - 1.0.1]
   * bump version to 1.0.1 for PyPI package description updating
 * [June 24, 2023 - 1.0.2]
   * remove unused fields add params in `asyncio_oss/http.py api.py` files
   * fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug
   * add `list_buckets` test case in `tests/service_test.py` for `Service` class
   * bump version to 1.0.2
+* [June 27, 2023 - 1.1.0]
+  * remove unused objects and methods in `asyncio_oss/models.py` and `asyncio_oss/utils.py` to streamline sdk package
+  * support oss2==2.18.0 newest apis
+  * support global log
+  * bump version to 1.1.0
 
-# Discussions
-Any questions can be raised in Discussions, I will answer them from time to time~
+# Discussions Or Issues
+Any questions can be raised in `Discussions` or `Issues`, I will answer them from time to time.
```

### Comparing `asyncio-oss-1.0.2/asyncio_oss/api.py` & `asyncio-oss-1.1.0/asyncio_oss/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,50 +178,58 @@
     - FieldDelimiter: CSV列分隔符，最多支持一个字符
     - QuoteCharacter: CSV转移Quote符，最多支持一个字符
     - OverwriteIfExists: true|false. true表示重新获得csv meta，并覆盖原有的meta。一般情况下不需要使用
 
 """
 import time
 import shutil
-import logging
 
-from oss2.headers import *
-from oss2 import models
+from . import http, exceptions
+# GetObjectResult needs to calculate crc, but the data stream is asynchronous and cannot be read directly,
+# so the GetObjectResult object in asyncio-oss is used to satisfy the crc check calculation.
+from .models import GetObjectResult as AsyncGetObjectResult
+
+from oss2 import xml_utils, select_params, defaults, models, utils
+from oss2.compat import urlquote, urlparse, to_unicode, to_string
 from oss2.models import *
+from oss2.headers import *
 from oss2.select_params import *
-from oss2 import xml_utils, defaults
-from oss2.compat import urlparse, to_unicode
+import logging
 
-from . import http
-from . import exceptions
-from .models import GetObjectResult as AsyncGetObjectResult
 
 logger = logging.getLogger(__name__)
 
 
 class _Base(object):
     def __init__(self, auth, endpoint, is_cname, session, connect_timeout,
-                 app_name='', enable_crc=True, proxy=None):
+                 app_name='', enable_crc=True, proxies=None, region=None, cloudbox_id=None):
         self.auth = auth
         self.endpoint = _normalize_endpoint(endpoint.strip())
         if utils.is_valid_endpoint(self.endpoint) is not True:
-            raise ClientError('The endpoint you has specified is not valid, endpoint: {0}'.format(endpoint))
+            raise exceptions.ClientError('The endpoint you has specified is not valid, endpoint: {0}'.format(endpoint))
         self.session = session or http.Session()
         self.timeout = defaults.get(connect_timeout, defaults.connect_timeout)
         self.app_name = app_name
         self.enable_crc = enable_crc
-        self.proxy = proxy
-
+        self.proxies = proxies
+        self.region = region
+        self.product = 'oss'
+        self.cloudbox_id = cloudbox_id
+        if self.cloudbox_id is not None:
+            self.product = 'oss-cloudbox'
         self._make_url = _UrlMaker(self.endpoint, is_cname)
 
     async def _do(self, method, bucket_name, key, **kwargs):
         key = to_string(key)
         req = http.Request(method, self._make_url(bucket_name, key),
                            app_name=self.app_name,
-                           proxy=self.proxy,
+                           proxies=self.proxies,
+                           region=self.region,
+                           product=self.product,
+                           cloudbox_id=self.cloudbox_id,
                            **kwargs)
         self.auth._sign_request(req, bucket_name, key)
 
         resp = await self.session.do_request(req, timeout=self.timeout)
 
         if resp.status // 100 != 2:
             e = await exceptions.make_exception(resp)
@@ -234,15 +242,15 @@
         content_length = models._hget(resp.headers, 'content-length', int)
         if content_length is not None and content_length == 0:
             await resp.read()
 
         return resp
 
     async def _do_url(self, method, sign_url, **kwargs):
-        req = http.Request(method, sign_url, app_name=self.app_name, proxy=self.proxy, **kwargs)
+        req = http.Request(method, sign_url, app_name=self.app_name, proxies=self.proxies, **kwargs)
         resp = await self.session.do_request(req, timeout=self.timeout)
         if resp.status // 100 != 2:
             e = await exceptions.make_exception(resp)
             logger.info("Exception: {0}".format(e))
             raise e
 
         # Note that connections are only released back to the pool for reuse once all body data has been read;
@@ -294,62 +302,79 @@
 
     :param float connect_timeout: 连接超时时间，以秒为单位。
     :param str app_name: 应用名。该参数不为空，则在User Agent中加入其值。
         注意到，最终这个字符串是要作为HTTP Header的值传输的，所以必须要遵循HTTP标准。
     """
 
     QOS_INFO = 'qosInfo'
+    REGIONS = 'regions'
 
     def __init__(self, auth, endpoint,
                  session=None,
                  connect_timeout=None,
                  app_name='',
-                 proxy=None):
-        logger.debug("Init oss service, endpoint: {0}, connect_timeout: {1}, app_name: {2}, proxy: {3}".format(
-            endpoint, connect_timeout, app_name, proxy))
+                 proxies=None,
+                 region=None,
+                 cloudbox_id=None):
+        logger.debug("Init oss service, endpoint: {0}, connect_timeout: {1}, app_name: {2}, proxies: {3}".format(
+            endpoint, connect_timeout, app_name, proxies))
         super(Service, self).__init__(auth, endpoint, False, session, connect_timeout,
-                                      app_name=app_name, proxy=proxy)
+                                      app_name=app_name, proxies=proxies,
+                                      region=region, cloudbox_id=cloudbox_id)
 
-    async def list_buckets(self, prefix='', marker='', max_keys=100, params=None):
+    async def list_buckets(self, prefix='', marker='', max_keys=100, params=None, headers=None):
         """根据前缀罗列用户的Bucket。
 
         :param str prefix: 只罗列Bucket名为该前缀的Bucket，空串表示罗列所有的Bucket
         :param str marker: 分页标志。首次调用传空串，后续使用返回值中的next_marker
         :param int max_keys: 每次调用最多返回的Bucket数目
         :param dict params: list操作参数，传入'tag-key','tag-value'对结果进行过滤
+        :param headers: 用户指定的HTTP头部。可以指定Content-Type、Content-MD5、x-oss-meta-开头的头部等。可以是dict，建议是oss2.CaseInsensitiveDict
 
         :return: 罗列的结果
         :rtype: oss2.models.ListBucketsResult
         """
         logger.debug("Start to list buckets, prefix: {0}, marker: {1}, max-keys: {2}".format(prefix, marker, max_keys))
 
         listParam = {}
         listParam['prefix'] = prefix
         listParam['marker'] = marker
         listParam['max-keys'] = str(max_keys)
 
+        headers = http.CaseInsensitiveDict(headers)
+
         if params is not None:
-            if 'tag-key' in params:
-                listParam['tag-key'] = params['tag-key']
-            if 'tag-value' in params:
-                listParam['tag-value'] = params['tag-value']
+            listParam.update(params)
 
-        resp = await self._do('GET', '', '', params=listParam)
+        resp = await self._do('GET', '', '', params=listParam, headers=headers)
         logger.debug("List buckets done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return await self._parse_result(resp, xml_utils.parse_list_buckets, ListBucketsResult)
 
     async def get_user_qos_info(self):
         """获取User的QoSInfo
         :return: :class:`GetUserQosInfoResult <oss2.models.GetUserQosInfoResult>`
         """
         logger.debug("Start to get user qos info.")
         resp = await self._do('GET', '', '', params={Service.QOS_INFO: ''})
         logger.debug("get use qos, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return await self._parse_result(resp, xml_utils.parse_get_qos_info, GetUserQosInfoResult)
 
+    async def describe_regions(self, regions=''):
+        """查询所有支持地域或者指定地域对应的Endpoint信息，包括外网Endpoint、内网Endpoint和传输加速Endpoint。
+
+        :param str regions : 地域。
+        :return: :class:`DescribeRegionsResult <oss2.models.DescribeRegionsResult>`
+        """
+        logger.debug("Start to describe regions")
+
+        resp = await self._do('GET', '', '', params={Service.REGIONS: regions})
+        logger.debug("Describe regions done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+
+        return await self._parse_result(resp, xml_utils.parse_describe_regions, DescribeRegionsResult)
+
 
 class Bucket(_Base):
     """用于Bucket和Object操作的类，诸如创建、删除Bucket，上传、下载Object等。
 
     用法（假设Bucket属于杭州区域） ::
 
         >>> import oss2
@@ -408,27 +433,39 @@
     WORM = "worm"
     WORM_ID = "wormId"
     WORM_EXTEND = "wormExtend"
     REPLICATION = "replication"
     REPLICATION_LOCATION = 'replicationLocation'
     REPLICATION_PROGRESS = 'replicationProgress'
     TRANSFER_ACCELERATION = 'transferAcceleration'
+    CNAME = 'cname'
+    META_QUERY = 'metaQuery'
+    ACCESS_MONITOR = 'accessmonitor'
+    RESOURCE_GROUP = 'resourceGroup'
+    STYLE = 'style'
+    STYLE_NAME = 'styleName'
+    ASYNC_PROCESS = 'x-oss-async-process'
+    CALLBACK = 'callback'
 
     def __init__(self, auth, endpoint, bucket_name,
                  is_cname=False,
                  session=None,
                  connect_timeout=None,
                  app_name='',
                  enable_crc=True,
-                 proxy=None):
-        logger.debug(
-            "Init Bucket: {0}, endpoint: {1}, isCname: {2}, connect_timeout: {3}, app_name: {4}, enabled_crc: {5}"
-            ", proxy: {6}".format(bucket_name, endpoint, is_cname, connect_timeout, app_name, enable_crc, proxy))
+                 proxies=None,
+                 region=None,
+                 cloudbox_id=None):
+        logger.debug(
+            "Init Bucket: {0}, endpoint: {1}, isCname: {2}, connect_timeout: {3}, app_name: {4}, enabled_crc: {5}, "
+            "region: {6}, proxies: {7}".format(bucket_name, endpoint, is_cname, connect_timeout, app_name, enable_crc,
+                                               region, proxies))
         super(Bucket, self).__init__(auth, endpoint, is_cname, session, connect_timeout,
-                                     app_name=app_name, enable_crc=enable_crc, proxy=proxy)
+                                     app_name=app_name, enable_crc=enable_crc, proxies=proxies,
+                                     region=region, cloudbox_id=cloudbox_id)
 
         self.bucket_name = bucket_name.strip()
         if utils.is_valid_bucket_name(self.bucket_name) is not True:
             raise ClientError("The bucket_name is invalid, please check it.")
 
     async def sign_url(self, method, key, expires, headers=None, params=None, slash_safe=False):
         """生成签名URL。
@@ -450,21 +487,26 @@
         :param params: 需要签名的HTTP查询参数
 
         :param slash_safe: 是否开启key名称中的‘/’转义保护，如果不开启'/'将会转义成%2F
         :type slash_safe: bool
 
         :return: 签名URL。
         """
+        if key is None or len(key.strip()) <= 0:
+            raise exceptions.ClientError("The key is invalid, please check it.")
         key = to_string(key)
         logger.debug(
             "Start to sign_url, method: {0}, bucket: {1}, key: {2}, expires: {3}, headers: {4}, params: {5}, slash_safe: {6}".format(
                 method, self.bucket_name, to_string(key), expires, headers, params, slash_safe))
         req = http.Request(method, self._make_url(self.bucket_name, key, slash_safe),
                            headers=headers,
-                           params=params)
+                           params=params,
+                           region=self.region,
+                           product=self.product,
+                           cloudbox_id=self.cloudbox_id)
         return self.auth._sign_url(req, self.bucket_name, key, expires)
 
     async def sign_rtmp_url(self, channel_name, playlist_name, expires):
         """生成RTMP推流的签名URL。
         常见的用法是生成加签的URL以供授信用户向OSS推RTMP流。
 
         :param channel_name: 直播频道的名称
@@ -496,15 +538,15 @@
 
         :return: :class:`ListObjectsResult <oss2.models.ListObjectsResult>`
         """
         headers = http.CaseInsensitiveDict(headers)
         logger.debug(
             "Start to List objects, bucket: {0}, prefix: {1}, delimiter: {2}, marker: {3}, max-keys: {4}".format(
                 self.bucket_name, to_string(prefix), delimiter, to_string(marker), max_keys))
-        resp = await self.__do_object('GET', '',
+        resp = await self.__do_bucket('GET',
                                       params={'prefix': prefix,
                                               'delimiter': delimiter,
                                               'marker': marker,
                                               'max-keys': str(max_keys),
                                               'encoding-type': 'url'},
                                       headers=headers)
         logger.debug("List objects done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
@@ -528,15 +570,15 @@
         """
         headers = http.CaseInsensitiveDict(headers)
         logger.debug(
             "Start to List objects, bucket: {0}, prefix: {1}, delimiter: {2}, continuation_token: {3}, "
             "start-after: {4}, fetch-owner: {5}, encoding_type: {6}, max-keys: {7}".format(
                 self.bucket_name, to_string(prefix), delimiter, continuation_token, start_after, fetch_owner,
                 encoding_type, max_keys))
-        resp = await self.__do_object('GET', '',
+        resp = await self.__do_bucket('GET',
                                       params={'list-type': '2',
                                               'prefix': prefix,
                                               'delimiter': delimiter,
                                               'continuation-token': continuation_token,
                                               'start-after': start_after,
                                               'fetch-owner': str(fetch_owner).lower(),
                                               'max-keys': str(max_keys),
@@ -741,14 +783,16 @@
             params.update({Bucket.PROCESS: process})
 
         logger.debug("Start to get object, bucket: {0}， key: {1}, range: {2}, headers: {3}, params: {4}".format(
             self.bucket_name, to_string(key), range_string, headers, params))
         resp = await self.__do_object('GET', key, headers=headers, params=params)
         logger.debug("Get object done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
 
+        # GetObjectResult needs to calculate crc, but the data stream is asynchronous and cannot be read directly,
+        # so the GetObjectResult object in asyncio-oss is used to satisfy the crc check calculation.
         return AsyncGetObjectResult(resp, progress_callback, self.enable_crc)
 
     async def select_object(self, key, sql,
                             progress_callback=None,
                             select_params=None,
                             byte_range=None,
                             headers=None
@@ -872,14 +916,16 @@
         range_string = _make_range_string(byte_range)
         if range_string:
             headers['range'] = range_string
 
         logger.debug("Start to get object with url, bucket: {0}, sign_url: {1}, range: {2}, headers: {3}".format(
             self.bucket_name, sign_url, range_string, headers))
         resp = await self._do_url('GET', sign_url, headers=headers)
+        # GetObjectResult needs to calculate crc, but the data stream is asynchronous and cannot be read directly,
+        # so the GetObjectResult object in asyncio-oss is used to satisfy the crc check calculation.
         return AsyncGetObjectResult(resp, progress_callback, self.enable_crc)
 
     async def get_object_with_url_to_file(self, sign_url,
                                           filename,
                                           byte_range=None,
                                           headers=None,
                                           progress_callback=None):
@@ -963,15 +1009,15 @@
         """
         logger.debug("Start to head object, bucket: {0}, key: {1}, headers: {2}".format(
             self.bucket_name, to_string(key), headers))
 
         resp = await self.__do_object('HEAD', key, headers=headers, params=params)
 
         logger.debug("Head object done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
-        return HeadObjectResult(resp)
+        return await self._parse_result(resp, xml_utils.parse_dummy_result, HeadObjectResult)
 
     async def create_select_object_meta(self, key, select_meta_params=None, headers=None):
         """获取或创建CSV,JSON LINES 文件元信息。如果元信息存在，返回之；不然则创建后返回之
 
         HTTP响应的头部包含了文件元信息，可以通过 `RequestResult` 的 `headers` 成员获得。
         CSV文件用法 ::
 
@@ -1029,15 +1075,15 @@
 
         if params is None:
             params = dict()
 
         if Bucket.OBJECTMETA not in params:
             params[Bucket.OBJECTMETA] = ''
 
-        resp = await self.__do_object('GET', key, params=params, headers=headers)
+        resp = await self.__do_object('HEAD', key, params=params, headers=headers)
         logger.debug("Get object metadata done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return GetObjectMetaResult(resp)
 
     async def object_exists(self, key, headers=None):
         """如果文件存在就返回True，否则返回False。如果Bucket不存在，或是发生其他错误，则抛出异常。"""
         #:param key: 文件名
 
@@ -1047,20 +1093,27 @@
         # 如果我们用head_object来实现的话，由于HTTP HEAD请求没有响应体，只有响应头部，这样当发生404时，
         # 我们无法区分是NoSuchBucket还是NoSuchKey错误。
         #
         # 2.2.0之前的实现是通过get_object的if-modified-since头部，把date设为当前时间24小时后，这样如果文件存在，则会返回
         # 304 (NotModified)；不存在，则会返回NoSuchKey。get_object会受回源的影响，如果配置会404回源，get_object会判断错误。
         #
         # 目前的实现是通过get_object_meta判断文件是否存在。
+        # get_object_meta 为200时，不会返回响应体，所以该接口把GET方法修改为HEAD 方式
+        # 同时, 对于head 请求，服务端会通过x-oss-err 返回 错误响应信息,
+        # 考虑到兼容之前的行为，增加exceptions.NotFound 异常 当作NoSuchKey
 
         logger.debug("Start to check if object exists, bucket: {0}, key: {1}".format(self.bucket_name, to_string(key)))
         try:
             await self.get_object_meta(key, headers=headers)
         except exceptions.NoSuchKey:
             return False
+        except exceptions.NoSuchBucket:
+            raise
+        except exceptions.NotFound:
+            return False
         except:
             raise
 
         return True
 
     async def copy_object(self, source_bucket_name, source_key, target_key, headers=None, params=None):
         """拷贝一个文件到当前Bucket。
@@ -1244,15 +1297,15 @@
         logger.debug("Start to delete objects, bucket: {0}, keys: {1}".format(self.bucket_name, key_list))
 
         data = xml_utils.to_batch_delete_objects_request(key_list, False)
 
         headers = http.CaseInsensitiveDict(headers)
         headers['Content-MD5'] = utils.content_md5(data)
 
-        resp = await self.__do_object('POST', '',
+        resp = await self.__do_bucket('POST',
                                       data=data,
                                       params={'delete': '', 'encoding-type': 'url'},
                                       headers=headers)
         logger.debug("Delete objects done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return await self._parse_result(resp, xml_utils.parse_batch_delete_objects, BatchDeleteObjectsResult)
 
     async def delete_object_versions(self, keylist_versions, headers=None):
@@ -1271,15 +1324,15 @@
         logger.debug("Start to delete object versions, bucket: {0}".format(self.bucket_name))
 
         data = xml_utils.to_batch_delete_objects_version_request(keylist_versions, False)
 
         headers = http.CaseInsensitiveDict(headers)
         headers['Content-MD5'] = utils.content_md5(data)
 
-        resp = await self.__do_object('POST', '',
+        resp = await self.__do_bucket('POST',
                                       data=data,
                                       params={'delete': '', 'encoding-type': 'url'},
                                       headers=headers)
         logger.debug("Delete object versions done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return await self._parse_result(resp, xml_utils.parse_batch_delete_objects, BatchDeleteObjectsResult)
 
     async def init_multipart_upload(self, key, headers=None, params=None):
@@ -1356,30 +1409,33 @@
 
         :param headers: HTTP头部
         :type headers: 可以是dict，建议是oss2.CaseInsensitiveDict
 
         :return: :class:`PutObjectResult <oss2.models.PutObjectResult>`
         """
         headers = http.CaseInsensitiveDict(headers)
-        parts = sorted(parts, key=lambda p: p.part_number)
-        data = xml_utils.to_complete_upload_request(parts)
+
+        data = None
+        if parts is not None:
+            parts = sorted(parts, key=lambda p: p.part_number)
+            data = xml_utils.to_complete_upload_request(parts)
 
         logger.debug("Start to complete multipart upload, bucket: {0}, key: {1}, upload_id: {2}, parts: {3}".format(
             self.bucket_name, to_string(key), upload_id, data))
 
         resp = await self.__do_object('POST', key,
                                       params={'uploadId': upload_id},
                                       data=data,
                                       headers=headers)
         logger.debug(
             "Complete multipart upload done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
 
         result = PutObjectResult(resp)
 
-        if self.enable_crc:
+        if self.enable_crc and parts is not None:
             object_crc = utils.calc_obj_crc_from_parts(parts)
             utils.check_crc('multipart upload', object_crc, result.crc, result.request_id)
 
         return result
 
     async def abort_multipart_upload(self, key, upload_id, headers=None):
         """取消分片上传。
@@ -1426,15 +1482,15 @@
         logger.debug("Start to list multipart uploads, bucket: {0}, prefix: {1}, delimiter: {2}, key_marker: {3}, "
                      "upload_id_marker: {4}, max_uploads: {5}".format(self.bucket_name, to_string(prefix), delimiter,
                                                                       to_string(key_marker), upload_id_marker,
                                                                       max_uploads))
 
         headers = http.CaseInsensitiveDict(headers)
 
-        resp = await self.__do_object('GET', '',
+        resp = await self.__do_bucket('GET',
                                       params={'uploads': '',
                                               'prefix': prefix,
                                               'delimiter': delimiter,
                                               'key-marker': key_marker,
                                               'upload-id-marker': upload_id_marker,
                                               'max-uploads': str(max_uploads),
                                               'encoding-type': 'url'},
@@ -1563,26 +1619,25 @@
         if Bucket.SYMLINK not in params:
             params[Bucket.SYMLINK] = ''
 
         resp = await self.__do_object('GET', symlink_key, params=params, headers=headers)
         logger.debug("Get symlink done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return GetSymlinkResult(resp)
 
-    async def create_bucket(self, permission=None, input=None):
+    async def create_bucket(self, permission=None, input=None, headers=None):
         """创建新的Bucket。
 
         :param str permission: 指定Bucket的ACL。可以是oss2.BUCKET_ACL_PRIVATE（推荐、缺省）、oss2.BUCKET_ACL_PUBLIC_READ或是
             oss2.BUCKET_ACL_PUBLIC_READ_WRITE。
 
         :param input: :class:`BucketCreateConfig <oss2.models.BucketCreateConfig>` object
         """
+        headers = http.CaseInsensitiveDict(headers)
         if permission:
-            headers = {OSS_CANNED_ACL: permission}
-        else:
-            headers = None
+            headers[OSS_CANNED_ACL] = permission
 
         data = self.__convert_data(BucketCreateConfig, xml_utils.to_put_bucket_config, input)
         logger.debug("Start to create bucket, bucket: {0}, permission: {1}, config: {2}".format(self.bucket_name,
                                                                                                 permission, data))
         resp = await self.__do_bucket('PUT', headers=headers, data=data)
         logger.debug("Create bucket done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return RequestResult(resp)
@@ -2086,22 +2141,28 @@
             self.bucket_name))
 
         resp = await self.__do_bucket('GET', params={Bucket.TAGGING: ''})
 
         logger.debug("Get bucket tagging done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return await self._parse_result(resp, xml_utils.parse_get_tagging, GetTaggingResult)
 
-    async def delete_bucket_tagging(self):
+    async def delete_bucket_tagging(self, params=None):
         """
         :return: :class:`RequestResult <oss2.models.RequestResult>`
         """
         logger.debug("Start to delete bucket tagging, bucket: {0}".format(
             self.bucket_name))
 
-        resp = await self.__do_bucket('DELETE', params={Bucket.TAGGING: ''})
+        if params is None:
+            params = dict()
+
+        if Bucket.TAGGING not in params:
+            params[Bucket.TAGGING] = ''
+
+        resp = await self.__do_bucket('DELETE', params=params)
 
         logger.debug("Delete bucket tagging done, req_id: {0}, status_code: {1}".format(
             resp.request_id, resp.status))
         return RequestResult(resp)
 
     async def list_object_versions(self, prefix='', delimiter='', key_marker='',
                                    max_keys=100, versionid_marker='', headers=None):
@@ -2462,16 +2523,15 @@
         :param rule :class:`ReplicationRule <oss2.models.ReplicationRule>`
         :return: :class:`RequestResult <oss2.models.RequestResult>`
         """
         logger.debug("Start to put bucket replication: {0}".format(self.bucket_name))
         data = xml_utils.to_put_bucket_replication(rule)
         headers = http.CaseInsensitiveDict()
         headers['Content-MD5'] = utils.content_md5(data)
-        resp = await self.__do_bucket('POST', data=data, params={Bucket.REPLICATION: '', 'comp': 'add'},
-                                      headers=headers)
+        resp = await self.__do_bucket('POST', data=data, params={Bucket.REPLICATION: '', 'comp': 'add'}, headers=headers)
         logger.debug("Put bucket replication done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
 
         return RequestResult(resp)
 
     async def get_bucket_replication(self):
         """获取bucket跨区域复制规则
 
@@ -2556,25 +2616,281 @@
             "bucket transfer acceleration done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
 
         return RequestResult(resp)
 
     async def get_bucket_transfer_acceleration(self):
         """获取目标存储空间（Bucket）的传输加速配置
 
-        :return: :class:`GetBucketReplicationResult <oss2.models.GetBucketReplicationResult>`
+        :return: :class:`GetBucketTransferAccelerationResult <oss2.models.GetBucketTransferAccelerationResult>`
         """
         logger.debug("Start to get bucket transfer acceleration: {0}".format(self.bucket_name))
         resp = await self.__do_bucket('GET', params={Bucket.TRANSFER_ACCELERATION: ''})
         logger.debug(
             "Get bucket transfer acceleration done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
 
         return await self._parse_result(resp, xml_utils.parse_get_bucket_transfer_acceleration_result,
                                         GetBucketTransferAccelerationResult)
 
+    async def create_bucket_cname_token(self, domain):
+        """创建域名所有权验证所需的CnameToken。
+
+        :param str domain : 绑定的Cname名称。
+        :return: :class:`CreateBucketCnameTokenResult <oss2.models.CreateBucketCnameTokenResult>`
+        """
+        logger.debug("Start to create bucket cname token, bucket: {0}.".format(self.bucket_name))
+        data = xml_utils.to_bucket_cname_configuration(domain)
+        resp = await self.__do_bucket('POST', data=data, params={Bucket.CNAME: '', Bucket.COMP: 'token'})
+        logger.debug("bucket cname token done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return await self._parse_result(resp, xml_utils.parse_create_bucket_cname_token, CreateBucketCnameTokenResult)
+
+    async def get_bucket_cname_token(self, domain):
+        """获取已创建的CnameToken。
+
+        :param str domain : 绑定的Cname名称。
+        :return: :class:`GetBucketCnameTokenResult <oss2.models.GetBucketCnameTokenResult>`
+        """
+        logger.debug("Start to get bucket cname: {0}".format(self.bucket_name))
+        resp = await self.__do_bucket('GET', params={Bucket.CNAME: domain, Bucket.COMP: 'token'})
+        logger.debug("Get bucket cname done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return await self._parse_result(resp, xml_utils.parse_get_bucket_cname_token, GetBucketCnameTokenResult)
+
+    async def put_bucket_cname(self, input):
+        """为某个存储空间（Bucket）绑定自定义域名。
+
+        :param input: PutBucketCnameRequest类型，包含了证书和自定义域名信息
+        :return: :class:`RequestResult <oss2.models.RequestResult>`
+        """
+        logger.debug("Start to add bucket cname, bucket: {0}.".format(self.bucket_name))
+        data = xml_utils.to_bucket_cname_configuration(input.domain, input.cert)
+        resp = await self.__do_bucket('POST', data=data, params={Bucket.CNAME: '', Bucket.COMP: 'add'})
+        logger.debug("bucket cname done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return RequestResult(resp)
+
+    async def list_bucket_cname(self):
+        """查询某个存储空间（Bucket）下绑定的所有Cname列表。
+
+        :return: :class:`ListBucketCnameResult <oss2.models.ListBucketCnameResult>`
+        """
+        logger.debug("Start to do query list bucket cname: {0}".format(self.bucket_name))
+
+        resp = await self.__do_bucket('GET', params={Bucket.CNAME: ''})
+        logger.debug("query list bucket cname done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return await self._parse_result(resp, xml_utils.parse_list_bucket_cname, ListBucketCnameResult)
+
+    async def delete_bucket_cname(self, domain):
+        """删除某个存储空间（Bucket）已绑定的Cname
+
+        :param str domain : 绑定的Cname名称。
+        :return: :class:`RequestResult <oss2.models.RequestResult>`
+        """
+        logger.debug("Start to delete bucket cname: {0}".format(self.bucket_name))
+        data = xml_utils.to_bucket_cname_configuration(domain)
+        resp = await self.__do_bucket('POST', data=data, params={Bucket.CNAME: '', Bucket.COMP: 'delete'})
+        logger.debug("delete bucket cname done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return RequestResult(resp)
+
+    async def open_bucket_meta_query(self):
+        """为存储空间（Bucket）开启元数据管理功能
+
+        :return: :class:`RequestResult <oss2.models.RequestResult>`
+        """
+        logger.debug("Start to bucket meta query, bucket: {0}.".format(self.bucket_name))
+        resp = await self.__do_bucket('POST', params={Bucket.META_QUERY: '', 'comp': 'add'})
+        logger.debug("bucket meta query done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return RequestResult(resp)
+
+    async def get_bucket_meta_query_status(self):
+        """获取指定存储空间（Bucket）的元数据索引库信息。
+
+        :return: :class:`GetBucketMetaQueryResult <oss2.models.GetBucketMetaQueryResult>`
+        """
+        logger.debug("Start to get bucket meta query: {0}".format(self.bucket_name))
+        resp = await self.__do_bucket('GET', params={Bucket.META_QUERY: ''})
+        logger.debug("Get bucket meta query done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return await self._parse_result(resp, xml_utils.parse_get_bucket_meta_query_result, GetBucketMetaQueryResult)
+
+    async def do_bucket_meta_query(self, do_meta_query_request):
+        """查询满足指定条件的文件（Object），并按照指定字段和排序方式列出文件信息。
+
+        :param do_meta_query_request :class:`MetaQuery <oss2.models.MetaQuery>`
+        :return: :class:`DoBucketMetaQueryResult <oss2.models.DoBucketMetaQueryResult>`
+        """
+        logger.debug("Start to do bucket meta query: {0}".format(self.bucket_name))
+
+        data = self.__convert_data(MetaQuery, xml_utils.to_do_bucket_meta_query_request, do_meta_query_request)
+        resp = await self.__do_bucket('POST', data=data, params={Bucket.META_QUERY: '', Bucket.COMP: 'query'})
+        logger.debug("do bucket meta query done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return await self._parse_result(resp, xml_utils.parse_do_bucket_meta_query_result, DoBucketMetaQueryResult)
+
+    async def close_bucket_meta_query(self):
+        """关闭存储空间（Bucket）的元数据管理功能
+
+        :return: :class:`RequestResult <oss2.models.RequestResult>`
+        """
+        logger.debug("Start to close bucket meta query: {0}".format(self.bucket_name))
+        resp = await self.__do_bucket('POST', params={Bucket.META_QUERY: '', Bucket.COMP: 'delete'})
+        logger.debug("bucket meta query done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return RequestResult(resp)
+
+    async def put_bucket_access_monitor(self, status):
+        """更新 Bucket 访问跟踪状态。
+
+        :param str status : bucket访问跟踪的开启状态
+        :return: :class:`RequestResult <oss2.models.RequestResult>`
+        """
+        logger.debug("Start to put bucket access monitor, bucket: {0}.".format(self.bucket_name))
+        data = xml_utils.to_put_bucket_access_monitor(status)
+        resp = await self.__do_bucket('PUT', data=data, params={Bucket.ACCESS_MONITOR: ''})
+        logger.debug("bucket access monitor done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return RequestResult(resp)
+
+    async def get_bucket_access_monitor(self):
+        """获取当前Bucket的访问跟踪的状态。
+
+        :return: :class:`GetBucketAccessMonitorResult <oss2.models.GetBucketAccessMonitorResult>`
+        """
+        logger.debug("Start to get bucket access monitor: {0}".format(self.bucket_name))
+
+        resp = await self.__do_bucket('GET', params={Bucket.ACCESS_MONITOR: ''})
+        logger.debug("query list bucket cname done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return await self._parse_result(resp, xml_utils.parse_get_bucket_access_monitor_result, GetBucketAccessMonitorResult)
+
+    async def get_bucket_resource_group(self):
+        """查询存储空间（Bucket）的资源组ID。
+
+        :return: :class:`GetBucketResourceGroupResult <oss2.models.GetBucketResourceGroupResult>`
+        """
+        logger.debug("Start to get bucket resource group: {0}".format(self.bucket_name))
+        resp = self.__do_bucket('GET', params={Bucket.RESOURCE_GROUP: ''})
+        logger.debug(
+            "Get bucket resource group done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+
+        return await self._parse_result(resp, xml_utils.parse_get_bucket_resource_group_result, GetBucketResourceGroupResult)
+
+    async def put_bucket_resource_group(self, resourceGroupId):
+        """为存储空间（Bucket）配置所属资源组。
+
+        :param str resourceGroupId : Bucket所属的资源组ID。
+        :return: :class:`RequestResult <oss2.models.RequestResult>`
+        """
+        logger.debug("Start to put bucket resource group, bucket: {0}.".format(self.bucket_name))
+        data = xml_utils.to_put_bucket_resource_group(resourceGroupId)
+        resp = await self.__do_bucket('PUT', data=data, params={Bucket.RESOURCE_GROUP: ''})
+        logger.debug("bucket resource group done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return RequestResult(resp)
+
+    async def put_bucket_style(self, styleName, content):
+        """新增图片样式。
+
+        :param str styleName : 样式名称。
+        :param str content : 图片样式内容，图片样式可以包含一个或多个图片处理操作。
+        :return: :class:`RequestResult <oss2.models.RequestResult>`
+        """
+        logger.debug("Start to put bucket style, bucket: {0}.".format(self.bucket_name))
+
+        data = xml_utils.to_put_bucket_style(content)
+        resp = await self.__do_bucket('PUT', data=data, params={Bucket.STYLE: '', Bucket.STYLE_NAME: styleName})
+        logger.debug("bucket style done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return RequestResult(resp)
+
+    async def get_bucket_style(self, styleName):
+        """查询某个Bucket下指定的图片样式信息。
+
+        :param str styleName : 样式名称。
+        :return: :class:`GetBucketStyleResult <oss2.models.GetBucketStyleResult>`
+        """
+        logger.debug("Start to get bucket style: {0}".format(self.bucket_name))
+
+        resp = await self.__do_bucket('GET', params={Bucket.STYLE: '', Bucket.STYLE_NAME: styleName})
+        logger.debug("Get bucket style done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+
+        return await self._parse_result(resp, xml_utils.parse_get_bucket_style_result, GetBucketStyleResult)
+
+    async def list_bucket_style(self):
+        """查询某个Bucket下已创建的所有图片样式。
+
+        :return: :class:`ListBucketStyleResult <oss2.models.ListBucketStyleResult>`
+        """
+        logger.debug("Start to list bucket style: {0}".format(self.bucket_name))
+
+        resp = await self.__do_bucket('GET', params={Bucket.STYLE: ''})
+        logger.debug("query list bucket style done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return await self._parse_result(resp, xml_utils.parse_list_bucket_style, ListBucketStyleResult)
+
+    async def delete_bucket_style(self, styleName):
+        """删除某个Bucket下指定的图片样式。
+
+        :param str styleName : 样式名称。
+        :return: :class:`RequestResult <oss2.models.RequestResult>`
+        """
+        logger.debug("Start to delete bucket style: {0}".format(self.bucket_name))
+
+        resp = await self.__do_bucket('DELETE', params={Bucket.STYLE: '', Bucket.STYLE_NAME: styleName})
+        logger.debug("delete bucket style done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return RequestResult(resp)
+
+    async def async_process_object(self, key, process, headers=None):
+        """异步处理多媒体接口。
+
+        :param str key: 处理的多媒体的对象名称
+        :param str process: 处理的字符串，例如"video/convert,f_mp4,vcodec_h265,s_1920x1080,vb_2000000,fps_30,acodec_aac,ab_100000,sn_1|sys/saveas,o_dGVzdC5qcGc,b_dGVzdA"
+
+        :param headers: HTTP头部
+        :type headers: 可以是dict，建议是oss2.CaseInsensitiveDict
+        """
+
+        headers = http.CaseInsensitiveDict(headers)
+
+        logger.debug("Start to async process object, bucket: {0}, key: {1}, process: {2}".format(
+            self.bucket_name, to_string(key), process))
+        process_data = "%s=%s" % (Bucket.ASYNC_PROCESS, process)
+        resp = await self.__do_object('POST', key, params={Bucket.ASYNC_PROCESS: ''}, headers=headers, data=process_data)
+        logger.debug("Async process object done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return await self._parse_result(resp, xml_utils.parse_async_process_object, AsyncProcessObject)
+
+    async def put_bucket_callback_policy(self, callbackPolicy):
+        """设置bucket回调策略
+
+        :param str callbackPolicy: 回调策略
+        """
+        logger.debug("Start to put bucket callback policy, bucket: {0}, callback policy: {1}".format(self.bucket_name,
+                                                                                                     callbackPolicy))
+        data = xml_utils.to_do_bucket_callback_policy_request(callbackPolicy)
+        resp = await self.__do_bucket('PUT', data=data, params={Bucket.POLICY: '', Bucket.COMP: Bucket.CALLBACK})
+        logger.debug(
+            "Put bucket callback policy done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+
+        return RequestResult(resp)
+
+    async def get_bucket_callback_policy(self):
+        """获取bucket回调策略
+        :return: :class:`GetBucketPolicyResult <oss2.models.CallbackPolicyResult>`
+        """
+
+        logger.debug("Start to get bucket callback policy, bucket: {0}".format(self.bucket_name))
+        resp = await self.__do_bucket('GET', params={Bucket.POLICY: '', Bucket.COMP: Bucket.CALLBACK})
+        logger.debug(
+            "Get bucket callback policy done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return await self._parse_result(resp, xml_utils.parse_callback_policy_result, CallbackPolicyResult)
+
+    async def delete_bucket_callback_policy(self):
+        """删除bucket回调策略
+        :return: :class:`RequestResult <oss2.models.RequestResult>`
+        """
+        logger.debug("Start to delete bucket callback policy, bucket: {0}".format(self.bucket_name))
+        resp = await self.__do_bucket('DELETE', params={Bucket.POLICY: '', Bucket.COMP: Bucket.CALLBACK})
+        logger.debug(
+            "Delete bucket callback policy done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+        return RequestResult(resp)
+
     async def __do_object(self, method, key, **kwargs):
+        if not self.bucket_name:
+            raise exceptions.ClientError("Bucket name should not be null or empty.")
+        if not key:
+            raise exceptions.ClientError("key should not be null or empty.")
         return await self._do(method, self.bucket_name, key, **kwargs)
 
     async def __do_bucket(self, method, **kwargs):
         return await self._do(method, self.bucket_name, '', **kwargs)
 
     def __convert_data(self, klass, converter, data):
         if isinstance(data, klass):
```

### Comparing `asyncio-oss-1.0.2/asyncio_oss/exceptions.py` & `asyncio-oss-1.1.0/asyncio_oss/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 oss2.exceptions
 ~~~~~~~~~~~~~~
 
 异常类。
 """
 
 import re
-
+import base64
 import xml.etree.ElementTree as ElementTree
 from xml.parsers import expat
 
 from oss2.compat import to_string
 from oss2.headers import *
 
 _OSS_ERROR_TO_EXCEPTION = {}  # populated at end of module
@@ -40,14 +40,20 @@
 
         #: OSS错误码
         self.code = self.details.get('Code', '')
 
         #: OSS错误信息
         self.message = self.details.get('Message', '')
 
+        #: OSS新的错误码
+        self.ec = self.details.get('EC', '')
+
+        #: header信息
+        self.headers = headers
+
     def __str__(self):
         error = {'status': self.status,
                  OSS_REQUEST_ID: self.request_id,
                  'details': self.details}
         return str(error)
 
     def _str_with_body(self):
@@ -330,15 +336,22 @@
     code = 'NoSuchTransferAccelerationConfiguration'
 
 
 async def make_exception(resp):
     status = resp.status
     headers = resp.headers
     body = await resp.read(4096)
-    details = _parse_error_body(body)
+    if not body and headers.get('x-oss-err') is not None:
+        try:
+            value = base64.b64decode(to_string(headers.get('x-oss-err')))
+        except:
+            value = body
+        details = _parse_error_body(value)
+    else:
+        details = _parse_error_body(body)
     code = details.get('Code', '')
 
     try:
         klass = _OSS_ERROR_TO_EXCEPTION[(status, code)]
         return klass(status, headers, body, details)
     except KeyError:
         return ServerError(status, headers, body, details)
```

### Comparing `asyncio-oss-1.0.2/asyncio_oss/http.py` & `asyncio-oss-1.1.0/asyncio_oss/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 
 这个模块包含了HTTP Adapters。尽管OSS Python SDK内部使用requests库进行HTTP通信，但是对使用者是透明的。
 该模块中的 `Session` 、 `Request` 、`Response` 对requests的对应的类做了简单的封装。
 """
 import logging
 import platform
 
+from .exceptions import RequestError
+
 import aiohttp
 from requests.structures import CaseInsensitiveDict
 
 from oss2 import __version__, defaults
 from oss2.compat import to_bytes
-from oss2.exceptions import RequestError
 from oss2.utils import file_object_remaining_bytes, SizedFileAdapter
 
 USER_AGENT = 'aliyun-sdk-python/{0}({1}/{2}/{3};{4})'.format(
     __version__, platform.system(), platform.release(), platform.machine(), platform.python_version())
 
 logger = logging.getLogger(__name__)
 
@@ -36,16 +37,16 @@
             pool_size = defaults.connection_pool_size
             connector = aiohttp.TCPConnector(limit=pool_size)
             self._aio_session = aiohttp.ClientSession(connector=connector)
 
     async def do_request(self, req, timeout):
         try:
             logger.debug(
-                "Send request, method: {0}, url: {1}, params: {2}, headers: {3}, timeout: {4}, proxy: {5}".format(
-                    req.method, req.url, req.params, req.headers, timeout, req.proxy))
+                "Send request, method: {0}, url: {1}, params: {2}, headers: {3}, timeout: {4}, proxies: {5}".format(
+                    req.method, req.url, req.params, req.headers, timeout, req.proxies))
 
             await self._create_session()
             # 1. When setting progress_callback or enabling crc verification, the data type will be converted to the
             # corresponding adapter object by oss make_progress_adapter / make_crc_adapter, and the process_callback
             # and crc verification calculation will be performed when read
             # 2. requests supports the reading of file-like-objects, while aiohttp does not, so you need to read the
             # data in advance
@@ -53,24 +54,25 @@
             resp = await self._aio_session.request(
                 req.method,
                 req.url,
                 data=req_data,
                 params=req.params,
                 headers=req.headers,
                 timeout=timeout,
-                proxy=req.proxy
+                proxy=req.proxies
             )
             self.resp = resp
             return Response(resp)
         except IOError as e:
             # catch read IO error
             raise RequestError(e)
-        except aiohttp.ClientError:
+        except aiohttp.ClientError as e:
             # catch all aiohttp client errors
             await self._aio_session.close()
+            raise RequestError(e)
 
     async def __aenter__(self):
         await self._create_session()
         await self._aio_session.__aenter__()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
@@ -79,20 +81,26 @@
 
 class Request(object):
     def __init__(self, method, url,
                  data=None,
                  params=None,
                  headers=None,
                  app_name='',
-                 proxy=None):
+                 proxies=None,
+                 region=None,
+                 product=None,
+                 cloudbox_id=None):
         self.method = method
         self.url = url
         self.data = _convert_request_body(data)
         self.params = params or {}
-        self.proxy = proxy
+        self.proxies = proxies
+        self.region = region
+        self.product = product
+        self.cloudbox_id = cloudbox_id
 
         if not isinstance(headers, CaseInsensitiveDict):
             self.headers = CaseInsensitiveDict(headers)
         else:
             self.headers = headers
 
         # tell requests not to add 'Accept-Encoding: gzip, deflate' by default
@@ -140,18 +148,21 @@
         if amt is None:
             content_list = []
             async for chunk in self.response.content.iter_chunked(_CHUNK_SIZE):
                 content_list.append(chunk)
             content = b''.join(content_list)
 
             self.__all_read = True
-            # logger.debug("Get response body, req-id: {0}, content: {1}", self.request_id, content)
             return content
         else:
-            return await self.response.content.read(amt)
+            try:
+                return await self.response.content.read(amt)
+            except StopAsyncIteration:
+                self.__all_read = True
+                return b''
 
     def __aiter__(self):
         return self.response.content
 
 
 # requests 对于具有 fileno() 方法的 file object，会用 fileno() 的返回值作为 Content-Length。
 # 这对于已经读取了部分内容，或执行了seek() 的 file object是不正确的。
```

### Comparing `asyncio-oss-1.0.2/asyncio_oss/iterators.py` & `asyncio-oss-1.1.0/asyncio_oss/iterators.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 """
 oss2.iterators
 ~~~~~~~~~~~~~~
 
 该模块包含了一些易于使用的迭代器，可以用来遍历Bucket、文件、分片上传等。
 """
 
-from oss2.models import MultipartUploadInfo, SimplifiedObjectInfo
-from oss2.exceptions import ServerError
+from .exceptions import ServerError
+from . import http
 
-from oss2 import defaults, http
+from oss2 import defaults
+from oss2.models import MultipartUploadInfo, SimplifiedObjectInfo
 
 
 class _BaseIterator(object):
     def __init__(self, marker, max_retries):
         self.is_truncated = True
         self.next_marker = marker
 
@@ -35,14 +36,17 @@
                 return self.entries.pop(0)
 
             if not self.is_truncated:
                 raise StopAsyncIteration
 
             await self.fetch_with_retry()
 
+    async def next(self):
+        return await self.__anext__()
+
     async def fetch_with_retry(self):
         for i in range(self.max_retries):
             try:
                 self.is_truncated, self.next_marker = await self._fetch()
             except ServerError as e:
                 if e.status // 100 != 5:
                     raise
@@ -59,15 +63,14 @@
     每次迭代返回的是 :class:`SimplifiedBucketInfo <oss2.models.SimplifiedBucketInfo>` 对象。
 
     :param service: :class:`Service <oss2.Service>` 对象
     :param prefix: 只列举匹配该前缀的Bucket
     :param marker: 分页符。只列举Bucket名字典序在此之后的Bucket
     :param max_keys: 每次调用 `list_buckets` 时的max_keys参数。注意迭代器返回的数目可能会大于该值。
     """
-
     def __init__(self, service, prefix='', marker='', max_keys=100, max_retries=None):
         super(BucketIterator, self).__init__(marker, max_retries)
         self.service = service
         self.prefix = prefix
         self.max_keys = max_keys
 
     async def _fetch(self):
@@ -90,15 +93,14 @@
     :param delimiter: 目录分隔符
     :param marker: 分页符
     :param max_keys: 每次调用 `list_objects` 时的max_keys参数。注意迭代器返回的数目可能会大于该值。
 
     :param headers: HTTP头部
     :type headers: 可以是dict，建议是oss2.CaseInsensitiveDict
     """
-
     def __init__(self, bucket, prefix='', delimiter='', marker='', max_keys=100, max_retries=None, headers=None):
         super(ObjectIterator, self).__init__(marker, max_retries)
 
         self.bucket = bucket
         self.prefix = prefix
         self.delimiter = delimiter
         self.max_keys = max_keys
@@ -158,15 +160,14 @@
                                              headers=self.headers)
         self.entries = result.object_list + [SimplifiedObjectInfo(prefix, None, None, None, None, None)
                                              for prefix in result.prefix_list]
         self.entries.sort(key=lambda obj: obj.key)
 
         return result.is_truncated, result.next_continuation_token
 
-
 class MultipartUploadIterator(_BaseIterator):
     """遍历Bucket里未完成的分片上传。
 
     每次返回 :class:`MultipartUploadInfo <oss2.models.MultipartUploadInfo>` 对象。
     当 `MultipartUploadInfo.is_prefix()` 返回True时，表明是公共前缀（目录）。
 
     :param bucket: :class:`Bucket <oss2.Bucket>` 对象
@@ -175,15 +176,14 @@
     :param key_marker: 文件名分页符
     :param upload_id_marker: 分片上传ID分页符
     :param max_uploads: 每次调用 `list_multipart_uploads` 时的max_uploads参数。注意迭代器返回的数目可能会大于该值。
 
     :param headers: HTTP头部
     :type headers: 可以是dict，建议是oss2.CaseInsensitiveDict
     """
-
     def __init__(self, bucket,
                  prefix='', delimiter='', key_marker='', upload_id_marker='',
                  max_uploads=1000, max_retries=None, headers=None):
         super(MultipartUploadIterator, self).__init__(key_marker, max_retries)
 
         self.bucket = bucket
         self.prefix = prefix
@@ -215,15 +215,14 @@
     :param bucket: :class:`Bucket <oss2.Bucket>` 对象
     :param key: 文件名
     :param max_uploads: 每次调用 `list_multipart_uploads` 时的max_uploads参数。注意迭代器返回的数目可能会大于该值。
 
     :param headers: HTTP头部
     :type headers: 可以是dict，建议是oss2.CaseInsensitiveDict
     """
-
     def __init__(self, bucket, key, max_uploads=1000, max_retries=None, headers=None):
         super(ObjectUploadIterator, self).__init__('', max_retries)
         self.bucket = bucket
         self.key = key
         self.next_upload_id_marker = ''
         self.max_uploads = max_uploads
         self.headers = http.CaseInsensitiveDict(headers)
@@ -257,15 +256,14 @@
     :param upload_id: 分片上传ID
     :param marker: 分页符
     :param max_parts: 每次调用 `list_parts` 时的max_parts参数。注意迭代器返回的数目可能会大于该值。
 
     :param headers: HTTP头部
     :type headers: 可以是dict，建议是oss2.CaseInsensitiveDict
     """
-
     def __init__(self, bucket, key, upload_id,
                  marker='0', max_parts=1000, max_retries=None, headers=None):
         super(PartIterator, self).__init__(marker, max_retries)
 
         self.bucket = bucket
         self.key = key
         self.upload_id = upload_id
@@ -288,15 +286,14 @@
     每次迭代返回的是 :class:`LiveChannelInfo <oss2.models.LiveChannelInfo>` 对象。
 
     :param bucket: :class:`Bucket <oss2.Bucket>` 对象
     :param prefix: 只列举匹配该前缀的文件
     :param marker: 分页符
     :param max_keys: 每次调用 `list_live_channel` 时的max_keys参数。注意迭代器返回的数目可能会大于该值。
     """
-
     def __init__(self, bucket, prefix='', marker='', max_keys=100, max_retries=None):
         super(LiveChannelIterator, self).__init__(marker, max_retries)
 
         self.bucket = bucket
         self.prefix = prefix
         self.max_keys = max_keys
```

### Comparing `asyncio-oss-1.0.2/asyncio_oss/test/__init__.py` & `asyncio-oss-1.1.0/asyncio_oss/test/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.0.2/asyncio_oss/test/object_test.py` & `asyncio-oss-1.1.0/asyncio_oss/test/object_test.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.0.2/asyncio_oss.egg-info/PKG-INFO` & `asyncio-oss-1.1.0/asyncio_oss.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio-oss
-Version: 1.0.2
+Version: 1.1.0
 Summary: An asynchronous python client SDK for OSS(Aliyun Object Storage Service).
 Home-page: https://github.com/Yaocool/async-oss
 Author: Ozzy
 Author-email: ozzycharon@gmail.com
 License: MIT
 Keywords: asyncio-oss,async-oss,oss
 Description-Content-Type: text/markdown
@@ -24,14 +24,16 @@
 $ git clone git@github.com:Yaocool/async-oss.git
 $ python setup.py bdist_wheel
 $ pip install ./dist/asyncio_oss-1.0.0-py3-none-any.whl
 ```
 
 # Example
 ```python
+import logging
+
 import asyncio_oss
 import asyncio
 import oss2
 
 OSS_ENDPOINT = 'https://oss-cn-hangzhou.aliyuncs.com'  # definition in https://help.aliyun.com/document_detail/31837.html
 OSS_KEY = '<Your AccessKeyID>'
 OSS_SECRET = '<Your AccessKeySecret>'
@@ -58,14 +60,17 @@
             print(obj.key)
 
         # Delete Object
         await bucket.delete_object(OBJECT_KEY)
 
 
 if __name__ == '__main__':
+    # open global log
+    log_file_path = "example_logfile.log"
+    asyncio_oss.set_file_logger(log_file_path, 'asyncio_oss', logging.DEBUG)
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
 # ChangeLogs
 * [Jul 29, 2022 - 1.0.0]
   * fix `http.py/do_request` method stream read bug
@@ -74,10 +79,15 @@
 * [May 30, 2023 - 1.0.1]
   * bump version to 1.0.1 for PyPI package description updating
 * [June 24, 2023 - 1.0.2]
   * remove unused fields add params in `asyncio_oss/http.py api.py` files
   * fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug
   * add `list_buckets` test case in `tests/service_test.py` for `Service` class
   * bump version to 1.0.2
+* [June 27, 2023 - 1.1.0]
+  * remove unused objects and methods in `asyncio_oss/models.py` and `asyncio_oss/utils.py` to streamline sdk package
+  * support oss2==2.18.0 newest apis
+  * support global log
+  * bump version to 1.1.0
 
-# Discussions
-Any questions can be raised in Discussions, I will answer them from time to time~
+# Discussions Or Issues
+Any questions can be raised in `Discussions` or `Issues`, I will answer them from time to time.
```

### Comparing `asyncio-oss-1.0.2/setup.py` & `asyncio-oss-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='asyncio-oss',
-    version='1.0.2',
+    version='1.1.0',
     description='An asynchronous python client SDK for OSS(Aliyun Object Storage Service).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Yaocool/async-oss",
     keywords="asyncio-oss, async-oss, oss",
     author='Ozzy',
     author_email='ozzycharon@gmail.com',
```

