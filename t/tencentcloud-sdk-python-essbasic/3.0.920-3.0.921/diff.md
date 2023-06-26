# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.920.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.920.tar", last modified: Thu Jun 22 00:23:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.921.tar", last modified: Mon Jun 26 00:24:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.920.tar` & `tencentcloud-sdk-python-essbasic-3.0.921.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   242551 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)    52742 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20210526/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/README.rst
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:23:55.000000 tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240452 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)    52742 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20210526/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:24:16.000000 tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20210526/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2452,45 +2452,14 @@
         :type ComponentPage: int
         :param ComponentPosX: 参数控件X位置，单位px
         :type ComponentPosX: float
         :param ComponentPosY: 参数控件Y位置，单位px
         :type ComponentPosY: float
         :param ComponentExtra: 扩展参数：
 为JSON格式。
-
-ComponentType为FILL_IMAGE时，支持以下参数：
-NotMakeImageCenter：bool。是否设置图片居中。false：居中（默认）。 true: 不居中
-FillMethod: int. 填充方式。0-铺满（默认）；1-等比例缩放
-
-ComponentType为SIGN_SIGNATURE类型可以控制签署方式
-{“ComponentTypeLimit”: [“xxx”]}
-xxx可以为：
-HANDWRITE – 手写签名
-OCR_ESIGN -- AI智能识别手写签名
-ESIGN -- 个人印章类型
-SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
-如：{“ComponentTypeLimit”: [“SYSTEM_ESIGN”]}
-
-ComponentType为SIGN_DATE时，支持以下参数：
-1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
-2 FontSize： 数字类型，范围6-72，默认值为12
-3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
-4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
-5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙中的空格个数
-如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
-特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
-参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}"
-
-ComponentType为SIGN_SEAL类型时，支持以下参数：
-1.PageRanges：PageRange的数组，通过PageRanges属性设置该印章在PDF所有页面上盖章（适用于标书在所有页面盖章的情况）
-参数样例： "ComponentExtra":"{\"PageRanges\":[\"PageRange\":{\"BeginPage\":1,\"EndPage\":-1}]}"
-
-
-参数控件样式，json格式表述
-
 不同类型的控件会有部分非通用参数
 
 TEXT/MULTI_LINE_TEXT控件可以指定
 1 Font：目前只支持黑体、宋体
 2 FontSize： 范围12-72
 3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
 例如：{"FontSize":12}
@@ -2499,33 +2468,32 @@
 NotMakeImageCenter：bool。是否设置图片居中。false：居中（默认）。 true: 不居中
 FillMethod: int. 填充方式。0-铺满（默认）；1-等比例缩放
 
 ComponentType为SIGN_SIGNATURE类型可以控制签署方式
 {“ComponentTypeLimit”: [“xxx”]}
 xxx可以为：
 HANDWRITE – 手写签名
-BORDERLESS_ESIGN – 自动生成无边框腾讯体
 OCR_ESIGN -- AI智能识别手写签名
 ESIGN -- 个人印章类型
 SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
-如：{“ComponentTypeLimit”: [“BORDERLESS_ESIGN”]}
+如：{“ComponentTypeLimit”: [“SYSTEM_ESIGN”]}
 
 ComponentType为SIGN_DATE时，支持以下参数：
 1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
 2 FontSize： 数字类型，范围6-72，默认值为12
 3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
-5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙钟的空格个数
+5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙中的空格个数
 如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
-参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}"
+参数样例： "ComponentExtra": "{"Format":“yyyy m d”,"FontSize":12,"Gaps":"2,2", "FontAlign":"Right"}"
 
 ComponentType为SIGN_SEAL类型时，支持以下参数：
 1.PageRanges：PageRange的数组，通过PageRanges属性设置该印章在PDF所有页面上盖章（适用于标书在所有页面盖章的情况）
-参数样例： "ComponentExtra":"{\"PageRanges\":[\"PageRange\":{\"BeginPage\":1,\"EndPage\":-1}]}"
+参数样例： "ComponentExtra":"{["PageRange":{"BeginPage":1,"EndPage":-1}]}"
         :type ComponentExtra: str
         :param ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
 CHECK_BOX - true/false
 FILL_IMAGE、ATTACHMENT - 附件的FileId，需要通过UploadFiles接口上传获取
 SELECTOR - 选项值
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.921/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.921/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.921/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.920/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.921/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.920
+Version: 3.0.921
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

