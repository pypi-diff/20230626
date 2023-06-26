# Comparing `tmp/qinglan-bot-0.1.3.tar.gz` & `tmp/qinglan-bot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qinglan-bot-0.1.3.tar", last modified: Mon Jun 26 06:51:07 2023, max compression
+gzip compressed data, was "qinglan-bot-0.1.4.tar", last modified: Mon Jun 26 07:20:53 2023, max compression
```

## Comparing `qinglan-bot-0.1.3.tar` & `qinglan-bot-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:51:07.006419 qinglan-bot-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 06:51:07.006419 qinglan-bot-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:51:07.002419 qinglan-bot-0.1.3/qinglan_bot/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/qinglan_bot/ws_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:51:07.006419 qinglan-bot-0.1.3/qinglan_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 06:51:06.000000 qinglan-bot-0.1.3/qinglan_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:51:07.006419 qinglan-bot-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-26 06:51:01.000000 qinglan-bot-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/cli/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/database/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/database/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/auto_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/connected_servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/display_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/display_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/on_msg/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/on_msg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/on_msg/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/change_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/change_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/change_port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/rcon_msg_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/rcon_msg_on.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/send_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/send_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/add_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/delete_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/sub_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/setup.py
```

### Comparing `qinglan-bot-0.1.3/LICENSE` & `qinglan-bot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.3/PKG-INFO` & `qinglan-bot-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qinglan-bot-0.1.3/README.md` & `qinglan-bot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.3/qinglan_bot/__init__.py` & `qinglan-bot-0.1.4/qinglan_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.3/qinglan_bot/utils.py` & `qinglan-bot-0.1.4/qinglan_bot/utils.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.3/qinglan_bot/ws_server.py` & `qinglan-bot-0.1.4/qinglan_bot/ws_server.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.3/qinglan_bot.egg-info/PKG-INFO` & `qinglan-bot-0.1.4/qinglan_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qinglan-bot-0.1.3/setup.py` & `qinglan-bot-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import setuptools
+from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
-setuptools.setup(
+setup(
     name="qinglan-bot",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.1.3",  # 程序版本
+    version="0.1.4",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通机器人",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/qinglan_bot",  # 项目地址
-    packages=["qinglan_bot"],
+    packages=find_packages(include=['qinglan_bot', 'qinglan_bot.*']),
     classifiers=[
         "Programming Language :: Python :: 3.9",  # 使用Python3.9
         "License :: OSI Approved :: GNU Affero General Public License v3",  # 开源协议
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'mcqq-tool==0.0.4',
```

