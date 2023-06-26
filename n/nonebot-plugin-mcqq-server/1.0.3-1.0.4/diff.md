# Comparing `tmp/nonebot_plugin_mcqq_server-1.0.3.tar.gz` & `tmp/nonebot_plugin_mcqq_server-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mcqq_server-1.0.3.tar", last modified: Sat Dec 24 14:52:09 2022, max compression
+gzip compressed data, was "nonebot_plugin_mcqq_server-1.0.4.tar", last modified: Mon Jun 26 18:53:42 2023, max compression
```

## Comparing `nonebot_plugin_mcqq_server-1.0.3.tar` & `nonebot_plugin_mcqq_server-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-24 14:52:09.348324 nonebot_plugin_mcqq_server-1.0.3/
--rw-rw-rw-   0        0        0     1086 2022-09-08 17:56:17.000000 nonebot_plugin_mcqq_server-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      275 2022-12-24 14:52:09.347823 nonebot_plugin_mcqq_server-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-24 14:52:09.338315 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server/
--rw-rw-rw-   0        0        0     2956 2022-09-12 02:55:46.000000 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server/__init__.py
--rw-rw-rw-   0        0        0      467 2022-09-09 19:46:05.000000 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server/config.py
--rw-rw-rw-   0        0        0     4563 2022-09-12 02:53:50.000000 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-24 14:52:09.346823 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server.egg-info/
--rw-rw-rw-   0        0        0      275 2022-12-24 14:52:09.000000 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2022-12-24 14:52:09.000000 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-24 14:52:09.000000 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2022-12-24 14:52:09.000000 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2022-12-24 14:52:09.000000 nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-24 14:52:09.348324 nonebot_plugin_mcqq_server-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      556 2022-12-24 14:52:06.000000 nonebot_plugin_mcqq_server-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:53:42.946040 nonebot_plugin_mcqq_server-1.0.4/
+-rw-rw-rw-   0        0        0     1086 2022-09-08 17:56:17.000000 nonebot_plugin_mcqq_server-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      275 2023-06-26 18:53:42.945539 nonebot_plugin_mcqq_server-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 18:53:42.934029 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/
+-rw-rw-rw-   0        0        0     3759 2023-06-26 18:51:48.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/__init__.py
+-rw-rw-rw-   0        0        0      420 2023-02-25 09:44:03.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/config.py
+-rw-rw-rw-   0        0        0     4331 2023-06-26 18:45:55.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:53:42.943537 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/
+-rw-rw-rw-   0        0        0      275 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-26 18:53:42.000000 nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:53:42.946040 nonebot_plugin_mcqq_server-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-06-26 18:53:38.000000 nonebot_plugin_mcqq_server-1.0.4/setup.py
```

### Comparing `nonebot_plugin_mcqq_server-1.0.3/LICENSE` & `nonebot_plugin_mcqq_server-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcqq_server-1.0.3/nonebot_plugin_mcqq_server/utils.py` & `nonebot_plugin_mcqq_server-1.0.4/nonebot_plugin_mcqq_server/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent, Event, Message
 from nonebot.log import logger
 from mcrcon import MCRcon
 
 import nonebot
+import re
 import time
 import asyncio
 
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
 from .config import Config
 
 global_config = nonebot.get_driver().config
 config = Config.parse_obj(global_config.dict())
 
 group_list = config.group_list
 guild_list = config.guild_list
 mc_log_path = config.mc_log_path
-mc_ip = config.mc_ip
 mcrcon_password = config.mcrcon_password
 mcrcon_port = config.mcrcon_port
 
-async def mcrcon_connect(mc_ip: str,mcrcon_password: str, mcrcon_port:int):
+async def mcrcon_connect(mc_ip: str,mcrcon_password: str, mcrcon_port:int) -> MCRcon:
     """
     与 mcrcon 建立连接
     :param mc_ip: 服务器 IP
     :param mcrcon_password: MCRcon password
     :param mcrcon_port: MCRcon 端口
     """
     mcr = MCRcon(mc_ip,mcrcon_password,mcrcon_port)
     try:
         mcr.connect()
         logger.success("与 MCRcon 连接成功！")
         return mcr
-    except (OSError, ConnectionRefusedError):
-        logger.info("与 MCRcon 连接失败，正在重新连接...")
-        await asyncio.sleep(0.5)
-        await mcrcon_connect(mc_ip, mcrcon_password, mcrcon_port)
+    except (OSError, ConnectionRefusedError) as e:
+        logger.info(f"与 MCRcon 连接失败，正在重新连接...{e}")
+        await asyncio.sleep(3)
+        return await mcrcon_connect(mc_ip, mcrcon_password, mcrcon_port)
 
 async def mc_translate(bot: Bot, event: Event):
     '''
     把信息翻译成 Minecraft 信息命令
     :param bot: Bot
     :param event: Event
     '''
@@ -51,15 +51,15 @@
         nikname = guild_nickname
         Tip = f"[QQ频道]"
     else:
         return ""
 
     command_msg = 'tellraw @a ["",'
     # 插件名与发言人昵称
-    command_msg += '{"text": "' + Tip + (event.sender.card or event.sender.nickname) + ' 说：","color": "white"},'
+    command_msg += '{"text": "' + Tip + (event.sender.nickname or event.sender.card) + ' 说：","color": "white"},'
     # 文本信息
     text_msg = ''
     for msg in event.message:
         # 文本
         if msg.type == "text":
             command_msg += '{"text": "' + msg.data['text'].replace("\r\n", " ") + ' ","color": "white"},'
         # 图片
@@ -99,22 +99,11 @@
 
 
 def log_to_dict(loginfo:str) -> dict:
     '''
     转换log信息
     :param loginfo:log信息
     '''
-    l = loginfo.find('<')
-    r = loginfo.find('>')
-    if l != -1 and r != -1:
-        return {
-            "type":"message",
-            "nickname":loginfo[l+1:r],
-            "message":loginfo[r+2:]
-            }
+    if res := re.search(": <(.+)>(.+)",loginfo):
+        return {"nickname":res.group(1),"message":res.group(2)}
     else:
-        x = loginfo.find(':')
-        return {
-            "type":"log",
-            "log":loginfo[:x],
-            "info":loginfo[x+2:]
-            }
+        return None
```

### Comparing `nonebot_plugin_mcqq_server-1.0.3/setup.py` & `nonebot_plugin_mcqq_server-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_mcqq_server',
-version='1.0.3',
+version='1.0.4',
 description='mcqq服主版',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_mcqq_server"]),
```

