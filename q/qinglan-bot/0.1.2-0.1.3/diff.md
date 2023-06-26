# Comparing `tmp/qinglan-bot-0.1.2.tar.gz` & `tmp/qinglan-bot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qinglan-bot-0.1.2.tar", last modified: Mon Jun 26 04:03:05 2023, max compression
+gzip compressed data, was "qinglan-bot-0.1.3.tar", last modified: Mon Jun 26 06:51:07 2023, max compression
```

## Comparing `qinglan-bot-0.1.2.tar` & `qinglan-bot-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/qinglan_bot/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/ws_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/qinglan_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:51:07.006419 qinglan-bot-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 06:51:07.006419 qinglan-bot-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:51:07.002419 qinglan-bot-0.1.3/qinglan_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:51:07.006419 qinglan-bot-0.1.3/qinglan_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:51:07.006419 qinglan-bot-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/setup.py
```

### Comparing `qinglan-bot-0.1.2/LICENSE` & `qinglan-bot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.2/PKG-INFO` & `qinglan-bot-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.1.2
+Version: 0.1.3
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qinglan-bot-0.1.2/README.md` & `qinglan-bot-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.2/qinglan_bot/__init__.py` & `qinglan-bot-0.1.3/qinglan_bot/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from nonebot import get_driver, require
 from nonebot.plugin import PluginMetadata
 from nonebot.plugin.manager import PluginLoader
-from .config import Config
 
-require("nonebot_plugin_guild_patch")
-
-__plugin_meta__ = PluginMetadata(
-    name="青岚Bot",
-    description="基于NoneBot的与Minecraft Server互通消息的机器人",
-    homepage="https://github.com/17TheWord/qinglan_bot",
-    usage="配置完成后在群聊发送消息即可同步至 Minecraft 服务器",
-    config=Config,
-    type="application",
-    supported_adapters={
-        "nonebot.adapters.onebot.v11"
-    }
-)
 if isinstance(globals()["__loader__"], PluginLoader):
+    require("nonebot_plugin_guild_patch")
+    from .config import Config
+
+    __plugin_meta__ = PluginMetadata(
+        name="青岚Bot",
+        description="基于NoneBot的与Minecraft Server互通消息的机器人",
+        homepage="https://github.com/17TheWord/qinglan_bot",
+        usage="配置完成后在群聊发送消息即可同步至 Minecraft 服务器",
+        config=Config,
+        type="application",
+        supported_adapters={
+            "nonebot.adapters.onebot.v11"
+        }
+    )
     driver = get_driver()
 
     plugin_config: Config = Config.parse_obj(get_driver().config)
 
     from .ws_server import start_ws_server, stop_ws_server
     from . import plugins
 
+
     # Bot 连接时
     @driver.on_bot_connect
     async def on_start():
         # 启动 WebSocket 服务器
         await start_ws_server()
 
+
     # Bot 断开时
     @driver.on_bot_disconnect
     async def on_close():
         # 关闭 WebSocket 服务器
         await stop_ws_server()
```

### Comparing `qinglan-bot-0.1.2/qinglan_bot/utils.py` & `qinglan-bot-0.1.3/qinglan_bot/utils.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.2/qinglan_bot/ws_server.py` & `qinglan-bot-0.1.3/qinglan_bot/ws_server.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.2/qinglan_bot.egg-info/PKG-INFO` & `qinglan-bot-0.1.3/qinglan_bot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.1.2
+Version: 0.1.3
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qinglan-bot-0.1.2/setup.py` & `qinglan-bot-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="qinglan-bot",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.1.2",  # 程序版本
+    version="0.1.3",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通机器人",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/qinglan_bot",  # 项目地址
     packages=["qinglan_bot"],
@@ -19,15 +19,14 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'mcqq-tool==0.0.4',
         'nonebot2>=2.0.0',
         'nonebot-adapter-onebot>=2.1.5',
         'nonebot-plugin-guild-patch>=0.2.0',
-        'nonebot-plugin-gocqhttp>=0.6.3',
         'websockets>=10.3',
         'tortoise-orm>=0.19.3',
         'aio-mc-rcon>=3.2.0',
         'click>=8.0.4',
     ],
     entry_points={'console_scripts': [
         'ql=qinglan_bot.cli_start:main',
```

