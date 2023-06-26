# Comparing `tmp/video_process-0.1.6.tar.gz` & `tmp/video_process-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_process-0.1.6.tar", max compression
+gzip compressed data, was "video_process-0.1.7.tar", max compression
```

## Comparing `video_process-0.1.6.tar` & `video_process-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      453 2023-06-25 04:04:26.548272 video_process-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-21 08:43:34.831508 video_process-0.1.6/video_process/__init__.py
--rw-r--r--   0        0        0     3960 2023-06-25 03:58:29.668830 video_process-0.1.6/video_process/graph_builder.py
--rwxr-xr-x   0        0        0     1316 2023-06-21 08:31:08.374374 video_process-0.1.6/video_process/index.py
--rw-r--r--   0        0        0     1685 2023-06-21 08:58:19.044108 video_process-0.1.6/video_process/lib.py
--rw-r--r--   0        0        0      664 2023-06-21 09:05:03.418463 video_process-0.1.6/video_process/subtitle.py
--rw-r--r--   0        0        0     2944 2023-06-21 06:40:24.748946 video_process-0.1.6/video_process/utils.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      453 2023-06-26 07:35:58.493388 video_process-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-21 08:43:34.831508 video_process-0.1.7/video_process/__init__.py
+-rw-r--r--   0        0        0     5111 2023-06-26 07:20:21.505280 video_process-0.1.7/video_process/graph_builder.py
+-rwxr-xr-x   0        0        0     1310 2023-06-26 06:41:03.502179 video_process-0.1.7/video_process/index.py
+-rw-r--r--   0        0        0     1685 2023-06-21 08:58:19.044108 video_process-0.1.7/video_process/lib.py
+-rw-r--r--   0        0        0      664 2023-06-21 09:05:03.418463 video_process-0.1.7/video_process/subtitle.py
+-rw-r--r--   0        0        0     3384 2023-06-26 06:38:17.094573 video_process-0.1.7/video_process/utils.py
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.1.7/PKG-INFO
```

### Comparing `video_process-0.1.6/video_process/index.py` & `video_process-0.1.7/video_process/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import os
 import logging
 import sys
-from video_process.utils import process_data, check_dir, get_video_length
+from video_process.utils import process_data, check_dir, get_video_min
 from video_process.graph_builder import GraphBuilder
 from video_process.lib import upload_file, get_cos_url
 
 logging.basicConfig(level=logging.INFO, stream=sys.stdout)
 logger = logging.getLogger()
 logger.setLevel(level=logging.INFO)
 
@@ -37,9 +37,9 @@
     gb.drop_first_frame()
     command = gb.build(output_path)
     gb.run(command)
 
     upload_file(body["key"], output_path)
     result = {}
     result["media_url"] = get_cos_url(body["key"])
-    result["duration"] = get_video_length(output_path)
+    result["duration"] = get_video_min(output_path)
     return result
```

### Comparing `video_process-0.1.6/video_process/lib.py` & `video_process-0.1.7/video_process/lib.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.6/video_process/subtitle.py` & `video_process-0.1.7/video_process/subtitle.py`

 * *Files identical despite different names*

### Comparing `video_process-0.1.6/video_process/utils.py` & `video_process-0.1.7/video_process/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import os
+import subprocess
 import ffmpeg
 import math
 import requests
-from video_process.subtitle import convert_to_ass, change_style
+from video_process.subtitle import change_style
 
 
 def download_file(url, path):
     response = requests.get(url)
     if response.status_code == 200:
         with open(path, "wb") as file:
             file.write(response.content)
 
 
 def process_data(data, base_dir):
-    # 处理背景图/视频字段
+    """
+    替换url为本地文件
+    """
     video_url = data["video_url"]
     video_path = os.path.join(base_dir, "video.webm")
     download_file(video_url, video_path)
     data["video_path"] = video_path
 
     if data.get("enable_bg"):
         bg = data["bg"]
@@ -29,21 +32,21 @@
         elif bg["bg_type"] == "image" and bg.get("bg_image_url"):
             image_url = bg["bg_image_url"]
             image_path = os.path.join(base_dir, "bg_image.jpg")
             download_file(image_url, image_path)
             bg["bg_image_path"] = image_path
 
     # 处理背景音乐字段
-    if data.get("enable_bg_music"):
-        bg_music = data["bg_music"]
-        if bg_music.get("bg_music_url"):
-            music_url = bg_music["bg_music_url"]
+    if data.get("enable_bgm"):
+        bg_music = data["bgm"]
+        if bg_music.get("bgm_url"):
+            music_url = bg_music["bgm_url"]
             music_path = os.path.join(base_dir, "bg_music.mp3")
             download_file(music_url, music_path)
-            bg_music["bg_music_path"] = music_path
+            bg_music["path"] = music_path
 
     # 处理字幕字段
     if data.get("enable_subtitle"):
         subtitle = data["subtitle"]
         if subtitle.get("url"):
             subtitle_url = subtitle["url"]
             subtitle_path = os.path.join(base_dir, "subtitle.srt")
@@ -66,17 +69,39 @@
                 download_file(layer_url, layer_path)
                 layer["layer_path"] = layer_path
 
         sorted_layers = sorted(layers, key=lambda x: x["index"])
         data["layers"] = sorted_layers
 
 
-def get_video_length(input_file):
+def get_video_min(input_file):
     video_info = ffmpeg.probe(input_file)
     duration = float(video_info["format"]["duration"])
     video_length = math.ceil(duration / 60)  # 将秒数转换为分钟，不满一分钟按一分钟算
     return video_length
 
 
 def check_dir(tar_dir):
     if not os.path.exists(tar_dir):
         os.makedirs(tar_dir)
+
+
+def get_video_duration(filename):
+    result = subprocess.run(
+        [
+            "ffprobe",
+            "-v",
+            "error",
+            "-select_streams",
+            "v:0",
+            "-show_entries",
+            "format=duration",
+            "-of",
+            "csv=p=0",
+            filename,
+        ],
+        capture_output=True,
+        text=True,
+    )
+    output = result.stdout.strip()
+    duration = float(output)
+    return duration
```

