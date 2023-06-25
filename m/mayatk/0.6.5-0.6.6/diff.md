# Comparing `tmp/mayatk-0.6.5.tar.gz` & `tmp/mayatk-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayatk-0.6.5.tar", last modified: Sat Jun 24 02:37:21 2023, max compression
+gzip compressed data, was "mayatk-0.6.6.tar", last modified: Sun Jun 25 23:03:14 2023, max compression
```

## Comparing `mayatk-0.6.5.tar` & `mayatk-0.6.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.909536 mayatk-0.6.5/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.5/LICENSE
--rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1246 2023-06-24 02:37:21.909536 mayatk-0.6.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.887192 mayatk-0.6.5/mayatk/
--rw-rw-rw-   0        0        0     5784 2023-06-24 02:37:18.000000 mayatk-0.6.5/mayatk/__init__.py
--rw-rw-rw-   0        0        0     8075 2023-06-05 16:23:13.000000 mayatk-0.6.5/mayatk/cam_utils.py
--rw-rw-rw-   0        0        0     8083 2023-05-30 18:39:58.000000 mayatk-0.6.5/mayatk/cam_utils.py.bak
--rw-rw-rw-   0        0        0    65402 2023-06-14 17:05:48.000000 mayatk-0.6.5/mayatk/cmpt_utils.py
--rw-rw-rw-   0        0        0    48216 2023-05-30 18:39:58.000000 mayatk-0.6.5/mayatk/cmpt_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.896705 mayatk-0.6.5/mayatk/display_utils/
--rw-rw-rw-   0        0        0      428 2023-04-16 16:33:47.000000 mayatk-0.6.5/mayatk/display_utils/__init__.py
--rw-rw-rw-   0        0        0     7433 2023-06-13 02:25:19.000000 mayatk-0.6.5/mayatk/display_utils/exploded_view.py
--rw-rw-rw-   0        0        0    30588 2023-06-23 22:00:50.000000 mayatk-0.6.5/mayatk/edit_utils.py
--rw-rw-rw-   0        0        0    22313 2023-05-28 17:20:26.000000 mayatk-0.6.5/mayatk/macro_utils.py
--rw-rw-rw-   0        0        0    13411 2023-06-05 16:23:13.000000 mayatk-0.6.5/mayatk/mash_utils.py
--rw-rw-rw-   0        0        0    13413 2023-05-29 19:59:22.000000 mayatk-0.6.5/mayatk/mash_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.898702 mayatk-0.6.5/mayatk/mat_utils/
--rw-rw-rw-   0        0        0      367 2023-04-16 16:33:48.000000 mayatk-0.6.5/mayatk/mat_utils/__init__.py
--rw-rw-rw-   0        0        0     9122 2023-06-12 14:32:54.000000 mayatk-0.6.5/mayatk/mat_utils/mat_utils.py
--rw-rw-rw-   0        0        0    19177 2023-06-20 19:06:12.000000 mayatk-0.6.5/mayatk/mat_utils/stingray_arnold_shader.py
--rw-rw-rw-   0        0        0    15178 2023-06-23 15:06:20.000000 mayatk-0.6.5/mayatk/misc_utils.py
--rw-rw-rw-   0        0        0    15374 2023-06-17 12:29:07.000000 mayatk-0.6.5/mayatk/misc_utils.py.bak
--rw-rw-rw-   0        0        0    29580 2023-06-22 00:27:45.000000 mayatk-0.6.5/mayatk/node_utils.py
--rw-rw-rw-   0        0        0    13413 2023-06-16 01:20:55.000000 mayatk-0.6.5/mayatk/project_utils.py
--rw-rw-rw-   0        0        0    11613 2023-05-20 16:09:43.000000 mayatk-0.6.5/mayatk/project_utils.py.bak
--rw-rw-rw-   0        0        0    20346 2023-06-06 18:19:16.000000 mayatk-0.6.5/mayatk/rig_utils.py
--rw-rw-rw-   0        0        0    20342 2023-05-30 18:34:56.000000 mayatk-0.6.5/mayatk/rig_utils.py.bak
--rw-rw-rw-   0        0        0     2771 2023-05-20 16:34:41.000000 mayatk-0.6.5/mayatk/script_utils.py
--rw-rw-rw-   0        0        0    32313 2023-06-06 18:19:16.000000 mayatk-0.6.5/mayatk/xform_utils.py
--rw-rw-rw-   0        0        0    32309 2023-06-05 16:23:13.000000 mayatk-0.6.5/mayatk/xform_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.894702 mayatk-0.6.5/mayatk.egg-info/
--rw-rw-rw-   0        0        0     1246 2023-06-24 02:37:21.000000 mayatk-0.6.5/mayatk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2023-05-20 15:52:44.000000 mayatk-0.6.5/mayatk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0     1016 2023-06-24 02:37:21.000000 mayatk-0.6.5/mayatk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.5/mayatk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-06-24 02:37:21.000000 mayatk-0.6.5/mayatk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-24 02:37:21.000000 mayatk-0.6.5/mayatk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 02:37:21.909536 mayatk-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     2238 2023-06-06 18:19:16.000000 mayatk-0.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.908531 mayatk-0.6.5/test/
--rw-rw-rw-   0        0        0     1289 2023-05-20 14:01:35.000000 mayatk-0.6.5/test/__init__.py
--rw-rw-rw-   0        0        0    26011 2023-06-14 17:56:40.000000 mayatk-0.6.5/test/cmpt_utils_test.py
--rw-rw-rw-   0        0        0     7670 2023-05-20 15:49:30.000000 mayatk-0.6.5/test/edit_utils_test.py
--rw-rw-rw-   0        0        0     4485 2023-06-11 12:52:05.000000 mayatk-0.6.5/test/mat_utils_test.py
--rw-rw-rw-   0        0        0     7863 2023-06-17 12:29:32.000000 mayatk-0.6.5/test/misc_utils_test.py
--rw-rw-rw-   0        0        0     8241 2023-06-14 16:56:33.000000 mayatk-0.6.5/test/node_utils_test.py
--rw-rw-rw-   0        0        0     5080 2023-05-20 16:17:57.000000 mayatk-0.6.5/test/rig_utils_test.py
--rw-rw-rw-   0        0        0     3406 2023-06-14 17:14:08.000000 mayatk-0.6.5/test/run_tests.py
--rw-rw-rw-   0        0        0     7292 2023-05-20 17:08:16.000000 mayatk-0.6.5/test/xform_utils_test.py
+drwxrwxrwx   0        0        0        0 2023-06-25 23:03:14.063437 mayatk-0.6.6/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1246 2023-06-25 23:03:14.063437 mayatk-0.6.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 23:03:14.044438 mayatk-0.6.6/mayatk/
+-rw-rw-rw-   0        0        0     5784 2023-06-25 23:03:11.000000 mayatk-0.6.6/mayatk/__init__.py
+-rw-rw-rw-   0        0        0     8075 2023-06-05 16:23:13.000000 mayatk-0.6.6/mayatk/cam_utils.py
+-rw-rw-rw-   0        0        0     8083 2023-05-30 18:39:58.000000 mayatk-0.6.6/mayatk/cam_utils.py.bak
+-rw-rw-rw-   0        0        0    65402 2023-06-14 17:05:48.000000 mayatk-0.6.6/mayatk/cmpt_utils.py
+-rw-rw-rw-   0        0        0    48216 2023-05-30 18:39:58.000000 mayatk-0.6.6/mayatk/cmpt_utils.py.bak
+drwxrwxrwx   0        0        0        0 2023-06-25 23:03:14.053437 mayatk-0.6.6/mayatk/display_utils/
+-rw-rw-rw-   0        0        0      397 2023-06-25 00:47:10.000000 mayatk-0.6.6/mayatk/display_utils/__init__.py
+-rw-rw-rw-   0        0        0     7433 2023-06-13 02:25:19.000000 mayatk-0.6.6/mayatk/display_utils/exploded_view.py
+-rw-rw-rw-   0        0        0    30588 2023-06-23 22:00:50.000000 mayatk-0.6.6/mayatk/edit_utils.py
+-rw-rw-rw-   0        0        0    22313 2023-05-28 17:20:26.000000 mayatk-0.6.6/mayatk/macro_utils.py
+-rw-rw-rw-   0        0        0    13411 2023-06-05 16:23:13.000000 mayatk-0.6.6/mayatk/mash_utils.py
+-rw-rw-rw-   0        0        0    13413 2023-05-29 19:59:22.000000 mayatk-0.6.6/mayatk/mash_utils.py.bak
+drwxrwxrwx   0        0        0        0 2023-06-25 23:03:14.055439 mayatk-0.6.6/mayatk/mat_utils/
+-rw-rw-rw-   0        0        0      337 2023-06-25 00:47:26.000000 mayatk-0.6.6/mayatk/mat_utils/__init__.py
+-rw-rw-rw-   0        0        0     9122 2023-06-12 14:32:54.000000 mayatk-0.6.6/mayatk/mat_utils/mat_utils.py
+-rw-rw-rw-   0        0        0    18613 2023-06-25 01:01:15.000000 mayatk-0.6.6/mayatk/mat_utils/stingray_arnold_shader.py
+-rw-rw-rw-   0        0        0    15178 2023-06-23 15:06:20.000000 mayatk-0.6.6/mayatk/misc_utils.py
+-rw-rw-rw-   0        0        0    15374 2023-06-17 12:29:07.000000 mayatk-0.6.6/mayatk/misc_utils.py.bak
+-rw-rw-rw-   0        0        0    29580 2023-06-22 00:27:45.000000 mayatk-0.6.6/mayatk/node_utils.py
+-rw-rw-rw-   0        0        0    13413 2023-06-16 01:20:55.000000 mayatk-0.6.6/mayatk/project_utils.py
+-rw-rw-rw-   0        0        0    11613 2023-05-20 16:09:43.000000 mayatk-0.6.6/mayatk/project_utils.py.bak
+-rw-rw-rw-   0        0        0    20346 2023-06-06 18:19:16.000000 mayatk-0.6.6/mayatk/rig_utils.py
+-rw-rw-rw-   0        0        0    20342 2023-05-30 18:34:56.000000 mayatk-0.6.6/mayatk/rig_utils.py.bak
+-rw-rw-rw-   0        0        0     2771 2023-05-20 16:34:41.000000 mayatk-0.6.6/mayatk/script_utils.py
+-rw-rw-rw-   0        0        0    32313 2023-06-06 18:19:16.000000 mayatk-0.6.6/mayatk/xform_utils.py
+-rw-rw-rw-   0        0        0    32309 2023-06-05 16:23:13.000000 mayatk-0.6.6/mayatk/xform_utils.py.bak
+drwxrwxrwx   0        0        0        0 2023-06-25 23:03:14.051439 mayatk-0.6.6/mayatk.egg-info/
+-rw-rw-rw-   0        0        0     1246 2023-06-25 23:03:13.000000 mayatk-0.6.6/mayatk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2023-05-20 15:52:44.000000 mayatk-0.6.6/mayatk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0     1016 2023-06-25 23:03:13.000000 mayatk-0.6.6/mayatk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.6/mayatk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-06-25 23:03:13.000000 mayatk-0.6.6/mayatk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-25 23:03:13.000000 mayatk-0.6.6/mayatk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 23:03:14.063437 mayatk-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     2238 2023-06-06 18:19:16.000000 mayatk-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 23:03:14.062438 mayatk-0.6.6/test/
+-rw-rw-rw-   0        0        0     1289 2023-05-20 14:01:35.000000 mayatk-0.6.6/test/__init__.py
+-rw-rw-rw-   0        0        0    26011 2023-06-14 17:56:40.000000 mayatk-0.6.6/test/cmpt_utils_test.py
+-rw-rw-rw-   0        0        0     7670 2023-05-20 15:49:30.000000 mayatk-0.6.6/test/edit_utils_test.py
+-rw-rw-rw-   0        0        0     4485 2023-06-11 12:52:05.000000 mayatk-0.6.6/test/mat_utils_test.py
+-rw-rw-rw-   0        0        0     7863 2023-06-17 12:29:32.000000 mayatk-0.6.6/test/misc_utils_test.py
+-rw-rw-rw-   0        0        0     8241 2023-06-14 16:56:33.000000 mayatk-0.6.6/test/node_utils_test.py
+-rw-rw-rw-   0        0        0     5080 2023-05-20 16:17:57.000000 mayatk-0.6.6/test/rig_utils_test.py
+-rw-rw-rw-   0        0        0     3406 2023-06-14 17:14:08.000000 mayatk-0.6.6/test/run_tests.py
+-rw-rw-rw-   0        0        0     7292 2023-05-20 17:08:16.000000 mayatk-0.6.6/test/xform_utils_test.py
```

### Comparing `mayatk-0.6.5/LICENSE` & `mayatk-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/PKG-INFO` & `mayatk-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayatk
-Version: 0.6.5
+Version: 0.6.6
 Summary: *mayattk is a collection of backend utilities for Autodesk Maya.*
 Home-page: https://github.com/m3trik/mayatk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mayatk-0.6.5/mayatk/__init__.py` & `mayatk-0.6.6/mayatk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 import inspect
 import importlib
 import pkgutil
 
 
 __package__ = "mayatk"
