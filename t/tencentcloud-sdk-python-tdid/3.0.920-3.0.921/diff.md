# Comparing `tmp/tencentcloud-sdk-python-tdid-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-tdid-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.920.tar", last modified: Thu Jun 22 00:36:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.921.tar", last modified: Mon Jun 26 00:34:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdid-3.0.920.tar` & `tencentcloud-sdk-python-tdid-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud_sdk_python_tdid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/tdid/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/tdid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/tdid/v20210519/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/tdid/v20210519/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111492 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/tdid/v20210519/models.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/tdid/v20210519/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    44514 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/tdid/v20210519/tdid_client.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-22 00:36:27.000000 tencentcloud-sdk-python-tdid-3.0.920/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45275 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/models.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    18789 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/tdid_client.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/setup.py
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.920/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdid-3.0.920/tencentcloud/tdid/v20210519/errorcodes.py` & `tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/errorcodes.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,48 +16,45 @@
 
 # CAM签名/鉴权错误。
 AUTHFAILURE = 'AuthFailure'
 
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
-# 无访问权限。
+# 用户接口鉴权失败
 FAILEDOPERATION_INVALIDAUTH = 'FailedOperation.InvalidAuth'
 
 # 操作失败。
 FAILEDOPERATION_OPERATIONEXCEPTION = 'FailedOperation.OperationException'
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 服务器异常。
 INTERNALERROR_SERVEREXCEPTION = 'InternalError.ServerException'
 
-# 服务内部错误。
+# 服务错误，请稍后重试，或联系客服
 INTERNALERROR_SERVICEERROR = 'InternalError.ServiceError'
 
 # 服务异常。
 INTERNALERROR_SERVICEPANIC = 'InternalError.ServicePanic'
 
-# 未知错误。
+# 服务错误，请稍后重试，或联系客服
 INTERNALERROR_UNKNOWNERROR = 'InternalError.UnknownError'
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
-# 参数错误。
+# 请求参数格式错误，请按照格式要求重新填写
 INVALIDPARAMETERVALUE_ILLEGALVALUE = 'InvalidParameterValue.IllegalValue'
 
 # 缺少参数错误。
 MISSINGPARAMETER = 'MissingParameter'
 
 # 资源不存在。
 RESOURCENOTFOUND = 'ResourceNotFound'
 
-# 资源不可用。
-RESOURCEUNAVAILABLE = 'ResourceUnavailable'
-
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.920/README.rst` & `tencentcloud-sdk-python-tdid-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdid-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.921/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.920/setup.py` & `tencentcloud-sdk-python-tdid-3.0.921/setup.py`

 * *Files identical despite different names*

