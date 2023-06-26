# Comparing `tmp/potato_tool-0.0.3.tar.gz` & `tmp/potato_tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potato_tool-0.0.3.tar", last modified: Mon Jun 26 05:21:40 2023, max compression
+gzip compressed data, was "potato_tool-0.0.4.tar", last modified: Mon Jun 26 05:53:37 2023, max compression
```

## Comparing `potato_tool-0.0.3.tar` & `potato_tool-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 05:21:40.756810 potato_tool-0.0.3/
--rw-r--r--   0 a          (501) staff       (20)     3395 2023-06-26 05:21:40.756560 potato_tool-0.0.3/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)     3113 2023-06-26 05:07:26.000000 potato_tool-0.0.3/README.md
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 05:21:40.753880 potato_tool-0.0.3/potato_tool/
--rw-r--r--   0 a          (501) staff       (20)       30 2023-06-26 05:17:26.000000 potato_tool-0.0.3/potato_tool/__init__.py
--rwxr-xr-x   0 a          (501) staff       (20)     8636 2023-06-26 05:10:25.000000 potato_tool-0.0.3/potato_tool/font.py
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 05:21:40.756143 potato_tool-0.0.3/potato_tool.egg-info/
--rw-r--r--   0 a          (501) staff       (20)     3395 2023-06-26 05:21:40.000000 potato_tool-0.0.3/potato_tool.egg-info/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)      274 2023-06-26 05:21:40.000000 potato_tool-0.0.3/potato_tool.egg-info/SOURCES.txt
--rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 05:21:40.000000 potato_tool-0.0.3/potato_tool.egg-info/dependency_links.txt
--rw-r--r--   0 a          (501) staff       (20)      950 2023-06-26 05:21:40.000000 potato_tool-0.0.3/potato_tool.egg-info/entry_points.txt
--rw-r--r--   0 a          (501) staff       (20)       25 2023-06-26 05:21:40.000000 potato_tool-0.0.3/potato_tool.egg-info/requires.txt
--rw-r--r--   0 a          (501) staff       (20)       12 2023-06-26 05:21:40.000000 potato_tool-0.0.3/potato_tool.egg-info/top_level.txt
--rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 05:21:40.756917 potato_tool-0.0.3/setup.cfg
--rw-r--r--   0 a          (501) staff       (20)     2024 2023-06-26 05:21:22.000000 potato_tool-0.0.3/setup.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 05:53:37.004525 potato_tool-0.0.4/
+-rw-r--r--   0 a          (501) staff       (20)     3597 2023-06-26 05:53:37.004280 potato_tool-0.0.4/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)     3315 2023-06-26 05:51:28.000000 potato_tool-0.0.4/README.md
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 05:53:37.002133 potato_tool-0.0.4/potato_tool/
+-rw-r--r--   0 a          (501) staff       (20)       30 2023-06-26 05:17:26.000000 potato_tool-0.0.4/potato_tool/__init__.py
+-rwxr-xr-x   0 a          (501) staff       (20)    11192 2023-06-26 05:47:46.000000 potato_tool-0.0.4/potato_tool/font.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 05:53:37.003875 potato_tool-0.0.4/potato_tool.egg-info/
+-rw-r--r--   0 a          (501) staff       (20)     3597 2023-06-26 05:53:36.000000 potato_tool-0.0.4/potato_tool.egg-info/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)      274 2023-06-26 05:53:36.000000 potato_tool-0.0.4/potato_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 05:53:36.000000 potato_tool-0.0.4/potato_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 a          (501) staff       (20)     1026 2023-06-26 05:53:36.000000 potato_tool-0.0.4/potato_tool.egg-info/entry_points.txt
+-rw-r--r--   0 a          (501) staff       (20)       25 2023-06-26 05:53:36.000000 potato_tool-0.0.4/potato_tool.egg-info/requires.txt
+-rw-r--r--   0 a          (501) staff       (20)       12 2023-06-26 05:53:36.000000 potato_tool-0.0.4/potato_tool.egg-info/top_level.txt
+-rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 05:53:37.004620 potato_tool-0.0.4/setup.cfg
+-rw-r--r--   0 a          (501) staff       (20)     2143 2023-06-26 05:53:10.000000 potato_tool-0.0.4/setup.py
```

### Comparing `potato_tool-0.0.3/PKG-INFO` & `potato_tool-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-Metadata-Version: 2.1
-Name: potato_tool
-Version: 0.0.3
-Summary: 输出染色、前置符、格式化输出及表格输出
-Home-page: https://potato.gold
-Author: Potato
-Author-email: ljy1058318852@163.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # 辅助函数
 - 打印 (return void)
   - `p(Str)`
 
 