-__version__ = '0.6.5'
+__version__ = '0.6.6'
 
 
 # Define dictionaries to map class names, method names, class method names, and sub-modules to their respective modules
 CLASS_TO_MODULE = {}
 METHOD_TO_MODULE = {}
 CLASS_METHOD_TO_MODULE = {}
 SUBMODULE_TO_MODULE = {}
```

### Comparing `mayatk-0.6.5/mayatk/cam_utils.py` & `mayatk-0.6.6/mayatk/cam_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/cam_utils.py.bak` & `mayatk-0.6.6/mayatk/cam_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/cmpt_utils.py` & `mayatk-0.6.6/mayatk/cmpt_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/cmpt_utils.py.bak` & `mayatk-0.6.6/mayatk/cmpt_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/display_utils/exploded_view.py` & `mayatk-0.6.6/mayatk/display_utils/exploded_view.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/edit_utils.py` & `mayatk-0.6.6/mayatk/edit_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/macro_utils.py` & `mayatk-0.6.6/mayatk/macro_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/mash_utils.py` & `mayatk-0.6.6/mayatk/mash_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/mash_utils.py.bak` & `mayatk-0.6.6/mayatk/mash_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/mat_utils/mat_utils.py` & `mayatk-0.6.6/mayatk/mat_utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/mat_utils/stingray_arnold_shader.py` & `mayatk-0.6.6/mayatk/mat_utils/stingray_arnold_shader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # !/usr/bin/python
 # coding=utf-8
