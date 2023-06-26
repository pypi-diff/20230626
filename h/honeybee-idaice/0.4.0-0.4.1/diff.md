# Comparing `tmp/honeybee-idaice-0.4.0.tar.gz` & `tmp/honeybee-idaice-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.4.0.tar", last modified: Thu Jun 22 18:49:33 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.4.1.tar", last modified: Mon Jun 26 21:26:27 2023, max compression
```

## Comparing `honeybee-idaice-0.4.0.tar` & `honeybee-idaice-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/bldgbody.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/face.py
--rw-r--r--   0 runner    (1001) docker     (123)    27746 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 18:49:33.000000 honeybee-idaice-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-22 18:48:25.000000 honeybee-idaice-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/bldgbody.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27806 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 21:26:27.000000 honeybee-idaice-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-26 21:25:08.000000 honeybee-idaice-0.4.1/setup.py
```

### Comparing `honeybee-idaice-0.4.0/LICENSE` & `honeybee-idaice-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/PKG-INFO` & `honeybee-idaice-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.4.0
+Version: 0.4.1
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.4.0/README.md` & `honeybee-idaice-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/archive.py` & `honeybee-idaice-0.4.1/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/bldgbody.py` & `honeybee-idaice-0.4.1/honeybee_idaice/bldgbody.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,25 +68,25 @@
 
             vc = sum(len(c) for c in contours)
             contours_formatted = ' '.join(str(len(c)) for c in contours)
 
             vertices_idm = ' '.join(
                 f'({v.x} {v.y} {v.z})' for vv in contours for v in vv
             )
-
+            identifier = wall_count + floor_count
             if type_ == 'CRAWL-FACE':
-                body = f' ((FACE :N "{face.identifier}" :T {type_} :INDEX {index})\n' \
+                body = f' ((FACE :N "f{identifier}" :T {type_} :INDEX {index})\n' \
                     '  (:PAR :N NCORN :V 0)\n' \
                     '  (:PAR :N CORNERS :DIM (0 3) :V #2A())\n' \
                     '  ((FACE :N GROUND-FACE)\n' \
                     f'   (:PAR :N NCORN :V {vc})\n' \
                     f'   (:PAR :N CORNERS :DIM ({vc} 3) :V #2A({vertices_idm}))\n' \
                     f'   (:PAR :N CONTOURS :V ({contours_formatted}))))'
             else:
-                body = f' ((FACE :N "{face.identifier}" :T {type_} :INDEX {index})\n' \
+                body = f' ((FACE :N "f{identifier}" :T {type_} :INDEX {index})\n' \
                     f'  (:PAR :N NCORN :V {vc})\n' \
                     f'  (:PAR :N CORNERS :DIM ({vc} 3) :V #2A({vertices_idm}))\n' \
                     f'  (:PAR :N CONTOURS :V ({contours_formatted}))\n' \
                     f'  (:PAR :N SLOPE :V {face.altitude + 90})\n' \
                     '  ((FACE :N GROUND-FACE)\n' \
                     '   (:PAR :N NCORN :V 0)\n' \
                     '   (:PAR :N CORNERS :DIM (0 3))))'
```

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.4.1/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/face.py` & `honeybee-idaice-0.4.1/honeybee_idaice/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.4.1/honeybee_idaice/geometry_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,18 +474,19 @@
     # floors are most likely horizontal - let's make them 2D polygons
     for floor in floor_geom:
         boundary = Polygon2D(
             [
                 Point2D(v.x, v.y) for v in floor.lower_left_counter_clockwise_vertices
             ]
         )
+        boundary = boundary.remove_colinear_vertices(0.01)
         boundaries.append(boundary)
 
     # find the union of the boundary polygons
-    if len(boundaries) > 1 and not boundaries[0].has_holes:
+    if len(boundaries) == 1 and not floor_geom[0].has_holes:
         boundary = boundaries[0]
     else:
         pf = Polyface3D.from_faces(floor_geom, tolerance=0.01)
         boundaries = Polyline3D.join_segments(pf.naked_edges, tolerance=0.01)
         assert boundaries, \
             f'Failed to calculate the floor boundary for {room.display_name}'
         boundary = Polyline2D([Point2D(v.x, v.y) for v in boundaries[0].vertices[:-1]])
```

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/shade.py` & `honeybee-idaice-0.4.1/honeybee_idaice/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.4.1/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.4.1/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.4.1/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.4.1/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.4.1/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.4.1/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/writer.py` & `honeybee-idaice-0.4.1/honeybee_idaice/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.4.1/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.4.1/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.4.0
+Version: 0.4.1
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.4.0/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.4.1/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.0/setup.py` & `honeybee-idaice-0.4.1/setup.py`

 * *Files identical despite different names*

