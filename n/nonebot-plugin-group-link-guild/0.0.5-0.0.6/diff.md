# Comparing `tmp/nonebot-plugin-group-link-guild-0.0.5.tar.gz` & `tmp/nonebot-plugin-group-link-guild-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-group-link-guild-0.0.5.tar", last modified: Sun Jun 18 16:54:13 2023, max compression
+gzip compressed data, was "nonebot-plugin-group-link-guild-0.0.6.tar", last modified: Mon Jun 26 03:57:15 2023, max compression
```

## Comparing `nonebot-plugin-group-link-guild-0.0.5.tar` & `nonebot-plugin-group-link-guild-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:54:13.061305 nonebot-plugin-group-link-guild-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 16:54:02.000000 nonebot-plugin-group-link-guild-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-18 16:54:13.061305 nonebot-plugin-group-link-guild-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-18 16:54:02.000000 nonebot-plugin-group-link-guild-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:54:13.061305 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-18 16:54:02.000000 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-18 16:54:02.000000 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-18 16:54:02.000000 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:54:13.061305 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-18 16:54:12.000000 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-18 16:54:13.000000 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:54:12.000000 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-18 16:54:12.000000 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 16:54:12.000000 nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:54:13.061305 nonebot-plugin-group-link-guild-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-18 16:54:02.000000 nonebot-plugin-group-link-guild-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:57:15.378539 nonebot-plugin-group-link-guild-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 03:57:03.000000 nonebot-plugin-group-link-guild-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-26 03:57:15.378539 nonebot-plugin-group-link-guild-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-26 03:57:03.000000 nonebot-plugin-group-link-guild-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:57:15.378539 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 03:57:03.000000 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 03:57:03.000000 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-26 03:57:03.000000 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:57:15.378539 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-26 03:57:15.000000 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-26 03:57:15.000000 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 03:57:15.000000 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 03:57:15.000000 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 03:57:15.000000 nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 03:57:15.378539 nonebot-plugin-group-link-guild-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-26 03:57:03.000000 nonebot-plugin-group-link-guild-0.0.6/setup.py
```

### Comparing `nonebot-plugin-group-link-guild-0.0.5/LICENSE` & `nonebot-plugin-group-link-guild-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-group-link-guild-0.0.5/PKG-INFO` & `nonebot-plugin-group-link-guild-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-group-link-guild
-Version: 0.0.5
+Version: 0.0.6
 Summary: 互通QQ群聊与QQ频道消息的插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-group-link-guild
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nonebot-plugin-group-link-guild-0.0.5/README.md` & `nonebot-plugin-group-link-guild-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild/__init__.py` & `nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Union
 
-from nonebot import on_message, on_command
+from nonebot import on_message, on_command, require
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import GroupMessageEvent, Bot, Message
 from nonebot.params import CommandArg
+require("nonebot_plugin_guild_patch")
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
 from .config import Config
 
 from .utils import (
     msg_rule_cmd,
     msg_rule_no_cmd,
```

### Comparing `nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild/config.py` & `nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild/utils.py` & `nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-group-link-guild-0.0.5/nonebot_plugin_group_link_guild.egg-info/PKG-INFO` & `nonebot-plugin-group-link-guild-0.0.6/nonebot_plugin_group_link_guild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-group-link-guild
-Version: 0.0.5
+Version: 0.0.6
 Summary: 互通QQ群聊与QQ频道消息的插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-group-link-guild
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nonebot-plugin-group-link-guild-0.0.5/setup.py` & `nonebot-plugin-group-link-guild-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-group-link-guild",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.5",  # 程序版本
+    version="0.0.6",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="互通QQ群聊与QQ频道消息的插件",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/nonebot-plugin-group-link-guild",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

