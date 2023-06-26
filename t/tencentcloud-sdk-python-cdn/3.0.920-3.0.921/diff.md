# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.920.tar", last modified: Thu Jun 22 00:19:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.921.tar", last modified: Mon Jun 26 00:19:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.920.tar` & `tencentcloud-sdk-python-cdn-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   573678 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)    80792 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)    21972 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-22 00:19:10.000000 tencentcloud-sdk-python-cdn-3.0.920/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   575031 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)    82219 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)    21972 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 00:19:05.000000 tencentcloud-sdk-python-cdn-3.0.921/setup.py
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10821,14 +10821,63 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ModifyDomainConfigRequest(AbstractModel):
+    """ModifyDomainConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Domain: 域名
+        :type Domain: str
+        :param Route: 配置路径
+        :type Route: str
+        :param Value: 配置路径值，使用 json 进行序列化，其中固定 update 作为 key
+        :type Value: str
+        """
+        self.Domain = None
+        self.Route = None
+        self.Value = None
+
+
+    def _deserialize(self, params):
+        self.Domain = params.get("Domain")
+        self.Route = params.get("Route")
+        self.Value = params.get("Value")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyDomainConfigResponse(AbstractModel):
+    """ModifyDomainConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyPurgeFetchTaskStatusRequest(AbstractModel):
     """ModifyPurgeFetchTaskStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1591,14 +1591,41 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyDomainConfig(self, request):
+        """ModifyDomainConfig 用于修改内容分发网络加速域名配置信息
+        注意：
+        Route 字段，使用点分隔，最后一段称为叶子节点，非叶子节点配置保持不变；
+        Value 字段，使用 json 进行序列化，其中固定 update 作为 key，配置路径值参考 https://cloud.tencent.com/document/product/228/41116 接口各配置项复杂类型，为配置路径对应复杂类型下的节点。
+        云审计相关：接口的入参可能包含密钥等敏感信息，所以此接口的入参不会上报到云审计。
+
+        :param request: Request instance for ModifyDomainConfig.
+        :type request: :class:`tencentcloud.cdn.v20180606.models.ModifyDomainConfigRequest`
+        :rtype: :class:`tencentcloud.cdn.v20180606.models.ModifyDomainConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyDomainConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyDomainConfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyPurgeFetchTaskStatus(self, request):
         """ModifyPurgeFetchTaskStatus 用于上报定时刷新预热任务执行状态
 
         :param request: Request instance for ModifyPurgeFetchTaskStatus.
         :type request: :class:`tencentcloud.cdn.v20180606.models.ModifyPurgeFetchTaskStatusRequest`
         :rtype: :class:`tencentcloud.cdn.v20180606.models.ModifyPurgeFetchTaskStatusResponse`
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.920/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.921/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.920/README.rst` & `tencentcloud-sdk-python-cdn-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.921/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.920/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.921/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.920/setup.py` & `tencentcloud-sdk-python-cdn-3.0.921/setup.py`

 * *Files identical despite different names*

