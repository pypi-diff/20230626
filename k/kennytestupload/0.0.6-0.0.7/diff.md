# Comparing `tmp/kennytestupload-0.0.6.tar.gz` & `tmp/kennytestupload-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kennytestupload-0.0.6.tar", last modified: Mon Jun 26 21:01:42 2023, max compression
+gzip compressed data, was "dist/kennytestupload-0.0.7.tar", last modified: Mon Jun 26 21:38:41 2023, max compression
```

## Comparing `kennytestupload-0.0.6.tar` & `kennytestupload-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:01:42.990807 kennytestupload-0.0.6/
--rw-r--r--   0 kenny      (501) staff       (20)      385 2023-06-26 21:01:42.990619 kennytestupload-0.0.6/PKG-INFO
--rw-r--r--   0 kenny      (501) staff       (20)       22 2023-06-26 19:38:53.000000 kennytestupload-0.0.6/README
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:01:42.989622 kennytestupload-0.0.6/kennytestupload/
--rw-r--r--   0 kenny      (501) staff       (20)      582 2023-06-12 20:55:20.000000 kennytestupload-0.0.6/kennytestupload/BasicDemo.py
--rw-r--r--   0 kenny      (501) staff       (20)     1543 2023-06-12 21:21:01.000000 kennytestupload-0.0.6/kennytestupload/ClassUsage.py
--rw-r--r--   0 kenny      (501) staff       (20)     1895 2023-06-20 00:05:55.000000 kennytestupload-0.0.6/kennytestupload/Collision.py
--rw-r--r--   0 kenny      (501) staff       (20)      989 2023-06-12 23:31:16.000000 kennytestupload-0.0.6/kennytestupload/Features.py
--rw-r--r--   0 kenny      (501) staff       (20)    11451 2023-06-26 19:31:00.000000 kennytestupload-0.0.6/kennytestupload/Main.py
--rw-r--r--   0 kenny      (501) staff       (20)     3018 2023-06-26 20:29:08.000000 kennytestupload-0.0.6/kennytestupload/SpaceInvader.py
--rw-r--r--   0 kenny      (501) staff       (20)     1613 2023-06-13 00:24:31.000000 kennytestupload-0.0.6/kennytestupload/Tets.py
--rw-r--r--   0 kenny      (501) staff       (20)      131 2023-06-26 20:29:08.000000 kennytestupload-0.0.6/kennytestupload/__init__.py
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:01:42.990285 kennytestupload-0.0.6/kennytestupload.egg-info/
--rw-r--r--   0 kenny      (501) staff       (20)      385 2023-06-26 21:01:42.000000 kennytestupload-0.0.6/kennytestupload.egg-info/PKG-INFO
--rw-r--r--   0 kenny      (501) staff       (20)      395 2023-06-26 21:01:42.000000 kennytestupload-0.0.6/kennytestupload.egg-info/SOURCES.txt
--rw-r--r--   0 kenny      (501) staff       (20)        1 2023-06-26 21:01:42.000000 kennytestupload-0.0.6/kennytestupload.egg-info/dependency_links.txt
--rw-r--r--   0 kenny      (501) staff       (20)       16 2023-06-26 21:01:42.000000 kennytestupload-0.0.6/kennytestupload.egg-info/top_level.txt
--rw-r--r--   0 kenny      (501) staff       (20)       38 2023-06-26 21:01:42.990867 kennytestupload-0.0.6/setup.cfg
--rw-r--r--   0 kenny      (501) staff       (20)      874 2023-06-26 21:01:38.000000 kennytestupload-0.0.6/setup.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:38:41.830726 kennytestupload-0.0.7/
+-rw-r--r--   0 kenny      (501) staff       (20)      348 2023-06-26 21:38:41.830529 kennytestupload-0.0.7/PKG-INFO
+-rw-r--r--   0 kenny      (501) staff       (20)       22 2023-06-26 19:38:53.000000 kennytestupload-0.0.7/README
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:38:41.829014 kennytestupload-0.0.7/kennytestupload/
+-rw-r--r--   0 kenny      (501) staff       (20)      582 2023-06-12 20:55:20.000000 kennytestupload-0.0.7/kennytestupload/BasicDemo.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1543 2023-06-12 21:21:01.000000 kennytestupload-0.0.7/kennytestupload/ClassUsage.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1895 2023-06-20 00:05:55.000000 kennytestupload-0.0.7/kennytestupload/Collision.py
+-rw-r--r--   0 kenny      (501) staff       (20)      989 2023-06-12 23:31:16.000000 kennytestupload-0.0.7/kennytestupload/Features.py
+-rw-r--r--   0 kenny      (501) staff       (20)    11451 2023-06-26 19:31:00.000000 kennytestupload-0.0.7/kennytestupload/Main.py
+-rw-r--r--   0 kenny      (501) staff       (20)     3075 2023-06-26 21:18:01.000000 kennytestupload-0.0.7/kennytestupload/SpaceInvader.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1613 2023-06-13 00:24:31.000000 kennytestupload-0.0.7/kennytestupload/Tets.py
+-rw-r--r--   0 kenny      (501) staff       (20)      131 2023-06-26 20:29:08.000000 kennytestupload-0.0.7/kennytestupload/__init__.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:38:41.830314 kennytestupload-0.0.7/kennytestupload.egg-info/
+-rw-r--r--   0 kenny      (501) staff       (20)      348 2023-06-26 21:38:41.000000 kennytestupload-0.0.7/kennytestupload.egg-info/PKG-INFO
+-rw-r--r--   0 kenny      (501) staff       (20)      395 2023-06-26 21:38:41.000000 kennytestupload-0.0.7/kennytestupload.egg-info/SOURCES.txt
+-rw-r--r--   0 kenny      (501) staff       (20)        1 2023-06-26 21:38:41.000000 kennytestupload-0.0.7/kennytestupload.egg-info/dependency_links.txt
+-rw-r--r--   0 kenny      (501) staff       (20)       16 2023-06-26 21:38:41.000000 kennytestupload-0.0.7/kennytestupload.egg-info/top_level.txt
+-rw-r--r--   0 kenny      (501) staff       (20)       38 2023-06-26 21:38:41.830792 kennytestupload-0.0.7/setup.cfg
+-rw-r--r--   0 kenny      (501) staff       (20)      874 2023-06-26 21:38:37.000000 kennytestupload-0.0.7/setup.py
```

### Comparing `kennytestupload-0.0.6/kennytestupload/BasicDemo.py` & `kennytestupload-0.0.7/kennytestupload/BasicDemo.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.6/kennytestupload/ClassUsage.py` & `kennytestupload-0.0.7/kennytestupload/ClassUsage.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.6/kennytestupload/Collision.py` & `kennytestupload-0.0.7/kennytestupload/Collision.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.6/kennytestupload/Features.py` & `kennytestupload-0.0.7/kennytestupload/Features.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.6/kennytestupload/Main.py` & `kennytestupload-0.0.7/kennytestupload/Main.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.6/kennytestupload/SpaceInvader.py` & `kennytestupload-0.0.7/kennytestupload/SpaceInvader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pygame
-
-
-
+import os
 
 #Setup game
 def Main():
     # Game Setup
     pygame.init()
     screen = pygame.display.set_mode((600, 500))
     pygame.display.set_caption('Demo')
