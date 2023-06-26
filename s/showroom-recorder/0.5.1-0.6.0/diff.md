# Comparing `tmp/showroom-recorder-0.5.1.tar.gz` & `tmp/showroom-recorder-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.5.1.tar", last modified: Fri Jun 23 17:53:44 2023, max compression
+gzip compressed data, was "showroom-recorder-0.6.0.tar", last modified: Mon Jun 26 16:15:07 2023, max compression
```

## Comparing `showroom-recorder-0.5.1.tar` & `showroom-recorder-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-21 05:55:33.000000 showroom-recorder-0.5.1/LICENSE
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-20 10:03:45.000000 showroom-recorder-0.5.1/MANIFEST.in
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-20 09:47:38.000000 showroom-recorder-0.5.1/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-20 10:02:46.000000 showroom-recorder-0.5.1/description.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-20 09:59:51.000000 showroom-recorder-0.5.1/setup.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      525 2023-06-21 05:43:58.000000 showroom-recorder-0.5.1/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.499310 showroom-recorder-0.5.1/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.499310 showroom-recorder-0.5.1/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3430 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     6020 2023-06-23 17:51:42.000000 showroom-recorder-0.5.1/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3532 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-23 17:53:09.000000 showroom-recorder-0.5.1/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      771 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       51 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:30:11.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/LICENSE
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/description.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      544 2023-06-26 13:42:26.000000 showroom-recorder-0.6.0/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.473387 showroom-recorder-0.6.0/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.473387 showroom-recorder-0.6.0/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3498 2023-06-26 13:22:02.000000 showroom-recorder-0.6.0/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1304 2023-06-26 13:07:36.000000 showroom-recorder-0.6.0/src/showroom_recorder/processor/uploader.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     7602 2023-06-26 16:11:59.000000 showroom-recorder-0.6.0/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     4375 2023-06-26 13:35:58.000000 showroom-recorder-0.6.0/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.0/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-26 13:43:09.000000 showroom-recorder-0.6.0/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-26 16:15:07.477387 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      815 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       59 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-26 16:15:07.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.0/src/showroom_recorder.egg-info/zip-safe
```

### Comparing `showroom-recorder-0.5.1/LICENSE` & `showroom-recorder-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.1/PKG-INFO` & `showroom-recorder-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.5.1
+Version: 0.6.0
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.5.1/README.md` & `showroom-recorder-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.1/description.md` & `showroom-recorder-0.6.0/description.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.1/setup.py` & `showroom-recorder-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.1/showroom-recorder.json` & `showroom-recorder-0.6.0/showroom-recorder.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907407407407407%*

 * *Differences: {"'install_requires'": "{insert: [(5, 'webdav4')]}"}*

```diff
@@ -6,14 +6,15 @@
     ],
     "description": "Recording Showroom Streaming Video",
     "install_requires": [
         "emoji",
         "pytz",
         "requests",
         "websocket_client",
-        "ffmpeg-python"
+        "ffmpeg-python",
+        "webdav4"
     ],
     "keywords": "video download showroom",
     "license": "GPL",
     "name": "showroom-recorder",
     "url": "https://github.com/vacabun/showroom-recorder"
 }
```

### Comparing `showroom-recorder-0.5.1/src/showroom_recorder/common.py` & `showroom-recorder-0.6.0/src/showroom_recorder/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import argparse
 import time
 
 from .utils import config
 from .processor import danmaku
 from .processor import video
 
+
 def main():
     room_url_keys = config.readRoomsFile('rooms.ini')
     danmaku_settings = config.readSettingsFile('config.ini')
-
+    video_settings = danmaku_settings['video_settings']
+    
     # build logging
     log = logging.getLogger()
     log.setLevel(logging.INFO)
 
     consoleHandler = logging.StreamHandler()
     consoleFmt = logging.Formatter(
         fmt='%(asctime)s %(message)s', datefmt='%H:%M:%S')
@@ -40,14 +42,15 @@
         description='download showroom video and  comments')
     parser.add_argument('-i', '--id', help='Only monitor this one showroom id. \
                 For more rooms, please edit file "romms.ini".', metavar='SHOWROOM_ID', dest='sr_id')
 
     log.debug('program_settings = {}'.format(danmaku_settings['program_settings']))
     log.debug('danmaku_settings = {}'.format(danmaku_settings['danmaku_settings']))
 
