# Comparing `tmp/tencentcloud-sdk-python-trp-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-trp-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.920.tar", last modified: Thu Jun 22 00:38:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.921.tar", last modified: Mon Jun 26 00:36:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trp-3.0.920.tar` & `tencentcloud-sdk-python-trp-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/v20210515/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/v20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43764 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/v20210515/trp_client.py
--rw-r--r--   0 root         (0) root         (0)   139995 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/v20210515/models.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/v20210515/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud_sdk_python_trp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:38:22.000000 tencentcloud-sdk-python-trp-3.0.920/tencentcloud_sdk_python_trp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/v20210515/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/v20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43764 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/v20210515/trp_client.py
+-rw-r--r--   0 root         (0) root         (0)   144848 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/v20210515/models.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/v20210515/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud_sdk_python_trp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:36:02.000000 tencentcloud-sdk-python-trp-3.0.921/tencentcloud_sdk_python_trp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trp-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trp-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/v20210515/trp_client.py` & `tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/v20210515/trp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/v20210515/models.py` & `tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/v20210515/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,81 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class AttrItem(AbstractModel):
+    """通用属性
+
+    Type 的枚举值
+    text:文本类型, longtext:长文本类型, banner:单图片类型, image:多图片类型, video:视频类型, mp:小程序类型
+
+    具体组合如下
+    - Type: "text" 文本类型, 对应值 Value: "文本字符串"
+    - Type: "longtext" 长文本类型, 对应值 Value: "长文本字符串, 支持换行\n"
+    - Type: "banner" 单图片类型, 对应图片地址 Value: "https://sample.cdn.com/xxx.jpg"
+    - Type: "image" 多图片类型, 对应图片地址 Values: ["https://sample.cdn.com/1.jpg", "https://sample.cdn.com/2.jpg"]
+    - Type: "video" 视频类型, 对应视频地址 Value: "https://sample.cdn.com/xxx.mp4"
+    - Type: "mp" 小程序类型, 对应配置 Values: ["WXAPPID", "WXAPP_PATH", "跳转说明"]
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 字段名称
+        :type Name: str
+        :param Value: 字段值
+        :type Value: str
+        :param Type: 字段类型
+text:文本类型, 
+longtext:长文本类型, banner:单图片类型, image:多图片类型,
+video:视频类型,
+mp:小程序类型
+        :type Type: str
+        :param ReadOnly: 只读
+        :type ReadOnly: bool
+        :param Hidden: 扫码展示
+        :type Hidden: bool
+        :param Values: 多个值
+        :type Values: list of str
+        :param Key: 类型标识
+        :type Key: str
+        :param Ext: 扩展字段
+        :type Ext: str
+        """
+        self.Name = None
+        self.Value = None
+        self.Type = None
+        self.ReadOnly = None
+        self.Hidden = None
+        self.Values = None
+        self.Key = None
+        self.Ext = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Value = params.get("Value")
+        self.Type = params.get("Type")
+        self.ReadOnly = params.get("ReadOnly")
+        self.Hidden = params.get("Hidden")
+        self.Values = params.get("Values")
+        self.Key = params.get("Key")
+        self.Ext = params.get("Ext")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AuthorizedTransferRequest(AbstractModel):
     """AuthorizedTransfer请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -156,14 +223,22 @@
         :type Ext: :class:`tencentcloud.trp.v20210515.models.Ext`
         :param TplName: 模板名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type TplName: str
         :param Job: 调度任务
 注意：此字段可能返回 null，表示取不到有效值。
         :type Job: :class:`tencentcloud.trp.v20210515.models.Job`
+        :param ProductionDate: 生产日期
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProductionDate: str
+        :param ValidDate: 有效期
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ValidDate: str
+        :param Attrs: 扩展属性
+        :type Attrs: list of AttrItem
         """
         self.BatchId = None
         self.CorpId = None
         self.BatchCode = None
         self.CodeCnt = None
         self.MerchantId = None
         self.ProductId = None
@@ -174,14 +249,17 @@
         self.CreateTime = None
         self.UpdateTime = None
         self.MerchantName = None
         self.ProductName = None
         self.Ext = None
         self.TplName = None
         self.Job = None
+        self.ProductionDate = None
+        self.ValidDate = None
+        self.Attrs = None
 
 
     def _deserialize(self, params):
         self.BatchId = params.get("BatchId")
         self.CorpId = params.get("CorpId")
         self.BatchCode = params.get("BatchCode")
         self.CodeCnt = params.get("CodeCnt")
