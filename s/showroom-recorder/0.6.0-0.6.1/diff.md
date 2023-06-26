# Comparing `tmp/showroom-recorder-0.6.0.tar.gz` & `tmp/showroom-recorder-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.6.0.tar", last modified: Mon Jun 26 16:15:07 2023, max compression
+gzip compressed data, was "showroom-recorder-0.6.1.tar", last modified: Mon Jun 26 17:05:43 2023, max compression
```

## Comparing `showroom-recorder-0.6.0.tar` & `showroom-recorder-0.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/LICENSE
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/MANIFEST.in
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/description.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/setup.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      544 2023-06-26 13:42:26.000000 showroom-recorder-0.6.0/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.473387 showroom-recorder-0.6.0/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.473387 showroom-recorder-0.6.0/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3498 2023-06-26 13:22:02.000000 showroom-recorder-0.6.0/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1304 2023-06-26 13:07:36.000000 showroom-recorder-0.6.0/src/showroom_recorder/processor/uploader.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     7602 2023-06-26 16:11:59.000000 showroom-recorder-0.6.0/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     4375 2023-06-26 13:35:58.000000 showroom-recorder-0.6.0/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-26 13:43:09.000000 showroom-recorder-0.6.0/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      815 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       59 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 17:05:43.079511 showroom-recorder-0.6.1/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/LICENSE
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-26 17:05:43.079511 showroom-recorder-0.6.1/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/description.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-26 17:05:43.079511 showroom-recorder-0.6.1/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      570 2023-06-26 17:05:37.000000 showroom-recorder-0.6.1/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 17:05:43.075511 showroom-recorder-0.6.1/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 17:05:43.079511 showroom-recorder-0.6.1/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3498 2023-06-26 13:22:02.000000 showroom-recorder-0.6.1/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 17:05:43.079511 showroom-recorder-0.6.1/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1304 2023-06-26 13:07:36.000000 showroom-recorder-0.6.1/src/showroom_recorder/processor/uploader.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     7893 2023-06-26 17:05:37.000000 showroom-recorder-0.6.1/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 17:05:43.079511 showroom-recorder-0.6.1/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     4375 2023-06-26 13:35:58.000000 showroom-recorder-0.6.1/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.1/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-26 17:05:37.000000 showroom-recorder-0.6.1/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 17:05:43.079511 showroom-recorder-0.6.1/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-26 17:05:43.000000 showroom-recorder-0.6.1/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      815 2023-06-26 17:05:43.000000 showroom-recorder-0.6.1/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 17:05:43.000000 showroom-recorder-0.6.1/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-26 17:05:43.000000 showroom-recorder-0.6.1/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       74 2023-06-26 17:05:43.000000 showroom-recorder-0.6.1/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-26 17:05:43.000000 showroom-recorder-0.6.1/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.1/src/showroom_recorder.egg-info/zip-safe
```

### Comparing `showroom-recorder-0.6.0/LICENSE` & `showroom-recorder-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.0/PKG-INFO` & `showroom-recorder-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.0
+Version: 0.6.1
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.0/README.md` & `showroom-recorder-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.0/description.md` & `showroom-recorder-0.6.1/description.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.0/setup.py` & `showroom-recorder-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.0/showroom-recorder.json` & `showroom-recorder-0.6.1/showroom-recorder.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920634920634921%*

 * *Differences: {"'install_requires'": "{insert: [(6, 'fake-useragent')]}"}*

```diff
@@ -7,14 +7,15 @@
     "description": "Recording Showroom Streaming Video",
     "install_requires": [
         "emoji",
         "pytz",
         "requests",
         "websocket_client",
         "ffmpeg-python",
-        "webdav4"
+        "webdav4",
+        "fake-useragent"
     ],
     "keywords": "video download showroom",
     "license": "GPL",
     "name": "showroom-recorder",
     "url": "https://github.com/vacabun/showroom-recorder"
 }
```

### Comparing `showroom-recorder-0.6.0/src/showroom_recorder/common.py` & `showroom-recorder-0.6.1/src/showroom_recorder/common.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.0/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.6.1/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.0/src/showroom_recorder/processor/uploader.py` & `showroom-recorder-0.6.1/src/showroom_recorder/processor/uploader.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.0/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.6.1/src/showroom_recorder/processor/video.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,40 +5,48 @@
 import threading
 import ffmpeg
 import json
 import requests
 import datetime
 import pytz
 from .uploader import UploaderQueue, UploaderWebDav
+import random
+from fake_useragent import UserAgent
 
 
+ua = UserAgent()
+
 fake_headers = {
-    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8',
+    'Accept': '*/*',
+    'Accept-Encoding': 'gzip, deflate, br',
+    'Accept-Language': 'zh,en-US;q=0.9,en;q=0.8,zh-CN;q=0.7,ja;q=0.6',
     'Accept-Charset': 'UTF-8,*;q=0.5',
-    'Accept-Encoding': 'gzip,deflate,sdch',
-    'Accept-Language': 'en-US,en;q=0.8',
-    'User-Agent': 'Mozilla/5.0 (Linux; Android 4.4.2; Nexus 4 Build/KOT49H) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.114 Mobile Safari/537.36'
+    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36'
 }
 
 
 def get_status_by_room_url_key(room_url_key):
     url = "https://www.showroom-live.com/api/room/status"
     params = {
         "room_url_key": room_url_key,
+        "_": str(int(time.time() * 1000))
     }
+    fake_headers['User-Agent'] = ua.chrome
     response = requests.get(url=url, headers=fake_headers, params=params)
     status = response.json()
     return status
 
 
 def get_online_by_roomid(room_id):
     url = "https://www.showroom-live.com/api/live/live_info"
     params = {
         "room_id": room_id,
+        "_": str(int(time.time() * 1000))
     }
+    fake_headers['User-Agent'] = ua.chrome
     response = requests.get(url=url, headers=fake_headers, params=params)
     response = response.json()
     if response['live_status'] == 2:
         return True
     else:
         return False
 
@@ -75,14 +83,15 @@
 
 
 def get_stream_url_by_roomid(room_id):
     stream_url = ''
     api_endpoint = 'https://www.showroom-live.com/api/live/streaming_url?room_id={room_id}&_={timestamp}&abr_available=1'.format(
         room_id=room_id, timestamp=str(int(time.time() * 1000)))
     try:
+        fake_headers['User-Agent'] = ua.chrome
         response = requests.get(url=api_endpoint, headers=fake_headers).text
         response = json.loads(response)
         stream_url = response['streaming_url_list'][0]['url']
         for streaming_url in response['streaming_url_list']:
             if streaming_url['type'] == 'hls_all':
                 stream_url = streaming_url['url']
     except Exception as e:
@@ -222,8 +231,9 @@
                             r = Recorder(status, self.uploader_queue, self.config)
                             r.start()
                             self.recorders[i] = r
                             continue
                     except Exception as e:
                         logging.error('{room_url_key}: {e}'.format(
                             room_url_key=room_url_key, e=e))
-            time.sleep(1)
+            delay_time = random.uniform(1, 3)
+            time.sleep(delay_time)
```

### Comparing `showroom-recorder-0.6.0/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.6.1/src/showroom_recorder/utils/config.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.0/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.6.1/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.0/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.6.1/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.0
+Version: 0.6.1
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.0/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.6.1/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