+    
     # handle args
     args = parser.parse_args()
 
     nRoom = len(room_url_keys)
     if args.sr_id:
         room_url_key = args.sr_id
         room_url_keys = [room_url_key]
@@ -69,15 +72,15 @@
             log.info('Comments on')
         else:
             log.info('Comments off')
         # start monitoring room
 
     danmaku_rm = danmaku.RoomMonitor(room_url_keys, danmaku_settings)
     danmaku_rm.start()
-    video_rm = video.RoomMonitor(room_url_keys, danmaku_settings)
+    video_rm = video.RecroderManager(room_url_keys, video_settings)
     video_rm.start()
 
     helptxt = '''
     Commands:
     - Type "h" or "help" for help.
     - Type "q" or "quit" to quit.
     '''
```

### Comparing `showroom-recorder-0.5.1/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.6.0/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.1/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.6.0/src/showroom_recorder/utils/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,46 +57,62 @@
 [danmaku_settings]
 width = 640
 height = 360
 font_name = MS PGothic
 font_size = 18
 alpha = 10                       # transparency percentage, a number between 0 and 100
 
+[video_settings]
+upload_webdav = 0                # 1: enable, 0: disable
+webdav_url = http://webdav_url
+webdav_username = username
+webdav_password = password
+
 """
     # create file if not present
     path = os.getcwd()
     filenamepath = os.path.join(path, filename)
     if not os.path.isfile(filenamepath):
         with open(filenamepath, 'w', encoding='utf8') as fp:
             fp.write(settingsTxt)
         print('Created {}'.format(filename))
 
     with open(filenamepath, 'r', encoding='utf8') as fp:
         lines = fp.readlines()
 
     foundProgSettings = False
     foundDanmakuSettings = False
+    foundVideoSettings = False
     program_settings = {}
     danmaku_settings = {}
+    video_settings = {}
     for line in lines:
         # remove # and line after it
         sharp = line.find('#')
         if sharp > -1:
             line = line[:sharp]
         line = line.strip()
         if len(line) == 0:
             continue
 
         if line.lower().find('[program_settings]') > -1:
             foundProgSettings = True
             foundDanmakuSettings = False
+            foundVideoSettings = False
             continue
         if line.lower().find('[danmaku_settings]') > -1:
             foundProgSettings = False
             foundDanmakuSettings = True
+            foundVideoSettings = False
+            continue
+
+        if line.lower().find('[video_settings]') > -1:
+            foundProgSettings = False
+            foundDanmakuSettings = False
+            foundVideoSettings = True
             continue
 
         if foundProgSettings:
             s1, s2 = line.split("=", 1)
             program_settings.update(
                 {s1.lower().strip(): int(s2.lower().strip())})
             continue
@@ -106,11 +122,23 @@
             s1 = s1.lower().strip()
             s2 = s2.strip()
             if s1.find('font_name') < 0:
                 s2 = int(s2)
             danmaku_settings.update({s1: s2})
             continue
 
+        if foundVideoSettings:
+            s1, s2 = line.split("=", 1)
+            s1 = s1.lower().strip()
+            s2 = s2.strip()
+            if s2 == '1':
+                s2 = True
+            if s2 == '0':
+                s2 = False
+            video_settings.update({s1: s2})
+            continue
+
     settings = {'program_settings': program_settings,
-                'danmaku_settings': danmaku_settings}
+                'danmaku_settings': danmaku_settings,
+                'video_settings': video_settings}
     return settings
```

### Comparing `showroom-recorder-0.5.1/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.6.0/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.1/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.6.0/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.5.1
+Version: 0.6.0
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.5.1/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.6.0/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 src/showroom_recorder.egg-info/dependency_links.txt
 src/showroom_recorder.egg-info/entry_points.txt
 src/showroom_recorder.egg-info/requires.txt
 src/showroom_recorder.egg-info/top_level.txt
 src/showroom_recorder.egg-info/zip-safe
 src/showroom_recorder/processor/__init__.py
 src/showroom_recorder/processor/danmaku.py
+src/showroom_recorder/processor/uploader.py
 src/showroom_recorder/processor/video.py
 src/showroom_recorder/utils/__init__.py
 src/showroom_recorder/utils/config.py
 src/showroom_recorder/utils/delete_emoji.py
```

