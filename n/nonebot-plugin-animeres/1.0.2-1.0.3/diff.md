# Comparing `tmp/nonebot_plugin_animeres-1.0.2.tar.gz` & `tmp/nonebot_plugin_animeres-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_animeres-1.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_animeres-1.0.3.tar", max compression
```

## Comparing `nonebot_plugin_animeres-1.0.2.tar` & `nonebot_plugin_animeres-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    18431 2023-05-27 11:30:14.108178 nonebot_plugin_animeres-1.0.2/LICENSE
--rw-r--r--   0        0        0     3155 2023-06-09 01:27:44.790697 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/__init__.py
--rw-r--r--   0        0        0      449 2023-06-09 01:27:42.657061 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/config.py
--rw-r--r--   0        0        0     2763 2023-06-09 01:27:44.930697 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/internal.py
--rw-r--r--   0        0        0     2284 2023-06-09 01:27:42.677060 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/__init__.py
--rw-r--r--   0        0        0     1186 2023-06-09 01:27:44.792697 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/anoneko.py
--rw-r--r--   0        0        0     1239 2023-06-09 01:27:44.787697 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/dongmanhuayuan.py
--rw-r--r--   0        0        0     1559 2023-06-09 01:27:42.699063 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/myheartsite.py
--rw-r--r--   0        0        0     1040 2023-06-09 01:27:42.704060 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/schemas.py
--rw-r--r--   0        0        0     1562 2023-06-09 01:27:42.712059 nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/utils.py
--rw-r--r--   0        0        0     1092 2023-06-09 01:00:48.674867 nonebot_plugin_animeres-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2009 2023-06-08 08:50:27.156567 nonebot_plugin_animeres-1.0.2/README.md
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 nonebot_plugin_animeres-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-05-27 11:30:14.108178 nonebot_plugin_animeres-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3343 2023-06-25 15:25:19.350171 nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/__init__.py
+-rw-r--r--   0        0        0      449 2023-06-09 01:27:42.657061 nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/config.py
+-rw-r--r--   0        0        0     2763 2023-06-09 01:27:44.930697 nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/internal.py
+-rw-r--r--   0        0        0     2284 2023-06-09 01:27:42.677060 nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/resources/__init__.py
+-rw-r--r--   0        0        0     1186 2023-06-09 01:27:44.792697 nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/resources/anoneko.py
+-rw-r--r--   0        0        0     1239 2023-06-09 01:27:44.787697 nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/resources/dongmanhuayuan.py
+-rw-r--r--   0        0        0     1559 2023-06-09 01:27:42.699063 nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/resources/myheartsite.py
+-rw-r--r--   0        0        0     1040 2023-06-09 01:27:42.704060 nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/schemas.py
+-rw-r--r--   0        0        0     1562 2023-06-09 01:27:42.712059 nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/utils.py
+-rw-r--r--   0        0        0     1056 2023-06-26 00:22:41.639111 nonebot_plugin_animeres-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2009 2023-06-08 08:50:27.156567 nonebot_plugin_animeres-1.0.3/README.md
+-rw-r--r--   0        0        0     2773 1970-01-01 00:00:00.000000 nonebot_plugin_animeres-1.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_animeres-1.0.2/LICENSE` & `nonebot_plugin_animeres-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/__init__.py` & `nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,10 +74,13 @@
     "资源 天气之子 mkv raws\n"
     "将这些关键字以空格的方式分开搜索，可以提高搜索结果的精准度。",
 }
 
 __plugin_meta__ = PluginMetadata(
     name="动漫资源插件",
     description="根据关键字搜索动漫资源",
-    usage="资源 你的名字",
+    usage="使用资源命令，然后追加资源的名称，例如：\n资源 你的名字",
+    type="application",
+    homepage="https://github.com/MelodyKnit/nonebot_plugin_animeres",
     config=Config,
+    supported_adapters=None,
 )
```

### Comparing `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/internal.py` & `nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/internal.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/__init__.py` & `nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/anoneko.py` & `nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/resources/anoneko.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/dongmanhuayuan.py` & `nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/resources/dongmanhuayuan.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/resources/myheartsite.py` & `nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/resources/myheartsite.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/schemas.py` & `nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/schemas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.2/nonebot_plugin_animeres/utils.py` & `nonebot_plugin_animeres-1.0.3/nonebot_plugin_animeres/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.2/pyproject.toml` & `nonebot_plugin_animeres-1.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "nonebot-plugin-animeres"
-version = "1.0.2"
+version = "1.0.3"
 description = "动漫资源获取插件"
 authors = ["MelodyKnit <2711402357@qq.com>"]
 readme = "README.md"
 license = "GPL-2.0"
 packages = [{include = "nonebot_plugin_animeres"}]
 keywords = ["nonebot", "nonebot2", "animeres", "anime"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 lxml = "^4.9.2"
 fake-useragent = "^1.1.3"
 httpx = ">=0.20.0,<1.0.0"
-nonebot2 = { version = "^2.0.0rc1", extras = ["fastapi"] }
+nonebot2 = "^2.0.0rc1"
 nonebot-adapter-onebot = { version = "^2.2.3", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pycln = "^2.1.2"
 isort = "^5.10.1"
 black = "^23.1.0"
 flake8 = "^4.0.1"
```

### Comparing `nonebot_plugin_animeres-1.0.2/README.md` & `nonebot_plugin_animeres-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animeres-1.0.2/PKG-INFO` & `nonebot_plugin_animeres-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-animeres
-Version: 1.0.2
+Version: 1.0.3
 Summary: 动漫资源获取插件
 License: GPL-2.0
 Keywords: nonebot,nonebot2,animeres,anime
 Author: MelodyKnit
 Author-email: 2711402357@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0rc1,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 动漫资源获取插件
 
 这个插件主要是网站爬取过来的数据，在使用命令进行搜索时候采用关键字的方式，比如`天气之子`这时搜索的是`天气之子`相关资源，如果获取的资源并不理想或者你只需要生肉（无字幕）资源时，你就需要用`天气之子 raw`或`天气之子 mkv`这种多个关键字空格方式进行获取，这种方式准确度会比直接用`天气之子`精准且效果好，建议采用多关键字的方式进行搜索。
 
 ## 使用例子
```

