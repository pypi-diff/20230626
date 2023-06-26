# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.920.tar", last modified: Thu Jun 22 00:32:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.921.tar", last modified: Mon Jun 26 00:30:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.920.tar` & `tencentcloud-sdk-python-postgres-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85773 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)   277941 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    20657 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/v20170312/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-22 00:32:05.000000 tencentcloud-sdk-python-postgres-3.0.920/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85773 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)   277957 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    20749 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/v20170312/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-26 00:30:10.000000 tencentcloud-sdk-python-postgres-3.0.921/setup.py
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1142,15 +1142,15 @@
 class CreateReadOnlyDBInstanceRequest(AbstractModel):
     """CreateReadOnlyDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param SpecCode: 售卖规格ID。该参数可以通过调用DescribeProductConfig的返回值中的SpecCode字段来获取。
+        :param SpecCode: 售卖规格ID。该参数可以通过调用DescribeClasses的返回值中的SpecCode字段来获取。
         :type SpecCode: str
         :param Storage: 实例容量大小，单位：GB。
         :type Storage: int
         :param InstanceCount: 一次性购买的实例数量。取值1-100
         :type InstanceCount: int
         :param Period: 购买时长，单位：月。目前只支持1,2,3,4,5,6,7,8,9,10,11,12,24,36这些值，按量计费模式下该参数传1。
         :type Period: int
@@ -1158,15 +1158,15 @@
         :type MasterDBInstanceId: str
         :param Zone: 可用区ID。该参数可以通过调用 DescribeZones 接口的返回值中的Zone字段来获取。
         :type Zone: str
         :param ProjectId: 项目ID。
         :type ProjectId: int
         :param DBVersion: 【废弃】不再需要指定，内核版本号与主实例保持一致
         :type DBVersion: str
-        :param InstanceChargeType: 实例计费类型。目前支持：PREPAID（预付费，即包年包月），POSTPAID_BY_HOUR（后付费，即按量计费）。如果主实例为后付费，只读实例必须也为后付费。
+        :param InstanceChargeType: 实例计费类型。目前支持：PREPAID（预付费，即包年包月），POSTPAID_BY_HOUR（后付费，即按量计费）。默认值：PREPAID。如果主实例为后付费，只读实例必须也为后付费。
         :type InstanceChargeType: str
         :param AutoVoucher: 是否自动使用代金券。1（是），0（否），默认不使用。
         :type AutoVoucher: int
         :param VoucherIds: 代金券ID列表，目前仅支持指定一张代金券。
         :type VoucherIds: list of str
         :param AutoRenewFlag: 续费标记：0-正常续费（默认）；1-自动续费；
         :type AutoRenewFlag: int
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.920/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.921/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,17 @@
 
 # 支付订单失败。
 FAILEDOPERATION_PAYORDERFAILED = 'FailedOperation.PayOrderFailed'
 
 # 按量计费实例账户解冻结失败，请稍后重试。如果持续不成功，请联系客服进行处理。
 FAILEDOPERATION_POSTPAIDUNBLOCKERROR = 'FailedOperation.PostPaidUnblockError'
 
+# 操作预检查失败。
+FAILEDOPERATION_PRECHECKERROR = 'FailedOperation.PreCheckError'
+
 # 获取预签名授权URL错误。
 FAILEDOPERATION_PRESIGNEDURLGETERROR = 'FailedOperation.PresignedURLGetError'
 
 # 查询订单信息失败。
 FAILEDOPERATION_QUERYDEALFAILED = 'FailedOperation.QueryDealFailed'
 
 # 批量获取实例信息失败，请稍后重试。如果持续不成功，请联系客服进行处理。
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.920/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.921/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.920/README.rst` & `tencentcloud-sdk-python-postgres-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.921/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.920/setup.py` & `tencentcloud-sdk-python-postgres-3.0.921/setup.py`

 * *Files identical despite different names*

