# Comparing `tmp/mediapy-1.1.6.tar.gz` & `tmp/mediapy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediapy-1.1.6.tar", last modified: Fri Feb 24 13:08:34 2023, max compression
+gzip compressed data, was "mediapy-1.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mediapy-1.1.6.tar` & `mediapy-1.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11358 2023-02-24 13:08:09.095990 mediapy-1.1.6/LICENSE
--rw-r--r--   0        0        0     3738 2023-02-24 13:08:09.095990 mediapy-1.1.6/README.md
--rw-r--r--   0        0        0    65687 2023-02-24 13:08:09.095990 mediapy-1.1.6/mediapy/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 13:08:09.095990 mediapy-1.1.6/mediapy/py.typed
--rw-r--r--   0        0        0     2243 2023-02-24 13:08:09.099990 mediapy-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 mediapy-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-26 18:02:57.144394 mediapy-1.1.7/LICENSE
+-rw-r--r--   0        0        0     3738 2023-06-26 18:02:57.144394 mediapy-1.1.7/README.md
+-rw-r--r--   0        0        0    65830 2023-06-26 18:02:57.144394 mediapy-1.1.7/mediapy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:02:57.144394 mediapy-1.1.7/mediapy/py.typed
+-rw-r--r--   0        0        0     2243 2023-06-26 18:02:57.152394 mediapy-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 mediapy-1.1.7/PKG-INFO
```

### Comparing `mediapy-1.1.6/LICENSE` & `mediapy-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mediapy-1.1.6/README.md` & `mediapy-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mediapy-1.1.6/mediapy/__init__.py` & `mediapy-1.1.7/mediapy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The mediapy Authors.
+# Copyright 2023 The mediapy Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -95,15 +95,15 @@
       w.add_image(darken_image(image))
 ```
 """
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '1.1.6'
+__version__ = '1.1.7'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 import base64
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 import contextlib
 import functools
 import importlib
@@ -1154,17 +1154,21 @@
       bps = int(match.group(1)) * 1000
     if matches := re.findall(r'frame= *([0-9]+) ', line):
       num_images = int(matches[-1])
     if 'Stream #0:' in line and ': Video:' in line:
       if not (match := re.search(r', ([0-9]+)x([0-9]+)', line)):
         raise RuntimeError(f'Unable to parse video dimensions in line {line}')
       width, height = int(match.group(1)), int(match.group(2))
-      if not (match := re.search(r', ([0-9.]+) fps', line)):
+      if match := re.search(r', ([0-9.]+) fps', line):
+        fps = float(match.group(1))
+      elif str(path).endswith('.gif'):
+        # Some GIF files lack a framerate attribute; use a reasonable default.
+        fps = 10
+      else:
         raise RuntimeError(f'Unable to parse video framerate in line {line}')
-      fps = float(match.group(1))
     if match := re.fullmatch(r'\s*rotate\s*:\s*(\d+)', line):
       rotation = int(match.group(1))
   if not num_images:
     raise RuntimeError(f'Unable to find frames in video: {err}')
   if not width:
     raise RuntimeError(f'Unable to parse video header: {err}')
   # By default, ffmpeg enables "-autorotate"; we just fix the dimensions.
@@ -1728,16 +1732,16 @@
   elif border:
     border = 'border:1px solid black; '
   else:
     border = ''
   options = (
       f'controls width="{width}" height="{height}"'
       f' style="{border}object-fit:cover;"'
-      f"{' loop' if loop else ''}"
-      f"{' autoplay muted' if autoplay else ''}"
+      f'{" loop" if loop else ""}'
+      f'{" autoplay muted" if autoplay else ""}'
   )
   s = f"""<video {options}>
       <source src="data:video/mp4;base64,{b64}" type="video/mp4"/>
       This browser does not support the video tag.
       </video>"""
   if title:
     s = f"""<div style="display:flex; align-items:left;">
```

### Comparing `mediapy-1.1.6/pyproject.toml` & `mediapy-1.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mediapy-1.1.6/PKG-INFO` & `mediapy-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediapy
-Version: 1.1.6
+Version: 1.1.7
 Summary: Read/write/show images and videos in an IPython notebook
 Keywords: 
 Author-email: Google LLC <mediapy-owners@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

