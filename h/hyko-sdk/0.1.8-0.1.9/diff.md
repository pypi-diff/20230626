# Comparing `tmp/hyko_sdk-0.1.8.tar.gz` & `tmp/hyko_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.1.8.tar", last modified: Mon Jun 26 11:56:27 2023, max compression
+gzip compressed data, was "hyko_sdk-0.1.9.tar", last modified: Mon Jun 26 13:17:25 2023, max compression
```

## Comparing `hyko_sdk-0.1.8.tar` & `hyko_sdk-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/PKG-INFO
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      411 2023-05-17 08:56:51.000000 hyko_sdk-0.1.8/README.md
-drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/hyko_sdk/
--rw-rw-r--   0 crptx     (1000) crptx     (1000)       60 2023-06-26 11:54:14.000000 hyko_sdk-0.1.8/hyko_sdk/__init__.py
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      682 2023-06-26 11:51:00.000000 hyko_sdk-0.1.8/hyko_sdk/error.py
--rw-rw-r--   0 crptx     (1000) crptx     (1000)     4785 2023-06-26 11:53:34.000000 hyko_sdk-0.1.8/hyko_sdk/io.py
--rw-rw-r--   0 crptx     (1000) crptx     (1000)     2791 2023-06-26 11:49:05.000000 hyko_sdk-0.1.8/hyko_sdk/metadata.py
-drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/hyko_sdk.egg-info/
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      268 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)        1 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)       37 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/requires.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/top_level.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)       80 2023-06-21 11:17:29.000000 hyko_sdk-0.1.8/pyproject.toml
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      357 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/setup.cfg
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-26 13:17:25.780210 hyko_sdk-0.1.9/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      192 2023-06-26 13:17:25.780210 hyko_sdk-0.1.9/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      411 2023-05-19 16:11:29.000000 hyko_sdk-0.1.9/README.md
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-26 13:17:25.780210 hyko_sdk-0.1.9/hyko_sdk/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       60 2023-06-26 13:00:23.000000 hyko_sdk-0.1.9/hyko_sdk/__init__.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-06-26 13:00:23.000000 hyko_sdk-0.1.9/hyko_sdk/error.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     4767 2023-06-26 13:16:13.000000 hyko_sdk-0.1.9/hyko_sdk/io.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2791 2023-06-26 13:00:23.000000 hyko_sdk-0.1.9/hyko_sdk/metadata.py
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-26 13:17:25.780210 hyko_sdk-0.1.9/hyko_sdk.egg-info/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      192 2023-06-26 13:17:25.000000 hyko_sdk-0.1.9/hyko_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      268 2023-06-26 13:17:25.000000 hyko_sdk-0.1.9/hyko_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-06-26 13:17:25.000000 hyko_sdk-0.1.9/hyko_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       37 2023-06-26 13:17:25.000000 hyko_sdk-0.1.9/hyko_sdk.egg-info/requires.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-06-26 13:17:25.000000 hyko_sdk-0.1.9/hyko_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      357 2023-06-26 13:17:25.780210 hyko_sdk-0.1.9/setup.cfg
```

### Comparing `hyko_sdk-0.1.8/hyko_sdk/error.py` & `hyko_sdk-0.1.9/hyko_sdk/error.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.1.8/hyko_sdk/io.py` & `hyko_sdk-0.1.9/hyko_sdk/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         with open("audio.webm", "wb") as f:
             f.write(base64_bytes)
         ffmpeg.input("audio.webm").output("audio.wav").run()
 
         meta_data: dict = ffmpeg.probe("audio.wav")
         with open("audio.wav", "rb") as f:
             audio = f.read()
-        return np.frombuffer(audio, dtype=np.float64), AudioMetadata(**meta_data), None
+        return np.frombuffer(audio), AudioMetadata(**meta_data), None
 # Keep the same
 class IOPortType(str, Enum):
     NUMBER = "number"
     INTEGER = "integer"
     STRING = "string"
     IMAGE = "image"
     AUDIO = "audio"
```

### Comparing `hyko_sdk-0.1.8/hyko_sdk/metadata.py` & `hyko_sdk-0.1.9/hyko_sdk/metadata.py`

 * *Files identical despite different names*

