# Comparing `tmp/nonebot_plugin_songpicker2-0.2.3.tar.gz` & `tmp/nonebot_plugin_songpicker2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_songpicker2-0.2.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_songpicker2-0.2.4.tar", max compression
```

## Comparing `nonebot_plugin_songpicker2-0.2.3.tar` & `nonebot_plugin_songpicker2-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    35148 2022-12-23 06:42:43.778930 nonebot_plugin_songpicker2-0.2.3/LICENSE
--rw-r--r--   0        0        0     1913 2022-12-23 12:58:52.514510 nonebot_plugin_songpicker2-0.2.3/nonebot_plugin_songpicker2/__init__.py
--rwxr-xr-x   0        0        0     5524 2022-12-23 06:42:43.778930 nonebot_plugin_songpicker2-0.2.3/nonebot_plugin_songpicker2/data_source.py
--rw-r--r--   0        0        0      573 2022-12-23 12:59:20.718428 nonebot_plugin_songpicker2-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      875 1970-01-01 00:00:00.000000 nonebot_plugin_songpicker2-0.2.3/setup.py
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 nonebot_plugin_songpicker2-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-26 15:32:50.796663 nonebot_plugin_songpicker2-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2151 2023-06-26 15:36:22.932663 nonebot_plugin_songpicker2-0.2.4/nonebot_plugin_songpicker2/__init__.py
+-rwxr-xr-x   0        0        0     5524 2023-06-26 15:32:50.796663 nonebot_plugin_songpicker2-0.2.4/nonebot_plugin_songpicker2/data_source.py
+-rw-r--r--   0        0        0      559 2023-06-26 15:42:36.352663 nonebot_plugin_songpicker2-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 nonebot_plugin_songpicker2-0.2.4/PKG-INFO
```

### Comparing `nonebot_plugin_songpicker2-0.2.3/LICENSE` & `nonebot_plugin_songpicker2-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_songpicker2-0.2.3/nonebot_plugin_songpicker2/__init__.py` & `nonebot_plugin_songpicker2-0.2.4/nonebot_plugin_songpicker2/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot.typing import T_State
 from nonebot.params import CommandArg
+from nonebot.plugin import PluginMetadata
 from nonebot import on_command
 
 from .data_source import DataGet, DataProcess
 
+__plugin_meta__ = PluginMetadata(
+    name="songpicker2",
+    description="点播歌曲，支持候选菜单、热评显示，数据源为网易云",
+    usage="点歌吧大概",
+    extra={},
+)
+
 songpicker = on_command("点歌")
 
 dataGet = DataGet()
 
 
 @songpicker.handle()
 async def _(state: T_State, args: Message = CommandArg()):
```

### Comparing `nonebot_plugin_songpicker2-0.2.3/nonebot_plugin_songpicker2/data_source.py` & `nonebot_plugin_songpicker2-0.2.4/nonebot_plugin_songpicker2/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_songpicker2-0.2.3/PKG-INFO` & `nonebot_plugin_songpicker2-0.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-songpicker2
-Version: 0.2.3
+Version: 0.2.4
 Summary: 点播歌曲，支持候选菜单、热评显示，数据源为网易云
 Home-page: https://github.com/maxesisn/nonebot_plugin_songpicker2
 Author: Maximilian Wu
 Author-email: me@maxng.cc
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: build (>=0.1.0,<0.2.0)
 Requires-Dist: httpx (>=0.21.3,<0.22.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: twine (>=3.3.0,<4.0.0)
 Project-URL: Repository, https://github.com/maxesisn/nonebot_plugin_songpicker2
```

