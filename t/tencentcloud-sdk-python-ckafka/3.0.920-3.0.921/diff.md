# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.920.tar", last modified: Thu Jun 22 00:20:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.921.tar", last modified: Mon Jun 26 00:20:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.920.tar` & `tencentcloud-sdk-python-ckafka-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   477031 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    70499 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-22 00:20:08.000000 tencentcloud-sdk-python-ckafka-3.0.920/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   486111 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    71620 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/setup.py
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2240,14 +2240,59 @@
     def _deserialize(self, params):
         if params.get("Result") is not None:
             self.Result = DatahubTopicResp()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class CreateInstancePostData(AbstractModel):
+    """创建后付费接口返回的 Data 数据结构
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: CreateInstancePre返回固定为0，不能作为CheckTaskStatus的查询条件。只是为了保证和后台数据结构对齐。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FlowId: int
+        :param DealNames: 订单号列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DealNames: list of str
+        :param InstanceId: 实例Id，当购买多个实例时，默认返回购买的第一个实例 id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param DealNameInstanceIdMapping: 订单和购买实例对应映射列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DealNameInstanceIdMapping: list of DealInstanceDTO
+        """
+        self.FlowId = None
+        self.DealNames = None
+        self.InstanceId = None
+        self.DealNameInstanceIdMapping = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.DealNames = params.get("DealNames")
+        self.InstanceId = params.get("InstanceId")
+        if params.get("DealNameInstanceIdMapping") is not None:
+            self.DealNameInstanceIdMapping = []
+            for item in params.get("DealNameInstanceIdMapping"):
+                obj = DealInstanceDTO()
+                obj._deserialize(item)
+                self.DealNameInstanceIdMapping.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CreateInstancePostRequest(AbstractModel):
     """CreateInstancePost请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2332,14 +2377,49 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CreateInstancePostResp(AbstractModel):
+    """后付费实例相关接口返回结构
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ReturnCode: 返回的code，0为正常，非0为错误
+        :type ReturnCode: str
+        :param ReturnMessage: 接口返回消息，当接口报错时提示错误信息
+        :type ReturnMessage: str
+        :param Data: 返回的Data数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Data: :class:`tencentcloud.ckafka.v20190819.models.CreateInstancePostData`
+        """
+        self.ReturnCode = None
+        self.ReturnMessage = None
+        self.Data = None
+
+
+    def _deserialize(self, params):
+        self.ReturnCode = params.get("ReturnCode")
+        self.ReturnMessage = params.get("ReturnMessage")
+        if params.get("Data") is not None:
+            self.Data = CreateInstancePostData()
+            self.Data._deserialize(params.get("Data"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CreateInstancePostResponse(AbstractModel):
     """CreateInstancePost返回参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2620,14 +2700,129 @@
     def _deserialize(self, params):
         if params.get("Result") is not None:
             self.Result = JgwOperateResponse()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class CreatePostPaidInstanceRequest(AbstractModel):
