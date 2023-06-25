# Comparing `tmp/pythontk-0.6.4.tar.gz` & `tmp/pythontk-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythontk-0.6.4.tar", last modified: Thu Jun 22 16:14:27 2023, max compression
+gzip compressed data, was "pythontk-0.6.6.tar", last modified: Sun Jun 25 23:02:01 2023, max compression
```

## Comparing `pythontk-0.6.4.tar` & `pythontk-0.6.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 16:14:27.119139 pythontk-0.6.4/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:38:48.000000 pythontk-0.6.4/LICENSE
--rw-rw-rw-   0        0        0     1286 2023-06-22 16:14:27.119139 pythontk-0.6.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 16:14:27.086134 pythontk-0.6.4/pythontk/
--rw-rw-rw-   0        0        0     7133 2023-06-22 16:14:18.000000 pythontk-0.6.4/pythontk/__init__.py
--rw-rw-rw-   0        0        0    25520 2023-06-06 01:08:03.000000 pythontk-0.6.4/pythontk/file_utils.py
--rw-rw-rw-   0        0        0    29207 2023-06-06 18:19:16.000000 pythontk-0.6.4/pythontk/img_utils.py
--rw-rw-rw-   0        0        0    16156 2023-06-06 18:19:16.000000 pythontk-0.6.4/pythontk/iter_utils.py
--rw-rw-rw-   0        0        0    18312 2023-05-30 18:39:59.000000 pythontk-0.6.4/pythontk/math_utils.py
--rw-rw-rw-   0        0        0    11452 2023-06-14 16:03:32.000000 pythontk-0.6.4/pythontk/misc_utils.py
--rw-rw-rw-   0        0        0    25433 2023-06-14 21:04:19.000000 pythontk-0.6.4/pythontk/str_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:14:27.117135 pythontk-0.6.4/pythontk.egg-info/
--rw-rw-rw-   0        0        0     1286 2023-06-22 16:14:26.000000 pythontk-0.6.4/pythontk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2023-05-20 13:28:19.000000 pythontk-0.6.4/pythontk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0      366 2023-06-22 16:14:26.000000 pythontk-0.6.4/pythontk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      265 2023-05-07 12:53:37.000000 pythontk-0.6.4/pythontk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-06-22 16:14:26.000000 pythontk-0.6.4/pythontk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 16:14:26.000000 pythontk-0.6.4/pythontk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 16:14:27.119139 pythontk-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     2212 2023-06-06 18:19:16.000000 pythontk-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 23:02:01.316895 pythontk-0.6.6/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:38:48.000000 pythontk-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0     1155 2023-06-25 23:02:01.316895 pythontk-0.6.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 23:02:01.303892 pythontk-0.6.6/pythontk/
+-rw-rw-rw-   0        0        0     7133 2023-06-25 23:01:58.000000 pythontk-0.6.6/pythontk/__init__.py
+-rw-rw-rw-   0        0        0    25612 2023-06-25 00:59:16.000000 pythontk-0.6.6/pythontk/file_utils.py
+-rw-rw-rw-   0        0        0    29224 2023-06-24 12:30:01.000000 pythontk-0.6.6/pythontk/img_utils.py
+-rw-rw-rw-   0        0        0    29221 2023-06-24 12:29:41.000000 pythontk-0.6.6/pythontk/img_utils.py.bak
+-rw-rw-rw-   0        0        0    16156 2023-06-06 18:19:16.000000 pythontk-0.6.6/pythontk/iter_utils.py
+-rw-rw-rw-   0        0        0    18312 2023-05-30 18:39:59.000000 pythontk-0.6.6/pythontk/math_utils.py
+-rw-rw-rw-   0        0        0    11452 2023-06-14 16:03:32.000000 pythontk-0.6.6/pythontk/misc_utils.py
+-rw-rw-rw-   0        0        0    25433 2023-06-14 21:04:19.000000 pythontk-0.6.6/pythontk/str_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 23:02:01.315894 pythontk-0.6.6/pythontk.egg-info/
+-rw-rw-rw-   0        0        0     1155 2023-06-25 23:02:01.000000 pythontk-0.6.6/pythontk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2023-05-20 13:28:19.000000 pythontk-0.6.6/pythontk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0      392 2023-06-25 23:02:01.000000 pythontk-0.6.6/pythontk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      265 2023-05-07 12:53:37.000000 pythontk-0.6.6/pythontk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-06-25 23:02:01.000000 pythontk-0.6.6/pythontk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 23:02:01.000000 pythontk-0.6.6/pythontk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 23:02:01.316895 pythontk-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     2212 2023-06-06 18:19:16.000000 pythontk-0.6.6/setup.py
```

### Comparing `pythontk-0.6.4/LICENSE` & `pythontk-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.4/PKG-INFO` & `pythontk-0.6.6/pythontk.egg-info/PKG-INFO.bak`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythontk
-Version: 0.6.4
+Version: 0.6.2
 Summary: *pythontk is a collection of backend utilities for Python.*
 Home-page: https://github.com/m3trik/pythontk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,12 +32,12 @@
 ### Example use-case:
 ###### Import the class `Iter` from the package.
 ###### As the name suggests, the class `Iter` holds the package's iterable related functions.
 ```python
 from pythontk import Iter
 Iter.filter_list([0, 1, 2, 3, 2], [1, 2, 3], 2) #returns: [1, 3]
 ```
-###### You can also import any function directly.
+###### You can also import a function directly.
 ```python
