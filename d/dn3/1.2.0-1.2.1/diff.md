# Comparing `tmp/dn3-1.2.0.tar.gz` & `tmp/dn3-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dn3-1.2.0.tar", last modified: Thu Mar  9 10:00:39 2023, max compression
+gzip compressed data, was "dn3-1.2.1.tar", last modified: Mon Jun 26 13:13:04 2023, max compression
```

## Comparing `dn3-1.2.0.tar` & `dn3-1.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:00:39.564075 dn3-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-09 10:00:17.000000 dn3-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-03-09 10:00:39.564075 dn3-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-03-09 10:00:17.000000 dn3-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:00:39.552075 dn3-1.2.0/dn3/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:00:39.556075 dn3-1.2.0/dn3/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/crypto/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:00:39.556075 dn3-1.2.0/dn3/l1ght/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/l1ght/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/l1ght/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/l1ght/elf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/l1ght/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/l1ght/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/l1ght/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/l1ght/sock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:00:39.560075 dn3-1.2.0/dn3/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/misc/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/misc/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/misc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:00:39.560075 dn3-1.2.0/dn3/pwn/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/pwn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/pwn/cyclic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/pwn/deathnot3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/pwn/fmtstr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:00:39.564075 dn3-1.2.0/dn3/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/tools/linkerpatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-09 10:00:17.000000 dn3-1.2.0/dn3/tools/templategen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:00:39.556075 dn3-1.2.0/dn3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-03-09 10:00:39.000000 dn3-1.2.0/dn3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-09 10:00:39.000000 dn3-1.2.0/dn3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 10:00:39.000000 dn3-1.2.0/dn3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-09 10:00:39.000000 dn3-1.2.0/dn3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-09 10:00:39.000000 dn3-1.2.0/dn3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-09 10:00:39.000000 dn3-1.2.0/dn3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 10:00:39.564075 dn3-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-09 10:00:17.000000 dn3-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:13:04.502221 dn3-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 13:12:36.000000 dn3-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-26 13:13:04.502221 dn3-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-26 13:12:36.000000 dn3-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:13:04.498221 dn3-1.2.1/dn3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:13:04.498221 dn3-1.2.1/dn3/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/crypto/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:13:04.498221 dn3-1.2.1/dn3/l1ght/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/l1ght/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/l1ght/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/l1ght/elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/l1ght/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/l1ght/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/l1ght/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/l1ght/sock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:13:04.498221 dn3-1.2.1/dn3/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/misc/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/misc/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/misc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:13:04.502221 dn3-1.2.1/dn3/pwn/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/pwn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/pwn/cyclic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/pwn/deathnot3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/pwn/fmtstr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:13:04.502221 dn3-1.2.1/dn3/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/tools/linkerpatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-26 13:12:36.000000 dn3-1.2.1/dn3/tools/templategen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:13:04.498221 dn3-1.2.1/dn3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-26 13:13:04.000000 dn3-1.2.1/dn3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-26 13:13:04.000000 dn3-1.2.1/dn3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:13:04.000000 dn3-1.2.1/dn3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 13:13:04.000000 dn3-1.2.1/dn3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 13:13:04.000000 dn3-1.2.1/dn3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-26 13:13:04.000000 dn3-1.2.1/dn3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:13:04.502221 dn3-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-26 13:12:36.000000 dn3-1.2.1/setup.py
```

### Comparing `dn3-1.2.0/LICENSE` & `dn3-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/PKG-INFO` & `dn3-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dn3
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/k1R4/deathnot3/
 Author: k1R4
 Author-email: srijiith@outlook.com
 Keywords: pwn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6, <4
```

### Comparing `dn3-1.2.0/README.md` & `dn3-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3/__init__.py` & `dn3-1.2.1/dn3/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,8 @@
             prefix = f"{BOLD}({GREEN}dn3{END}{BOLD}){END} "
         return prefix +  super(LoggerFormatter, self).format(record)
 
 handler = StreamHandler()
 handler.setFormatter(LoggerFormatter("%(message)s"))
 logger = getLogger(__name__)
 logger.setLevel(INFO)