@@ -198,14 +276,22 @@
         if params.get("Ext") is not None:
             self.Ext = Ext()
             self.Ext._deserialize(params.get("Ext"))
         self.TplName = params.get("TplName")
         if params.get("Job") is not None:
             self.Job = Job()
             self.Job._deserialize(params.get("Job"))
+        self.ProductionDate = params.get("ProductionDate")
+        self.ValidDate = params.get("ValidDate")
+        if params.get("Attrs") is not None:
+            self.Attrs = []
+            for item in params.get("Attrs"):
+                obj = AttrItem()
+                obj._deserialize(item)
+                self.Attrs.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -465,36 +551,44 @@
         :type Remark: str
         :param MpTpl: 模版ID，或者活动ID
         :type MpTpl: str
         :param CloneId: 克隆批次ID，同时会复制溯源信息
         :type CloneId: str
         :param BatchCode: 批次编号，业务字段不判断唯一性
         :type BatchCode: str
+        :param ValidDate: 有效期
+        :type ValidDate: str
+        :param ProductionDate: 生产日期
+        :type ProductionDate: str
         """
         self.CorpId = None
         self.MerchantId = None
         self.ProductId = None
         self.BatchType = None
         self.BatchId = None
         self.Remark = None
         self.MpTpl = None
         self.CloneId = None
         self.BatchCode = None
+        self.ValidDate = None
+        self.ProductionDate = None
 
 
     def _deserialize(self, params):
         self.CorpId = params.get("CorpId")
         self.MerchantId = params.get("MerchantId")
         self.ProductId = params.get("ProductId")
         self.BatchType = params.get("BatchType")
         self.BatchId = params.get("BatchId")
         self.Remark = params.get("Remark")
         self.MpTpl = params.get("MpTpl")
         self.CloneId = params.get("CloneId")
         self.BatchCode = params.get("BatchCode")
+        self.ValidDate = params.get("ValidDate")
+        self.ProductionDate = params.get("ProductionDate")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2382,26 +2476,38 @@
 class DescribeScanLogsRequest(AbstractModel):
     """DescribeScanLogs请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Code: 码
-        :type Code: str
         :param CorpId: 企业ID
         :type CorpId: int
+        :param PageSize: 分页数量
+        :type PageSize: int
+        :param PageNumber: 当前分页
+        :type PageNumber: int
+        :param Code: 安心码
+        :type Code: str
+        :param Openid: 小程序用户ID
+        :type Openid: str
         """
-        self.Code = None
         self.CorpId = None
+        self.PageSize = None
+        self.PageNumber = None
+        self.Code = None
+        self.Openid = None
 
 
     def _deserialize(self, params):
-        self.Code = params.get("Code")
         self.CorpId = params.get("CorpId")
+        self.PageSize = params.get("PageSize")
+        self.PageNumber = params.get("PageNumber")
+        self.Code = params.get("Code")
+        self.Openid = params.get("Openid")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2411,15 +2517,14 @@
     """DescribeScanLogs返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param Products: 【弃用】
-注意：此字段可能返回 null，表示取不到有效值。
         :type Products: list of ScanLog
         :param TotalCount: 条数
         :type TotalCount: int
         :param ScanLogs: 扫描记录
         :type ScanLogs: list of ScanLog
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
@@ -2600,25 +2705,29 @@
 
     """
 
     def __init__(self):
         r"""
         :param TraceCode: 无
         :type TraceCode: :class:`tencentcloud.trp.v20210515.models.TraceCode`
+        :param CodePath: 码路径，如level是2，则为 [1级, 2级]
+        :type CodePath: list of str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TraceCode = None
+        self.CodePath = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("TraceCode") is not None:
             self.TraceCode = TraceCode()
             self.TraceCode._deserialize(params.get("TraceCode"))
+        self.CodePath = params.get("CodePath")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeTraceCodesRequest(AbstractModel):
     """DescribeTraceCodes请求参数结构体
 
     """
@@ -3022,34 +3131,42 @@
         :type MerchantId: str
         :param ProductId: 商品ID
         :type ProductId: str
         :param Remark: 备注
         :type Remark: str
         :param BatchCode: 批次编码，业务字段不判断唯一性
         :type BatchCode: str
+        :param ValidDate: 有效期
+        :type ValidDate: str
+        :param ProductionDate: 生产日期
+        :type ProductionDate: str
         """
         self.BatchId = None
         self.CorpId = None
         self.Status = None
         self.MpTpl = None
         self.MerchantId = None
         self.ProductId = None
         self.Remark = None
         self.BatchCode = None
+        self.ValidDate = None
+        self.ProductionDate = None
 
 
     def _deserialize(self, params):
         self.BatchId = params.get("BatchId")
         self.CorpId = params.get("CorpId")
         self.Status = params.get("Status")
         self.MpTpl = params.get("MpTpl")
         self.MerchantId = params.get("MerchantId")
         self.ProductId = params.get("ProductId")
         self.Remark = params.get("Remark")
         self.BatchCode = params.get("BatchCode")
+        self.ValidDate = params.get("ValidDate")
+        self.ProductionDate = params.get("ProductionDate")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3750,24 +3867,24 @@
 class Product(AbstractModel):
     """商品信息
 
     """
 
     def __init__(self):
         r"""