-from pythontk import filter_dict
-filter_dict({1:'1', 'two':2, 3:'three'}, exc='t*', keys=True) #returns: {1: '1', 3: 'three'}
+from pythontk.Iter import filterDict
+filterDict({1:'1', 'two':2, 3:'three'}, exc='t*', keys=True) #returns: {1: '1', 3: 'three'}
 ```
```

### Comparing `pythontk-0.6.4/pythontk/__init__.py` & `pythontk-0.6.6/pythontk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 import inspect
 import importlib
 import pkgutil
 
 
 __package__ = "pythontk"
-__version__ = '0.6.4'
+__version__ = '0.6.6'
 
 
 # Define dictionaries to map class names, method names, and class method names to their respective modules
 CLASS_TO_MODULE = {}
 METHOD_TO_MODULE = {}
 CLASS_METHOD_TO_MODULE = {}
```

### Comparing `pythontk-0.6.4/pythontk/file_utils.py` & `pythontk-0.6.6/pythontk/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     @staticmethod
     def get_file_info(paths, returned_type):
         """Get specific file information for a list of paths.
 
         Parameters:
             paths (list): List of paths to retrieve file information from.
             returned_type (str): Return specific file information. Multiple types can be given using '|'.
-                              ex. 'file|filename|filepath|dir|dirpath|timestamp|unixtimestamp|size|filetype'
+                    ex. 'file|filename|filepath|dir|dirpath|timestamp|unixtimestamp|size|filetype'
         Returns:
             (list): List of tuples containing requested file information.
         """
         import time
         from pathlib import Path
 
         returnTypes = [t.strip().rstrip("s").lower() for t in returned_type.split("|")]
@@ -262,19 +262,22 @@
             if filepath is None and hasattr(
                 obj, "__path__"
             ):  # handle namespace packages
                 filepath = obj.__path__[0]
         elif callable(obj) or isinstance(obj, object):
             try:
                 module = inspect.getmodule(obj)
-                filepath = getattr(module, "__file__", None)
-                if filepath is None and hasattr(
-                    module, "__path__"
-                ):  # handle namespace packages
-                    filepath = module.__path__[0]
+                if module.__name__ == "__main__":
+                    filepath = sys.argv[0]
+                else:
+                    filepath = getattr(module, "__file__", None)
+                    if filepath is None and hasattr(
+                        module, "__path__"
+                    ):  # handle namespace packages
+                        filepath = module.__path__[0]
             except AttributeError:
                 raise ValueError(
                     "Unable to determine file path for object of type: ", type(obj)
                 )
         else:
             raise ValueError("Invalid type for obj: ", type(obj))
 
