# Comparing `tmp/hydrusvideodeduplicator-0.1.6.tar.gz` & `tmp/hydrusvideodeduplicator-0.1.7.tar.gz`

## Comparing `hydrusvideodeduplicator-0.1.6.tar` & `hydrusvideodeduplicator-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/README.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    11301 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/pdq_utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_faiss.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36568 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/LICENSE
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/README.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/README.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    13565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/pdq_utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_faiss.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36568 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/README.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/README.md` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/dedup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from io import IOBase
 import logging
 import tempfile
 from itertools import islice
 import json
 from pathlib import Path
+import subprocess
 
 import hydrusvideodeduplicator.hydrus_api as hydrus_api
 import hydrusvideodeduplicator.hydrus_api.utils
 from tqdm import tqdm
 from rich import print as rprint
 from sqlitedict import SqliteDict
 
@@ -75,16 +76,66 @@
     # dir is where you're writing the video file
     def _add_perceptual_hash_to_db(cls, video_hash: str, video: str | bytes, video_dir: Path | str, db) -> None:
         with tempfile.NamedTemporaryFile(mode="w+b", dir=video_dir) as tmp_vid_file:
             # Write video to file to be able to calculate hash
             tmp_vid_file.write(video)
             tmp_vid_file.seek(0)
 
-            # Set perceptual_hash column
-            perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file.name)
+            ffprobe_cmd = [
+                        'ffprobe',
+                        '-v',
+                        'error',
+                        '-select_streams',
+                        'v:0',
+                        '-show_entries',
+                        'stream=codec_name',
+                        '-of',
+                        'default=noprint_wrappers=1:nokey=1',
+                        tmp_vid_file.name
+                        ]
+
+            # Execute the ffprobe command and capture the output
+            video_codec = subprocess.check_output(ffprobe_cmd).decode('utf-8').strip()
+
+            # These are found by trial and error. If you find an unsupported codec, create an issue on GitHub please.
+            # Unsupported codecs appear to be an OpenCV issue more than an FFmpeg issue but I can't solve it at the moment.
+            # For now, just transcode the video to avc1
+            unsupported_codecs = ["av1"]
+
+            if video_codec in unsupported_codecs:
+                rprint(f"[yellow] Video file has unsupported codec: {video_codec}")
+                rprint("[yellow] Falling back to transcoding (this may take a bit)")
+
+                try:
+
+                    with tempfile.NamedTemporaryFile(mode="w+b", dir=video_dir, suffix=".mp4") as tmp_vid_file_transcoded:
+                        ffmpeg_cmd = [
+                            'ffmpeg',
+                            '-y',
+                            '-i',
+                            tmp_vid_file.name,
+                            '-c:v',
+                            'libx264',
+                            '-preset',
+                            'veryfast',
+                            '-crf',
+                            '28',
+                            tmp_vid_file_transcoded.name,
+                        ]
+
+                        # Execute the ffmpeg command
+                        with open(os.devnull, "w") as devnull: subprocess.call(ffmpeg_cmd, stdout=devnull, stderr=devnull)
+
+                        perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file_transcoded.name)
+
+                        print("[yellow] Fallback to transcode successful.")
+                except:
+                    print("[red] Transcode and/or hashing the transcode failed.")
+            else:
+                perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file.name)
 
             row = db.get(video_hash, {})
             row["perceptual_hash"] = perceptual_hash
             db[video_hash] = row
             cls.hydlog.debug(f"Perceptual hash calculated and added to DB.")
     
     # Add perceptual hash for videos to the database
```

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/pdq_utils.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/pdq_utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_brute_matcher.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_brute_matcher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_faiss.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_faiss.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/vpdq_util.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/.gitignore` & `hydrusvideodeduplicator-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/LICENSE` & `hydrusvideodeduplicator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/README.md` & `hydrusvideodeduplicator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/pyproject.toml` & `hydrusvideodeduplicator-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.6/PKG-INFO` & `hydrusvideodeduplicator-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author: appleappleapplenanner
 License-Expression: MIT
 License-File: LICENSE
```

