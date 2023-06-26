# Comparing `tmp/tencentcloud-sdk-python-tbaas-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-tbaas-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tbaas-3.0.920.tar", last modified: Thu Jun 22 00:35:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tbaas-3.0.921.tar", last modified: Mon Jun 26 00:32:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tbaas-3.0.920.tar` & `tencentcloud-sdk-python-tbaas-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/v20180416/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33385 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/v20180416/tbaas_client.py
--rw-r--r--   0 root         (0) root         (0)   111915 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)    11811 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud_sdk_python_tbaas.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud_sdk_python_tbaas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud_sdk_python_tbaas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud_sdk_python_tbaas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-22 00:35:17.000000 tencentcloud-sdk-python-tbaas-3.0.920/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/v20180416/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27553 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/v20180416/tbaas_client.py
+-rw-r--r--   0 root         (0) root         (0)    95691 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)    11697 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud_sdk_python_tbaas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud_sdk_python_tbaas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud_sdk_python_tbaas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud_sdk_python_tbaas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-26 00:32:55.000000 tencentcloud-sdk-python-tbaas-3.0.921/setup.py
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/v20180416/tbaas_client.py` & `tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/v20180416/tbaas_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,39 +91,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DeployDynamicBcosContract(self, request):
-        """Bcos区块链引擎已下线，请选用其他区块链引擎
-
-        动态部署并发布Bcos合约
-
-        :param request: Request instance for DeployDynamicBcosContract.
-        :type request: :class:`tencentcloud.tbaas.v20180416.models.DeployDynamicBcosContractRequest`
-        :rtype: :class:`tencentcloud.tbaas.v20180416.models.DeployDynamicBcosContractResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DeployDynamicBcosContract", params, headers=headers)
-            response = json.loads(body)
-            model = models.DeployDynamicBcosContractResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DownloadUserCert(self, request):
         """下载用户证书
 
         :param request: Request instance for DownloadUserCert.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.DownloadUserCertRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.DownloadUserCertResponse`
 
@@ -139,114 +114,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def GetBcosBlockByNumber(self, request):
-        """Bcos区块链引擎已下线，请选用其他区块链引擎
-
-        使用块高查询Bcos区块信息
-
-        :param request: Request instance for GetBcosBlockByNumber.
-        :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBcosBlockByNumberRequest`
-        :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetBcosBlockByNumberResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetBcosBlockByNumber", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetBcosBlockByNumberResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def GetBcosBlockList(self, request):
-        """Bcos区块链引擎已下线，请选用其他区块链引擎
-
-        Bcos分页查询当前群组下的区块列表
-
-        :param request: Request instance for GetBcosBlockList.
-        :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBcosBlockListRequest`
-        :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetBcosBlockListResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetBcosBlockList", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetBcosBlockListResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def GetBcosTransByHash(self, request):
-        """Bcos区块链引擎已下线，请选用其他区块链引擎
-
-        Bcos根据交易哈希查看交易详细信息
-
-        :param request: Request instance for GetBcosTransByHash.
-        :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBcosTransByHashRequest`
-        :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetBcosTransByHashResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetBcosTransByHash", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetBcosTransByHashResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def GetBcosTransList(self, request):
-        """Bcos区块链引擎已下线，请选用其他区块链引擎
-
-        Bcos分页查询当前群组的交易信息列表
-
-        :param request: Request instance for GetBcosTransList.
-        :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBcosTransListRequest`
-        :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetBcosTransListResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetBcosTransList", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetBcosTransListResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def GetBlockList(self, request):
         """查看当前网络下的所有区块列表，分页展示
 
         :param request: Request instance for GetBlockList.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBlockListRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetBlockListResponse`
 
@@ -582,39 +457,14 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
-
-
-    def InvokeBcosTrans(self, request):
-        """Bcos区块链引擎已下线，请选用其他区块链引擎
-
-        执行Bcos交易，支持动态部署的合约
-
-        :param request: Request instance for InvokeBcosTrans.
-        :type request: :class:`tencentcloud.tbaas.v20180416.models.InvokeBcosTransRequest`
-        :rtype: :class:`tencentcloud.tbaas.v20180416.models.InvokeBcosTransResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("InvokeBcosTrans", params, headers=headers)
-            response = json.loads(body)
-            model = models.InvokeBcosTransResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
 
 
     def InvokeChainMakerContract(self, request):
         """调用长安链合约执行交易
 
         :param request: Request instance for InvokeChainMakerContract.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.InvokeChainMakerContractRequest`
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/v20180416/models.py` & `tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/v20180416/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -150,114 +150,14 @@
 
     def _deserialize(self, params):
         self.CertId = params.get("CertId")
         self.CertDn = params.get("CertDn")
         self.RequestId = params.get("RequestId")
 
 