+        :param MerchantId: 商户标识码
+        :type MerchantId: str
+        :param Name: 商品名称
+        :type Name: str
         :param ProductId: 商品id
         :type ProductId: str
         :param CorpId: 企业id
         :type CorpId: int
-        :param MerchantId: 商户标识码
-        :type MerchantId: str
         :param ProductCode: 商品编号
         :type ProductCode: str
-        :param Name: 商品名称
-        :type Name: str
         :param Specification: 商品规格
 注意：此字段可能返回 null，表示取不到有效值。
         :type Specification: str
         :param Remark: 备注
 注意：此字段可能返回 null，表示取不到有效值。
         :type Remark: str
         :param Logo: 商品图片
@@ -3779,34 +3896,34 @@
         :type UpdateTime: str
         :param Ext: 预留字段
 注意：此字段可能返回 null，表示取不到有效值。
         :type Ext: :class:`tencentcloud.trp.v20210515.models.Ext`
         :param MerchantName: 商户名称
         :type MerchantName: str
         """
+        self.MerchantId = None
+        self.Name = None
         self.ProductId = None
         self.CorpId = None
-        self.MerchantId = None
         self.ProductCode = None
-        self.Name = None
         self.Specification = None
         self.Remark = None
         self.Logo = None
         self.CreateTime = None
         self.UpdateTime = None
         self.Ext = None
         self.MerchantName = None
 
 
     def _deserialize(self, params):
+        self.MerchantId = params.get("MerchantId")
+        self.Name = params.get("Name")
         self.ProductId = params.get("ProductId")
         self.CorpId = params.get("CorpId")
-        self.MerchantId = params.get("MerchantId")
         self.ProductCode = params.get("ProductCode")
-        self.Name = params.get("Name")
         self.Specification = params.get("Specification")
         self.Remark = params.get("Remark")
         self.Logo = params.get("Logo")
         self.CreateTime = params.get("CreateTime")
         self.UpdateTime = params.get("UpdateTime")
         if params.get("Ext") is not None:
             self.Ext = Ext()
@@ -3959,15 +4076,14 @@
     """扫码明细
 
     """
 
     def __init__(self):
         r"""
         :param LogId: 行ID
-注意：此字段可能返回 null，表示取不到有效值。
         :type LogId: int
         :param Openid: 微信openid
 注意：此字段可能返回 null，表示取不到有效值。
         :type Openid: str
         :param Nickname: 微信昵称
 注意：此字段可能返回 null，表示取不到有效值。
         :type Nickname: str
@@ -4006,14 +4122,22 @@
         :type Unionid: str
         :param First: 首次扫码 0:否, 1:是
 注意：此字段可能返回 null，表示取不到有效值。
         :type First: int
         :param BatchId: 批次ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type BatchId: str
+        :param Type: 扫码类型 0:无效扫码 1: 小程序扫码 2: 商家扫码
+        :type Type: int
+        :param MerchantName: 商户名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MerchantName: str
+        :param ProductName: 产品名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProductName: str
         """
         self.LogId = None
         self.Openid = None
         self.Nickname = None
         self.CreateTime = None
         self.Code = None
         self.CorpId = None
@@ -4023,14 +4147,17 @@
         self.Country = None
         self.Province = None
         self.City = None
         self.District = None
         self.Unionid = None
         self.First = None
         self.BatchId = None
+        self.Type = None
+        self.MerchantName = None
+        self.ProductName = None
 
 
     def _deserialize(self, params):
         self.LogId = params.get("LogId")
         self.Openid = params.get("Openid")
         self.Nickname = params.get("Nickname")
         self.CreateTime = params.get("CreateTime")
@@ -4042,14 +4169,17 @@
         self.Country = params.get("Country")
         self.Province = params.get("Province")
         self.City = params.get("City")
         self.District = params.get("District")
         self.Unionid = params.get("Unionid")
         self.First = params.get("First")
         self.BatchId = params.get("BatchId")
+        self.Type = params.get("Type")
+        self.MerchantName = params.get("MerchantName")
+        self.ProductName = params.get("ProductName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4212,16 +4342,14 @@
         :param Phase: 溯源阶段 0:商品 1:通用 2:生产溯源 3:销售溯源
         :type Phase: int
         :param PhaseName: 溯源环节名称
         :type PhaseName: str
         :param TraceTime: 溯源时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type TraceTime: str
-        :param TraceItems: 无
-        :type TraceItems: list of TraceItem
         :param CreateTime: 创建时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreateTime: str
         :param ChainStatus: 上链状态 0: 未上链 1: 上链中 2: 已上链 -1: 异常
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChainStatus: int
         :param ChainTime: 上链时间
@@ -4231,57 +4359,59 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChainData: :class:`tencentcloud.trp.v20210515.models.ChainData`
         :param PhaseData: 溯源阶段配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type PhaseData: :class:`tencentcloud.trp.v20210515.models.PhaseData`
         :param Status: 溯源阶段状态 0: 无效, 1: 有效
         :type Status: int
+        :param TraceItems: 无
+        :type TraceItems: list of TraceItem
         """
         self.TraceId = None
         self.CorpId = None
         self.Type = None
         self.Code = None
         self.Rank = None
         self.Phase = None
         self.PhaseName = None
         self.TraceTime = None