+- 清理屏幕输出 (兼容不同OS) (return void)
+  - `clear()`
+
+
 # 字体效果
 - 红色
    - `red(Str)` (return str)
    - `redP(Str)` (return void)
 
 
 - 绿色
@@ -131,7 +124,11 @@
 
 |  ip   | domain | icp | id |
 |  :----:  | :----:  | :----: | :----: |
 | ip  | 域名 | 备案 | 编号 |
 
 </div>
 
+
+# logo输出
+- `logo_1(ScriptName="potato",Author="potato", QQemil="2431111111", Type="Penetration", Version="0.2.4")`
+- `logo_2()`
```

### Comparing `potato_tool-0.0.3/potato_tool.egg-info/PKG-INFO` & `potato_tool-0.0.4/potato_tool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: potato-tool
-Version: 0.0.3
+Version: 0.0.4
 Summary: 输出染色、前置符、格式化输出及表格输出
 Home-page: https://potato.gold
 Author: Potato
 Author-email: ljy1058318852@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 辅助函数
 - 打印 (return void)
   - `p(Str)`
 
 
+- 清理屏幕输出 (兼容不同OS) (return void)
+  - `clear()`
+
+
 # 字体效果
 - 红色
    - `red(Str)` (return str)
    - `redP(Str)` (return void)
 
 
 - 绿色
@@ -131,7 +135,12 @@
 
 |  ip   | domain | icp | id |
 |  :----:  | :----:  | :----: | :----: |
 | ip  | 域名 | 备案 | 编号 |
 
 </div>
 
+
+# logo输出
+- `logo_1(ScriptName="potato",Author="potato", QQemil="2431111111", Type="Penetration", Version="0.2.4")`
+- `logo_2()`
+
```

### Comparing `potato_tool-0.0.3/potato_tool.egg-info/entry_points.txt` & `potato_tool-0.0.4/potato_tool.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 bold = potato_tool:bold
 boldP = potato_tool:boldP
 cyan = potato_tool:cyan
 cyanP = potato_tool:cyanP
 green = potato_tool:green
 greenP = potato_tool:greenP
 listPT = potato_tool:listPT
+logo_1=potato_tool:logo_1logo_2 = potato_tool:logo_2
 magenta = potato_tool:magenta
 magentaP = potato_tool:magentaP
-p=potato_tool:pred = potato_tool:red
+p=potato_tool:pclear=potato_tool:clearred = potato_tool:red
 pF = potato_tool:pF
 pT = potato_tool:pT
 printF = potato_tool:printF
 printT = potato_tool:printT
 redP = potato_tool:redP
 yellow = potato_tool:yellow
 yellowP = potato_tool:yellowP
```

### Comparing `potato_tool-0.0.3/setup.py` & `potato_tool-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='potato_tool',
-    version='0.0.3',
+    version='0.0.4',
     author='Potato',
     author_email='ljy1058318852@163.com',
     url='https://potato.gold',
     description=u'输出染色、前置符、格式化输出及表格输出',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
@@ -20,14 +20,15 @@
         'terminal',
         'console',
         'wcwidth'
     ],
     entry_points={
         'console_scripts': [
             'p=potato_tool:p'
+            'clear=potato_tool:clear'
             'red=potato_tool:red',
             'redP=potato_tool:redP',
             'green=potato_tool:green',
             'greenP=potato_tool:greenP',
             'blue=potato_tool:blue',
             'blueP=potato_tool:blueP',
             'magenta=potato_tool:magenta',
@@ -51,11 +52,13 @@
             'Input=potato_tool:Input',
             'InputP=potato_tool:InputP',
             'Input_lines=potato_tool:Input_lines',
             'printF=potato_tool:printF',
             'pF=potato_tool:pF',
             'printT=potato_tool:printT',
             'pT=potato_tool:pT',
-            'listPT=potato_tool:listPT'
+            'listPT=potato_tool:listPT',
+            'logo_1=potato_tool:logo_1'
+            'logo_2=potato_tool:logo_2'
         ]
     }
 )
```