-import sys, os
-from PySide2 import QtCore, QtWidgets
+from PySide2 import QtWidgets
 
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
-
 from uitk import Switchboard
-from pythontk import File, Img, Str
+import pythontk as ptk
 
 # from this package:
 from mayatk.misc_utils import Misc
 from mayatk.node_utils import Node
 
 
 __version__ = "0.5.3"
@@ -30,15 +28,15 @@
 
     @property
     def hdr_env(self) -> object:
         """ """
         node = pm.ls(self.hdr_env_name, exactType="aiSkyDomeLight")
         try:
             return node[0]
-        except IndexError as error:
+        except IndexError:
             return None
 
     @hdr_env.setter
     def hdr_env(self, tex) -> None:
         """ """
         node = self.hdr_env  # Node.node_exists('aiSkyDomeLight', search='exactType')
         if not node:
@@ -103,41 +101,33 @@
             )  # assure stringray plugin is loaded.
 
             sr_node = Node.create_render_node("StingrayPBS", name=name)
             ai_node = Node.create_render_node(
                 "aiStandardSurface", name=name + "_ai" if name else ""
             )
 
-            opacityMap = Img.filter_images_by_type(textures, "Opacity")
+            opacityMap = ptk.filter_images_by_type(textures, "Opacity")
             if opacityMap:
                 pm.shaderfx(
                     sfxnode="StingrayPBS1",
                     loadGraph=r"C:/_local/_test/shaderfx/Standard_Transparent.sfx",
                 )
 
