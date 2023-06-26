# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.920.tar", last modified: Thu Jun 22 00:21:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.921.tar", last modified: Mon Jun 26 00:21:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.920.tar` & `tencentcloud-sdk-python-cynosdb-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   414005 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)   117543 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)    11095 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-22 00:21:47.000000 tencentcloud-sdk-python-cynosdb-3.0.920/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   415832 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)   118494 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    11095 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/setup.py
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6541,14 +6541,69 @@
         self.PoolId = params.get("PoolId")
         self.QueryId = params.get("QueryId")
         self.Status = params.get("Status")
         self.SuggestTime = params.get("SuggestTime")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeSupportProxyVersionRequest(AbstractModel):
+    """DescribeSupportProxyVersion请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
+        """
+        self.ClusterId = None
+        self.ProxyGroupId = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.ProxyGroupId = params.get("ProxyGroupId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeSupportProxyVersionResponse(AbstractModel):
+    """DescribeSupportProxyVersion返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SupportProxyVersions: 支持的数据库代理版本集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SupportProxyVersions: list of str
+        :param CurrentProxyVersion: 当前proxy版本号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CurrentProxyVersion: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.SupportProxyVersions = None
+        self.CurrentProxyVersion = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.SupportProxyVersions = params.get("SupportProxyVersions")
+        self.CurrentProxyVersion = params.get("CurrentProxyVersion")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeZonesRequest(AbstractModel):
     """DescribeZones请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1563,14 +1563,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeSupportProxyVersion(self, request):
+        """查询支持的数据库代理版本
+
+        :param request: Request instance for DescribeSupportProxyVersion.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeSupportProxyVersionRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeSupportProxyVersionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeSupportProxyVersion", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeSupportProxyVersionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeZones(self, request):
         """本接口(DescribeZones)用于查询可售卖地域可用区信息。
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeZonesRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeZonesResponse`
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.920/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.920/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.921/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.920/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.921/setup.py`

 * *Files identical despite different names*