+    """CreatePostPaidInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceName: 实例名称，是一个不超过 64 个字符的字符串，必须以字母为首字符，剩余部分可以包含字母、数字和横划线(-)
+        :type InstanceName: str
+        :param VpcId: 创建的实例默认接入点所在的 vpc 对应 vpcId。目前不支持创建基础网络实例，因此该参数必填
+        :type VpcId: str
+        :param SubnetId: 子网id。创建实例默认接入点所在的子网对应的子网 id
+        :type SubnetId: str
+        :param InstanceType: 实例规格。当创建标准版实例时必填，创建专业版实例时不需要填写。1：入门型；2：标准型；3：进阶型；4：容量型；5：高阶型1；6：高阶性2；7：高阶型3；8：高阶型4；9 ：独占型
+        :type InstanceType: int
+        :param MsgRetentionTime: 实例日志的默认最长保留时间，单位分钟。不传入该参数时默认为 1440 分钟（1天），最大30天。当 topic 显式设置消息保留时间时，以 topic 保留时间为准
+        :type MsgRetentionTime: int
+        :param ClusterId: 创建实例时可以选择集群Id, 该入参表示集群Id。不指定实例所在集群则不传入该参数
+        :type ClusterId: int
+        :param KafkaVersion: 实例版本。目前支持 "0.10.2","1.1.1","2.4.2","2.8.1"
+        :type KafkaVersion: str
+        :param SpecificationsType: 实例类型。"standard"：标准版，"profession"：专业版
+        :type SpecificationsType: str
+        :param DiskType: 实例硬盘类型，"CLOUD_BASIC"：云硬盘，"CLOUD_SSD"：高速云硬盘。不传默认为 "CLOUD_BASIC"
+        :type DiskType: str
+        :param BandWidth: 实例内网峰值带宽。单位 MB/s。标准版需传入当前实例规格所对应的峰值带宽。注意如果创建的实例为专业版实例，峰值带宽，分区数等参数配置需要满足专业版的计费规格。
+        :type BandWidth: int
+        :param DiskSize: 实例硬盘大小，需要满足当前实例的计费规格
+        :type DiskSize: int
+        :param Partition: 实例最大分区数量，需要满足当前实例的计费规格
+        :type Partition: int
+        :param TopicNum: 实例最大 topic 数量，需要满足当前实例的计费规格
+        :type TopicNum: int
+        :param ZoneId: 实例所在的可用区。当创建多可用区实例时，该参数为创建的默认接入点所在子网的可用区 id
+        :type ZoneId: int
+        :param MultiZoneFlag: 当前实例是否为多可用区实例。
+        :type MultiZoneFlag: bool
+        :param ZoneIds: 当实例为多可用区实例时，多可用区 id 列表。注意参数 ZoneId 对应的多可用区需要包含在该参数数组中
+        :type ZoneIds: list of int
+        :param InstanceNum: 购买实例数量。非必填，默认值为 1。当传入该参数时，会创建多个 instanceName 加后缀区分的实例
+        :type InstanceNum: int
+        :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 4Mbps 公网带宽，此处传 1
+        :type PublicNetworkMonthly: int
+        """
+        self.InstanceName = None
+        self.VpcId = None
+        self.SubnetId = None
+        self.InstanceType = None
+        self.MsgRetentionTime = None
+        self.ClusterId = None
+        self.KafkaVersion = None
+        self.SpecificationsType = None
+        self.DiskType = None
+        self.BandWidth = None
+        self.DiskSize = None
+        self.Partition = None
+        self.TopicNum = None
+        self.ZoneId = None
+        self.MultiZoneFlag = None
+        self.ZoneIds = None
+        self.InstanceNum = None
+        self.PublicNetworkMonthly = None
+
+
+    def _deserialize(self, params):
+        self.InstanceName = params.get("InstanceName")
+        self.VpcId = params.get("VpcId")
+        self.SubnetId = params.get("SubnetId")
+        self.InstanceType = params.get("InstanceType")
+        self.MsgRetentionTime = params.get("MsgRetentionTime")
+        self.ClusterId = params.get("ClusterId")
+        self.KafkaVersion = params.get("KafkaVersion")
+        self.SpecificationsType = params.get("SpecificationsType")
+        self.DiskType = params.get("DiskType")
+        self.BandWidth = params.get("BandWidth")
+        self.DiskSize = params.get("DiskSize")
+        self.Partition = params.get("Partition")
+        self.TopicNum = params.get("TopicNum")
+        self.ZoneId = params.get("ZoneId")
+        self.MultiZoneFlag = params.get("MultiZoneFlag")
+        self.ZoneIds = params.get("ZoneIds")
+        self.InstanceNum = params.get("InstanceNum")
+        self.PublicNetworkMonthly = params.get("PublicNetworkMonthly")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreatePostPaidInstanceResponse(AbstractModel):
+    """CreatePostPaidInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Result: 返回结果
+        :type Result: :class:`tencentcloud.ckafka.v20190819.models.CreateInstancePostResp`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Result") is not None:
+            self.Result = CreateInstancePostResp()
+            self.Result._deserialize(params.get("Result"))
+        self.RequestId = params.get("RequestId")
+
+
 class CreateRouteRequest(AbstractModel):
     """CreateRoute请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,14 +390,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreatePostPaidInstance(self, request):
+        """当前接口用来替代 CreateInstancePost 接口。创建按量计费实例。通常用于 SDK 或云 API 控制台调用接口，创建后付费 CKafka 实例。调用接口与在 CKafka 控制台购买按量付费实例效果相同。
+
+        :param request: Request instance for CreatePostPaidInstance.
+        :type request: :class:`tencentcloud.ckafka.v20190819.models.CreatePostPaidInstanceRequest`
+        :rtype: :class:`tencentcloud.ckafka.v20190819.models.CreatePostPaidInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreatePostPaidInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreatePostPaidInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateRoute(self, request):
         """添加实例路由
 
         :param request: Request instance for CreateRoute.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateRouteRequest`
         :rtype: :class:`tencentcloud.ckafka.v20190819.models.CreateRouteResponse`
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.920/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.921/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.920/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.920/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.921/setup.py`

 * *Files identical despite different names*