@@ -502,15 +505,15 @@
         """Get the current json filepath.
 
         Returns:
             (str)
         """
         try:
             return cls._jsonFile
-        except AttributeError as error:
+        except AttributeError:
             return ""
 
     @classmethod
     def set_json(cls, key, value, file=None):
         """
         Parameters:
             key () = Set the json key.
@@ -535,15 +538,15 @@
             __file__, type(file).__name__
         )
 
         try:
             with open(file, "r") as f:
                 dct = json.loads(f.read())
                 dct[key] = value
-        except json.decoder.JSONDecodeError as error:
+        except json.decoder.JSONDecodeError:
             dct = {}
             dct[key] = value
 
         with open(file, "w") as f:
             f.write(json.dumps(dct))
 
     @classmethod
@@ -575,18 +578,18 @@
             __file__, type(file).__name__
         )
 
         try:
             with open(file, "r") as f:
                 return json.loads(f.read())[key]
 
-        except KeyError as error:
+        except KeyError:
             # print ('# Error: {}: get_json: KeyError: {}'.format(__file__, error))
             pass
-        except FileNotFoundError as error:
+        except FileNotFoundError:
             # print ('# Error: {}: get_json: FileNotFoundError: {}'.format(__file__, error))
             pass
         except json.decoder.JSONDecodeError as error:
             print(
                 "{} in get_json\n\t# Error: JSONDecodeError: {} #".format(
                     __file__, error
                 )
```

### Comparing `pythontk-0.6.4/pythontk/img_utils.py` & `pythontk-0.6.6/pythontk/img_utils.py.bak`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class Img:
     """Helper methods for working with image file formats."""
 
     app = QtWidgets.QApplication.instance() or QtWidgets.QApplication(
         sys.argv
     )  # return the existing QApplication object, or create a new one if none exists.
 
-    mapTypes = {  # Get map type from filename suffix.
+    map_types = {  # Get map type from filename suffix.
         "Base_Color": ("Base_Color", "BaseColor", "_BC"),
         "Roughness": ("Roughness", "Rough", "_R"),
         "Metallic": ("Metallic", "Metal", "Metalness", "_M"),
         "Ambient_Occlusion": (
             "Mixed_AO",
             "AmbientOcclusion",
             "Ambient_Occlusion",
@@ -48,15 +48,15 @@
         "Glossiness": ("Glossiness", "Gloss", "Glos", "Glo", "_G"),
         "Displacement": ("Displacement", "_DP", "Displace", "Disp", "Dis", "_D"),
         "Refraction": ("Refraction", "IndexofRefraction", "_IOR"),
         "Reflection": ("Reflection", "_RF"),
         "Opacity": ("Opacity", "Transparancy", "Alpha", "Alpha_Mask", "_O"),
     }
 
-    mapBackgrounds = {  # Get default map backgrounds in RGBA format from map type.
+    map_backgrounds = {  # Get default map backgrounds in RGBA format from map type.
         "Base_Color": (127, 127, 127, 255),
         "Roughness": (255, 255, 255, 255),
         "Metallic": (0, 0, 0, 255),
         "Ambient_Occlusion": (255, 255, 255, 255),
         "Normal": (127, 127, 255, 255),
         "Normal_DirectX": (127, 127, 255, 255),
         "Normal_OpenGL": (127, 127, 255, 255),
@@ -66,15 +66,15 @@
         "Specular": (0, 0, 0, 255),
         "Glossiness": (0, 0, 0, 255),
         "Displacement": (0, 0, 0, 255),
         "Refraction": (0, 0, 0, 255),
         "Reflection": (0, 0, 0, 255),
     }
 
-    mapModes = {  # Get default map mode from map type.
+    map_modes = {  # Get default map mode from map type.
         "Base_Color": "RGB",
         "Roughness": "L",
         "Metallic": "L",
         "Ambient_Occlusion": "L",
         "Normal": "RGB",
         "Normal_DirectX": "RGB",
         "Normal_OpenGL": "RGB",
@@ -243,37 +243,37 @@
         return image_dir
 
     @classmethod
     def get_image_type_from_filename(cls, file, key=True):
         """
         Parameters:
                 file (str): Image filename, fullpath, or map type suffix.
