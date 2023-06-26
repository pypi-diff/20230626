# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.920.tar", last modified: Thu Jun 22 00:23:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.921.tar", last modified: Mon Jun 26 00:24:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.920.tar` & `tencentcloud-sdk-python-ess-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   258617 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)    59451 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24640 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-22 00:23:49.000000 tencentcloud-sdk-python-ess-3.0.920/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   258602 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)    59451 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24756 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/setup.py
```

### Comparing `tencentcloud-sdk-python-ess-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -728,15 +728,15 @@
 5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙中的空格个数
 如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
 参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}"
 
 ComponentType为SIGN_SEAL类型时，支持以下参数：
 1.PageRanges：PageRange的数组，通过PageRanges属性设置该印章在PDF所有页面上盖章（适用于标书在所有页面盖章的情况）
-参数样例： "ComponentExtra":"{\"PageRanges\":[\"PageRange\":{\"BeginPage\":1,\"EndPage\":-1}]}"
+参数样例："ComponentExtra":"{\"PageRanges\":[{\"BeginPage\":1,\"EndPage\":-1}]}"
         :type ComponentExtra: str
         :param IsFormType: 是否是表单域类型，默认不false-不是
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsFormType: bool
         :param ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
```

### Comparing `tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.920/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 # 当前无可用的许可
 FAILEDOPERATION_LICENSENOQUOTA = 'FailedOperation.LicenseNoQuota'
 
 # 签署审核未通过，请先完成审核。
 FAILEDOPERATION_NOSIGNREVIEWPASS = 'FailedOperation.NoSignReviewPass'
 
+# 此合同流程不支持审批
+FAILEDOPERATION_NOTAVAILABLESIGNREVIEW = 'FailedOperation.NotAvailableSignReview'
+
 # 未找到集团子企业相关用户信息，请检查用户相关参数
 FAILEDOPERATION_NOTFOUNDSHADOWUSER = 'FailedOperation.NotFoundShadowUser'
 
 # 企业经营状态与工商局信息不符。
 FAILEDOPERATION_ORGANIZATIONEXPERIENCECHANGE = 'FailedOperation.OrganizationExperienceChange'
 
 # 企业名称与工商局信息不符。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.920/README.rst` & `tencentcloud-sdk-python-ess-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.921/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.920/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.920/setup.py` & `tencentcloud-sdk-python-ess-3.0.921/setup.py`

 * *Files identical despite different names*

