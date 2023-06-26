# Comparing `tmp/GameWidgets-0.1.6.tar.gz` & `tmp/GameWidgets-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWidgets-0.1.6.tar", last modified: Mon Jun 26 00:07:58 2023, max compression
+gzip compressed data, was "GameWidgets-0.1.7.tar", last modified: Mon Jun 26 18:44:21 2023, max compression
```

## Comparing `GameWidgets-0.1.6.tar` & `GameWidgets-0.1.7.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.433323 GameWidgets-0.1.6/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.413323 GameWidgets-0.1.6/GameWidgets/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.417322 GameWidgets-0.1.6/GameWidgets/Engine/
--rw-------   0 runner    (1000) runner    (1000)     1011 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/Engine/Backdrop.py
--rw-------   0 runner    (1000) runner    (1000)      602 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/Engine/Entity.py
--rw-------   0 runner    (1000) runner    (1000)     1041 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/Engine/Group.py
--rw-------   0 runner    (1000) runner    (1000)      122 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/Engine/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.417322 GameWidgets-0.1.6/GameWidgets/Examples/
--rw-------   0 runner    (1000) runner    (1000)     1766 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/Examples/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.421322 GameWidgets-0.1.6/GameWidgets/GameWidgets/
--rw-------   0 runner    (1000) runner    (1000)     1422 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/Animatrix.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.421322 GameWidgets-0.1.6/GameWidgets/GameWidgets/Controller/
--rw-------   0 runner    (1000) runner    (1000)     1497 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/Controller/Button.py
--rw-------   0 runner    (1000) runner    (1000)     1404 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/Controller/Joystick.py
--rw-------   0 runner    (1000) runner    (1000)       13 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/Controller/R1_R2.py
--rw-------   0 runner    (1000) runner    (1000)      148 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/Controller/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      735 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/Draw.py
--rw-------   0 runner    (1000) runner    (1000)      652 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/ScreenSlide.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.421322 GameWidgets-0.1.6/GameWidgets/GameWidgets/TileMaps/
--rw-------   0 runner    (1000) runner    (1000)      424 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/TileMaps/Sprite.py
--rw-------   0 runner    (1000) runner    (1000)      703 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/TileMaps/Tile.py
--rw-------   0 runner    (1000) runner    (1000)      124 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/TileMaps/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      121 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/GameWidgets/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.425323 GameWidgets-0.1.6/GameWidgets/RuntimeTests/
--rw-------   0 runner    (1000) runner    (1000)      649 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/RuntimeTests/AllTest.py
--rw-------   0 runner    (1000) runner    (1000)      397 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/RuntimeTests/GameWidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)      359 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/RuntimeTests/SetUpTest.py
--rw-------   0 runner    (1000) runner    (1000)      369 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/RuntimeTests/WidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/RuntimeTests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.425323 GameWidgets-0.1.6/GameWidgets/SetUp/
--rw-------   0 runner    (1000) runner    (1000)     1689 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/SetUp/ScreenCommands.py
--rw-------   0 runner    (1000) runner    (1000)      109 2023-06-26 00:02:07.000000 GameWidgets-0.1.6/GameWidgets/SetUp/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.429323 GameWidgets-0.1.6/GameWidgets/Widgets/
--rw-------   0 runner    (1000) runner    (1000)     3691 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/Btn.py
--rw-------   0 runner    (1000) runner    (1000)      597 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/Clock.py
--rw-------   0 runner    (1000) runner    (1000)     3643 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/Colors.py
--rw-------   0 runner    (1000) runner    (1000)     1489 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/Cursor.py
--rw-------   0 runner    (1000) runner    (1000)     2761 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/DialogeBox.py
--rw-------   0 runner    (1000) runner    (1000)     1574 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/ImgDecoder.py
--rw-------   0 runner    (1000) runner    (1000)      246 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/Sound.py
--rw-------   0 runner    (1000) runner    (1000)     1914 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/TextInp.py
--rw-------   0 runner    (1000) runner    (1000)     1380 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/ToggleBtn.py
--rw-------   0 runner    (1000) runner    (1000)      159 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/Widgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      620 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      567 2023-06-26 00:02:06.000000 GameWidgets-0.1.6/GameWidgets/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 00:07:58.417322 GameWidgets-0.1.6/GameWidgets.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      732 2023-06-26 00:07:57.000000 GameWidgets-0.1.6/GameWidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1467 2023-06-26 00:07:58.000000 GameWidgets-0.1.6/GameWidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-26 00:07:57.000000 GameWidgets-0.1.6/GameWidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-06-26 00:07:57.000000 GameWidgets-0.1.6/GameWidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-06-26 00:07:57.000000 GameWidgets-0.1.6/GameWidgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      732 2023-06-26 00:07:58.429323 GameWidgets-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-26 00:07:58.433323 GameWidgets-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.623480 GameWidgets-0.1.7/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.611480 GameWidgets-0.1.7/GameWidgets/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.611480 GameWidgets-0.1.7/GameWidgets/Assets/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Assets/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.611480 GameWidgets-0.1.7/GameWidgets/Engine/
+-rw-------   0 runner    (1000) runner    (1000)     1011 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Engine/Backdrop.py
+-rw-------   0 runner    (1000) runner    (1000)      602 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Engine/Entity.py
+-rw-------   0 runner    (1000) runner    (1000)     1041 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Engine/Group.py
+-rw-------   0 runner    (1000) runner    (1000)      122 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Engine/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.615480 GameWidgets-0.1.7/GameWidgets/Examples/
+-rw-------   0 runner    (1000) runner    (1000)     1766 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Examples/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.615480 GameWidgets-0.1.7/GameWidgets/GameWidgets/
+-rw-------   0 runner    (1000) runner    (1000)     1422 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Animatrix.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.615480 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/
+-rw-------   0 runner    (1000) runner    (1000)     1497 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/Button.py
+-rw-------   0 runner    (1000) runner    (1000)     1404 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/Joystick.py
+-rw-------   0 runner    (1000) runner    (1000)       13 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/R1_R2.py
+-rw-------   0 runner    (1000) runner    (1000)      148 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/Draw.py
+-rw-------   0 runner    (1000) runner    (1000)      652 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/ScreenSlide.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.615480 GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/
+-rw-------   0 runner    (1000) runner    (1000)      424 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/Sprite.py
+-rw-------   0 runner    (1000) runner    (1000)      703 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/Tile.py
+-rw-------   0 runner    (1000) runner    (1000)      124 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      121 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/GameWidgets/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.619480 GameWidgets-0.1.7/GameWidgets/RuntimeTests/
+-rw-------   0 runner    (1000) runner    (1000)      649 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/AllTest.py
+-rw-------   0 runner    (1000) runner    (1000)      397 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/GameWidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)      359 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/SetUpTest.py
+-rw-------   0 runner    (1000) runner    (1000)      369 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/WidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/RuntimeTests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.619480 GameWidgets-0.1.7/GameWidgets/SetUp/
+-rw-------   0 runner    (1000) runner    (1000)     1689 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/SetUp/ScreenCommands.py
+-rw-------   0 runner    (1000) runner    (1000)      109 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/SetUp/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.619480 GameWidgets-0.1.7/GameWidgets/Widgets/
+-rw-------   0 runner    (1000) runner    (1000)     3691 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Btn.py
+-rw-------   0 runner    (1000) runner    (1000)      597 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Clock.py
+-rw-------   0 runner    (1000) runner    (1000)     3643 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Colors.py
+-rw-------   0 runner    (1000) runner    (1000)     1489 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Cursor.py
+-rw-------   0 runner    (1000) runner    (1000)     2761 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/DialogeBox.py
+-rw-------   0 runner    (1000) runner    (1000)     1574 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/ImgDecoder.py
+-rw-------   0 runner    (1000) runner    (1000)      246 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/Sound.py
+-rw-------   0 runner    (1000) runner    (1000)     1914 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/TextInp.py
+-rw-------   0 runner    (1000) runner    (1000)     2801 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/ToggleBtn.py
+-rw-------   0 runner    (1000) runner    (1000)      159 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/Widgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      620 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      567 2023-06-26 18:43:15.000000 GameWidgets-0.1.7/GameWidgets/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 18:44:21.611480 GameWidgets-0.1.7/GameWidgets.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      732 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1498 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-06-26 18:44:21.000000 GameWidgets-0.1.7/GameWidgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      732 2023-06-26 18:44:21.623480 GameWidgets-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-26 18:44:21.623480 GameWidgets-0.1.7/setup.cfg
```

### Comparing `GameWidgets-0.1.6/GameWidgets/Engine/Backdrop.py` & `GameWidgets-0.1.7/GameWidgets/Engine/Backdrop.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Engine/Entity.py` & `GameWidgets-0.1.7/GameWidgets/Engine/Entity.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Engine/Group.py` & `GameWidgets-0.1.7/GameWidgets/Engine/Group.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py` & `GameWidgets-0.1.7/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/GameWidgets/Animatrix.py` & `GameWidgets-0.1.7/GameWidgets/GameWidgets/Animatrix.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/GameWidgets/Controller/Button.py` & `GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/Button.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/GameWidgets/Controller/Joystick.py` & `GameWidgets-0.1.7/GameWidgets/GameWidgets/Controller/Joystick.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/GameWidgets/Draw.py` & `GameWidgets-0.1.7/GameWidgets/GameWidgets/Draw.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/GameWidgets/ScreenSlide.py` & `GameWidgets-0.1.7/GameWidgets/GameWidgets/ScreenSlide.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/GameWidgets/TileMaps/Tile.py` & `GameWidgets-0.1.7/GameWidgets/GameWidgets/TileMaps/Tile.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/RuntimeTests/AllTest.py` & `GameWidgets-0.1.7/GameWidgets/RuntimeTests/AllTest.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/SetUp/ScreenCommands.py` & `GameWidgets-0.1.7/GameWidgets/SetUp/ScreenCommands.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Widgets/Btn.py` & `GameWidgets-0.1.7/GameWidgets/Widgets/Btn.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Widgets/Clock.py` & `GameWidgets-0.1.7/GameWidgets/Widgets/Clock.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Widgets/Colors.py` & `GameWidgets-0.1.7/GameWidgets/Widgets/Colors.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Widgets/Cursor.py` & `GameWidgets-0.1.7/GameWidgets/Widgets/Cursor.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Widgets/DialogeBox.py` & `GameWidgets-0.1.7/GameWidgets/Widgets/DialogeBox.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Widgets/ImgDecoder.py` & `GameWidgets-0.1.7/GameWidgets/Widgets/ImgDecoder.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/Widgets/TextInp.py` & `GameWidgets-0.1.7/GameWidgets/Widgets/TextInp.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/__init__.py` & `GameWidgets-0.1.7/GameWidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.6/GameWidgets/setup.py` & `GameWidgets-0.1.7/GameWidgets/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
   
 with open("GameWidgets/README.md", "r") as fh:
     description = fh.read()
   
 setup(
     name="GameWidgets",
-    version="0.1.6",
+    version="0.1.7",
     author="Manomay tyagi",
     author_email="tyagimanomay57@gmail.com",
     description="Make Game Easier with pygame and GameWidgets",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/SuperGuy123456/GameWidgets",
     license='MIT',
```

### Comparing `GameWidgets-0.1.6/GameWidgets.egg-info/PKG-INFO` & `GameWidgets-0.1.7/GameWidgets.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWidgets
-Version: 0.1.6
+Version: 0.1.7
 Summary: Make Game Easier with pygame and GameWidgets
 Home-page: https://github.com/SuperGuy123456/GameWidgets
 Author: Manomay tyagi
 Author-email: tyagimanomay57@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `GameWidgets-0.1.6/GameWidgets.egg-info/SOURCES.txt` & `GameWidgets-0.1.7/GameWidgets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 GameWidgets/__init__.py
 GameWidgets/setup.py
 GameWidgets.egg-info/PKG-INFO
 GameWidgets.egg-info/SOURCES.txt
 GameWidgets.egg-info/dependency_links.txt
 GameWidgets.egg-info/requires.txt
 GameWidgets.egg-info/top_level.txt
+GameWidgets/Assets/__init__.py
 GameWidgets/Engine/Backdrop.py
 GameWidgets/Engine/Entity.py
 GameWidgets/Engine/Group.py
 GameWidgets/Engine/__init__.py
 GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
 GameWidgets/Examples/__init__.py
 GameWidgets/GameWidgets/Animatrix.py
```

### Comparing `GameWidgets-0.1.6/PKG-INFO` & `GameWidgets-0.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWidgets
-Version: 0.1.6
+Version: 0.1.7
 Summary: Make Game Easier with pygame and GameWidgets
 Home-page: https://github.com/SuperGuy123456/GameWidgets
 Author: Manomay tyagi
 Author-email: tyagimanomay57@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