-                key (bool): Get the corresponding key from the type in 'mapTypes'.
+                key (bool): Get the corresponding key from the type in 'map_types'.
                         ie. Base_Color from <filename>_BC or BC. else: _BC from <filename>_BC.
 
         Returns:
                 (str)
         """
         name = File.format_path(file, "name")
 
         if key:
             result = next(
                 (
                     k
-                    for k, v in cls.mapTypes.items()
+                    for k, v in cls.map_types.items()
                     for i in v
                     if name.lower().endswith(i.lower())
                 ),
                 None,
             )
         else:
             result = next(
                 (
                     i
-                    for v in cls.mapTypes.values()
+                    for v in cls.map_types.values()
                     for i in v
                     if name.lower().endswith(i.lower())
                 ),
                 ("".join(name.split("_")[-1]) if "_" in name else None),
             )
         if result:
             return result
@@ -352,28 +352,28 @@
             False,
         )
 
         return True if result else False
 
     @classmethod
     def is_normal_map(cls, file):
-        """Check the map type for one of the normal values in mapTypes.
+        """Check the map type for one of the normal values in map_types.
 
         Parameters:
                 file (str): Image filename, fullpath, or map type suffix.
 
         Returns:
                 (bool)
         """
         typ = cls.get_image_type_from_filename(file)
         return any(
             (
-                typ in cls.mapTypes["Normal_DirectX"],
-                typ in cls.mapTypes["Normal_OpenGL"],
-                typ in cls.mapTypes["Normal"],
+                typ in cls.map_types["Normal_DirectX"],
+                typ in cls.map_types["Normal_OpenGL"],
+                typ in cls.map_types["Normal"],
             )
         )
 
     @classmethod
     def invert_channels(cls, image, channels="RGB"):
         """Invert RGB channels.
 
@@ -415,16 +415,16 @@
 
         output_dir = File.format_path(file, "path")
         name = File.format_path(file, "name")
         ext = File.format_path(file, "ext")
 
         typ = cls.get_image_type_from_filename(file, key=False)
         try:
-            index = cls.mapTypes["Normal_OpenGL"].index(typ)
-            new_type = cls.mapTypes["Normal_DirectX"][index]
+            index = cls.map_types["Normal_OpenGL"].index(typ)
+            new_type = cls.map_types["Normal_DirectX"][index]
         except (IndexError, ValueError) as error:
             print("{} in create_dx_from_gl\n\t# Error: {} #".format(__file__, error))
             new_type = "Normal_DirectX"
 
         name = name.removesuffix(typ)
         filepath = "{}/{}{}.{}".format(output_dir, name, new_type, ext)
         inverted_image.save(filepath)
@@ -446,16 +446,16 @@
 
         output_dir = File.format_path(file, "path")
         name = File.format_path(file, "name")
         ext = File.format_path(file, "ext")
 
         typ = cls.get_image_type_from_filename(file, key=False)
         try:
-            index = cls.mapTypes["Normal_DirectX"].index(typ)
-            new_type = cls.mapTypes["Normal_OpenGL"][index]
+            index = cls.map_types["Normal_DirectX"].index(typ)
+            new_type = cls.map_types["Normal_OpenGL"][index]
         except IndexError as error:
             print("{} in create_gl_from_dx\n\t# Error: {} #".format(__file__, error))
             new_type = "Normal_OpenGL"
 
         name = name.removesuffix(typ)
         filepath = "{}/{}{}.{}".format(output_dir, name, new_type, ext)
         inverted_image.save(filepath)
```

### Comparing `pythontk-0.6.4/pythontk/iter_utils.py` & `pythontk-0.6.6/pythontk/iter_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.4/pythontk/math_utils.py` & `pythontk-0.6.6/pythontk/math_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.4/pythontk/misc_utils.py` & `pythontk-0.6.6/pythontk/misc_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.4/pythontk/str_utils.py` & `pythontk-0.6.6/pythontk/str_utils.py`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.4/setup.py` & `pythontk-0.6.6/setup.py`

 * *Files identical despite different names*

