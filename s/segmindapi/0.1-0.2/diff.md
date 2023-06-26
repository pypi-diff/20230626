# Comparing `tmp/segmindapi-0.1.tar.gz` & `tmp/segmindapi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmindapi-0.1.tar", last modified: Mon Jun 26 13:02:59 2023, max compression
+gzip compressed data, was "segmindapi-0.2.tar", last modified: Mon Jun 26 13:42:13 2023, max compression
```

## Comparing `segmindapi-0.1.tar` & `segmindapi-0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 13:02:59.602810 segmindapi-0.1/
--rw-rw-rw-   0        0        0      223 2023-06-26 13:02:59.602810 segmindapi-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 13:02:59.594811 segmindapi-0.1/segmindapi/
--rw-rw-rw-   0        0        0     1363 2023-06-26 12:47:29.000000 segmindapi-0.1/segmindapi/BackgroundRemoval.py
--rw-rw-rw-   0        0        0     2265 2023-06-26 12:47:35.000000 segmindapi-0.1/segmindapi/Codeformer.py
--rw-rw-rw-   0        0        0     3642 2023-06-26 12:51:53.000000 segmindapi-0.1/segmindapi/ControlNet.py
--rw-rw-rw-   0        0        0     1528 2023-06-26 12:47:42.000000 segmindapi-0.1/segmindapi/ESRGAN.py
--rw-rw-rw-   0        0        0     1336 2023-06-26 12:20:05.000000 segmindapi-0.1/segmindapi/FaceSwap.py
--rw-rw-rw-   0        0        0     2533 2023-06-26 12:47:48.000000 segmindapi-0.1/segmindapi/Kadinsky.py
--rw-rw-rw-   0        0        0     1238 2023-06-26 12:23:26.000000 segmindapi-0.1/segmindapi/SAM.py
--rw-rw-rw-   0        0        0     3001 2023-06-26 12:48:05.000000 segmindapi-0.1/segmindapi/SD1_5.py
--rw-rw-rw-   0        0        0     2512 2023-06-26 12:48:10.000000 segmindapi-0.1/segmindapi/SD2_1.py
--rw-rw-rw-   0        0        0      286 2023-06-26 12:39:29.000000 segmindapi-0.1/segmindapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 13:02:59.602810 segmindapi-0.1/segmindapi.egg-info/
--rw-rw-rw-   0        0        0      223 2023-06-26 13:02:59.000000 segmindapi-0.1/segmindapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-06-26 13:02:59.000000 segmindapi-0.1/segmindapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 13:02:59.000000 segmindapi-0.1/segmindapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-26 13:02:59.000000 segmindapi-0.1/segmindapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-26 13:02:59.000000 segmindapi-0.1/segmindapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 13:02:59.000000 segmindapi-0.1/segmindapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 13:02:59.610815 segmindapi-0.1/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-06-26 13:02:20.000000 segmindapi-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:42:13.622136 segmindapi-0.2/
+-rw-rw-rw-   0        0        0     3437 2023-06-26 13:42:13.622136 segmindapi-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3165 2023-06-26 13:41:53.000000 segmindapi-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 13:42:13.614041 segmindapi-0.2/segmindapi/
+-rw-rw-rw-   0        0        0     1363 2023-06-26 12:47:29.000000 segmindapi-0.2/segmindapi/BackgroundRemoval.py
+-rw-rw-rw-   0        0        0     2265 2023-06-26 12:47:35.000000 segmindapi-0.2/segmindapi/Codeformer.py
+-rw-rw-rw-   0        0        0     3651 2023-06-26 13:31:23.000000 segmindapi-0.2/segmindapi/ControlNet.py
+-rw-rw-rw-   0        0        0     1528 2023-06-26 12:47:42.000000 segmindapi-0.2/segmindapi/ESRGAN.py
+-rw-rw-rw-   0        0        0     1336 2023-06-26 12:20:05.000000 segmindapi-0.2/segmindapi/FaceSwap.py
+-rw-rw-rw-   0        0        0     2533 2023-06-26 12:47:48.000000 segmindapi-0.2/segmindapi/Kadinsky.py
+-rw-rw-rw-   0        0        0     1238 2023-06-26 12:23:26.000000 segmindapi-0.2/segmindapi/SAM.py
+-rw-rw-rw-   0        0        0     3001 2023-06-26 12:48:05.000000 segmindapi-0.2/segmindapi/SD1_5.py
+-rw-rw-rw-   0        0        0     2512 2023-06-26 12:48:10.000000 segmindapi-0.2/segmindapi/SD2_1.py
+-rw-rw-rw-   0        0        0      286 2023-06-26 12:39:29.000000 segmindapi-0.2/segmindapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:42:13.622136 segmindapi-0.2/segmindapi.egg-info/
+-rw-rw-rw-   0        0        0     3437 2023-06-26 13:42:13.000000 segmindapi-0.2/segmindapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-26 13:42:13.000000 segmindapi-0.2/segmindapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 13:42:13.000000 segmindapi-0.2/segmindapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 13:02:59.000000 segmindapi-0.2/segmindapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-26 13:42:13.000000 segmindapi-0.2/segmindapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 13:42:13.000000 segmindapi-0.2/segmindapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 13:42:13.622136 segmindapi-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      664 2023-06-26 13:09:59.000000 segmindapi-0.2/setup.py
```

### Comparing `segmindapi-0.1/segmindapi/BackgroundRemoval.py` & `segmindapi-0.2/segmindapi/BackgroundRemoval.py`

 * *Files identical despite different names*

### Comparing `segmindapi-0.1/segmindapi/Codeformer.py` & `segmindapi-0.2/segmindapi/Codeformer.py`

 * *Files identical despite different names*

### Comparing `segmindapi-0.1/segmindapi/ControlNet.py` & `segmindapi-0.2/segmindapi/ControlNet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 from PIL import Image
 from io import BytesIO
 
 class ControlNet:
     """
-        This API allows you to generate Segmentation Masks using ControlNet and is available at https://api.segmind.com/v1/sd1.5-controlnet-canny, https://api.segmind.com/v1/sd1.5-controlnet-depth, https://api.segmind.com/v1/sd1.5-controlnet-openpose, https://api.segmind.com/v1/sd1.5-controlnet-scribble, https://api.segmind.com/v1/sd1.5-controlnet-softedge.
+        This API allows you to generate images using various images using ControlNet and is available at https://api.segmind.com/v1/sd1.5-controlnet-canny, https://api.segmind.com/v1/sd1.5-controlnet-depth, https://api.segmind.com/v1/sd1.5-controlnet-openpose, https://api.segmind.com/v1/sd1.5-controlnet-scribble, https://api.segmind.com/v1/sd1.5-controlnet-softedge.
 
         The API accepts the following parameters:
         
         prompt: str
             Prompt to render, eg. "Stormtrooper giving a lecture"  
 
         imageUrl: str
```

### Comparing `segmindapi-0.1/segmindapi/ESRGAN.py` & `segmindapi-0.2/segmindapi/ESRGAN.py`

 * *Files identical despite different names*

### Comparing `segmindapi-0.1/segmindapi/FaceSwap.py` & `segmindapi-0.2/segmindapi/FaceSwap.py`

 * *Files identical despite different names*

### Comparing `segmindapi-0.1/segmindapi/Kadinsky.py` & `segmindapi-0.2/segmindapi/Kadinsky.py`

 * *Files identical despite different names*

### Comparing `segmindapi-0.1/segmindapi/SAM.py` & `segmindapi-0.2/segmindapi/SAM.py`

 * *Files identical despite different names*

### Comparing `segmindapi-0.1/segmindapi/SD1_5.py` & `segmindapi-0.2/segmindapi/SD1_5.py`

 * *Files identical despite different names*

### Comparing `segmindapi-0.1/segmindapi/SD2_1.py` & `segmindapi-0.2/segmindapi/SD2_1.py`

 * *Files identical despite different names*

