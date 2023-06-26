# Comparing `tmp/Abg-1.9.2.tar.gz` & `tmp/Abg-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-1.9.2.tar", last modified: Mon Jun 19 09:46:33 2023, max compression
+gzip compressed data, was "Abg-2.0.tar", last modified: Mon Jun 26 02:44:09 2023, max compression
```

## Comparing `Abg-1.9.2.tar` & `Abg-2.0.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg/
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg/pyro/
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg/pyro/chat_status/
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/chat_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/chat_status/chat_status.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/chat_status/custom_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg/pyro/helpers/
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3179 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/human_read.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/pyro_progress.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/helpers/ratelimit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/inline/
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6105 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/patch/
--rw-r--r--   0 root         (0) root         (0)       79 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11979 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/patch/listen/
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12016 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/listen/listen.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/listen/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.105302 Abg-1.9.2/Abg/pyro/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-06-19 09:46:08.000000 Abg-1.9.2/Abg/pyro/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:46:33.101302 Abg-1.9.2/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4992 2023-06-19 09:46:33.000000 Abg-1.9.2/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2023-06-19 09:46:33.000000 Abg-1.9.2/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:46:33.000000 Abg-1.9.2/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-19 09:46:33.000000 Abg-1.9.2/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4992 2023-06-19 09:46:33.105302 Abg-1.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2479 2023-06-19 09:46:08.000000 Abg-1.9.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 09:46:33.105302 Abg-1.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2987 2023-06-19 09:46:08.000000 Abg-1.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.677948 Abg-2.0/Abg/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-26 02:43:45.000000 Abg-2.0/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.677948 Abg-2.0/Abg/chat_status/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-26 02:43:45.000000 Abg-2.0/Abg/chat_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-06-26 02:43:45.000000 Abg-2.0/Abg/chat_status/chat_status.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-06-26 02:43:45.000000 Abg-2.0/Abg/chat_status/custom_filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/helpers/
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/human_read.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/pyro_progress.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/ratelimit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/inline/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-26 02:43:45.000000 Abg-2.0/Abg/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2023-06-26 02:43:45.000000 Abg-2.0/Abg/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-06-26 02:43:45.000000 Abg-2.0/Abg/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-26 02:43:45.000000 Abg-2.0/Abg/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/patch/
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/patch/listen/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12016 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/listen/listen.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/listen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.677948 Abg-2.0/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-06-26 02:44:09.000000 Abg-2.0/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      830 2023-06-26 02:44:09.000000 Abg-2.0/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 02:44:09.000000 Abg-2.0/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-26 02:44:09.000000 Abg-2.0/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-06-26 02:44:09.681949 Abg-2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-26 02:43:45.000000 Abg-2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 02:44:09.681949 Abg-2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-06-26 02:43:45.000000 Abg-2.0/setup.py
```

### Comparing `Abg-1.9.2/Abg/pyro/chat_status/chat_status.py` & `Abg-2.0/Abg/chat_status/chat_status.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/chat_status/custom_filters.py` & `Abg-2.0/Abg/chat_status/custom_filters.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/helpers/__init__.py` & `Abg-2.0/Abg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/helpers/helpers.py` & `Abg-2.0/Abg/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/helpers/http_helper.py` & `Abg-2.0/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/helpers/human_read.py` & `Abg-2.0/Abg/helpers/human_read.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/helpers/parser.py` & `Abg-2.0/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/helpers/pyro_progress.py` & `Abg-2.0/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/helpers/ratelimit.py` & `Abg-2.0/Abg/helpers/ratelimit.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/inline/inline_keyboard.py` & `Abg-2.0/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/inline/inline_pagination_keyboard.py` & `Abg-2.0/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/inline/reply_keyboard.py` & `Abg-2.0/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/patch/bound/message.py` & `Abg-2.0/Abg/patch/bound/message.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/patch/listen/listen.py` & `Abg-2.0/Abg/patch/listen/listen.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/patch/listen/utils.py` & `Abg-2.0/Abg/patch/listen/utils.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/patch/methods/edit_message_text.py` & `Abg-2.0/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/patch/methods/send_as_file.py` & `Abg-2.0/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg/pyro/patch/methods/send_message.py` & `Abg-2.0/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-1.9.2/Abg.egg-info/PKG-INFO` & `Abg-2.0/Abg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.9.2
-Summary: Bot Helpers
+Version: 2.0
+Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
 Description: # ᴀʙɢ :->
         > 
