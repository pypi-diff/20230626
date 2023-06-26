# Comparing `tmp/LogTranslate-0.1.tar.gz` & `tmp/LogTranslate-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogTranslate-0.1.tar", last modified: Mon Jun 26 16:13:47 2023, max compression
+gzip compressed data, was "LogTranslate-0.2.tar", last modified: Mon Jun 26 17:00:35 2023, max compression
```

## Comparing `LogTranslate-0.1.tar` & `LogTranslate-0.2.tar`

### file list

```diff
@@ -1,12 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:47.393162 LogTranslate-0.1/
--rw-rw-rw-   0        0        0     1079 2023-06-26 15:57:52.000000 LogTranslate-0.1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 16:13:47.390318 LogTranslate-0.1/LogTranslate.egg-info/
--rw-rw-rw-   0        0        0      618 2023-06-26 16:13:47.000000 LogTranslate-0.1/LogTranslate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-06-26 16:13:47.000000 LogTranslate-0.1/LogTranslate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:13:47.000000 LogTranslate-0.1/LogTranslate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:13:47.000000 LogTranslate-0.1/LogTranslate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      618 2023-06-26 16:13:47.393162 LogTranslate-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2250 2023-06-26 15:52:28.000000 LogTranslate-0.1/README.md
--rw-rw-rw-   0        0        0      389 2023-06-26 16:13:36.000000 LogTranslate-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 16:13:47.393162 LogTranslate-0.1/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-06-26 16:13:36.000000 LogTranslate-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:00:35.205118 LogTranslate-0.2/
+-rw-rw-rw-   0        0        0     1079 2023-06-26 15:57:52.000000 LogTranslate-0.2/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 17:00:35.188491 LogTranslate-0.2/LogTranslate.egg-info/
+-rw-rw-rw-   0        0        0      618 2023-06-26 17:00:35.000000 LogTranslate-0.2/LogTranslate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-06-26 17:00:35.000000 LogTranslate-0.2/LogTranslate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 17:00:35.000000 LogTranslate-0.2/LogTranslate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 17:00:35.000000 LogTranslate-0.2/LogTranslate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      618 2023-06-26 17:00:35.205118 LogTranslate-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2331 2023-06-26 16:22:25.000000 LogTranslate-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 17:00:35.205118 LogTranslate-0.2/log_translate/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:36:52.000000 LogTranslate-0.2/log_translate/__init__.py
+-rw-rw-rw-   0        0        0      287 2023-06-26 13:36:45.000000 LogTranslate-0.2/log_translate/config_demo.py
+-rw-rw-rw-   0        0        0     1266 2023-06-26 15:04:12.000000 LogTranslate-0.2/log_translate/data_struct.py
+-rw-rw-rw-   0        0        0       11 2023-06-26 15:04:11.000000 LogTranslate-0.2/log_translate/gloable.py
+-rw-rw-rw-   0        0        0     4348 2023-06-26 13:54:10.000000 LogTranslate-0.2/log_translate/log_translator.py
+-rw-rw-rw-   0        0        0     2990 2023-06-26 15:04:12.000000 LogTranslate-0.2/log_translate/read_log_file.py
+-rw-rw-rw-   0        0        0     5419 2023-06-26 15:04:11.000000 LogTranslate-0.2/log_translate/ui_pyqt6.py
+-rw-rw-rw-   0        0        0     5571 2023-06-26 15:04:11.000000 LogTranslate-0.2/log_translate/ui_pyside2.py
+-rw-rw-rw-   0        0        0      393 2023-06-26 16:22:25.000000 LogTranslate-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 17:00:35.205118 LogTranslate-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      966 2023-06-26 17:00:32.000000 LogTranslate-0.2/setup.py
```

### Comparing `LogTranslate-0.1/LICENSE.txt` & `LogTranslate-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-0.1/LogTranslate.egg-info/PKG-INFO` & `LogTranslate-0.2/LogTranslate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 0.1
+Version: 0.2
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `LogTranslate-0.1/PKG-INFO` & `LogTranslate-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 0.1
+Version: 0.2
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `LogTranslate-0.1/README.md` & `LogTranslate-0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,77 @@
-
 ## 作用
