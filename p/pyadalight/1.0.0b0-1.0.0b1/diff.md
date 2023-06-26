# Comparing `tmp/pyadalight-1.0.0b0.tar.gz` & `tmp/pyadalight-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyadalight-1.0.0b0.tar", last modified: Sun Jun 25 16:48:32 2023, max compression
+gzip compressed data, was "pyadalight-1.0.0b1.tar", last modified: Mon Jun 26 14:01:52 2023, max compression
```

## Comparing `pyadalight-1.0.0b0.tar` & `pyadalight-1.0.0b1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-25 16:48:32.781554 pyadalight-1.0.0b0/
--rwxrwxrwx   0 root         (0) root         (0)     1072 2023-06-25 16:38:05.000000 pyadalight-1.0.0b0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      745 2023-06-25 16:48:32.781101 pyadalight-1.0.0b0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-06-25 16:38:34.000000 pyadalight-1.0.0b0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-25 16:48:32.774689 pyadalight-1.0.0b0/pyadalight/
--rwxrwxrwx   0 root         (0) root         (0)       24 2023-06-25 16:39:28.000000 pyadalight-1.0.0b0/pyadalight/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6145 2023-06-25 16:22:29.000000 pyadalight-1.0.0b0/pyadalight/adalight.py
--rwxrwxrwx   0 root         (0) root         (0)      239 2023-06-25 14:37:51.000000 pyadalight-1.0.0b0/pyadalight/singleton.py
--rwxrwxrwx   0 root         (0) root         (0)     1456 2023-06-25 15:26:30.000000 pyadalight-1.0.0b0/pyadalight/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-25 16:48:32.779856 pyadalight-1.0.0b0/pyadalight.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      745 2023-06-25 16:48:32.000000 pyadalight-1.0.0b0/pyadalight.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      285 2023-06-25 16:48:32.000000 pyadalight-1.0.0b0/pyadalight.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-25 16:48:32.000000 pyadalight-1.0.0b0/pyadalight.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       63 2023-06-25 16:48:32.000000 pyadalight-1.0.0b0/pyadalight.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-06-25 16:48:32.000000 pyadalight-1.0.0b0/pyadalight.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-25 16:48:32.781800 pyadalight-1.0.0b0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1223 2023-06-25 16:45:04.000000 pyadalight-1.0.0b0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 14:01:52.110104 pyadalight-1.0.0b1/
+-rwxrwxrwx   0 root         (0) root         (0)     1072 2023-06-25 16:38:05.000000 pyadalight-1.0.0b1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1318 2023-06-26 14:01:52.089574 pyadalight-1.0.0b1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      616 2023-06-26 14:01:19.000000 pyadalight-1.0.0b1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 14:01:52.070184 pyadalight-1.0.0b1/pyadalight/
+-rwxrwxrwx   0 root         (0) root         (0)       24 2023-06-25 16:39:28.000000 pyadalight-1.0.0b1/pyadalight/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       64 2023-06-26 09:29:43.000000 pyadalight-1.0.0b1/pyadalight/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6233 2023-06-26 13:49:19.000000 pyadalight-1.0.0b1/pyadalight/adalight.py
+-rwxrwxrwx   0 root         (0) root         (0)     3406 2023-06-26 13:53:44.000000 pyadalight-1.0.0b1/pyadalight/main.py
+-rwxrwxrwx   0 root         (0) root         (0)      239 2023-06-25 14:37:51.000000 pyadalight-1.0.0b1/pyadalight/singleton.py
+-rwxrwxrwx   0 root         (0) root         (0)     1456 2023-06-25 15:26:30.000000 pyadalight-1.0.0b1/pyadalight/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 14:01:52.088315 pyadalight-1.0.0b1/pyadalight.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1318 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      364 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       76 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-26 14:01:52.110762 pyadalight-1.0.0b1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1267 2023-06-26 09:36:23.000000 pyadalight-1.0.0b1/setup.py
```

### Comparing `pyadalight-1.0.0b0/LICENSE` & `pyadalight-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyadalight-1.0.0b0/pyadalight/adalight.py` & `pyadalight-1.0.0b1/pyadalight/adalight.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,165 +1,163 @@
-"""
-MIT License
-
-Copyright (c) 2023-present RuslanUC
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from threading import Thread, get_ident, local
-from time import sleep
-
-import cv2
-import numpy as np
-from mss import mss
-from mss.base import MSSBase
-from serial import Serial
-
-from .singleton import Singleton
-from .utils import mkHeader, mkPayload
-
-
-class Mss(metaclass=Singleton):
-    def __init__(self):
-        self._threads = {}
-
-    def _get(self) -> MSSBase:
-        if get_ident() in self._threads and not hasattr(self._threads[get_ident()]._handles, "display"):
-            self.deleteThread(get_ident())
-        if get_ident() not in self._threads:
-            self._threads[get_ident()] = mss()
-        return self._threads[get_ident()]
-
-    def deleteThread(self, threadId: int) -> None:
-        if threadId in self._threads:
-            try:
-                self._threads[threadId].close()
-            except:
-                pass
-            del self._threads[threadId]
-
-    @property
-    def monitors(self) -> list[dict]:
-        return self._get().monitors
-
-    def getImage(self, monitor: dict) -> np.array:
-        return np.array(self._get().grab(monitor))
-
-
-class Adalight(metaclass=Singleton):
-    def __init__(self, h_led_count: int=None, v_led_count: int=None, port: str=None, monitor: dict=None):
-        self._h_led_count = h_led_count
-        self._v_led_count = v_led_count
-        self._port = port
-        self._monitor = monitor
-        self._ser = None
-        self._brightness = 1
-        self._running = False
-        self._thread_running = False
-        self._thread: Thread = None
-
-    @property
-    def led_count(self) -> int:
-        return self._h_led_count * 2 + self._v_led_count * 2
-
-    def _adjustBrightness(self, img: np.array) -> np.array:
-        return cv2.convertScaleAbs(img, beta=32*self._brightness)
-
-    def getZonesColors(self, image: np.array) -> np.array:
-        image = self._adjustBrightness(image)
-        assert self._h_led_count is not None, "Horizontal led count is not set!"
-        assert self._v_led_count is not None, "Vertical led count is not set!"
-        assert self._monitor is not None, "Monitor is not set!"
-        hlc = self._h_led_count
-        vlc = self._v_led_count
-        mon = self._monitor
-
-        zones = [None] * self.led_count
-
-        hw = (mon["width"] - 100) // hlc
-        hh = 100
-        vw = 100
-        vh = (mon["height"] - 50) // vlc
-        for i in range(self.led_count):  # Right to left direction
-            if i in range(hlc):
-                _i = i
-                im = image[mon["height"] - hh:mon["height"], mon["width"] - 50 - hw - hw * _i:mon["width"] - 50 - hw * _i]  # 50 is corner offset
-            elif i in range(hlc, hlc + vlc):
-                _i = i - hlc
-                im = image[mon["height"] - 25 - vh - vh * _i:mon["height"] - 25 - vh * _i, 0:vw]  # 25 is corner offset
-            elif i in range(hlc + vlc, hlc * 2 + vlc):
-                _i = i - hlc - vlc
-                im = image[0:hh, 50 + hw * _i:50 + hw + hw * _i]  # 50 is corner offset
-            elif i in range(hlc * 2 + vlc, hlc * 2 + vlc * 2):
-                _i = i - hlc * 2 - vlc
-                im = image[25 + vh * _i:25 + vh + vh * _i, mon["width"] - vw:mon["width"]]  # 25 is corner offset
-            else:
-                assert False, "This error must never happen"
-
-            zones[i] = np.mean(im, axis=(0, 1)).astype(np.uint8)[:3][::-1]
-
-        return zones
-
-    def connect(self) -> None:
-        if isinstance(self._ser, Serial) and self._ser.is_open:
-            self._ser.close()
-
-        assert self._port is not None, "Port is not set!"
-
-        self._ser = Serial(self._port, 115200)
-        assert self._ser.read(4) == b"Ada\n", "This is not adalight device!"
-
-    def disconnect(self) -> None:
-        if isinstance(self._ser, Serial) and self._ser.is_open:
-            self._ser.close()
-        self._ser = None
-
-    def writeZones(self, zones: np.array) -> None:
-        if not isinstance(self._ser, Serial) or not self._ser.is_open: return
-        self._ser.write(mkHeader(self.led_count) + mkPayload(zones))
-
-    def writeImage(self, image: np.array) -> None:
-        if not isinstance(self._ser, Serial) or not self._ser.is_open: return
-        self.writeZones(self.getZonesColors(image))
-
-    def _run(self) -> None:
-        self.connect()
-        self._running = True
-        while True:
-            if not self._running: break
-            img = Mss().getImage(self._monitor)
-            self.writeImage(img)
-        self._running = False
-        self.disconnect()
-
-    def run(self) -> None:
-        if self._thread is not None or self._running or (self._ser is not None and self._ser.is_open): return
-        self._run()
-
-    def stop(self) -> None:
-        self._running = False
-        self.disconnect()
-        if self._thread:
-            Mss().deleteThread(self._thread.ident)
-            self._thread = None
-
-    def run_in_thread(self) -> None:
-        if self._thread is not None or self._running or (self._ser is not None and self._ser.is_open): return
-
-        self._thread = Thread(target=self._run)
-        self._thread.start()
+"""
+MIT License
+
+Copyright (c) 2023-present RuslanUC
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from threading import Thread, get_ident
+
+import cv2
+import numpy as np
+from mss import mss
+from mss.base import MSSBase
+from serial import Serial
+
+from .singleton import Singleton
+from .utils import mkHeader, mkPayload
+
+
+class Mss(metaclass=Singleton):
+    def __init__(self):
+        self._threads = {}
+
+    def _get(self) -> MSSBase:
+        if get_ident() in self._threads and not hasattr(self._threads[get_ident()]._handles, "display"):
+            self.deleteThread(get_ident())
+        if get_ident() not in self._threads:
+            self._threads[get_ident()] = mss()
+        return self._threads[get_ident()]
+
+    def deleteThread(self, threadId: int) -> None:
+        if threadId in self._threads:
+            try:
+                self._threads[threadId].close()
+            except:
+                pass
+            del self._threads[threadId]
+
+    @property
+    def monitors(self) -> list[dict]:
+        return self._get().monitors
+
+    def getImage(self, monitor: dict) -> np.array:
+        return np.array(self._get().grab(monitor))
+
+
+class Adalight(metaclass=Singleton):
+    def __init__(self, h_led_count: int=None, v_led_count: int=None, port: str=None, monitor: dict=None):
+        self._h_led_count = h_led_count
+        self._v_led_count = v_led_count
+        self._port = port
+        self._monitor = monitor
+        self._ser = None
+        self._brightness = 1
+        self._running = False
+        self._thread = None
+
+    @property
+    def led_count(self) -> int:
+        return self._h_led_count * 2 + self._v_led_count * 2
+
+    def _adjustBrightness(self, img: np.array) -> np.array:
+        return cv2.convertScaleAbs(img, beta=32*self._brightness)
+
+    def getZonesColors(self, image: np.array) -> np.array:
+        image = self._adjustBrightness(image)
+        assert self._h_led_count is not None, "Horizontal led count is not set!"
+        assert self._v_led_count is not None, "Vertical led count is not set!"
+        assert self._monitor is not None, "Monitor is not set!"
+        hlc = self._h_led_count
+        vlc = self._v_led_count
+        mon = self._monitor
+
+        zones = [None] * self.led_count
+
+        hw = (mon["width"] - 100) // hlc
+        hh = 100
+        vw = 100
+        vh = (mon["height"] - 50) // vlc
+        for i in range(self.led_count):  # Right to left direction
+            if i in range(hlc):
+                _i = i
+                im = image[mon["height"] - hh:mon["height"], mon["width"] - 50 - hw - hw * _i:mon["width"] - 50 - hw * _i]  # 50 is corner offset
+            elif i in range(hlc, hlc + vlc):
+                _i = i - hlc
+                im = image[mon["height"] - 25 - vh - vh * _i:mon["height"] - 25 - vh * _i, 0:vw]  # 25 is corner offset
+            elif i in range(hlc + vlc, hlc * 2 + vlc):
+                _i = i - hlc - vlc
+                im = image[0:hh, 50 + hw * _i:50 + hw + hw * _i]  # 50 is corner offset
+            elif i in range(hlc * 2 + vlc, hlc * 2 + vlc * 2):
+                _i = i - hlc * 2 - vlc
+                im = image[25 + vh * _i:25 + vh + vh * _i, mon["width"] - vw:mon["width"]]  # 25 is corner offset
+            else:
+                assert False, "This error must never happen"
+
+            zones[i] = np.mean(im, axis=(0, 1)).astype(np.uint8)[:3][::-1]
+
+        return zones
+
+    def connect(self) -> None:
+        if isinstance(self._ser, Serial) and self._ser.is_open:
+            self._ser.close()
+
+        assert self._port is not None, "Port is not set!"
+
+        self._ser = Serial(self._port, 115200)
+        assert self._ser.read(4) == b"Ada\n", "This is not adalight device!"
+
+    def disconnect(self) -> None:
+        if isinstance(self._ser, Serial) and self._ser.is_open:
+            self._ser.close()
+        self._ser = None
+
+    def writeZones(self, zones: np.array) -> None:
+        if not isinstance(self._ser, Serial) or not self._ser.is_open: return
+        self._ser.write(mkHeader(self.led_count) + mkPayload(zones))
+
+    def writeImage(self, image: np.array) -> None:
+        if not isinstance(self._ser, Serial) or not self._ser.is_open: return
+        self.writeZones(self.getZonesColors(image))
+
+    def _run(self) -> None:
+        self.connect()
+        self._running = True
+        while True:
+            if not self._running: break
+            img = Mss().getImage(self._monitor)
+            self.writeImage(img)
+        self._running = False
+        self.disconnect()
+
+    def run(self) -> None:
+        if self._thread is not None or self._running or (self._ser is not None and self._ser.is_open): return
+        self._run()
+
+    def stop(self) -> None:
+        self._running = False
+        self.disconnect()
+        if self._thread:
+            Mss().deleteThread(self._thread.ident)
+            self._thread = None
+
+    def run_in_thread(self) -> None:
+        if self._thread is not None or self._running or (self._ser is not None and self._ser.is_open): return
+
+        self._thread = Thread(target=self._run)
+        self._thread.start()
```

### Comparing `pyadalight-1.0.0b0/pyadalight/utils.py` & `pyadalight-1.0.0b1/pyadalight/utils.py`

 * *Files identical despite different names*