-class BcosBlockObj(AbstractModel):
-    """Bcos区块对象
-
-    """
-
-    def __init__(self):
-        r"""
-        :param BlockHash: 区块哈希
-        :type BlockHash: str
-        :param BlockNumber: 区块高度
-        :type BlockNumber: int
-        :param BlockTimestamp: 区块时间戳
-        :type BlockTimestamp: str
-        :param Sealer: 打包节点ID
-        :type Sealer: str
-        :param SealerIndex: 打包节点索引
-        :type SealerIndex: int
-        :param CreateTime: 记录保存时间
-        :type CreateTime: str
-        :param TransCount: 交易数量
-        :type TransCount: int
-        :param ModifyTime: 记录修改时间
-        :type ModifyTime: str
-        """
-        self.BlockHash = None
-        self.BlockNumber = None
-        self.BlockTimestamp = None
-        self.Sealer = None
-        self.SealerIndex = None
-        self.CreateTime = None
-        self.TransCount = None
-        self.ModifyTime = None
-
-
-    def _deserialize(self, params):
-        self.BlockHash = params.get("BlockHash")
-        self.BlockNumber = params.get("BlockNumber")
-        self.BlockTimestamp = params.get("BlockTimestamp")
-        self.Sealer = params.get("Sealer")
-        self.SealerIndex = params.get("SealerIndex")
-        self.CreateTime = params.get("CreateTime")
-        self.TransCount = params.get("TransCount")
-        self.ModifyTime = params.get("ModifyTime")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class BcosTransInfo(AbstractModel):
-    """Bcos交易信息对象
-
-    """
-
-    def __init__(self):
-        r"""
-        :param BlockNumber: 所属区块高度
-        :type BlockNumber: int
-        :param BlockTimestamp: 区块时间戳
-        :type BlockTimestamp: str
-        :param TransHash: 交易哈希
-        :type TransHash: str
-        :param TransFrom: 交易发起者
-        :type TransFrom: str
-        :param TransTo: 交易接收者
-        :type TransTo: str
-        :param CreateTime: 落库时间
-        :type CreateTime: str
-        :param ModifyTime: 修改时间
-        :type ModifyTime: str
-        """
-        self.BlockNumber = None
-        self.BlockTimestamp = None
-        self.TransHash = None
-        self.TransFrom = None
-        self.TransTo = None
-        self.CreateTime = None
-        self.ModifyTime = None
-
-
-    def _deserialize(self, params):
-        self.BlockNumber = params.get("BlockNumber")
-        self.BlockTimestamp = params.get("BlockTimestamp")
-        self.TransHash = params.get("TransHash")
-        self.TransFrom = params.get("TransFrom")
-        self.TransTo = params.get("TransTo")
-        self.CreateTime = params.get("CreateTime")
-        self.ModifyTime = params.get("ModifyTime")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class Block(AbstractModel):
     """区块对象
 
     """
 
     def __init__(self):
         r"""
@@ -545,79 +445,14 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
-class DeployDynamicBcosContractRequest(AbstractModel):
-    """DeployDynamicBcosContract请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClusterId: 网络ID，可在区块链网络详情或列表中获取
-        :type ClusterId: str
-        :param GroupId: 群组编号，可在群组列表中获取
-        :type GroupId: int
-        :param AbiInfo: 合约编译后的ABI，可在合约详情获取
-        :type AbiInfo: str
-        :param ByteCodeBin: 合约编译得到的字节码，hex编码，可在合约详情获取
-        :type ByteCodeBin: str
-        :param SignUserId: 签名用户编号，可在私钥管理页面获取
-        :type SignUserId: str
-        :param ConstructorParams: 构造函数入参，Json数组，多个参数以逗号分隔（参数为数组时同理），如：["str1",["arr1","arr2"]]
-        :type ConstructorParams: str
-        """
-        self.ClusterId = None
-        self.GroupId = None
-        self.AbiInfo = None
-        self.ByteCodeBin = None
-        self.SignUserId = None
-        self.ConstructorParams = None
-
-
-    def _deserialize(self, params):
-        self.ClusterId = params.get("ClusterId")
-        self.GroupId = params.get("GroupId")
-        self.AbiInfo = params.get("AbiInfo")
-        self.ByteCodeBin = params.get("ByteCodeBin")
-        self.SignUserId = params.get("SignUserId")
-        self.ConstructorParams = params.get("ConstructorParams")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DeployDynamicBcosContractResponse(AbstractModel):
-    """DeployDynamicBcosContract返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ContractAddress: 部署成功返回的合约地址
-        :type ContractAddress: str
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.ContractAddress = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.ContractAddress = params.get("ContractAddress")
-        self.RequestId = params.get("RequestId")
-
-
 class DownloadUserCertRequest(AbstractModel):
     """DownloadUserCert请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -707,268 +542,14 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class GetBcosBlockByNumberRequest(AbstractModel):
-    """GetBcosBlockByNumber请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClusterId: 网络ID，可在区块链网络详情或列表中获取
-        :type ClusterId: str
-        :param GroupId: 群组编号，可在群组列表中获取
-        :type GroupId: int
-        :param BlockNumber: 区块高度，可以从InvokeBcosTrans接口的返回值中解析获取
-        :type BlockNumber: int
-        """
-        self.ClusterId = None
-        self.GroupId = None
-        self.BlockNumber = None
-
-
-    def _deserialize(self, params):
-        self.ClusterId = params.get("ClusterId")
-        self.GroupId = params.get("GroupId")
-        self.BlockNumber = params.get("BlockNumber")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class GetBcosBlockByNumberResponse(AbstractModel):
-    """GetBcosBlockByNumber返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param BlockJson: 返回区块json字符串
-        :type BlockJson: str
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.BlockJson = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.BlockJson = params.get("BlockJson")
-        self.RequestId = params.get("RequestId")
-
-
-class GetBcosBlockListRequest(AbstractModel):
-    """GetBcosBlockList请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClusterId: 网络ID，可在区块链网络详情或列表中获取
-        :type ClusterId: str
-        :param GroupId: 群组编号，可在群组列表中获取
-        :type GroupId: int
-        :param PageNumber: 当前页数，默认为1
-        :type PageNumber: int
-        :param PageSize: 每页记录数，默认为10
-        :type PageSize: int
-        :param BlockNumber: 区块高度，可以从InvokeBcosTrans接口的返回值中解析获取
-        :type BlockNumber: int
-        :param BlockHash: 区块哈希，可以从InvokeBcosTrans接口的返回值中解析获取
-        :type BlockHash: str
-        """
-        self.ClusterId = None
-        self.GroupId = None
-        self.PageNumber = None
-        self.PageSize = None
-        self.BlockNumber = None
-        self.BlockHash = None
-
-
-    def _deserialize(self, params):
-        self.ClusterId = params.get("ClusterId")
-        self.GroupId = params.get("GroupId")
-        self.PageNumber = params.get("PageNumber")
-        self.PageSize = params.get("PageSize")
-        self.BlockNumber = params.get("BlockNumber")
-        self.BlockHash = params.get("BlockHash")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class GetBcosBlockListResponse(AbstractModel):
-    """GetBcosBlockList返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TotalCount: 总记录数
-        :type TotalCount: int
-        :param List: 返回数据列表
-        :type List: list of BcosBlockObj
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.TotalCount = None
-        self.List = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.TotalCount = params.get("TotalCount")
-        if params.get("List") is not None:
-            self.List = []
-            for item in params.get("List"):
-                obj = BcosBlockObj()
-                obj._deserialize(item)
-                self.List.append(obj)
-        self.RequestId = params.get("RequestId")
-
-
-class GetBcosTransByHashRequest(AbstractModel):
-    """GetBcosTransByHash请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClusterId: 网络ID，可在区块链网络详情或列表中获取
-        :type ClusterId: str
-        :param GroupId: 群组编号，可在群组列表中获取
-        :type GroupId: int
-        :param TransHash: 交易哈希值，可以从InvokeBcosTrans接口的返回值中解析获取
-        :type TransHash: str
-        """
-        self.ClusterId = None
-        self.GroupId = None
-        self.TransHash = None
-
-
-    def _deserialize(self, params):
-        self.ClusterId = params.get("ClusterId")
-        self.GroupId = params.get("GroupId")
-        self.TransHash = params.get("TransHash")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class GetBcosTransByHashResponse(AbstractModel):
-    """GetBcosTransByHash返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TransactionJson: 交易信息json字符串
-        :type TransactionJson: str
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.TransactionJson = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.TransactionJson = params.get("TransactionJson")
-        self.RequestId = params.get("RequestId")
-
-
-class GetBcosTransListRequest(AbstractModel):
-    """GetBcosTransList请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClusterId: 网络ID，可在区块链网络详情或列表中获取
-        :type ClusterId: str
-        :param GroupId: 群组编号，可在群组列表中获取
-        :type GroupId: int
-        :param PageNumber: 当前页数，默认是1
-        :type PageNumber: int
-        :param PageSize: 每页记录数，默认为10
-        :type PageSize: int
-        :param BlockNumber: 区块高度，可以从InvokeBcosTrans接口的返回值中解析获取
-        :type BlockNumber: int
-        :param TransHash: 交易哈希，可以从InvokeBcosTrans接口的返回值中解析获取
-        :type TransHash: str
-        """
-        self.ClusterId = None
-        self.GroupId = None
-        self.PageNumber = None
-        self.PageSize = None
-        self.BlockNumber = None
-        self.TransHash = None
-
-
-    def _deserialize(self, params):
-        self.ClusterId = params.get("ClusterId")
-        self.GroupId = params.get("GroupId")
-        self.PageNumber = params.get("PageNumber")
-        self.PageSize = params.get("PageSize")
-        self.BlockNumber = params.get("BlockNumber")
-        self.TransHash = params.get("TransHash")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class GetBcosTransListResponse(AbstractModel):
-    """GetBcosTransList返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TotalCount: 总记录数
-        :type TotalCount: int
-        :param List: 返回数据列表
-        :type List: list of BcosTransInfo
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.TotalCount = None
-        self.List = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.TotalCount = params.get("TotalCount")
-        if params.get("List") is not None:
-            self.List = []
-            for item in params.get("List"):
-                obj = BcosTransInfo()
-                obj._deserialize(item)
-                self.List.append(obj)
-        self.RequestId = params.get("RequestId")
-
-
 class GetBlockListRequest(AbstractModel):
     """GetBlockList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2201,83 +1782,14 @@
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.RequestId = params.get("RequestId")
 
 
-class InvokeBcosTransRequest(AbstractModel):
-    """InvokeBcosTrans请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClusterId: 网络ID，可在区块链网络详情或列表中获取
-        :type ClusterId: str
-        :param GroupId: 群组编号，可在群组列表中获取
-        :type GroupId: int
-        :param ContractAddress: 合约地址，可在合约详情获取
-        :type ContractAddress: str
-        :param AbiInfo: 合约Abi的json数组格式的字符串，可在合约详情获取
-        :type AbiInfo: str
-        :param FuncName: 合约方法名
-        :type FuncName: str
-        :param SignUserId: 签名用户编号，可在私钥管理页面获取
-        :type SignUserId: str
-        :param FuncParam: 合约方法入参，json格式字符串
-        :type FuncParam: str
-        """
-        self.ClusterId = None
-        self.GroupId = None
-        self.ContractAddress = None
-        self.AbiInfo = None
-        self.FuncName = None
-        self.SignUserId = None
-        self.FuncParam = None
-
-
-    def _deserialize(self, params):
-        self.ClusterId = params.get("ClusterId")
-        self.GroupId = params.get("GroupId")
-        self.ContractAddress = params.get("ContractAddress")
-        self.AbiInfo = params.get("AbiInfo")
-        self.FuncName = params.get("FuncName")
-        self.SignUserId = params.get("SignUserId")
-        self.FuncParam = params.get("FuncParam")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class InvokeBcosTransResponse(AbstractModel):
-    """InvokeBcosTrans返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TransactionRsp: 交易结果json字符串
-        :type TransactionRsp: str
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.TransactionRsp = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.TransactionRsp = params.get("TransactionRsp")
-        self.RequestId = params.get("RequestId")
-
-
 class InvokeChainMakerContractRequest(AbstractModel):
     """InvokeChainMakerContract请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud/tbaas/v20180416/errorcodes.py` & `tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud/tbaas/v20180416/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,17 +211,14 @@
 
 # 后台服务请求超时。
 FAILEDOPERATION_TIMEOUTURL = 'FailedOperation.TimeOutUrl'
 
 # 交易执行超时，请稍后再试。
 FAILEDOPERATION_TRANSACTIONTIMEOUT = 'FailedOperation.TransactionTimeout'
 
-# Bcos更新已部署合约。
-FAILEDOPERATION_UPDATEDEPLOYEDCONTRACT = 'FailedOperation.UpdateDeployedContract'
-
 # 获取用户认证类型出错。
 FAILEDOPERATION_USERAUTHTYPE = 'FailedOperation.UserAuthType'
 
 # 您因违反用户协议，目前无法使用长安链体验网络。
 FAILEDOPERATION_USERINBLACKLIST = 'FailedOperation.UserInBlackList'
 
 # 用户未加入体验网络。
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.920/README.rst` & `tencentcloud-sdk-python-tbaas-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbaas-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-tbaas-3.0.921/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbaas
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Tbaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.920/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tbaas-3.0.921/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbaas
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Tbaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.920/setup.py` & `tencentcloud-sdk-python-tbaas-3.0.921/setup.py`

 * *Files identical despite different names*

