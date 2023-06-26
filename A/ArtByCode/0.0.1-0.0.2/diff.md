# Comparing `tmp/ArtByCode-0.0.1.tar.gz` & `tmp/ArtByCode-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArtByCode-0.0.1.tar", last modified: Sun Jun 25 15:08:54 2023, max compression
+gzip compressed data, was "ArtByCode-0.0.2.tar", last modified: Sun Jun 25 18:53:22 2023, max compression
```

## Comparing `ArtByCode-0.0.1.tar` & `ArtByCode-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 15:08:54.875625 ArtByCode-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-25 15:08:54.871600 ArtByCode-0.0.1/ArtByCode.egg-info/
--rw-rw-rw-   0        0        0     1802 2023-06-25 15:08:54.000000 ArtByCode-0.0.1/ArtByCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-25 15:08:54.000000 ArtByCode-0.0.1/ArtByCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 15:08:54.000000 ArtByCode-0.0.1/ArtByCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-06-25 15:08:54.000000 ArtByCode-0.0.1/ArtByCode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-25 15:08:54.000000 ArtByCode-0.0.1/ArtByCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1062 2023-06-25 14:49:05.000000 ArtByCode-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1802 2023-06-25 15:08:54.875625 ArtByCode-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 15:08:54.873614 ArtByCode-0.0.1/art_by_code/
--rw-rw-rw-   0        0        0        0 2023-06-25 11:27:48.000000 ArtByCode-0.0.1/art_by_code/__init__.py
--rw-rw-rw-   0        0        0     2660 2023-06-25 11:43:38.000000 ArtByCode-0.0.1/art_by_code/abc.py
--rw-rw-rw-   0        0        0       42 2023-06-25 15:08:54.875625 ArtByCode-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2145 2023-06-25 15:08:30.000000 ArtByCode-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/ArtByCode.egg-info/
+-rw-rw-rw-   0        0        0     1843 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-25 18:53:21.000000 ArtByCode-0.0.2/ArtByCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1062 2023-06-25 14:49:05.000000 ArtByCode-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1843 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/art_by_code/
+-rw-rw-rw-   0        0        0        0 2023-06-25 11:27:48.000000 ArtByCode-0.0.2/art_by_code/__init__.py
+-rw-rw-rw-   0        0        0     2660 2023-06-25 17:01:42.000000 ArtByCode-0.0.2/art_by_code/abc.py
+-rw-rw-rw-   0        0        0       42 2023-06-25 18:53:22.025702 ArtByCode-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2170 2023-06-25 18:33:23.000000 ArtByCode-0.0.2/setup.py
```

### Comparing `ArtByCode-0.0.1/ArtByCode.egg-info/PKG-INFO` & `ArtByCode-0.0.2/ArtByCode.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArtByCode
-Version: 0.0.1
+Version: 0.0.2
 Summary: ArtByCode
 Author: Coder Artist
 Author-email: abc4artbycode@gmail.com
 Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -12,31 +12,31 @@
 License-File: LICENSE.txt
 
 
 # Welcome to ArtByCode Family
 
 ## Description
 
-This is the beginning level python project to do some awesome drawing animation using the `turtle` module, hope it grows in the future
+This is a beginner-level Python project, in this project we utilizes the Turtle graphics library to draw images using the coordinates derived form an external docx file.
 
 ### Usage
 
 - Just install the package `pip install ArtByCode`
 - Import it to you project `import ArtByCode` 
-- Now you are good to enjoy our arts in our gallery
+- Now you are good to enjoy our artworks in our gallery
 
 ### Built with
 
 - Turtle 
 
 
 ### Example
 
 ```
-    from ArtByCode import draw
+    from ArtByCode import abc
     
     name = 'lord_ganesh'
 
     abc(name).draw()
 ```
 
 ### OUTPUT
@@ -44,24 +44,24 @@
    <img src = "https://github.com/Art-by-Code/Coordinates/assets/114793988/2addc356-8db9-4404-b0ad-2ce0755c3511">
 </div>
 
 
 
 ### Troubleshooting
 
