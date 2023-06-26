# Comparing `tmp/telegram_types-1.8.tar.gz` & `tmp/telegram_types-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_types-1.8.tar", last modified: Wed Jul 27 06:34:16 2022, max compression
+gzip compressed data, was "telegram_types-1.9.tar", last modified: Wed Jul 27 09:59:19 2022, max compression
```

## Comparing `telegram_types-1.8.tar` & `telegram_types-1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 06:34:16.556868 telegram_types-1.8/
--rw-r--r--   0 arsen     (1000) arsen     (1000)       25 2022-05-22 17:33:42.000000 telegram_types-1.8/MANIFEST.in
--rw-r--r--   0 arsen     (1000) arsen     (1000)     1451 2022-07-27 06:34:16.556868 telegram_types-1.8/PKG-INFO
--rw-r--r--   0 arsen     (1000) arsen     (1000)       41 2022-05-22 16:22:13.000000 telegram_types-1.8/requirements.txt
--rw-r--r--   0 arsen     (1000) arsen     (1000)       38 2022-07-27 06:34:16.556868 telegram_types-1.8/setup.cfg
--rw-r--r--   0 arsen     (1000) arsen     (1000)     1908 2022-05-22 16:37:08.000000 telegram_types-1.8/setup.py
-drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 06:34:16.532867 telegram_types-1.8/telegram_types/
--rw-r--r--   0 arsen     (1000) arsen     (1000)      261 2022-07-27 06:34:02.000000 telegram_types-1.8/telegram_types/__init__.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      990 2022-06-16 13:07:52.000000 telegram_types-1.8/telegram_types/base.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)     1427 2022-06-18 16:58:59.000000 telegram_types-1.8/telegram_types/media_attributes.py
-drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 06:34:16.536867 telegram_types-1.8/telegram_types/types/
--rw-r--r--   0 arsen     (1000) arsen     (1000)      401 2022-07-27 06:31:51.000000 telegram_types-1.8/telegram_types/types/__init__.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      324 2022-05-22 16:18:43.000000 telegram_types-1.8/telegram_types/types/callback_query.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)     1900 2022-06-20 21:53:26.000000 telegram_types-1.8/telegram_types/types/chat.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      185 2022-05-22 00:26:23.000000 telegram_types-1.8/telegram_types/types/chat_photo.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      492 2022-07-27 06:33:33.000000 telegram_types-1.8/telegram_types/types/deleted_messages.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      748 2022-05-22 16:00:17.000000 telegram_types-1.8/telegram_types/types/keyboard.py
-drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 06:34:16.552868 telegram_types-1.8/telegram_types/types/media/
--rw-r--r--   0 arsen     (1000) arsen     (1000)      474 2022-05-21 00:11:07.000000 telegram_types-1.8/telegram_types/types/media/__init__.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      387 2022-05-22 00:23:48.000000 telegram_types-1.8/telegram_types/types/media/animation.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      406 2022-05-22 00:23:58.000000 telegram_types-1.8/telegram_types/types/media/audio.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      212 2022-05-22 00:24:05.000000 telegram_types-1.8/telegram_types/types/media/contact.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)       87 2022-05-22 00:25:02.000000 telegram_types-1.8/telegram_types/types/media/dice.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      337 2022-05-22 00:25:07.000000 telegram_types-1.8/telegram_types/types/media/document.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      234 2022-05-22 00:25:09.000000 telegram_types-1.8/telegram_types/types/media/game.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      102 2022-05-22 00:25:20.000000 telegram_types-1.8/telegram_types/types/media/location.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      318 2022-05-22 00:25:27.000000 telegram_types-1.8/telegram_types/types/media/photo.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      613 2022-05-22 00:24:48.000000 telegram_types-1.8/telegram_types/types/media/poll.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      108 2022-05-22 00:25:38.000000 telegram_types-1.8/telegram_types/types/media/reaction.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      461 2022-05-22 00:25:45.000000 telegram_types-1.8/telegram_types/types/media/sticker.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      171 2022-05-22 00:25:48.000000 telegram_types-1.8/telegram_types/types/media/thumbnail.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      241 2022-05-22 00:25:53.000000 telegram_types-1.8/telegram_types/types/media/venue.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      453 2022-05-22 00:25:59.000000 telegram_types-1.8/telegram_types/types/media/video.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      343 2022-05-22 00:26:03.000000 telegram_types-1.8/telegram_types/types/media/video_note.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      274 2022-05-22 00:26:05.000000 telegram_types-1.8/telegram_types/types/media/voice.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      624 2022-05-22 00:26:11.000000 telegram_types-1.8/telegram_types/types/media/webpage.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)     3293 2022-07-25 03:50:42.000000 telegram_types-1.8/telegram_types/types/message.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      112 2022-05-22 00:26:33.000000 telegram_types-1.8/telegram_types/types/restriction.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)     1060 2022-05-22 00:26:37.000000 telegram_types-1.8/telegram_types/types/user.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)      130 2022-05-19 12:30:33.000000 telegram_types-1.8/telegram_types/utils.py
-drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 06:34:16.532867 telegram_types-1.8/telegram_types.egg-info/
--rw-r--r--   0 arsen     (1000) arsen     (1000)     1451 2022-07-27 06:34:16.000000 telegram_types-1.8/telegram_types.egg-info/PKG-INFO
--rw-r--r--   0 arsen     (1000) arsen     (1000)     1355 2022-07-27 06:34:16.000000 telegram_types-1.8/telegram_types.egg-info/SOURCES.txt
--rw-r--r--   0 arsen     (1000) arsen     (1000)        1 2022-07-27 06:34:16.000000 telegram_types-1.8/telegram_types.egg-info/dependency_links.txt
--rw-r--r--   0 arsen     (1000) arsen     (1000)        1 2022-06-12 17:55:11.000000 telegram_types-1.8/telegram_types.egg-info/not-zip-safe
--rw-r--r--   0 arsen     (1000) arsen     (1000)       41 2022-07-27 06:34:16.000000 telegram_types-1.8/telegram_types.egg-info/requires.txt
--rw-r--r--   0 arsen     (1000) arsen     (1000)       15 2022-07-27 06:34:16.000000 telegram_types-1.8/telegram_types.egg-info/top_level.txt
+drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 09:59:19.430888 telegram_types-1.9/
+-rw-r--r--   0 arsen     (1000) arsen     (1000)       25 2022-05-22 17:33:42.000000 telegram_types-1.9/MANIFEST.in
+-rw-r--r--   0 arsen     (1000) arsen     (1000)     1451 2022-07-27 09:59:19.430888 telegram_types-1.9/PKG-INFO
+-rw-r--r--   0 arsen     (1000) arsen     (1000)       41 2022-05-22 16:22:13.000000 telegram_types-1.9/requirements.txt
+-rw-r--r--   0 arsen     (1000) arsen     (1000)       38 2022-07-27 09:59:19.430888 telegram_types-1.9/setup.cfg
+-rw-r--r--   0 arsen     (1000) arsen     (1000)     1908 2022-05-22 16:37:08.000000 telegram_types-1.9/setup.py
+drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 09:59:19.418887 telegram_types-1.9/telegram_types/
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      278 2022-07-27 09:59:10.000000 telegram_types-1.9/telegram_types/__init__.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      990 2022-06-16 13:07:52.000000 telegram_types-1.9/telegram_types/base.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)     1427 2022-06-18 16:58:59.000000 telegram_types-1.9/telegram_types/media_attributes.py
+drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 09:59:19.422887 telegram_types-1.9/telegram_types/types/
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      401 2022-07-27 06:31:51.000000 telegram_types-1.9/telegram_types/types/__init__.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      324 2022-05-22 16:18:43.000000 telegram_types-1.9/telegram_types/types/callback_query.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)     1900 2022-06-20 21:53:26.000000 telegram_types-1.9/telegram_types/types/chat.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      185 2022-05-22 00:26:23.000000 telegram_types-1.9/telegram_types/types/chat_photo.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      963 2022-07-27 09:58:42.000000 telegram_types-1.9/telegram_types/types/deleted_messages.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      748 2022-05-22 16:00:17.000000 telegram_types-1.9/telegram_types/types/keyboard.py
+drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 09:59:19.430888 telegram_types-1.9/telegram_types/types/media/
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      474 2022-05-21 00:11:07.000000 telegram_types-1.9/telegram_types/types/media/__init__.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      387 2022-05-22 00:23:48.000000 telegram_types-1.9/telegram_types/types/media/animation.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      406 2022-05-22 00:23:58.000000 telegram_types-1.9/telegram_types/types/media/audio.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      212 2022-05-22 00:24:05.000000 telegram_types-1.9/telegram_types/types/media/contact.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)       87 2022-05-22 00:25:02.000000 telegram_types-1.9/telegram_types/types/media/dice.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      337 2022-05-22 00:25:07.000000 telegram_types-1.9/telegram_types/types/media/document.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      234 2022-05-22 00:25:09.000000 telegram_types-1.9/telegram_types/types/media/game.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      102 2022-05-22 00:25:20.000000 telegram_types-1.9/telegram_types/types/media/location.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      318 2022-05-22 00:25:27.000000 telegram_types-1.9/telegram_types/types/media/photo.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      613 2022-05-22 00:24:48.000000 telegram_types-1.9/telegram_types/types/media/poll.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      108 2022-05-22 00:25:38.000000 telegram_types-1.9/telegram_types/types/media/reaction.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      461 2022-05-22 00:25:45.000000 telegram_types-1.9/telegram_types/types/media/sticker.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      171 2022-05-22 00:25:48.000000 telegram_types-1.9/telegram_types/types/media/thumbnail.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      241 2022-05-22 00:25:53.000000 telegram_types-1.9/telegram_types/types/media/venue.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      453 2022-05-22 00:25:59.000000 telegram_types-1.9/telegram_types/types/media/video.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      343 2022-05-22 00:26:03.000000 telegram_types-1.9/telegram_types/types/media/video_note.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      274 2022-05-22 00:26:05.000000 telegram_types-1.9/telegram_types/types/media/voice.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      624 2022-05-22 00:26:11.000000 telegram_types-1.9/telegram_types/types/media/webpage.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)     3293 2022-07-25 03:50:42.000000 telegram_types-1.9/telegram_types/types/message.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      112 2022-05-22 00:26:33.000000 telegram_types-1.9/telegram_types/types/restriction.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)     1060 2022-05-22 00:26:37.000000 telegram_types-1.9/telegram_types/types/user.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      130 2022-05-19 12:30:33.000000 telegram_types-1.9/telegram_types/utils.py
+drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-07-27 09:59:19.418887 telegram_types-1.9/telegram_types.egg-info/
+-rw-r--r--   0 arsen     (1000) arsen     (1000)     1451 2022-07-27 09:59:19.000000 telegram_types-1.9/telegram_types.egg-info/PKG-INFO
+-rw-r--r--   0 arsen     (1000) arsen     (1000)     1355 2022-07-27 09:59:19.000000 telegram_types-1.9/telegram_types.egg-info/SOURCES.txt
+-rw-r--r--   0 arsen     (1000) arsen     (1000)        1 2022-07-27 09:59:19.000000 telegram_types-1.9/telegram_types.egg-info/dependency_links.txt
+-rw-r--r--   0 arsen     (1000) arsen     (1000)        1 2022-06-12 17:55:11.000000 telegram_types-1.9/telegram_types.egg-info/not-zip-safe
+-rw-r--r--   0 arsen     (1000) arsen     (1000)       41 2022-07-27 09:59:19.000000 telegram_types-1.9/telegram_types.egg-info/requires.txt
+-rw-r--r--   0 arsen     (1000) arsen     (1000)       15 2022-07-27 09:59:19.000000 telegram_types-1.9/telegram_types.egg-info/top_level.txt
```

### Comparing `telegram_types-1.8/PKG-INFO` & `telegram_types-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram_types
-Version: 1.8
+Version: 1.9
 Home-page: https://github.com/telectron
 Download-URL: https://github.com/telectron/telectron/releases/latest
 Author: Dan
 Author-email: dan@telectron.org
 License: LGPLv3+
 Keywords: telegram chat messenger mtproto api client library python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `telegram_types-1.8/setup.py` & `telegram_types-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `telegram_types-1.8/telegram_types/base.py` & `telegram_types-1.9/telegram_types/base.py`

 * *Files identical despite different names*

### Comparing `telegram_types-1.8/telegram_types/media_attributes.py` & `telegram_types-1.9/telegram_types/media_attributes.py`

 * *Files identical despite different names*

### Comparing `telegram_types-1.8/telegram_types/types/chat.py` & `telegram_types-1.9/telegram_types/types/chat.py`

 * *Files identical despite different names*

### Comparing `telegram_types-1.8/telegram_types/types/keyboard.py` & `telegram_types-1.9/telegram_types/types/keyboard.py`

 * *Files identical despite different names*

### Comparing `telegram_types-1.8/telegram_types/types/media/poll.py` & `telegram_types-1.9/telegram_types/types/media/poll.py`

 * *Files identical despite different names*

### Comparing `telegram_types-1.8/telegram_types/types/media/webpage.py` & `telegram_types-1.9/telegram_types/types/media/webpage.py`

 * *Files identical despite different names*

### Comparing `telegram_types-1.8/telegram_types/types/message.py` & `telegram_types-1.9/telegram_types/types/message.py`

 * *Files identical despite different names*

### Comparing `telegram_types-1.8/telegram_types/types/user.py` & `telegram_types-1.9/telegram_types/types/user.py`

 * *Files identical despite different names*

### Comparing `telegram_types-1.8/telegram_types.egg-info/PKG-INFO` & `telegram_types-1.9/telegram_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-types
-Version: 1.8
+Version: 1.9
 Home-page: https://github.com/telectron
 Download-URL: https://github.com/telectron/telectron/releases/latest
 Author: Dan
 Author-email: dan@telectron.org
 License: LGPLv3+
 Keywords: telegram chat messenger mtproto api client library python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `telegram_types-1.8/telegram_types.egg-info/SOURCES.txt` & `telegram_types-1.9/telegram_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