-            openGLMap = Img.filter_images_by_type(textures, "Normal_OpenGL")
-            directXMap = Img.filter_images_by_type(textures, "Normal_DirectX")
+            openGLMap = ptk.filter_images_by_type(textures, "Normal_OpenGL")
+            directXMap = ptk.filter_images_by_type(textures, "Normal_DirectX")
             if directXMap and not openGLMap and normalMapType == "Normal_OpenGL":
-                mapPath = Img.create_gl_from_dx(directXMap[0])
+                mapPath = ptk.create_gl_from_dx(directXMap[0])
                 textures.append(mapPath)
                 normal_map_created_from_other_type = True
-                callback(
-                    "OpenGL map created using {}.".format(
-                        Str.truncate(directXMap[0], 20)
-                    )
-                )
+                callback(f"OpenGL map created using {ptk.truncate(directXMap[0], 20)}.")
             if openGLMap and not directXMap and normalMapType == "Normal_DirectX":
-                mapPath = Img.create_dx_from_gl(openGLMap[0])
+                mapPath = ptk.create_dx_from_gl(openGLMap[0])
                 textures.append(mapPath)
                 normal_map_created_from_other_type = True
-                callback(
-                    "DirectX map created using {}.".format(
-                        Str.truncate(openGLMap[0], 20)
-                    )
-                )
+                callback(f"DirectX map created using {ptk.truncate(openGLMap[0], 20)}.")
 
             srSG_node = Node.get_outgoing_node_by_type(sr_node, "shadingEngine")
 
             aiMult_node = pm.shadingNode("aiMultiply", asShader=True)
 
             bump_node = pm.shadingNode("bump2d", asShader=True)
             bump_node.bumpInterp.set(1)  # set bump node to 'tangent space normals'
