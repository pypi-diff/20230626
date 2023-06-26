# Comparing `tmp/ArtByCode-0.0.2.tar.gz` & `tmp/ArtByCode-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArtByCode-0.0.2.tar", last modified: Sun Jun 25 18:53:22 2023, max compression
+gzip compressed data, was "ArtByCode-0.0.3.tar", last modified: Mon Jun 26 16:29:18 2023, max compression
```

## Comparing `ArtByCode-0.0.2.tar` & `ArtByCode-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/ArtByCode.egg-info/
--rw-rw-rw-   0        0        0     1843 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1062 2023-06-25 14:49:05.000000 ArtByCode-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1843 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/art_by_code/
--rw-rw-rw-   0        0        0        0 2023-06-25 11:27:48.000000 ArtByCode-0.0.2/art_by_code/__init__.py
--rw-rw-rw-   0        0        0     2660 2023-06-25 17:01:42.000000 ArtByCode-0.0.2/art_by_code/abc.py
--rw-rw-rw-   0        0        0       42 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2170 2023-06-25 18:33:23.000000 ArtByCode-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:29:18.484768 ArtByCode-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-26 16:29:18.484768 ArtByCode-0.0.3/ArtByCode/
+-rw-rw-rw-   0        0        0        0 2023-06-25 11:27:48.000000 ArtByCode-0.0.3/ArtByCode/__init__.py
+-rw-rw-rw-   0        0        0     2668 2023-06-26 16:28:39.000000 ArtByCode-0.0.3/ArtByCode/abc.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:29:18.484768 ArtByCode-0.0.3/ArtByCode.egg-info/
+-rw-rw-rw-   0        0        0     1843 2023-06-26 16:29:18.000000 ArtByCode-0.0.3/ArtByCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-06-26 16:29:18.000000 ArtByCode-0.0.3/ArtByCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 16:29:18.000000 ArtByCode-0.0.3/ArtByCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-26 16:29:18.000000 ArtByCode-0.0.3/ArtByCode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 16:29:18.000000 ArtByCode-0.0.3/ArtByCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1062 2023-06-25 14:49:05.000000 ArtByCode-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1843 2023-06-26 16:29:18.484768 ArtByCode-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-26 16:29:18.484768 ArtByCode-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2170 2023-06-26 16:26:44.000000 ArtByCode-0.0.3/setup.py
```

### Comparing `ArtByCode-0.0.2/ArtByCode.egg-info/PKG-INFO` & `ArtByCode-0.0.3/ArtByCode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArtByCode
-Version: 0.0.2
+Version: 0.0.3
 Summary: ArtByCode
 Author: Coder Artist
 Author-email: abc4artbycode@gmail.com
 Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ArtByCode-0.0.2/LICENSE.txt` & `ArtByCode-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ArtByCode-0.0.2/PKG-INFO` & `ArtByCode-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArtByCode
-Version: 0.0.2
+Version: 0.0.3
 Summary: ArtByCode
 Author: Coder Artist
 Author-email: abc4artbycode@gmail.com
 Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ArtByCode-0.0.2/art_by_code/abc.py` & `ArtByCode-0.0.3/ArtByCode/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import turtle as tu
 import re
 import docx
 import requests
 import io
 
-class abc():
+class subscribe():
     
     def __init__(self, name, speed = 25, bg_color = '#ffffff'):
         self.name = name
         self.speed = speed
         self.bg_color = bg_color
 
-    def draw(self):
+    def follow(self):
         
         message = '''
         
         For more updates: 
         Follow abc (art by code) on Youtube and on instagram
         Youtube   : https://www.youtube.com/@artbycode
         Instagram : https://www.instagram.com/art_by_code?r=nametag
```

### Comparing `ArtByCode-0.0.2/setup.py` & `ArtByCode-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 - If you like our content, please do like, follow & subscribe to our YouTube channel (https://www.youtube.com/@artbycode) and Instagram (https://www.instagram.com/art_by_code?r=nametag).
 - Thanks ❤
 """
 # Setting up
 setup(
     name="ArtByCode",
-    version='0.0.2',
+    version='0.0.3',
     author="Coder Artist",
     author_email="abc4artbycode@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['turtle==0.0.1', 'docx', 'python-docx','requests'],
```

