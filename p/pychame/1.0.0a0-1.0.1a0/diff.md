# Comparing `tmp/pychame-1.0.0a0.tar.gz` & `tmp/pychame-1.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychame-1.0.0a0.tar", last modified: Mon Jun 26 16:15:02 2023, max compression
+gzip compressed data, was "pychame-1.0.1a0.tar", last modified: Mon Jun 26 17:08:38 2023, max compression
```

## Comparing `pychame-1.0.0a0.tar` & `pychame-1.0.1a0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 16:15:02.891197 pychame-1.0.0a0/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1070 2023-06-26 16:01:24.000000 pychame-1.0.0a0/LICENCE.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       71 2023-06-26 16:14:38.000000 pychame-1.0.0a0/MANIFEST.in
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4424 2023-06-26 16:15:02.892197 pychame-1.0.0a0/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)     2996 2023-06-26 16:12:23.000000 pychame-1.0.0a0/README.md
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 16:15:02.873197 pychame-1.0.0a0/keys/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1310 2023-06-25 14:22:25.000000 pychame-1.0.0a0/keys/cert.pem
--rw-------   0 lucas     (1000) lucas     (1000)     1679 2023-06-25 14:21:52.000000 pychame-1.0.0a0/keys/key.pem
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 16:15:02.875197 pychame-1.0.0a0/page/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3078 2023-06-26 03:38:24.000000 pychame-1.0.0a0/page/index.html
--rw-r--r--   0 lucas     (1000) lucas     (1000)       78 2023-06-26 16:15:02.894197 pychame-1.0.0a0/setup.cfg
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1172 2023-06-26 16:12:09.000000 pychame-1.0.0a0/setup.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 16:15:02.837197 pychame-1.0.0a0/src/
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 16:15:02.891197 pychame-1.0.0a0/src/pychame.egg-info/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4424 2023-06-26 16:15:02.000000 pychame-1.0.0a0/src/pychame.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)      269 2023-06-26 16:15:02.000000 pychame-1.0.0a0/src/pychame.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)        1 2023-06-26 16:15:02.000000 pychame-1.0.0a0/src/pychame.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       26 2023-06-26 16:15:02.000000 pychame-1.0.0a0/src/pychame.egg-info/requires.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)        1 2023-06-26 16:15:02.000000 pychame-1.0.0a0/src/pychame.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 17:08:38.696226 pychame-1.0.1a0/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1070 2023-06-26 16:01:24.000000 pychame-1.0.1a0/LICENCE.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       71 2023-06-26 16:14:38.000000 pychame-1.0.1a0/MANIFEST.in
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     4384 2023-06-26 17:08:38.698227 pychame-1.0.1a0/PKG-INFO
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     2972 2023-06-26 16:54:57.000000 pychame-1.0.1a0/README.md
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 17:08:38.667227 pychame-1.0.1a0/keys/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1310 2023-06-25 14:22:25.000000 pychame-1.0.1a0/keys/cert.pem
+-rw-------   0 lucas     (1000) lucas     (1000)     1679 2023-06-25 14:21:52.000000 pychame-1.0.1a0/keys/key.pem
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 17:08:38.673226 pychame-1.0.1a0/page/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     3078 2023-06-26 03:38:24.000000 pychame-1.0.1a0/page/index.html
+-rw-r--r--   0 lucas     (1000) lucas     (1000)      697 2023-06-26 17:08:28.000000 pychame-1.0.1a0/pyproject.toml
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       78 2023-06-26 17:08:38.703227 pychame-1.0.1a0/setup.cfg
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1172 2023-06-26 17:08:22.000000 pychame-1.0.1a0/setup.py
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 17:08:38.644227 pychame-1.0.1a0/src/
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 17:08:38.680227 pychame-1.0.1a0/src/pychame/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     2275 2023-06-26 16:13:02.000000 pychame-1.0.1a0/src/pychame/__init__.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     2275 2023-06-26 17:07:44.000000 pychame-1.0.1a0/src/pychame/pychame.py
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-26 17:08:38.695227 pychame-1.0.1a0/src/pychame.egg-info/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     4384 2023-06-26 17:08:38.000000 pychame-1.0.1a0/src/pychame.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1000) lucas     (1000)      331 2023-06-26 17:08:38.000000 pychame-1.0.1a0/src/pychame.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)        1 2023-06-26 17:08:38.000000 pychame-1.0.1a0/src/pychame.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       26 2023-06-26 17:08:38.000000 pychame-1.0.1a0/src/pychame.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)        8 2023-06-26 17:08:38.000000 pychame-1.0.1a0/src/pychame.egg-info/top_level.txt
```

### Comparing `pychame-1.0.0a0/LICENCE.txt` & `pychame-1.0.1a0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pychame-1.0.0a0/PKG-INFO` & `pychame-1.0.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychame
-Version: 1.0.0a0
+Version: 1.0.1a0
 Summary: A simple way to use the ChromeBook integred camera to OpenCV
 Home-page: https://github.com/LucasOliveiraaa/Pychame
 Author: Lucas Barros
 Author-email: lucas.barros1804@gmail.com
 License: MIT
 Description: # Pychame
         