@@ -147,28 +137,28 @@
                 (aiMult_node.outColor, ai_node.baseColor),
                 (bump_node.outNormal, ai_node.normalCamera),
             )
 
             length = len(textures)
             progress = 0
             for f in textures:
-                typ = Img.get_image_type_from_filename(f)
+                typ = ptk.get_image_type_from_filename(f)
 
                 progress += 1
 
                 # filter normal maps for the correct type.
                 if typ == "Normal" and (openGLMap or directXMap):
                     continue
                 elif typ == "Normal_DirectX" and normalMapType == "Normal_OpenGL":
                     continue
                 elif typ == "Normal_OpenGL" and normalMapType == "Normal_DirectX":
                     continue
 
                 callback(
-                    "creating nodes and connections for <b>{}</b> map ..".format(typ),
+                    f"creating nodes and connections for <b>{typ}</b> map ..",
                     [progress, length],
                 )
 
                 if typ == "Base_Color":
                     n1 = Node.create_render_node("file", "as2DTexture", tex=f)
                     pm.connectAttr(n1.outColor, sr_node.TEX_color_map, force=True)
                     sr_node.use_color_map.set(1)
@@ -267,76 +257,68 @@
                     pm.connectAttr(n2.outAlpha, ai_node.transmission, force=True)
                     pm.connectAttr(n2.outColor, ai_node.opacity, force=True)
 
                 else:
                     if normal_map_created_from_other_type:
                         continue  # do not show a warning for unconnected normal maps if it resulted from being converted to a different output type.
                     callback(
-                        '<br><hl style="color:rgb(255, 100, 100);"><b>Map type: <b>{}</b> not connected:<br></hl>'.format(
-                            typ, Str.truncate(f, 60)
-                        ),
+                        f'<br><hl style="color:rgb(255, 100, 100);"><b>Map type: <b>{typ, ptk.truncate(f, 60)}</b> not connected:<br></hl>',
                         [progress, length],
                     )
                     continue
 
                 callback(
-                    '<font style="color: rgb(80,180,100)">{}..connected successfully.</font>'.format(
-                        typ
-                    )
+                    f'<font style="color: rgb(80,180,100)">{typ}..connected successfully.</font>'
                 )
-        except Exception as error:
+        except Exception as e:
             callback(
-                '<br><hl style="color:rgb(255, 100, 100);"><b>Error:</b>{}.</hl>'.format(
-                    error
-                )
+                f'<br><hl style="color:rgb(255, 100, 100);"><b>Error:</b>{e}.</hl>'
             )
 
         self.hdr_env = hdrMap
         self.set_hdr_map_visibility(hdrMapVisibility)
 
 
 class StingrayArnoldShaderSlots(StingrayArnoldShader):
     msg_intro = """<u>To setup the material:</u>
         <br>• Use the <b>Get Texture Maps</b> button to load the images you intend to use.
         <br>• Click the <b>Create Network</b> button to create the shader connections.
         <br>• The HDR map, it's visiblity, and rotation can be changed after creation.
     """
     msg_completed = '<br><hl style="color:rgb(0, 255, 255);"><b>COMPLETED.</b></hl>'
 
-    proj_root_dir = File.get_filepath(__file__)
+    proj_root_dir = ptk.get_filepath(__file__)
 
     def __init__(self, **kwargs):
         super().__init__()
         """
         """
         self.sb = self.switchboard()
         self.image_files = None
 
         # set json file location.