-- If you find any problem, you can contact me on either [insta](https://www.instagram.com/art_by_code?r=nametag)
+- If you find any problem, you can contact me on [Instagram](https://www.instagram.com/art_by_code?r=nametag)
 - You can also find more of my artworks on my youtube channel(https://www.youtube.com/@artbycode)
 
 
 ### Acknowledgements
 
 Thanks to all my followers & friends.❤
 
 ### See also
 
-- [Youtube Videos](https://www.youtube.com/@artbycode)
-- [My insta ID](https://www.instagram.com/art_by_code?r=nametag)
+- [Please visit my Youtube](https://www.youtube.com/@artbycode)
+- [Please visit my Instagram](https://www.instagram.com/art_by_code?r=nametag)
 
 ### Consider supporting me
 
-- Just a simple like, follow & subscribe to our YouTube channel (https://www.youtube.com/@artbycode) and Instagram (https://www.instagram.com/art_by_code?r=nametag) fills our hearts with you warm welcome
+- If you like our content, please do like, follow & subscribe to our YouTube channel (https://www.youtube.com/@artbycode) and Instagram (https://www.instagram.com/art_by_code?r=nametag).
 - Thanks ❤
```

### Comparing `ArtByCode-0.0.1/LICENSE.txt` & `ArtByCode-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ArtByCode-0.0.1/PKG-INFO` & `ArtByCode-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArtByCode
-Version: 0.0.1
+Version: 0.0.2
 Summary: ArtByCode
 Author: Coder Artist
 Author-email: abc4artbycode@gmail.com
 Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -12,31 +12,31 @@
 License-File: LICENSE.txt
 
 
 # Welcome to ArtByCode Family
 
 ## Description
 
-This is the beginning level python project to do some awesome drawing animation using the `turtle` module, hope it grows in the future
+This is a beginner-level Python project, in this project we utilizes the Turtle graphics library to draw images using the coordinates derived form an external docx file.
 
 ### Usage
 
 - Just install the package `pip install ArtByCode`
 - Import it to you project `import ArtByCode` 
-- Now you are good to enjoy our arts in our gallery
+- Now you are good to enjoy our artworks in our gallery
 
 ### Built with
 
 - Turtle 
 
 
 ### Example
 
 ```
-    from ArtByCode import draw
+    from ArtByCode import abc
     
     name = 'lord_ganesh'
 
     abc(name).draw()
 ```
 
 ### OUTPUT
@@ -44,24 +44,24 @@
    <img src = "https://github.com/Art-by-Code/Coordinates/assets/114793988/2addc356-8db9-4404-b0ad-2ce0755c3511">
 </div>
 
 
 
 ### Troubleshooting
 
-- If you find any problem, you can contact me on either [insta](https://www.instagram.com/art_by_code?r=nametag)
+- If you find any problem, you can contact me on [Instagram](https://www.instagram.com/art_by_code?r=nametag)
 - You can also find more of my artworks on my youtube channel(https://www.youtube.com/@artbycode)
 
 
 ### Acknowledgements
 
 Thanks to all my followers & friends.❤
 
 ### See also
 
-- [Youtube Videos](https://www.youtube.com/@artbycode)
-- [My insta ID](https://www.instagram.com/art_by_code?r=nametag)
+- [Please visit my Youtube](https://www.youtube.com/@artbycode)
+- [Please visit my Instagram](https://www.instagram.com/art_by_code?r=nametag)
 
 ### Consider supporting me
 
-- Just a simple like, follow & subscribe to our YouTube channel (https://www.youtube.com/@artbycode) and Instagram (https://www.instagram.com/art_by_code?r=nametag) fills our hearts with you warm welcome
+- If you like our content, please do like, follow & subscribe to our YouTube channel (https://www.youtube.com/@artbycode) and Instagram (https://www.instagram.com/art_by_code?r=nametag).
 - Thanks ❤
```

### Comparing `ArtByCode-0.0.1/art_by_code/abc.py` & `ArtByCode-0.0.2/art_by_code/abc.py`

 * *Files identical despite different names*