+
 把日志文件拖动到窗口即可解析日志
 
 ## 使用
+
 项目根目录 创建 config.py
 里面定义字段 translator数组
+
 ```commandline
 translators = [SysLogTranslator(tag_translators=[BluetoothTranslator(), CrashPatternTranslator()])]
 ```
+
 SysLogTranslator是将文件中每行字符串解析出 tag,time,pid,msg
 SysLogTranslator的参数 tag_translators 是数组 用来解析 各种tag对应的内容
-解析tag的基类有 
- - TagPatternTranslator 通过正则匹配tag然后解析
+解析tag的基类有
+
+- TagPatternTranslator 通过正则匹配tag然后解析
+  ```python
+  class CrashPatternTranslator(TagPatternTranslator):
+       def __init__(self):
+           super().__init__({
+               r"AndroidRuntime|FATAL.*|System.err.*": activity_task_translator
+           })
+      
+       def activity_task_translator(tag, msg): # 这里两个参数
+           # todo 这里需要过滤包名
+           return Log(translated=" ------ %s > %s----- " % (tag, msg), level=Level.e)
+
+  ```
+
+- TagStrTranslator 通过字符串匹配tag然后解析
    ```python
-   class CrashPatternTranslator(TagPatternTranslator):
-        def __init__(self):
-            super().__init__({
-                r"AndroidRuntime|FATAL.*|System.err.*": activity_task_translator
-            })
-       
-        def activity_task_translator(tag, msg): #这里两个参数
-            # todo 这里需要过滤包名
-            return Log(translated=" ------ %s > %s----- " % (tag, msg), level=Level.e)
-
-   ```
-
- - TagStrTranslator 通过字符串匹配tag然后解析
-    ```python
-   class BluetoothTranslator(TagStrTranslator):
-        def __init__(self):
-            super().__init__({
-                "BluetoothAdapter": bluetooth_adapter,
-            })
-           
-        def bluetooth_adapter(msg):# 这里一个参数
-            # todo 这里需要过滤包名
-            return Log(translated=" ------ %s > %s----- " % (tag, msg), level=Level.e)
-
-   ```
- - SecStrTagTranslator 解析二级tag
-    ```python
-    class SecTagDemoTranslator(SecStrTagTranslator):
-        def __init__(self):
-            super().__init__("DFJ",
-                             lambda string: re.search(r"(?P<tag>.*?) *:(?P<msg>.*)", string),
-                             [
-                                 SysLogTranslator({
-                                     "sec_tag": self.new_tag
-                                 })
-                             ])
-
-        def new_tag(self, tag, msg):#这里两个参数
-            return Log(translated=msg)
-   ```
-       
+  class BluetoothTranslator(TagStrTranslator):
+       def __init__(self):
+           super().__init__({
+               "BluetoothAdapter": bluetooth_adapter,
+           })
+          
+       def bluetooth_adapter(msg):# 这里一个参数
+           # todo 这里需要过滤包名
+           return Log(translated=" ------ %s > %s----- " % (tag, msg), level=Level.e)
+
+  ```
+- SecStrTagTranslator 解析二级tag
+   ```python
+   class SecTagDemoTranslator(SecStrTagTranslator):
+       def __init__(self):
+           super().__init__("DFJ",
+                            lambda string: re.search(r"(?P<tag>.*?) *:(?P<msg>.*)", string),
+                            [
+                                SysLogTranslator({
+                                    "sec_tag": self.new_tag
+                                })
+                            ])
+
+       def new_tag(self, tag, msg):# 这里两个参数
+           return Log(translated=msg)
+  ```
 
 ## 打包成 exe
+
 ```commandline
 
 pyinstaller -n log_translator --hidden-import config -F -w -i tools.ico ui_pyqt6.py
 
 pyinstaller --hidden-import -n log_translator -F -w -i tools.ico ui_pyside2.py
 
+```
+
+### 库地址
+
+https://pypi.org/project/LogTranslate/0.1/
+
+```commandline
+pip install LogTranslate==0.1
 ```
```

