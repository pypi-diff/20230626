# Comparing `tmp/ArtByCode-0.0.4.tar.gz` & `tmp/ArtByCode-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArtByCode-0.0.4.tar", last modified: Mon Jun 26 16:39:05 2023, max compression
+gzip compressed data, was "ArtByCode-0.0.5.tar", last modified: Mon Jun 26 17:05:41 2023, max compression
```

## Comparing `ArtByCode-0.0.4.tar` & `ArtByCode-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:39:05.162255 ArtByCode-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-26 16:39:05.144938 ArtByCode-0.0.4/ArtByCode/
--rw-rw-rw-   0        0        0        0 2023-06-25 11:27:48.000000 ArtByCode-0.0.4/ArtByCode/__init__.py
--rw-rw-rw-   0        0        0     2668 2023-06-26 16:36:25.000000 ArtByCode-0.0.4/ArtByCode/abc.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:39:05.159505 ArtByCode-0.0.4/ArtByCode.egg-info/
--rw-rw-rw-   0        0        0     1851 2023-06-26 16:39:05.000000 ArtByCode-0.0.4/ArtByCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-06-26 16:39:05.000000 ArtByCode-0.0.4/ArtByCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:39:05.000000 ArtByCode-0.0.4/ArtByCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-26 16:39:05.000000 ArtByCode-0.0.4/ArtByCode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 16:39:05.000000 ArtByCode-0.0.4/ArtByCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1062 2023-06-25 14:49:05.000000 ArtByCode-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1851 2023-06-26 16:39:05.162255 ArtByCode-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-26 16:39:05.162255 ArtByCode-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2178 2023-06-26 16:37:31.000000 ArtByCode-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:05:41.987907 ArtByCode-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-26 17:05:41.956631 ArtByCode-0.0.5/ArtByCode/
+-rw-rw-rw-   0        0        0        0 2023-06-25 11:27:48.000000 ArtByCode-0.0.5/ArtByCode/__init__.py
+-rw-rw-rw-   0        0        0     2666 2023-06-26 17:04:31.000000 ArtByCode-0.0.5/ArtByCode/abc.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:05:41.987907 ArtByCode-0.0.5/ArtByCode.egg-info/
+-rw-rw-rw-   0        0        0     1851 2023-06-26 17:05:41.000000 ArtByCode-0.0.5/ArtByCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-06-26 17:05:41.000000 ArtByCode-0.0.5/ArtByCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 17:05:41.000000 ArtByCode-0.0.5/ArtByCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-26 17:05:41.000000 ArtByCode-0.0.5/ArtByCode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 17:05:41.000000 ArtByCode-0.0.5/ArtByCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1062 2023-06-25 14:49:05.000000 ArtByCode-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1851 2023-06-26 17:05:41.987907 ArtByCode-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-26 17:05:41.987907 ArtByCode-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2178 2023-06-26 17:05:11.000000 ArtByCode-0.0.5/setup.py
```

### Comparing `ArtByCode-0.0.4/ArtByCode/abc.py` & `ArtByCode-0.0.5/ArtByCode/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import turtle as tu
 import re
 import docx
 import requests
 import io
 
-class subscribe():
+class like():
     
     def __init__(self, name, speed = 25, bg_color = '#ffffff'):
         self.name = name
         self.speed = speed
         self.bg_color = bg_color
 
-    def follow(self):
+    def subscribe(self):
         
         message = '''
         
         For more updates: 
         Follow abc (art by code) on Youtube and on instagram
         Youtube   : https://www.youtube.com/@artbycode
         Instagram : https://www.instagram.com/art_by_code?r=nametag
```

### Comparing `ArtByCode-0.0.4/ArtByCode.egg-info/PKG-INFO` & `ArtByCode-0.0.5/ArtByCode.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArtByCode
-Version: 0.0.4
+Version: 0.0.5
 Summary: ArtByCode
 Author: Coder Artist
 Author-email: abc4artbycode@gmail.com
 Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -30,17 +30,17 @@
 
 
 ### Example
 
 ```
     from ArtByCode import abc
 
-    like = 'lord_ganesh'
+    share = 'lord_ganesh'
 
-    abc.subscribe(like).follow()
+    abc.like(share).subscribe()
 ```
 
 ### OUTPUT
 <div align = "center">
    <img src = "https://github.com/Art-by-Code/Coordinates/assets/114793988/2addc356-8db9-4404-b0ad-2ce0755c3511">
 </div>
```

### Comparing `ArtByCode-0.0.4/LICENSE.txt` & `ArtByCode-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ArtByCode-0.0.4/PKG-INFO` & `ArtByCode-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArtByCode
-Version: 0.0.4
+Version: 0.0.5
 Summary: ArtByCode
 Author: Coder Artist
 Author-email: abc4artbycode@gmail.com
 Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -30,17 +30,17 @@
 
 
 ### Example
 
 ```
     from ArtByCode import abc
 
-    like = 'lord_ganesh'
+    share = 'lord_ganesh'
 
-    abc.subscribe(like).follow()
+    abc.like(share).subscribe()
 ```
 
 ### OUTPUT
 <div align = "center">
    <img src = "https://github.com/Art-by-Code/Coordinates/assets/114793988/2addc356-8db9-4404-b0ad-2ce0755c3511">
 </div>
```

### Comparing `ArtByCode-0.0.4/setup.py` & `ArtByCode-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 
 ### Example
 
 ```
     from ArtByCode import abc
 
-    like = 'lord_ganesh'
+    share = 'lord_ganesh'
 
-    abc.subscribe(like).follow()
+    abc.like(share).subscribe()
 ```
 
 ### OUTPUT
 <div align = "center">
    <img src = "https://github.com/Art-by-Code/Coordinates/assets/114793988/2addc356-8db9-4404-b0ad-2ce0755c3511">
 </div>
 
@@ -55,15 +55,15 @@
 
 - If you like our content, please do like, follow & subscribe to our YouTube channel (https://www.youtube.com/@artbycode) and Instagram (https://www.instagram.com/art_by_code?r=nametag).
 - Thanks ❤
 """
 # Setting up
 setup(
     name="ArtByCode",
-    version='0.0.4',
+    version='0.0.5',
     author="Coder Artist",
     author_email="abc4artbycode@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['turtle==0.0.1', 'docx', 'python-docx','requests'],
```