-logger.addHandler(handler)
-
-def signal_handler(*args):
-    logger.error("Interrupted!")
-    exit(-1)
-
-signal(SIGINT,signal_handler)
+logger.addHandler(handler)
```

### Comparing `dn3-1.2.0/dn3/l1ght/gdb.py` & `dn3-1.2.1/dn3/l1ght/gdb.py`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3/l1ght/pipe.py` & `dn3-1.2.1/dn3/l1ght/pipe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from abc import abstractmethod
+from dn3.tools.config import cfg
 from dn3.l1ght.context import ctx
 from dn3.misc.encoding import *
 from dn3.misc.colors import *
 from dn3.misc.utils import msleep
 from threading import Thread, Lock
 from logging import getLogger
 from binascii import hexlify
 
 logger = getLogger(__name__)
 
 
 DEBUG = 1
 INFO = 0
 
-IOs = []
-
 
 def IO_debug(x, mode="Received"):
     if not x:
         return
 
     if mode == "Received":
         color = RED
@@ -55,20 +54,16 @@
 
 class BufferedPipe():
 
 
     def __init__(self):
         self._buf = b""
         self._max_buf = 4096
-        self._is_interactive = False
-        self._run_thread = True
-        self._lock = Lock()
-        self._thread = Thread(target=self._reader)
+        self._thread = Thread(target=self._interactive_output)
         self._thread.daemon = True
-        self._thread.start()
 
     @abstractmethod
     def kill():
         pass
 
     @abstractmethod
     def interactive():
@@ -79,102 +74,109 @@
         pass
 
     @abstractmethod
     def _write():
         pass
 
 
-    def _reader(self):
+    def _interactive_output(self):
+
+        if hasattr(self, "_sock"):
+            timeout = int(cfg.timeout)
+        else:
+            timeout = 0.1
 
-        while self._run_thread:
-            if len(self._buf) < self._max_buf:
-                x = b""
-                self._lock.acquire()
-                x = self._read(self._max_buf-len(self._buf),timeout=5)
+        while True:
+                x = self._read(4096,timeout)
                 if x:
-                    if self._is_interactive:
-                        print(x.decode(),end="",flush=True)
-                    else:
-                        self._buf += x
-                    self._lock.release()
-                    msleep(1)
-                    continue
-                else:
-                    self._lock.release()
-                    msleep(1)
-                    continue
+                    try:
+                        x = x.decode()
+                    except:
+                        x = bytes2str(x)
+                    print("\r"+x,end="",flush=True)
+                    print("%s%sdn3>%s " % (YELLOW,BOLD,END), end="", flush=True)
 
-    def recv(self, n, timeout=1000):
+
+    def recv(self, n, timeout=None):
         
-        x = b""
+        if n > 4096:
+            logger.error("Can only recv 4096 bytes at a time")
 
-        self._lock.acquire()
+        x = b""
+        
         if n > len(self._buf):
             x += self._buf
-            self._buf = b""
-            x += self._read(n-len(x),timeout)
+            if not timeout:
+                self._buf = self._read(self._max_buf)
+            else:
+                self._buf = self._read(self._max_buf,timeout)
+            n -= len(x)
 
-        else:
-            x += self._buf[:n]
-            self._buf = self._buf[n:]
+        x += self._buf[:n]
+        self._buf = self._buf[n:]
 
         if len(x) != n:
             logger.error("EOF!")
 
         if ctx.log == DEBUG:
             IO_debug(x)
 
         if ctx.mode == str:
             x = bytes2str(x)
 
-        self._lock.release()
         return x
 
     
     def recvuntil(self,x):
 
         x = x2bytes(x)
         t = b""
 
         if not x:
             logger.error("Invalid delimiter length!")
 
-        mode,log = ctx.mode,ctx.log
-        ctx.mode,ctx.log = bytes,INFO
-        while True:
-            k = self.recv(1)
-            t += k
-            if t.find(x) != -1:
-                break
-        ctx.mode,ctx.log = mode,log
+        n = self._buf.find(x)
+        if n == -1:
+            t = self._buf
+            self._buf = b""
+            while True:
+                k = self._read(1)
+                if not k:
+                    logger.error("EOF!")
+                t += k
+                if t.find(x) != -1:
+                    break
+
+        else:
+            t = self._buf[:n+len(x)]
+            self._buf = self._buf[n+len(x):]
         
         if ctx.log == DEBUG:
             IO_debug(t)
 
         if ctx.mode == str:
             t = bytes2str(t)
         
         return t
 
     
     def recvline(self):
         return self.recvuntil(b"\n")
 
     def recvall(self):
-        self._lock.acquire()
+
         x = self._buf
         self._buf = b""
 
         if ctx.log == DEBUG:
             IO_debug(x)
 
         if ctx.mode == str:
             x = bytes2str(x)
 
-        self._lock.release()
         return x
 
     def send(self,x):
         x = x2bytes(x)
 
         if not x:
             logger.error("Invalid input")
```

### Comparing `dn3-1.2.0/dn3/l1ght/proc.py` & `dn3-1.2.1/dn3/l1ght/proc.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self._pid = self._process.pid
 
         super().__init__()
 
         logger.info("Spawned process %s with PID: %s%d%s" % (self._cmd.split()[0],BOLD,self._pid,END))
         ctx.io = self
 
-    def _read(self,n,timeout=1):
+    def _read(self,n,timeout=-1):
         if not self._process:
             logger.error("Process Ended!")
         while timeout:
             x = b""
             x = self._process.stdout.read(n)
             if not x and self._poll():
                 msleep(1)