@@ -82,16 +82,14 @@
         
                 cv2.imshow("Camera Frame", frame)
         
         
                 if cv2.waitKey(1) & 0xFF == ord('q'):
                     break
         
-                cv2.waitKey(1)
-        
             video.Release()
             cv2.destroyAllWindows()
         ```
         
         ## Limitations
         
         1. Pychame is specifically designed for Chromebooks and may not work with other operating systems or devices.
```

### Comparing `pychame-1.0.0a0/README.md` & `pychame-1.0.1a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,14 @@
 
         cv2.imshow("Camera Frame", frame)
 
 
         if cv2.waitKey(1) & 0xFF == ord('q'):
             break
 
-        cv2.waitKey(1)
-
     video.Release()
     cv2.destroyAllWindows()
 ```
 
 ## Limitations
 
 1. Pychame is specifically designed for Chromebooks and may not work with other operating systems or devices.
```

### Comparing `pychame-1.0.0a0/keys/cert.pem` & `pychame-1.0.1a0/keys/cert.pem`

 * *Files identical despite different names*

### Comparing `pychame-1.0.0a0/keys/key.pem` & `pychame-1.0.1a0/keys/key.pem`

 * *Files identical despite different names*

### Comparing `pychame-1.0.0a0/page/index.html` & `pychame-1.0.1a0/page/index.html`

 * *Files identical despite different names*

### Comparing `pychame-1.0.0a0/setup.py` & `pychame-1.0.1a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent.resolve()
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='pychame',
-    version='1.0.0a',
+    version='1.0.1a',
     description='A simple way to use the ChromeBook integred camera to OpenCV',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Lucas Barros',
     author_email='lucas.barros1804@gmail.com',
     url="https://github.com/LucasOliveiraaa/Pychame",
     license="MIT",
```

### Comparing `pychame-1.0.0a0/src/pychame.egg-info/PKG-INFO` & `pychame-1.0.1a0/src/pychame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychame
-Version: 1.0.0a0
+Version: 1.0.1a0
 Summary: A simple way to use the ChromeBook integred camera to OpenCV
 Home-page: https://github.com/LucasOliveiraaa/Pychame
 Author: Lucas Barros
 Author-email: lucas.barros1804@gmail.com
 License: MIT
 Description: # Pychame
         
@@ -82,16 +82,14 @@
         
                 cv2.imshow("Camera Frame", frame)
         
         
                 if cv2.waitKey(1) & 0xFF == ord('q'):
                     break
         
-                cv2.waitKey(1)
-        
             video.Release()
             cv2.destroyAllWindows()
         ```
         
         ## Limitations
         
         1. Pychame is specifically designed for Chromebooks and may not work with other operating systems or devices.
```

