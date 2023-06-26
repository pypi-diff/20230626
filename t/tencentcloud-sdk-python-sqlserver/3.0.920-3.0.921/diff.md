# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.920.tar", last modified: Thu Jun 22 00:33:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.921.tar", last modified: Mon Jun 26 00:31:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.920.tar` & `tencentcloud-sdk-python-sqlserver-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:33:55.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:33:55.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:33:55.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)   349517 2023-06-22 00:33:55.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)   106575 2023-06-22 00:33:55.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-06-22 00:33:55.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-06-22 00:33:55.000000 tencentcloud-sdk-python-sqlserver-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-22 00:33:55.000000 tencentcloud-sdk-python-sqlserver-3.0.920/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:33:56.000000 tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   351489 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)   106575 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:31:52.000000 tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/v20180328/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2174,22 +2174,25 @@
         :type CreateTime: str
         :param Status: 数据库状态。1--创建中， 2--运行中， 3--修改中，-1--删除中
         :type Status: int
         :param Accounts: 数据库账号权限信息
         :type Accounts: list of AccountPrivilege
         :param InternalStatus: 内部状态。ONLINE表示运行中
         :type InternalStatus: str
+        :param Encryption: 是否已开启TDE加密，enable-已加密，disable-未加密
+        :type Encryption: str
         """
         self.Name = None
         self.Charset = None
         self.Remark = None
         self.CreateTime = None
         self.Status = None
         self.Accounts = None
         self.InternalStatus = None
+        self.Encryption = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Charset = params.get("Charset")
         self.Remark = params.get("Remark")
         self.CreateTime = params.get("CreateTime")
@@ -2197,14 +2200,15 @@
         if params.get("Accounts") is not None:
             self.Accounts = []
             for item in params.get("Accounts"):
                 obj = AccountPrivilege()
                 obj._deserialize(item)
                 self.Accounts.append(obj)
         self.InternalStatus = params.get("InternalStatus")
+        self.Encryption = params.get("Encryption")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4033,37 +4037,43 @@
         :type RegularBackupCounts: int
         :param RegularBackupStartTime: 定期备份开始日期，格式-YYYY-MM-DD 默认当前日期
         :type RegularBackupStartTime: str
         :param BlockedThreshold: 阻塞进程阈值，单位毫秒
         :type BlockedThreshold: int
         :param EventSaveDays: 慢SQL、阻塞、死锁扩展事件文件保留时长
         :type EventSaveDays: int
+        :param TDEConfig: TDE透明数据加密配置
+        :type TDEConfig: :class:`tencentcloud.sqlserver.v20180328.models.TDEConfigAttribute`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.InstanceId = None
         self.RegularBackupEnable = None
         self.RegularBackupSaveDays = None
         self.RegularBackupStrategy = None
         self.RegularBackupCounts = None
         self.RegularBackupStartTime = None
         self.BlockedThreshold = None
         self.EventSaveDays = None
+        self.TDEConfig = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.RegularBackupEnable = params.get("RegularBackupEnable")
         self.RegularBackupSaveDays = params.get("RegularBackupSaveDays")
         self.RegularBackupStrategy = params.get("RegularBackupStrategy")
         self.RegularBackupCounts = params.get("RegularBackupCounts")
         self.RegularBackupStartTime = params.get("RegularBackupStartTime")
         self.BlockedThreshold = params.get("BlockedThreshold")
         self.EventSaveDays = params.get("EventSaveDays")
+        if params.get("TDEConfig") is not None:
+            self.TDEConfig = TDEConfigAttribute()
+            self.TDEConfig._deserialize(params.get("TDEConfig"))
         self.RequestId = params.get("RequestId")
 
 
 class DescribeDBInstancesRequest(AbstractModel):
     """DescribeDBInstances请求参数结构体
 
     """
@@ -4306,28 +4316,32 @@
         :type Limit: int
         :param Offset: 分页返回，页编号，默认值为第0页
         :type Offset: int
         :param Name: 数据库名称
         :type Name: str
         :param OrderByType: 排序规则（desc-降序，asc-升序），默认desc
         :type OrderByType: str
+        :param Encryption: 是否已开启TDE加密，enable-已加密，disable-未加密
+        :type Encryption: str
         """
         self.InstanceIdSet = None
         self.Limit = None
         self.Offset = None
         self.Name = None
         self.OrderByType = None
+        self.Encryption = None
 
 
     def _deserialize(self, params):
         self.InstanceIdSet = params.get("InstanceIdSet")
         self.Limit = params.get("Limit")
         self.Offset = params.get("Offset")
         self.Name = params.get("Name")
         self.OrderByType = params.get("OrderByType")
+        self.Encryption = params.get("Encryption")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -9673,14 +9687,47 @@
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.RequestId = params.get("RequestId")
 
 
+class TDEConfigAttribute(AbstractModel):
+    """TDE透明数据加密配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Encryption: 是否已开通TDE加密，enable-已开通，disable-未开通
+        :type Encryption: str
+        :param CertificateAttribution: 证书归属。self-表示使用该账号自身的证书，others-表示引用其他账号的证书，none-表示没有证书
+        :type CertificateAttribution: str
+        :param QuoteUin: 开通TDE加密时引用的其他主账号ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QuoteUin: str
+        """
+        self.Encryption = None
+        self.CertificateAttribution = None
+        self.QuoteUin = None
+
+
+    def _deserialize(self, params):
+        self.Encryption = params.get("Encryption")
+        self.CertificateAttribution = params.get("CertificateAttribution")
+        self.QuoteUin = params.get("QuoteUin")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class TerminateDBInstanceRequest(AbstractModel):
     """TerminateDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.920/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.921/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.920/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.921/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.920/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.921/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

