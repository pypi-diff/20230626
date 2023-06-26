# Comparing `tmp/showcues-1.0.5.tar.gz` & `tmp/showcues-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showcues-1.0.5.tar", last modified: Sun Jun 25 18:09:08 2023, max compression
+gzip compressed data, was "showcues-1.0.7.tar", last modified: Mon Jun 26 08:33:59 2023, max compression
```

## Comparing `showcues-1.0.5.tar` & `showcues-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-25 18:09:08.056223 showcues-1.0.5/
--rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-25 18:09:08.056223 showcues-1.0.5/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)        0 2023-06-20 17:59:12.000000 showcues-1.0.5/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-25 18:09:08.056223 showcues-1.0.5/bin/
--rwxr-xr-x   0 a         (1000) a         (1000)       86 2023-06-20 17:41:41.000000 showcues-1.0.5/bin/showcues
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-25 18:09:08.056223 showcues-1.0.5/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1096 2023-06-25 18:07:35.000000 showcues-1.0.5/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-25 18:09:08.056223 showcues-1.0.5/showcues.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-25 18:09:07.000000 showcues-1.0.5/showcues.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      202 2023-06-25 18:09:08.000000 showcues-1.0.5/showcues.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-25 18:09:07.000000 showcues-1.0.5/showcues.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       50 2023-06-25 18:09:07.000000 showcues-1.0.5/showcues.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)        9 2023-06-25 18:09:07.000000 showcues-1.0.5/showcues.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)    13940 2023-06-25 02:22:06.000000 showcues-1.0.5/showcues.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-26 08:33:59.238585 showcues-1.0.7/
+-rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-26 08:33:59.238585 showcues-1.0.7/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)        0 2023-06-20 17:59:12.000000 showcues-1.0.7/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-26 08:33:59.234585 showcues-1.0.7/bin/
+-rwxr-xr-x   0 a         (1000) a         (1000)       86 2023-06-20 17:41:41.000000 showcues-1.0.7/bin/showcues
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-26 08:33:59.238585 showcues-1.0.7/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1096 2023-06-25 18:07:35.000000 showcues-1.0.7/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-26 08:33:59.238585 showcues-1.0.7/showcues.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)      593 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      202 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       50 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)        9 2023-06-26 08:33:59.000000 showcues-1.0.7/showcues.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)    14262 2023-06-26 08:18:34.000000 showcues-1.0.7/showcues.py
```

### Comparing `showcues-1.0.5/PKG-INFO` & `showcues-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showcues
-Version: 1.0.5
+Version: 1.0.7
 Summary: showcues displays HLS CUE-IN and CUE-OUT tags with wallclock time
 Home-page: https://github.com/futzu/showcues
 Author: Adrian of Doom.
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `showcues-1.0.5/setup.py` & `showcues-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `showcues-1.0.5/showcues.egg-info/PKG-INFO` & `showcues-1.0.7/showcues.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showcues
-Version: 1.0.5
+Version: 1.0.7
 Summary: showcues displays HLS CUE-IN and CUE-OUT tags with wallclock time
 Home-page: https://github.com/futzu/showcues
 Author: Adrian of Doom.
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `showcues-1.0.5/showcues.py` & `showcues-1.0.7/showcues.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                 return line
             if cue.startswith("#EXT-X-CUE-OUT"):
                 self.break_timer == 0.0
                 try:
                     self.break_duration = atoif(line.split(":")[1])
                 finally:
                     self.cue_state = "OUT"
-                print(f"{iso8601()} {cue_stuff}{media_stuff}")
+                print(f"{iso8601()} {cue_stuff} {REV}Duration:{NORM} {self.break_duration} {media_stuff}")
                 return line
         cue2 = self.six2five(cue)
         cue2data = Cue(cue2)
         cue2data.decode()
         line = line.replace(cue, cue2)
         return line
 
@@ -239,15 +239,15 @@
         if self.cue_state is None:
             self.reset_break()
             self.cue_state = "OUT"
             if self.break_timer is None:
                 self.break_timer = 0.0
             if ":" in line:
                 self.break_duration = atoif(line.split(":")[1])
-                print("set duration to ", self.break_duration)
+               # print("Duration:", self.break_duration)
             return self.add_cue(line, line)
         return "## " + line
 
     def chk_x_scte35(self, tags, line):
         if "CUE" in tags["#EXT-X-SCTE35"]:
             return self.add_cue(tags["#EXT-X-SCTE35"]["CUE"], line)
         return line
@@ -348,15 +348,15 @@
 
     def mk_window_size(self, lines):
         if not self.window_size:
             self.window_size = len(
                 [line for line in lines if line.startswith("#EXTINF:")]
             )
             self.sliding_window.size = self.window_size
-            print(f"window_size:{self.window_size}")
+            print(f"{REV}Window_size:{NORM} {self.window_size}\n")
 
     def update_cue_state(self):
         if self.cue_state == "OUT":
             self.cue_state = "CONT"
         if self.cue_state == "IN":
             self.cue_state = None
 
@@ -377,15 +377,16 @@
         splitline = line.split(":", 1)
         if splitline[0] in HEADER_TAGS:
             self.headers.append(line)
             return True
         return False
 
     def pull(self, manifest):
-        print("started")
+        print(f"{REV}Started{NORM}\n")
+        print(f"\n{REV}variant m3u8:{NORM} {manifest}\n")
         self.base_uri = manifest.rsplit("/", 1)[0]
         self.sliding_window = SlidingWindow()
         while self.reload:
             lines = []
             self.headers = []
             with reader(manifest) as m3u8:
                 m3u8_lines = self.decode_lines(m3u8.readlines())
@@ -410,25 +411,31 @@
             ##                out.write("".join(self.headers))
             ##                out.write(self.sliding_window.all_panes())
             self.update_cue_state()
             time.sleep(self.sleep_duration)
 
 
 def cli():
-    fu = M3uFu()
-    fu.m3u8 = sys.argv[1]
-    fu.decode()
+    playlists=None
     m3u8 = None
-    playlists = [
-        segment for segment in fu.segments if "#EXT-X-STREAM-INF" in segment.tags
-    ]
+    with reader(sys.argv[1]) as arg:
+        variants = [line for line in arg if b"#EXT-X-STREAM-INF" in line]
+        if variants:
+            fu = M3uFu()
+            reload =False
+            fu.m3u8 = sys.argv[1]
+            fu.decode()
+            playlists = [
+                segment for segment in fu.segments if "#EXT-X-STREAM-INF" in segment.tags
+            ]
     if playlists:
         m3u8 = playlists[0].media
     else:
         m3u8 = sys.argv[1]
     cp = CuePuller()
-    print(f"m3u8: {m3u8}\n")
     cp.pull(m3u8)
 
 
+
+
 if __name__ == "__main__":
     cli()
```

