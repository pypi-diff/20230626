# Comparing `tmp/asyncio_mqtt-0.9.0.tar.gz` & `tmp/asyncio_mqtt-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asyncio_mqtt-0.9.0.tar", last modified: Mon May  3 08:08:07 2021, max compression
+gzip compressed data, was "dist/asyncio_mqtt-0.9.1.tar", last modified: Thu May 13 09:08:17 2021, max compression
```

## Comparing `asyncio_mqtt-0.9.0.tar` & `asyncio_mqtt-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 fpa       (1000) fpa       (1000)        0 2021-05-03 08:08:07.317052 asyncio_mqtt-0.9.0/
--rw-rw-r--   0 fpa       (1000) fpa       (1000)    10520 2021-05-03 08:08:07.317052 asyncio_mqtt-0.9.0/PKG-INFO
--rw-rw-r--   0 fpa       (1000) fpa       (1000)     8150 2021-05-03 07:34:18.000000 asyncio_mqtt-0.9.0/README.md
-drwxrwxr-x   0 fpa       (1000) fpa       (1000)        0 2021-05-03 08:08:07.313052 asyncio_mqtt-0.9.0/asyncio_mqtt/
--rw-rw-r--   0 fpa       (1000) fpa       (1000)      225 2021-05-03 07:34:18.000000 asyncio_mqtt-0.9.0/asyncio_mqtt/__init__.py
--rw-rw-r--   0 fpa       (1000) fpa       (1000)    21302 2021-05-03 07:34:18.000000 asyncio_mqtt-0.9.0/asyncio_mqtt/client.py
--rw-rw-r--   0 fpa       (1000) fpa       (1000)     1267 2021-05-03 07:34:18.000000 asyncio_mqtt-0.9.0/asyncio_mqtt/error.py
--rw-rw-r--   0 fpa       (1000) fpa       (1000)        0 2021-05-03 07:34:18.000000 asyncio_mqtt-0.9.0/asyncio_mqtt/py.typed
--rw-rw-r--   0 fpa       (1000) fpa       (1000)      128 2021-05-03 07:34:18.000000 asyncio_mqtt-0.9.0/asyncio_mqtt/types.py
--rw-rw-r--   0 fpa       (1000) fpa       (1000)       62 2021-05-03 07:51:02.000000 asyncio_mqtt-0.9.0/asyncio_mqtt/version.py
-drwxrwxr-x   0 fpa       (1000) fpa       (1000)        0 2021-05-03 08:08:07.317052 asyncio_mqtt-0.9.0/asyncio_mqtt.egg-info/
--rw-rw-r--   0 fpa       (1000) fpa       (1000)    10520 2021-05-03 08:08:07.000000 asyncio_mqtt-0.9.0/asyncio_mqtt.egg-info/PKG-INFO
--rw-rw-r--   0 fpa       (1000) fpa       (1000)      335 2021-05-03 08:08:07.000000 asyncio_mqtt-0.9.0/asyncio_mqtt.egg-info/SOURCES.txt
--rw-rw-r--   0 fpa       (1000) fpa       (1000)        1 2021-05-03 08:08:07.000000 asyncio_mqtt-0.9.0/asyncio_mqtt.egg-info/dependency_links.txt
--rw-rw-r--   0 fpa       (1000) fpa       (1000)       60 2021-05-03 08:08:07.000000 asyncio_mqtt-0.9.0/asyncio_mqtt.egg-info/requires.txt
--rw-rw-r--   0 fpa       (1000) fpa       (1000)       13 2021-05-03 08:08:07.000000 asyncio_mqtt-0.9.0/asyncio_mqtt.egg-info/top_level.txt
--rw-rw-r--   0 fpa       (1000) fpa       (1000)       38 2021-05-03 08:08:07.317052 asyncio_mqtt-0.9.0/setup.cfg
--rw-rw-r--   0 fpa       (1000) fpa       (1000)     1277 2021-05-03 07:34:18.000000 asyncio_mqtt-0.9.0/setup.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2021-05-13 09:08:17.505339 asyncio_mqtt-0.9.1/
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)    10520 2021-05-13 09:08:17.505339 asyncio_mqtt-0.9.1/PKG-INFO
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)     8150 2021-03-11 16:46:10.000000 asyncio_mqtt-0.9.1/README.md
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2021-05-13 09:08:17.501339 asyncio_mqtt-0.9.1/asyncio_mqtt/
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)      225 2021-03-11 08:08:18.000000 asyncio_mqtt-0.9.1/asyncio_mqtt/__init__.py
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)    21386 2021-05-13 08:57:35.000000 asyncio_mqtt-0.9.1/asyncio_mqtt/client.py
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)     1586 2021-05-13 08:57:35.000000 asyncio_mqtt-0.9.1/asyncio_mqtt/error.py
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)        0 2021-03-11 08:08:18.000000 asyncio_mqtt-0.9.1/asyncio_mqtt/py.typed
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)      128 2021-03-11 08:08:18.000000 asyncio_mqtt-0.9.1/asyncio_mqtt/types.py
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)       62 2021-05-13 09:06:51.000000 asyncio_mqtt-0.9.1/asyncio_mqtt/version.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2021-05-13 09:08:17.505339 asyncio_mqtt-0.9.1/asyncio_mqtt.egg-info/
+-rw-r--r--   0 frederik  (1000) frederik  (1000)    10520 2021-05-13 09:08:17.000000 asyncio_mqtt-0.9.1/asyncio_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 frederik  (1000) frederik  (1000)      335 2021-05-13 09:08:17.000000 asyncio_mqtt-0.9.1/asyncio_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 frederik  (1000) frederik  (1000)        1 2021-05-13 09:08:17.000000 asyncio_mqtt-0.9.1/asyncio_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 frederik  (1000) frederik  (1000)       60 2021-05-13 09:08:17.000000 asyncio_mqtt-0.9.1/asyncio_mqtt.egg-info/requires.txt
+-rw-r--r--   0 frederik  (1000) frederik  (1000)       13 2021-05-13 09:08:17.000000 asyncio_mqtt-0.9.1/asyncio_mqtt.egg-info/top_level.txt
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)       38 2021-05-13 09:08:17.505339 asyncio_mqtt-0.9.1/setup.cfg
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)     1277 2021-03-11 08:08:18.000000 asyncio_mqtt-0.9.1/setup.py
```

### Comparing `asyncio_mqtt-0.9.0/PKG-INFO` & `asyncio_mqtt-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio_mqtt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Idomatic asyncio wrapper around paho-mqtt.
 Home-page: https://github.com/sbtinstruments/asyncio-mqtt
 Author: Frederik Aalund
 Author-email: fpa@sbtinstruments.com
 License: BSD 3-clause License
 Description: ![license](https://img.shields.io/github/license/sbtinstruments/asyncio-mqtt)
         ![semver](https://img.shields.io/github/v/tag/sbtinstruments/asyncio-mqtt?sort=semver)
```

### Comparing `asyncio_mqtt-0.9.0/README.md` & `asyncio_mqtt-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `asyncio_mqtt-0.9.0/asyncio_mqtt/client.py` & `asyncio_mqtt-0.9.1/asyncio_mqtt/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,16 +472,19 @@
             self._misc_task = self._loop.create_task(self._misc_loop())
 
         self._loop.call_soon_threadsafe(create_task_cb)
 
     def _on_socket_close(
         self, client: mqtt.Client, userdata: Any, sock: socket.socket
     ) -> None:
-        self._loop.remove_reader(sock.fileno())
-        if self._misc_task is not None:
+
+        fileno = sock.fileno()
+        if fileno > -1:
+            self._loop.remove_reader(fileno)
+        if self._misc_task is not None and not self._misc_task.done():
             with suppress(asyncio.CancelledError):
                 self._misc_task.cancel()
 
     def _on_socket_register_write(
         self, client: mqtt.Client, userdata: Any, sock: socket.socket
     ) -> None:
         def cb() -> None:
```

### Comparing `asyncio_mqtt-0.9.0/asyncio_mqtt/error.py` & `asyncio_mqtt-0.9.1/asyncio_mqtt/error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # SPDX-License-Identifier: BSD-3-Clause
 
 
-from typing import Any, Dict
+from typing import Any, Dict, Union
+
+import paho.mqtt.client as mqtt  # type: ignore
 
 
 class MqttError(Exception):
     """Base exception for all asyncio-mqtt exceptions."""
 
     pass
 
 
 class MqttCodeError(MqttError):
-    def __init__(self, rc: int, *args: Any):
+    def __init__(self, rc: Union[int, mqtt.ReasonCodes], *args: Any):
         super().__init__(*args)
         self.rc = rc
 
     def __str__(self) -> str:
-        return f"[code:{self.rc}] {super().__str__()}"
+        if isinstance(self.rc, mqtt.ReasonCodes):
+            return f"[code:{self.rc.value}] {str(self.rc)}"
+        else:
+            return f"[code:{self.rc}] {super().__str__()}"
 
 
 class MqttConnectError(MqttCodeError):
-    def __init__(self, rc: int):
+    def __init__(self, rc: Union[int, mqtt.ReasonCodes]):
+        if isinstance(rc, mqtt.ReasonCodes):
+            return super().__init__(rc)
         msg = "Connection refused"
         try:
             msg += f": {_CONNECT_RC_STRINGS[rc]}"
         except KeyError:
             pass
         super().__init__(rc, msg)
```

### Comparing `asyncio_mqtt-0.9.0/asyncio_mqtt.egg-info/PKG-INFO` & `asyncio_mqtt-0.9.1/asyncio_mqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio-mqtt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Idomatic asyncio wrapper around paho-mqtt.
 Home-page: https://github.com/sbtinstruments/asyncio-mqtt
 Author: Frederik Aalund
 Author-email: fpa@sbtinstruments.com
 License: BSD 3-clause License
 Description: ![license](https://img.shields.io/github/license/sbtinstruments/asyncio-mqtt)
         ![semver](https://img.shields.io/github/v/tag/sbtinstruments/asyncio-mqtt?sort=semver)
```

### Comparing `asyncio_mqtt-0.9.0/setup.py` & `asyncio_mqtt-0.9.1/setup.py`

 * *Files identical despite different names*