-        path = "{}/stingray_arnold_shader.json".format(self.sb.defaultDir)
-        File.set_json_file(path)  # set json file name
+        path = f"{self.sb.default_dir}/stingray_arnold_shader.json"
+        ptk.set_json_file(path)  # set json file name
 
         # add filenames|filepaths to the comboBox.
-        hdr_path = "{}/resources/hdr".format(self.proj_root_dir)
-        hdr_filenames = File.get_dir_contents(hdr_path, "filenames", inc_files="*.exr")
-        hdr_fullpaths = File.get_dir_contents(hdr_path, "filepaths", inc_files="*.exr")
-        self.sb.ui.cmb000.add(
-            dict(zip(hdr_filenames, hdr_fullpaths)), ascending=False
-        )
+        hdr_path = f"{self.proj_root_dir}/resources/hdr"
+        hdr_filenames = ptk.get_dir_contents(hdr_path, "filenames", inc_files="*.exr")
+        hdr_fullpaths = ptk.get_dir_contents(hdr_path, "filepaths", inc_files="*.exr")
+        self.sb.ui.cmb000.add(dict(zip(hdr_filenames, hdr_fullpaths)), ascending=False)
 
         # initialize widgets with any saved values.
-        self.sb.ui.txt000.setText(File.get_json("mat_name"))
+        self.sb.ui.txt000.setText(ptk.get_json("mat_name"))
         self.sb.ui.txt001.setText(self.msg_intro)
-        hdr_map_visibility = File.get_json("hdr_map_visibility")
+        hdr_map_visibility = ptk.get_json("hdr_map_visibility")
         if hdr_map_visibility:
             self.sb.ui.chk000.setChecked(hdr_map_visibility)
-        hdr_map = File.get_json("hdr_map")
+        hdr_map = ptk.get_json("hdr_map")
         if hdr_map:
             self.sb.ui.cmb000.setCurrentItem(hdr_map)
-        normal_map_type = File.get_json("normal_map_type")
+        normal_map_type = ptk.get_json("normal_map_type")
         if normal_map_type:
             self.sb.ui.cmb001.setCurrentItem(normal_map_type)
         node = self.hdr_env_transform
         if node:
             rotation = node.rotateY.get()
             self.sb.ui.slider000.setSliderPosition(rotation)
 
@@ -376,43 +358,39 @@
 
         Returns:
                 (str)
         """
         text = self.sb.ui.cmb001.currentText()
         return text
 
-    def cmb000(self, index):
+    def cmb000(self, index, widget):
         """HDR map selection."""
-        cmb = self.sb.ui.cmb000
-        text = cmb.currentText()
-        data = cmb.currentData()
+        text = widget.currentText()
+        data = widget.currentData()
 
         self.hdr_env = data  # set the HDR map.
-        File.set_json("hdr_map", text)
+        ptk.set_json("hdr_map", text)
 
-    def chk000(self, state):
-        """ """
-        chk = self.sb.ui.chk000
-
-        self.set_hdr_map_visibility(state)  # set the HDR map visibility.
-        File.set_json("hdr_map_visibility", state)
-
-    def cmb001(self, index):
+    def cmb001(self, index, widget):
         """Normal map output selection."""
         cmb = self.sb.ui.cmb001
         text = cmb.currentText()
-        File.set_json("normal_map_type", text)
+        ptk.set_json("normal_map_type", text)
+
+    def chk000(self, state, widget):
+        """ """
+        self.set_hdr_map_visibility(state)  # set the HDR map visibility.
+        ptk.set_json("hdr_map_visibility", state)
 
-    def txt000(self, text=None):
+    def txt000(self, text, widget):
         """Material name."""
-        txt = self.sb.ui.txt000
-        text = txt.text()
-        File.set_json("mat_name", text)
+        text = widget.text()
+        ptk.set_json("mat_name", text)
 
-    def slider000(self, value):
+    def slider000(self, value, widget):
         """Rotate the HDR map."""
         if self.hdr_env:
             transform = Node.get_transform_node(self.hdr_env)
             pm.rotate(
                 transform,
                 value,
                 rotateY=True,
@@ -439,25 +417,25 @@
             )
 
             self.callback(self.msg_completed)
             # pm.mel.hyperShadePanelGraphCommand('hyperShadePanel1', 'rearrangeGraph')
 
     def b001(self):
         """Get texture maps."""
-        image_files = Img.get_image_files()
+        image_files = ptk.get_image_files()
 
         if image_files:
             self.image_files = image_files
             self.sb.ui.txt001.clear()
 
             msg_mat_selection = self.image_files
             for (
                 i
-            ) in msg_mat_selection:  # format msg_intro using the mapTypes in imtools.
-                self.callback(Str.truncate(i, 60))
+            ) in msg_mat_selection:  # format msg_intro using the map_types in imtools.
+                self.callback(ptk.truncate(i, 60))
 
             self.sb.ui.b000.setDisabled(False)
         elif not self.image_files:
             self.sb.ui.b000.setDisabled(True)
 
     def callback(self, string, progress=None, clear=False):
         """