@@ -91,31 +91,31 @@
                 logger.error("Process %s stopped with code: %d" % (self._cmd.split()[0],returncode))
             return False
 
 
     def kill(self):
         if not self._process:
             return
-        self._run_thread = False
-        self._thread.join()
+        if self._thread.is_alive():
+            self._thread.join()
         self._process.terminate()
         self._process = None
         logger.info("Process %s with PID: %d was killed!" % (self._cmd.split()[0], self._pid))
 
 
     def interactive(self):
-        self._is_interactive = True
+
         ctx.log = INFO
-        self._lock.acquire()
         print(self._buf.decode(),flush=True,end="")
-        self._lock.release()
+        self._thread.start()
+
         while True:
             if self._poll():
                 try:
-                    print("%s%sdn3>%s " % (YELLOW,BOLD,END), end="", flush=True)
+                    print("\r%s%sdn3>%s " % (YELLOW,BOLD,END), end="", flush=True)
                     self.sendline(input())
                     if self._poll():
                         msleep(10)
                         continue
                 except:
                     break
             else:
```

### Comparing `dn3-1.2.0/dn3/l1ght/sock.py` & `dn3-1.2.1/dn3/l1ght/sock.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if not self._sock:
             logger.error("Socket closed!")
 
         self._sock.settimeout(timeout/1000)
         try:
             x = self._sock.recv(n)
             return x
-        except TimeoutError:
+        except socket.timeout:
             return b""
         except ConnectionAbortedError:
             self.kill()
             logger.error("Connection reset!")
 
 
     def _write(self,x):
@@ -60,30 +60,30 @@
         try:
             return self._sock.send(x)
         except:
             logger.error("Socket closed unexpectedly!")
 
 
     def kill(self):
-        self._run_thread = False
-        self._thread.join()
+        if self._thread.is_alive():
+            self._thread.join()
         self._sock.close()
         self._sock = None
         logger.info("Connection closed to %s:%s" % (self._host,self._port))
 
 
     def interactive(self):
-        self._is_interactive = True
+
         ctx.log = INFO
-        self._lock.acquire()
         print(self._buf.decode(),flush=True,end="")
-        self._lock.release()
+        self._thread.start()
+
         while True:
             try:
-                print("%s%sdn3>%s " % (YELLOW,BOLD,END), end="", flush=True)
+                print("\r%s%sdn3>%s " % (YELLOW,BOLD,END), end="", flush=True)
                 self.sendline(input())
-                msleep(200)
+                msleep(10)
                 continue
             except:
                 break
 
 remote = sock
```

### Comparing `dn3-1.2.0/dn3/misc/encoding.py` & `dn3-1.2.1/dn3/misc/encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,21 @@
 def p16(x):
 	if isinstance(x,int):
 		return bytes2str(pack("<H",x))
 	else:
 		logger.error("%s provided, int expected!" % type(x))
 
 
+def p8(x):
+	if isinstance(x,int):
+		return chr(x&0xff)
+	else:
+		logger.error("%s provided, int expected!" % type(x))
+
+
 def upk(x):
 	if isinstance(x,str):
 		return unpack("<Q",str2bytes((x[:8]).ljust(8,"\x00")))[0]
 	elif isinstance(x,bytes):
 		return unpack("<Q",(x[:8]).ljust(8,b"\x00"))[0]
 	else:
 		logger.error("%s provided, string expected!" % type(x))
```

### Comparing `dn3-1.2.0/dn3/misc/utils.py` & `dn3-1.2.1/dn3/misc/utils.py`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3/pwn/cyclic.py` & `dn3-1.2.1/dn3/pwn/cyclic.py`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3/pwn/deathnot3.py` & `dn3-1.2.1/dn3/pwn/deathnot3.py`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3/pwn/fmtstr.py` & `dn3-1.2.1/dn3/pwn/fmtstr.py`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3/tools/cli.py` & `dn3-1.2.1/dn3/tools/cli.py`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3/tools/config.py` & `dn3-1.2.1/dn3/tools/config.py`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3/tools/linkerpatcher.py` & `dn3-1.2.1/dn3/tools/linkerpatcher.py`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3/tools/templategen.py` & `dn3-1.2.1/dn3/tools/templategen.py`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/dn3.egg-info/PKG-INFO` & `dn3-1.2.1/dn3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dn3
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/k1R4/deathnot3/
 Author: k1R4
 Author-email: srijiith@outlook.com
 Keywords: pwn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6, <4
```

### Comparing `dn3-1.2.0/dn3.egg-info/SOURCES.txt` & `dn3-1.2.1/dn3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dn3-1.2.0/setup.py` & `dn3-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
-from setuptools import setup, find_packages
+from setuptools import setup
 from io import open
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='dn3',
-    version='1.2.0',
+    version='1.2.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/k1R4/deathnot3/',
     author='k1R4',
     author_email='srijiith@outlook.com',
     classifiers=[
```

