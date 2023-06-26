# Comparing `tmp/tencentcloud-sdk-python-icr-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-icr-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-icr-3.0.920.tar", last modified: Thu Jun 22 00:25:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-icr-3.0.921.tar", last modified: Mon Jun 26 00:25:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-icr-3.0.920.tar` & `tencentcloud-sdk-python-icr-3.0.921.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud_sdk_python_icr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud_sdk_python_icr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud_sdk_python_icr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud_sdk_python_icr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud_sdk_python_icr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:25:16.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:25:16.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/v20211014/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:25:16.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/v20211014/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-06-22 00:25:16.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/v20211014/icr_client.py
--rw-r--r--   0 root         (0) root         (0)    17883 2023-06-22 00:25:16.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/v20211014/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-06-22 00:25:16.000000 tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/v20211014/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-22 00:25:16.000000 tencentcloud-sdk-python-icr-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:25:17.000000 tencentcloud-sdk-python-icr-3.0.920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-22 00:25:16.000000 tencentcloud-sdk-python-icr-3.0.920/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud_sdk_python_icr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud_sdk_python_icr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud_sdk_python_icr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud_sdk_python_icr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud_sdk_python_icr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/v20211014/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/v20211014/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/v20211014/icr_client.py
+-rw-r--r--   0 root         (0) root         (0)    17883 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/v20211014/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/v20211014/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 00:25:53.000000 tencentcloud-sdk-python-icr-3.0.921/setup.py
```

### Comparing `tencentcloud-sdk-python-icr-3.0.920/tencentcloud_sdk_python_icr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-icr-3.0.921/tencentcloud_sdk_python_icr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-icr
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Icr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-icr-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-icr-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/v20211014/icr_client.py` & `tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/v20211014/icr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/v20211014/models.py` & `tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/v20211014/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.920/tencentcloud/icr/v20211014/errorcodes.py` & `tencentcloud-sdk-python-icr-3.0.921/tencentcloud/icr/v20211014/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.920/README.rst` & `tencentcloud-sdk-python-icr-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-icr-3.0.921/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-icr
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Icr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-icr-3.0.920/setup.py` & `tencentcloud-sdk-python-icr-3.0.921/setup.py`

 * *Files identical despite different names*