@@ -16,15 +14,15 @@
     game_active = True
 
     # Player Class
     class Player(pygame.sprite.Sprite):
 
         def __init__(self, startLocation):
             super().__init__()
-            player_image_frame1 = pygame.image.load('kennytestupload/data/alien3.png').convert_alpha()
+            player_image_frame1 = pygame.image.load(os.path.join(os.path.dirname(__file__), 'data/alien3.png')).convert_alpha()
             player_image_frames = [player_image_frame1]
             self.image = player_image_frames[0]
             self.rect = self.image.get_rect(center=startLocation)
             self.speed = 4
 
         def player_input(self):
             keys = pygame.key.get_pressed()
@@ -41,15 +39,15 @@
             self.player_input()
 
     # Player Class
     class Enemy(pygame.sprite.Sprite):
 
         def __init__(self, startLocation):
             super().__init__()
-            enemy_image_frame1 = pygame.image.load('kennytestupload/data/enemy2.png').convert_alpha()
+            enemy_image_frame1 = pygame.image.load(os.path.join(os.path.dirname(__file__), 'data/enemy2.png')).convert_alpha()
             enemy_image_frame1 = pygame.transform.scale(enemy_image_frame1, (50, 50))
             player_image_frames = [enemy_image_frame1]
             self.image = player_image_frames[0]
             self.rect = self.image.get_rect(center=startLocation)
             self.speed = 1
             self.direction = 1
             self.move_timer = 0
```

### Comparing `kennytestupload-0.0.6/kennytestupload/Tets.py` & `kennytestupload-0.0.7/kennytestupload/Tets.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.6/setup.py` & `kennytestupload-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "kennytestupload",
-    version = "0.0.6",
+    version = "0.0.7",
     author = "Kenny C",
     author_email = "kennycheung388@yahoo.com.hk",
     description = ("An demonstration of how to upload project to pypi."),
     license = "MIT License",
     keywords = "tutorial",
     url = "",
     packages=['kennytestupload'],
```