@@ -466,16 +444,16 @@
                 progress (int/list): The progress amount to register with the progressBar.
                         Can be given as an int or a tuple as: (progress, total_len)
         """
         if clear:
             self.sb.ui.txt003.clear()
 
         if isinstance(progress, (list, tuple, set)):
-            p, l = progress
-            progress = (p / l) * 100
+            p, length = progress
+            progress = (p / length) * 100
 
         self.sb.ui.txt001.append(string)
 
         if progress is not None:
             self.sb.ui.progressBar.setValue(progress)
             QtWidgets.QApplication.instance().processEvents()
 
@@ -510,21 +488,19 @@
                 if hasattr(self, "_height_open")
                 else self.ui.sizeHint().height(),
             )
 
 
 # -----------------------------------------------------------------------------
 
-
-# -----------------------------------------------------------------------------
-
 if __name__ == "__main__":
     parent = Misc.get_main_window()
     sb = StingrayArnoldShaderUI(parent)
-    sb.ui.show()
+    sb.ui.set_style(theme="dark")
+    sb.ui.show(app_exec=True)
 
 # -----------------------------------------------------------------------------
 # Notes
 # -----------------------------------------------------------------------------
 
 
-# Deprecated ------------------------------------------------------------------
+# Deprecated ------------------------------------
```

### Comparing `mayatk-0.6.5/mayatk/misc_utils.py` & `mayatk-0.6.6/mayatk/misc_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/misc_utils.py.bak` & `mayatk-0.6.6/mayatk/misc_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/node_utils.py` & `mayatk-0.6.6/mayatk/node_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/project_utils.py` & `mayatk-0.6.6/mayatk/project_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/project_utils.py.bak` & `mayatk-0.6.6/mayatk/project_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/rig_utils.py` & `mayatk-0.6.6/mayatk/rig_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/rig_utils.py.bak` & `mayatk-0.6.6/mayatk/rig_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/script_utils.py` & `mayatk-0.6.6/mayatk/script_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/xform_utils.py` & `mayatk-0.6.6/mayatk/xform_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk/xform_utils.py.bak` & `mayatk-0.6.6/mayatk/xform_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk.egg-info/PKG-INFO` & `mayatk-0.6.6/mayatk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayatk
-Version: 0.6.5
+Version: 0.6.6
 Summary: *mayattk is a collection of backend utilities for Autodesk Maya.*
 Home-page: https://github.com/m3trik/mayatk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mayatk-0.6.5/mayatk.egg-info/PKG-INFO.bak` & `mayatk-0.6.6/mayatk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk.egg-info/SOURCES.txt` & `mayatk-0.6.6/mayatk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/mayatk.egg-info/SOURCES.txt.bak` & `mayatk-0.6.6/mayatk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/setup.py` & `mayatk-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/test/__init__.py` & `mayatk-0.6.6/test/__init__.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/test/cmpt_utils_test.py` & `mayatk-0.6.6/test/cmpt_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/test/edit_utils_test.py` & `mayatk-0.6.6/test/edit_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/test/mat_utils_test.py` & `mayatk-0.6.6/test/mat_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/test/misc_utils_test.py` & `mayatk-0.6.6/test/misc_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/test/node_utils_test.py` & `mayatk-0.6.6/test/node_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/test/rig_utils_test.py` & `mayatk-0.6.6/test/rig_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/test/run_tests.py` & `mayatk-0.6.6/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.5/test/xform_utils_test.py` & `mayatk-0.6.6/test/xform_utils_test.py`

 * *Files identical despite different names*

