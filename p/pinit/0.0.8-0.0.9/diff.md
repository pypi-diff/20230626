# Comparing `tmp/pinit-0.0.8.tar.gz` & `tmp/pinit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinit-0.0.8.tar", max compression
+gzip compressed data, was "pinit-0.0.9.tar", max compression
```

## Comparing `pinit-0.0.8.tar` & `pinit-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      425 2023-06-03 10:35:28.564339 pinit-0.0.8/README.md
--rw-r--r--   0        0        0      323 2023-01-23 13:34:30.831156 pinit-0.0.8/pinit/.pinit/install.py
--rw-r--r--   0        0        0     7174 2023-06-12 14:50:36.568359 pinit-0.0.8/pinit/.pinit/main.py
--rwxr-xr-x   0        0        0     2210 2023-01-06 17:49:58.404041 pinit-0.0.8/pinit/.pinit/pinit.svg
--rw-r--r--   0        0        0       52 2023-03-27 12:23:42.562490 pinit-0.0.8/pinit/.pinit/requirements.txt
--rw-r--r--   0        0        0      897 2023-01-06 18:07:43.742132 pinit-0.0.8/pinit/.pinit/shortcut.py
--rw-r--r--   0        0        0    79440 2023-06-12 15:02:46.186498 pinit-0.0.8/pinit/.pinit/ui/assets/index-800b0b32.css
--rw-r--r--   0        0        0    79260 2023-06-03 10:08:22.908252 pinit-0.0.8/pinit/.pinit/ui/assets/index-88a0609b.css
--rw-r--r--   0        0        0   201367 2023-06-12 15:02:46.186498 pinit-0.0.8/pinit/.pinit/ui/assets/index-95facd96.js
--rw-r--r--   0        0        0   201367 2023-06-03 10:08:22.909252 pinit-0.0.8/pinit/.pinit/ui/assets/index-a407b3b0.js
--rw-r--r--   0        0        0   128352 2023-06-12 15:02:46.186498 pinit-0.0.8/pinit/.pinit/ui/assets/w1-8265f647.woff2
--rw-r--r--   0        0        0   155276 2023-06-12 15:02:46.183498 pinit-0.0.8/pinit/.pinit/ui/assets/w2-35dca8a7.woff2
--rwxr-xr-x   0        0        0     2210 2023-06-12 15:02:45.564473 pinit-0.0.8/pinit/.pinit/ui/icon.svg
--rw-r--r--   0        0        0      899 2023-06-12 15:02:46.187498 pinit-0.0.8/pinit/.pinit/ui/index.html
--rw-r--r--   0        0        0      255 2023-06-03 10:23:04.373699 pinit-0.0.8/pinit/.pinit/uninstall.py
--rw-r--r--   0        0        0       16 2023-01-06 18:08:51.649138 pinit-0.0.8/pinit/.pinit/upgrade.py
--rw-r--r--   0        0        0        0 2023-01-01 08:59:18.230362 pinit-0.0.8/pinit/__init__.py
--rw-r--r--   0        0        0     2194 2023-06-12 15:01:27.732246 pinit-0.0.8/pinit/main.py
--rw-r--r--   0        0        0      457 2023-06-12 15:06:04.997365 pinit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 pinit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      425 2023-06-03 10:35:28.564339 pinit-0.0.9/README.md
+-rw-r--r--   0        0        0      323 2023-01-23 13:34:30.831156 pinit-0.0.9/pinit/.pinit/install.py
+-rw-r--r--   0        0        0     7174 2023-06-12 14:50:36.568359 pinit-0.0.9/pinit/.pinit/main.py
+-rwxr-xr-x   0        0        0     2210 2023-01-06 17:49:58.404041 pinit-0.0.9/pinit/.pinit/pinit.svg
+-rw-r--r--   0        0        0       52 2023-03-27 12:23:42.562490 pinit-0.0.9/pinit/.pinit/requirements.txt
+-rw-r--r--   0        0        0      897 2023-01-06 18:07:43.742132 pinit-0.0.9/pinit/.pinit/shortcut.py
+-rw-r--r--   0        0        0    79440 2023-06-12 15:02:46.186498 pinit-0.0.9/pinit/.pinit/ui/assets/index-800b0b32.css
+-rw-r--r--   0        0        0    79260 2023-06-03 10:08:22.908252 pinit-0.0.9/pinit/.pinit/ui/assets/index-88a0609b.css
+-rw-r--r--   0        0        0    79443 2023-06-12 15:18:48.021319 pinit-0.0.9/pinit/.pinit/ui/assets/index-8ab05031.css
+-rw-r--r--   0        0        0   201367 2023-06-12 15:02:46.186498 pinit-0.0.9/pinit/.pinit/ui/assets/index-95facd96.js
+-rw-r--r--   0        0        0   201367 2023-06-03 10:08:22.909252 pinit-0.0.9/pinit/.pinit/ui/assets/index-a407b3b0.js
+-rw-r--r--   0        0        0   201367 2023-06-12 15:18:48.021319 pinit-0.0.9/pinit/.pinit/ui/assets/index-bc4d2d1e.js
+-rw-r--r--   0        0        0   128352 2023-06-12 15:18:48.017320 pinit-0.0.9/pinit/.pinit/ui/assets/w1-8265f647.woff2
+-rw-r--r--   0        0        0   155276 2023-06-12 15:18:48.021319 pinit-0.0.9/pinit/.pinit/ui/assets/w2-35dca8a7.woff2
+-rwxr-xr-x   0        0        0     2210 2023-06-12 15:18:47.263316 pinit-0.0.9/pinit/.pinit/ui/icon.svg
+-rw-r--r--   0        0        0      899 2023-06-12 15:18:48.022319 pinit-0.0.9/pinit/.pinit/ui/index.html
+-rw-r--r--   0        0        0      255 2023-06-03 10:23:04.373699 pinit-0.0.9/pinit/.pinit/uninstall.py
+-rw-r--r--   0        0        0       16 2023-01-06 18:08:51.649138 pinit-0.0.9/pinit/.pinit/upgrade.py
+-rw-r--r--   0        0        0        0 2023-01-01 08:59:18.230362 pinit-0.0.9/pinit/__init__.py
+-rw-r--r--   0        0        0     2194 2023-06-12 15:01:27.732246 pinit-0.0.9/pinit/main.py
+-rw-r--r--   0        0        0      457 2023-06-12 15:24:45.856178 pinit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 pinit-0.0.9/PKG-INFO
```

### Comparing `pinit-0.0.8/pinit/.pinit/main.py` & `pinit-0.0.9/pinit/.pinit/main.py`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/pinit.svg` & `pinit-0.0.9/pinit/.pinit/pinit.svg`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/shortcut.py` & `pinit-0.0.9/pinit/.pinit/shortcut.py`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/ui/assets/index-800b0b32.css` & `pinit-0.0.9/pinit/.pinit/ui/assets/index-800b0b32.css`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/ui/assets/index-88a0609b.css` & `pinit-0.0.9/pinit/.pinit/ui/assets/index-88a0609b.css`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/ui/assets/index-95facd96.js` & `pinit-0.0.9/pinit/.pinit/ui/assets/index-95facd96.js`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/ui/assets/index-a407b3b0.js` & `pinit-0.0.9/pinit/.pinit/ui/assets/index-a407b3b0.js`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/ui/assets/w1-8265f647.woff2` & `pinit-0.0.9/pinit/.pinit/ui/assets/w1-8265f647.woff2`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/ui/assets/w2-35dca8a7.woff2` & `pinit-0.0.9/pinit/.pinit/ui/assets/w2-35dca8a7.woff2`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/ui/icon.svg` & `pinit-0.0.9/pinit/.pinit/ui/icon.svg`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/pinit/.pinit/ui/index.html` & `pinit-0.0.9/pinit/.pinit/ui/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
     <script type="text/javascript" src="/eel.js"></script>
 
 
 
 
 
-    <script type="module" crossorigin src="/assets/index-95facd96.js"></script>
-    <link rel="stylesheet" href="/assets/index-800b0b32.css">
+    <script type="module" crossorigin src="/assets/index-bc4d2d1e.js"></script>
+    <link rel="stylesheet" href="/assets/index-8ab05031.css">
   </head>
   <body>
     <div id="app"></div>
     
   </body>
 </html>
```

### Comparing `pinit-0.0.8/pinit/main.py` & `pinit-0.0.9/pinit/main.py`

 * *Files identical despite different names*

### Comparing `pinit-0.0.8/PKG-INFO` & `pinit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinit
-Version: 0.0.8
+Version: 0.0.9
 Summary: an application for creating shortcut for apps and scripts in linux
 Home-page: https://github.com/rraammiinn/pinit.git
 License: MIT
 Author: ramin
 Author-email: ramin.kishani.farahani@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

