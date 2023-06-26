# Comparing `tmp/qinglan-bot-0.1.1.tar.gz` & `tmp/qinglan-bot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qinglan-bot-0.1.1.tar", last modified: Mon Jun 26 04:02:30 2023, max compression
+gzip compressed data, was "qinglan-bot-0.1.2.tar", last modified: Mon Jun 26 04:03:05 2023, max compression
```

## Comparing `qinglan-bot-0.1.1.tar` & `qinglan-bot-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:02:30.499602 qinglan-bot-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 04:02:23.000000 qinglan-bot-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 04:02:30.499602 qinglan-bot-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-26 04:02:23.000000 qinglan-bot-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:02:30.499602 qinglan-bot-0.1.1/qinglan_bot/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-26 04:02:23.000000 qinglan-bot-0.1.1/qinglan_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 04:02:23.000000 qinglan-bot-0.1.1/qinglan_bot/cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 04:02:23.000000 qinglan-bot-0.1.1/qinglan_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-26 04:02:23.000000 qinglan-bot-0.1.1/qinglan_bot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 04:02:23.000000 qinglan-bot-0.1.1/qinglan_bot/ws_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:02:30.499602 qinglan-bot-0.1.1/qinglan_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 04:02:30.000000 qinglan-bot-0.1.1/qinglan_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 04:02:30.000000 qinglan-bot-0.1.1/qinglan_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:02:30.000000 qinglan-bot-0.1.1/qinglan_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 04:02:30.000000 qinglan-bot-0.1.1/qinglan_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-26 04:02:30.000000 qinglan-bot-0.1.1/qinglan_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 04:02:30.000000 qinglan-bot-0.1.1/qinglan_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 04:02:30.499602 qinglan-bot-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-26 04:02:23.000000 qinglan-bot-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/qinglan_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/qinglan_bot/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/qinglan_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 04:03:05.000000 qinglan-bot-0.1.2/qinglan_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 04:03:05.593927 qinglan-bot-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-26 04:02:59.000000 qinglan-bot-0.1.2/setup.py
```

### Comparing `qinglan-bot-0.1.1/LICENSE` & `qinglan-bot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.1/PKG-INFO` & `qinglan-bot-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.1.1
+Version: 0.1.2
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qinglan-bot-0.1.1/README.md` & `qinglan-bot-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.1/qinglan_bot/__init__.py` & `qinglan-bot-0.1.2/qinglan_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.1/qinglan_bot/utils.py` & `qinglan-bot-0.1.2/qinglan_bot/utils.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.1/qinglan_bot/ws_server.py` & `qinglan-bot-0.1.2/qinglan_bot/ws_server.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.1/qinglan_bot.egg-info/PKG-INFO` & `qinglan-bot-0.1.2/qinglan_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.1.1
+Version: 0.1.2
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qinglan-bot-0.1.1/setup.py` & `qinglan-bot-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="qinglan-bot",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.1.1",  # 程序版本
+    version="0.1.2",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通机器人",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/qinglan_bot",  # 项目地址
     packages=["qinglan_bot"],
```

