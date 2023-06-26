# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.920.tar", last modified: Thu Jun 22 00:37:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.921.tar", last modified: Mon Jun 26 00:35:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.920.tar` & `tencentcloud-sdk-python-tke-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   190354 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)   682751 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)    19455 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:37:50.000000 tencentcloud-sdk-python-tke-3.0.920/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   190375 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)   682738 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)    19455 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:35:29.000000 tencentcloud-sdk-python-tke-3.0.921/tencentcloud_sdk_python_tke.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tke-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/v20180525/tke_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateClusterEndpointVip(self, request):
-        """创建托管集群外网访问端口（老的方式，仅支持托管集群外网端口）
+        """创建托管集群外网访问端口（不再维护，准备下线）请使用新接口：CreateClusterEndpoint
 
         :param request: Request instance for CreateClusterEndpointVip.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterEndpointVipRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.CreateClusterEndpointVipResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2155,20 +2155,20 @@
         :type SubnetId: str
         :param IsExtranet: 是否为外网访问（TRUE 外网访问 FALSE 内网访问，默认值： FALSE）
         :type IsExtranet: bool
         :param Domain: 设置域名
         :type Domain: str
         :param SecurityGroup: 使用的安全组，只有外网访问需要传递（开启外网访问时必传）
         :type SecurityGroup: str
-        :param ExtensiveParameters: 创建lb参数，只有外网访问需要设置，是一个json格式化后的字符串：{"InternetAccessible":{"InternetChargeType":"TRAFFIC_POSTPAID_BY_HOUR","InternetMaxBandwidthOut":"200"},"VipIsp":"","BandwidthPackageId":""}。
+        :param ExtensiveParameters: 创建lb参数，只有外网访问需要设置，是一个json格式化后的字符串：{"InternetAccessible":{"InternetChargeType":"TRAFFIC_POSTPAID_BY_HOUR","InternetMaxBandwidthOut":200},"VipIsp":"","BandwidthPackageId":""}。
 各个参数意义：
 InternetAccessible.InternetChargeType含义：TRAFFIC_POSTPAID_BY_HOUR按流量按小时后计费;BANDWIDTH_POSTPAID_BY_HOUR 按带宽按小时后计费;InternetAccessible.BANDWIDTH_PACKAGE 按带宽包计费。
 InternetMaxBandwidthOut含义：最大出带宽，单位Mbps，范围支持0到2048，默认值10。
-VipIsp含义：CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 DescribeSingleIsp 接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
-BandwidthPackageId含义：带宽包ID，指定此参数时，网络计费方式（InternetAccessible.InternetChargeType）只支持按带宽包计费（BANDWIDTH_PACKAGE。
+VipIsp含义：CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 DescribeSingleIsp 接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费BANDWIDTH_PACKAGE。
+BandwidthPackageId含义：带宽包ID，指定此参数时，网络计费方式InternetAccessible.InternetChargeType只支持按带宽包计费BANDWIDTH_PACKAGE。
         :type ExtensiveParameters: str
         """
         self.ClusterId = None
         self.SubnetId = None
         self.IsExtranet = None
         self.Domain = None
         self.SecurityGroup = None
```

### Comparing `tencentcloud-sdk-python-tke-3.0.920/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.921/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.920/README.rst` & `tencentcloud-sdk-python-tke-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.921/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.920/setup.py` & `tencentcloud-sdk-python-tke-3.0.921/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.920/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.921/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

