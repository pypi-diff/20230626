# Comparing `tmp/nonebot_plugin_matcher_block-0.0.3.tar.gz` & `tmp/nonebot_plugin_matcher_block-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_matcher_block-0.0.3.tar", last modified: Tue Jun 13 13:40:43 2023, max compression
+gzip compressed data, was "nonebot_plugin_matcher_block-0.0.4.tar", last modified: Mon Jun 26 15:25:34 2023, max compression
```

## Comparing `nonebot_plugin_matcher_block-0.0.3.tar` & `nonebot_plugin_matcher_block-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:40:43.460952 nonebot_plugin_matcher_block-0.0.3/
--rw-rw-rw-   0        0        0     1086 2022-12-05 12:34:39.000000 nonebot_plugin_matcher_block-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      284 2023-06-13 13:40:43.460452 nonebot_plugin_matcher_block-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 13:40:43.451944 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block/
--rw-rw-rw-   0        0        0     7160 2023-06-13 13:35:48.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:40:43.458950 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/
--rw-rw-rw-   0        0        0      284 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-06-13 13:40:43.000000 nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 13:40:43.460952 nonebot_plugin_matcher_block-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      530 2023-06-13 13:40:39.000000 nonebot_plugin_matcher_block-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:25:34.909158 nonebot_plugin_matcher_block-0.0.4/
+-rw-rw-rw-   0        0        0     1086 2022-12-05 12:34:39.000000 nonebot_plugin_matcher_block-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      284 2023-06-26 15:25:34.907158 nonebot_plugin_matcher_block-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 15:25:34.896147 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block/
+-rw-rw-rw-   0        0        0     7015 2023-06-26 15:23:03.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:25:34.905155 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:25:34.909158 nonebot_plugin_matcher_block-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      530 2023-06-26 15:25:30.000000 nonebot_plugin_matcher_block-0.0.4/setup.py
```

### Comparing `nonebot_plugin_matcher_block-0.0.3/LICENSE` & `nonebot_plugin_matcher_block-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_matcher_block-0.0.3/nonebot_plugin_matcher_block/__init__.py` & `nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,24 +175,22 @@
         msg += f"【{command}】：{time_config[command]}s\n"
 
     await show_block.finish(msg[:-1])
 
 from nonebot import get_driver
 
 driver = get_driver()
-bot_list = set()
-driver.on_bot_connect(lambda bot:bot_list.add(int(bot.self_id)))
-driver.on_bot_disconnect(lambda bot:bot_list.discard(int(bot.self_id)))
+bots = driver.bots
 
 history = []
 
 @event_preprocessor
 async def do_something(event: GroupMessageEvent):
-    if len(bot_list) > 1:
-        if event.user_id in bot_list:
+    if len(bots) > 1:
+        if event.user_id in bots:
             raise IgnoredException("event来自其他bot")
         global history
         history = history[:20]
         message_id = event.message_id
         if message_id in history:
             raise IgnoredException("event已被其他bot处理")
         else:
```

### Comparing `nonebot_plugin_matcher_block-0.0.3/setup.py` & `nonebot_plugin_matcher_block-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_matcher_block',
-version='0.0.3',
+version='0.0.4',
 description='通用指令阻断',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_matcher_block"]),
```

