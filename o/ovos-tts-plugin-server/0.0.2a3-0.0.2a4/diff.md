# Comparing `tmp/ovos-tts-plugin-server-0.0.2a3.tar.gz` & `tmp/ovos-tts-plugin-server-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-tts-plugin-server-0.0.2a3.tar", last modified: Thu Jun 22 01:55:16 2023, max compression
+gzip compressed data, was "ovos-tts-plugin-server-0.0.2a4.tar", last modified: Mon Jun 26 18:25:36 2023, max compression
```

## Comparing `ovos-tts-plugin-server-0.0.2a3.tar` & `ovos-tts-plugin-server-0.0.2a4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-06-22 01:55:11.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 01:55:11.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3279 2023-06-22 01:55:11.000000 ovos-tts-plugin-server-0.0.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-06-26 18:25:31.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 18:25:31.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3279 2023-06-26 18:25:31.000000 ovos-tts-plugin-server-0.0.2a4/setup.py
```

### Comparing `ovos-tts-plugin-server-0.0.2a3/PKG-INFO` & `ovos-tts-plugin-server-0.0.2a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-server
-Version: 0.0.2a3
+Version: 0.0.2a4
 Summary: ovos tts server plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft OpenVoiceOS OVOS plugin tts
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server/__init__.py` & `ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,19 @@
         super().__init__(*args, **kwargs, audio_ext="wav",
                          validator=OVOSServerTTSValidator(self))
         self.host = self.config.get("host") or "http://0.0.0.0:9666"
 
     def get_tts(self, sentence, wav_file, lang=None, voice=None):
         lang = lang or self.lang
         voice = voice or self.voice
+        params = {"lang": lang, "voice": voice}
+        if not voice or voice == "default":
+            params.pop("voice")
         data = requests.get(f"{self.host}/synthesize/{sentence}",
-                            params={"lang": lang, "voice": voice}).content
+                            params=params).content
         with open(wav_file, "wb") as f:
             f.write(data)
         return wav_file, None
 
 
 class OVOSServerTTSValidator(TTSValidator):
     def __init__(self, tts):
```

### Comparing `ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/PKG-INFO` & `ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-server
-Version: 0.0.2a3
+Version: 0.0.2a4
 Summary: ovos tts server plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft OpenVoiceOS OVOS plugin tts
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-tts-plugin-server-0.0.2a3/setup.py` & `ovos-tts-plugin-server-0.0.2a4/setup.py`

 * *Files identical despite different names*