-        ### • Conversation in pyrogram
+        ### • Conversation ingram
         
         ```python
         from pyrogram import filters, Client
         from pyrogram.types import Message
-        from Abg.pyro import patch  # type : ignore
+        from Abg import patch  # type : ignore
         
         app = Client("my_account")
         
         @app.on_message(filters.command(["myinfo"]))
         async def my_info(self: Client, ctx: Message):
             if not ctx.from_user:
                 return
@@ -37,15 +37,15 @@
         
           app.run()
         ```
         >
         ### • User Rights 
         
         ```python 
-        from Abg.pyro.chat_status import adminsOnly, command
+        from Abg.chat_status import adminsOnly, command
         from pyrogram.enums import ChatType
         from pyrogram.types import Message
         from pyrogram import Client
         
         app = Client("my_account")
         
         @app.on_message(command("del"))
@@ -68,15 +68,15 @@
         ```
         
         
         >
         ### • Keyboards
         
         ```python
-        from Abg.pyro.inline import InlineKeyboard, InlineButton
+        from Abg.inline import InlineKeyboard, InlineButton
         
         
         keyboard = InlineKeyboard(row_width=3)
         keyboard.add(
             InlineButton('1', 'inline_keyboard:1'),
             InlineButton('2', 'inline_keyboard:2'),
             InlineButton('3', 'inline_keyboard:3'),
@@ -104,14 +104,15 @@
         - This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
         - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
         
         - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
         
         ━━━━━━━━━━━━━━━━━━━━ 
         
+        
 Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch botapi https
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `Abg-1.9.2/PKG-INFO` & `Abg-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 1.9.2
-Summary: Bot Helpers
+Version: 2.0
+Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
 Description: # ᴀʙɢ :->
         > 
-        ### • Conversation in pyrogram
+        ### • Conversation ingram
         
         ```python
         from pyrogram import filters, Client
         from pyrogram.types import Message
-        from Abg.pyro import patch  # type : ignore
+        from Abg import patch  # type : ignore
         
         app = Client("my_account")
         
         @app.on_message(filters.command(["myinfo"]))
         async def my_info(self: Client, ctx: Message):
             if not ctx.from_user:
                 return
@@ -37,15 +37,15 @@
         
           app.run()
         ```
         >
         ### • User Rights 
         
         ```python 
-        from Abg.pyro.chat_status import adminsOnly, command
+        from Abg.chat_status import adminsOnly, command
         from pyrogram.enums import ChatType
         from pyrogram.types import Message
         from pyrogram import Client
         
         app = Client("my_account")
         
         @app.on_message(command("del"))
@@ -68,15 +68,15 @@
         ```
         
         
         >
         ### • Keyboards
         
         ```python
-        from Abg.pyro.inline import InlineKeyboard, InlineButton
+        from Abg.inline import InlineKeyboard, InlineButton
         
         
         keyboard = InlineKeyboard(row_width=3)
         keyboard.add(
             InlineButton('1', 'inline_keyboard:1'),
             InlineButton('2', 'inline_keyboard:2'),
             InlineButton('3', 'inline_keyboard:3'),
@@ -104,14 +104,15 @@
         - This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
         - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
         
         - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
         
         ━━━━━━━━━━━━━━━━━━━━ 
         
+        
 Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch botapi https
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `Abg-1.9.2/README.md` & `Abg-2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ᴀʙɢ :->
 > 
-### • Conversation in pyrogram
+### • Conversation ingram
 
 ```python
 from pyrogram import filters, Client
 from pyrogram.types import Message
-from Abg.pyro import patch  # type : ignore
+from Abg import patch  # type : ignore
 
 app = Client("my_account")
 
 @app.on_message(filters.command(["myinfo"]))
 async def my_info(self: Client, ctx: Message):
     if not ctx.from_user:
         return
@@ -24,15 +24,15 @@
 
   app.run()
 ```
 >
 ### • User Rights 
 
 ```python 
-from Abg.pyro.chat_status import adminsOnly, command
+from Abg.chat_status import adminsOnly, command
 from pyrogram.enums import ChatType
 from pyrogram.types import Message
 from pyrogram import Client
 
 app = Client("my_account")
 
 @app.on_message(command("del"))
@@ -55,15 +55,15 @@
 ```
 
 
 >
 ### • Keyboards
 
 ```python
-from Abg.pyro.inline import InlineKeyboard, InlineButton
+from Abg.inline import InlineKeyboard, InlineButton
 
 
 keyboard = InlineKeyboard(row_width=3)
 keyboard.add(
     InlineButton('1', 'inline_keyboard:1'),
     InlineButton('2', 'inline_keyboard:2'),
     InlineButton('3', 'inline_keyboard:3'),
@@ -90,7 +90,8 @@
 
 - This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
 - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
 
 - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
 
 ━━━━━━━━━━━━━━━━━━━━ 
+
```

### Comparing `Abg-1.9.2/setup.py` & `Abg-2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="1.9.2",
-    description="Bot Helpers",
+    version="2.0",
+    description="Telegram bot helpers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi1M",
     author_email="Abishnoi69@Abg.org",
     license="MIT",
```