-        self.TraceItems = None
         self.CreateTime = None
         self.ChainStatus = None
         self.ChainTime = None
         self.ChainData = None
         self.PhaseData = None
         self.Status = None
+        self.TraceItems = None
 
 
     def _deserialize(self, params):
         self.TraceId = params.get("TraceId")
         self.CorpId = params.get("CorpId")
         self.Type = params.get("Type")
         self.Code = params.get("Code")
         self.Rank = params.get("Rank")
         self.Phase = params.get("Phase")
         self.PhaseName = params.get("PhaseName")
         self.TraceTime = params.get("TraceTime")
-        if params.get("TraceItems") is not None:
-            self.TraceItems = []
-            for item in params.get("TraceItems"):
-                obj = TraceItem()
-                obj._deserialize(item)
-                self.TraceItems.append(obj)
         self.CreateTime = params.get("CreateTime")
         self.ChainStatus = params.get("ChainStatus")
         self.ChainTime = params.get("ChainTime")
         if params.get("ChainData") is not None:
             self.ChainData = ChainData()
             self.ChainData._deserialize(params.get("ChainData"))
         if params.get("PhaseData") is not None:
             self.PhaseData = PhaseData()
             self.PhaseData._deserialize(params.get("PhaseData"))
         self.Status = params.get("Status")
+        if params.get("TraceItems") is not None:
+            self.TraceItems = []
+            for item in params.get("TraceItems"):
+                obj = TraceItem()
+                obj._deserialize(item)
+                self.TraceItems.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4310,48 +4440,48 @@
         :type Value: str
         :param Type: 字段类型
 text:文本类型, 
 longtext:长文本类型, banner:单图片类型, image:多图片类型,
 video:视频类型,
 mp:小程序类型
         :type Type: str
+        :param Values: 多个值
+        :type Values: list of str
         :param ReadOnly: 只读
         :type ReadOnly: bool
         :param Hidden: 扫码展示
         :type Hidden: bool
-        :param Values: 多个值
-        :type Values: list of str
         :param Key: 类型标识
         :type Key: str
         :param Ext: 扩展字段
         :type Ext: str
         :param Attrs: 额外属性
         :type Attrs: list of TraceItem
         :param List: 子页面，只读
         :type List: list of TraceData
         """
         self.Name = None
         self.Value = None
         self.Type = None
+        self.Values = None
         self.ReadOnly = None
         self.Hidden = None
-        self.Values = None
         self.Key = None
         self.Ext = None
         self.Attrs = None
         self.List = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Value = params.get("Value")
         self.Type = params.get("Type")
+        self.Values = params.get("Values")
         self.ReadOnly = params.get("ReadOnly")
         self.Hidden = params.get("Hidden")
-        self.Values = params.get("Values")
         self.Key = params.get("Key")
         self.Ext = params.get("Ext")
         if params.get("Attrs") is not None:
             self.Attrs = []
             for item in params.get("Attrs"):
                 obj = TraceItem()
                 obj._deserialize(item)
```

### Comparing `tencentcloud-sdk-python-trp-3.0.920/tencentcloud/trp/v20210515/errorcodes.py` & `tencentcloud-sdk-python-trp-3.0.921/tencentcloud/trp/v20210515/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.920/README.rst` & `tencentcloud-sdk-python-trp-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.921/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.920/setup.py` & `tencentcloud-sdk-python-trp-3.0.921/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.920/tencentcloud_sdk_python_trp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.921/tencentcloud_sdk_python_trp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

