# Comparing `tmp/powerbeatsvr-0.2.0.tar.gz` & `tmp/powerbeatsvr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/powerbeatsvr-0.2.0.tar", last modified: Fri Sep  3 12:33:37 2021, max compression
+gzip compressed data, was "dist/powerbeatsvr-0.3.0.tar", last modified: Sun Jun 25 22:24:36 2023, max compression
```

## Comparing `powerbeatsvr-0.2.0.tar` & `powerbeatsvr-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-09-03 12:33:35.000000 powerbeatsvr-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      972 2021-09-03 12:33:35.000000 powerbeatsvr-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/src/powerbeatsvr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-03 12:33:35.000000 powerbeatsvr-0.2.0/src/powerbeatsvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1994 2021-09-03 12:33:35.000000 powerbeatsvr-0.2.0/src/powerbeatsvr/bs_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-09-03 12:33:35.000000 powerbeatsvr-0.2.0/src/powerbeatsvr/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    11724 2021-09-03 12:33:35.000000 powerbeatsvr-0.2.0/src/powerbeatsvr/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/src/powerbeatsvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/src/powerbeatsvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      370 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/src/powerbeatsvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/src/powerbeatsvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/src/powerbeatsvr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/src/powerbeatsvr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-03 12:33:37.000000 powerbeatsvr-0.2.0/src/powerbeatsvr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:24:36.000000 powerbeatsvr-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-25 22:24:36.000000 powerbeatsvr-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-25 22:24:33.000000 powerbeatsvr-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 22:24:36.000000 powerbeatsvr-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-25 22:24:33.000000 powerbeatsvr-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:24:35.000000 powerbeatsvr-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:24:35.000000 powerbeatsvr-0.3.0/src/powerbeatsvr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:24:33.000000 powerbeatsvr-0.3.0/src/powerbeatsvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-25 22:24:33.000000 powerbeatsvr-0.3.0/src/powerbeatsvr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-25 22:24:33.000000 powerbeatsvr-0.3.0/src/powerbeatsvr/bs_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-25 22:24:33.000000 powerbeatsvr-0.3.0/src/powerbeatsvr/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15454 2023-06-25 22:24:33.000000 powerbeatsvr-0.3.0/src/powerbeatsvr/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:24:36.000000 powerbeatsvr-0.3.0/src/powerbeatsvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-25 22:24:35.000000 powerbeatsvr-0.3.0/src/powerbeatsvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-25 22:24:35.000000 powerbeatsvr-0.3.0/src/powerbeatsvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:24:35.000000 powerbeatsvr-0.3.0/src/powerbeatsvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-25 22:24:35.000000 powerbeatsvr-0.3.0/src/powerbeatsvr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 22:24:35.000000 powerbeatsvr-0.3.0/src/powerbeatsvr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 22:24:35.000000 powerbeatsvr-0.3.0/src/powerbeatsvr.egg-info/top_level.txt
```

### Comparing `powerbeatsvr-0.2.0/PKG-INFO` & `powerbeatsvr-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: powerbeatsvr
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convert beats saber levels to PowerBeatsVR
 Home-page: https://github.com/guysoft/PowerBeatsVR_song_writer
 Author: Guy Sheffer
 Author-email: gusyoft@gmail.com
 License: GPLv3
 Description: # PowerBeatsVR_song_writer
         Convert a BeatSaber level in to a PowerBeatsVR level.
-        Currently does not work. Because something in the PowerBeatsVR format makes no sense.
+        Walls might be buggy, notes work perfectly.
         
         
         ## Usage
         
         ### Website
         There is a website where you can convert downloaded file, its source code is in this repository too so you can request changes:
         https://powerbeatsvr.gnethomelinux.com/
```

### Comparing `powerbeatsvr-0.2.0/setup.py` & `powerbeatsvr-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 import sys
-version = "0.2.0"
+version = "0.3.0"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 install_requires=["pyunpack"]
 
 setuptools.setup(
```

### Comparing `powerbeatsvr-0.2.0/src/powerbeatsvr/bs_lib.py` & `powerbeatsvr-0.3.0/src/powerbeatsvr/bs_lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,35 @@
         #data = json.load(f)
     #return int(data["_beatsPerMinute"])
     
 NOTE_TYPE = {"BOMB": 3}
 OBSTACLE_TYPE = {"FULL_HEIGHT": 0,
                  "CROUCH": 1}
 
+VERSION_KEYS = {
+    2:
+    {
+        "_time": "_time",
+        "_lineIndex": "_lineIndex",
+        "_lineLayer": "_lineLayer",
+        "_duration": "_duration",
+        "_width": "_width",
+        "_height": None,
+    },
+    3:
+    {
+        "_time": "b",
+        "_lineIndex": "x",
+        "_lineLayer": "y",
+        "_duration": "d",
+        "_width": "w",
+        "_height": "h",
+    }
+}
+
 
 def get_data(bs_info_path):
     data = None
     with open(bs_info_path) as f:
         data = json.load(f)
     return {
         "bpm": int(data["_beatsPerMinute"]),
@@ -26,21 +47,21 @@
 
 # The width from each side in the center (the total width is twice this number)
 LEVEL_WITH = 1.1
 # Lowest point in the game map beneeth your center
 LEVEL_LOW = -0.5
 # Highest point in the map
 LEVEL_HIGH = 1.0
-def line_index_layer_to_position(note):
+def line_index_layer_to_position(note_x, note_y):
     # beat saber layer moves between 0-2
     # beat saber index moves between 0-3
     # max posy in beat saber = 0.5 - 1.0
     # max posx in beat saber = -1.3 - 1.3
-    position_x = -LEVEL_WITH + (2*LEVEL_WITH/3) * note["_lineIndex"]
-    position_y = LEVEL_LOW + (LEVEL_HIGH - LEVEL_LOW)/2 * note["_lineLayer"]
+    position_x = -LEVEL_WITH + (2*LEVEL_WITH/3) *note_x
+    position_y = LEVEL_LOW + (LEVEL_HIGH - LEVEL_LOW)/2 * note_y
     return [position_x, position_y]
 
 
 def obstacle_line_index_layer_to_position(obstacle):
     # index 0 to 3
     # width 0-4 (can be negative but it creates bugs in beat saber)
     # posy = 0.5 - 1.3
```

### Comparing `powerbeatsvr-0.2.0/src/powerbeatsvr/reader.py` & `powerbeatsvr-0.3.0/src/powerbeatsvr/reader.py`

 * *Files identical despite different names*

### Comparing `powerbeatsvr-0.2.0/src/powerbeatsvr/writer.py` & `powerbeatsvr-0.3.0/src/powerbeatsvr/writer.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,28 @@
 import sys
 import shutil
 import os
 from pyunpack import Archive
 import tempfile
 import powerbeatsvr.bs_lib as bs_lib
 import glob
-from powerbeatsvr.bs_lib import NOTE_TYPE, OBSTACLE_TYPE, line_index_layer_to_position, obstacle_line_index_layer_to_position
+from powerbeatsvr.bs_lib import NOTE_TYPE, OBSTACLE_TYPE, VERSION_KEYS, line_index_layer_to_position, obstacle_line_index_layer_to_position
 
 BS_LEVELS = ["Easy", "NormalStandard", "Normal", "HardStandard", "Hard", "Expert", "ExpertStandard", "ExpertPlusStandard", "ExpertPlus"]
 
-POWER_BEATS_VR_OBSTACLE_TYPES = {"FULL_HEIGHT": 0, "CROUCH": 7}
+POWER_BEATS_VR_OBSTACLE_TYPES = {
+    "FULL_HEIGHT": 0,
+    "CROUCH": 7,
+    "Double_Column": 1,
+    "Archway Center": 2,
+    "Archway Left": 3,
+    "Archway Right": 4,
+    "Opening Left": 5,
+    "Opening Right": 6,
+    }
 
 
 def ensure_dir(d, chmod=0o777):
     """
     Ensures a folder exists.
     Returns True if the folder already exists
     """
@@ -46,20 +55,37 @@
         "maxHighscore" : 0,
                 "isGenerated" : True,
         "beats": []}
     }
     return data
 
 def convert_action_type(note):
+    # In verson 2 there is a _type value for bombs and notes
+    # In version 3 its two seprate lists
     if note["_type"] == NOTE_TYPE["BOMB"]:
         action = "BallObstacle"
     else:
         action = "NormalBall"
     return action
 
+def merge_notes_and_bombs_v3(bs_note_data):
+    return_value = []
+    color_notes = []
+    bombs = []
+    for note in bs_note_data["colorNotes"]:
+        note["_type"] = note["c"]
+        color_notes.append(note)
+
+    for bomb in bs_note_data["bombNotes"]:
+        bomb["_type"] = NOTE_TYPE["BOMB"]
+        bombs.append(bomb)
+
+    return_value = color_notes + bombs
+    return sorted(return_value, key=lambda d: d['b'])
+
 class Map():
     def __init__(self, name, author="unknown", bpm=140, offset=0):
         self.data = create(name, author=author, bpm=bpm, offset=offset)
     
     def add_beat(self, difficulty, beat_no, actions, sub_beats=[]):
         beat = {
             "beatNo": beat_no,
@@ -83,68 +109,93 @@
         if beat_index is None:
             return None
         for i, sub_beat in enumerate(self.data[difficulty]["beats"][beat_index]["subBeats"]):
             if sub_beat["offset"] == offset:
                 return i
         return None
 
-    def add_obstacle(self, difficulty, obstacle):
-        current_time = obstacle["_time"]
+    def add_obstacle(self, difficulty, obstacle, version=2):
+        current_time = obstacle[VERSION_KEYS[version]["_time"]]
         current_beat = int(current_time)
         
         # Handle intiger beat, goes in actions
         beat_index = self.get_beat(current_beat, difficulty)
             
         if beat_index is None:
             self.add_beat(difficulty, beat_no=current_beat, actions=[], sub_beats=[])
         beat_index = self.get_beat(current_beat, difficulty)
         
         
         # Get obstacle data
-        x_position = obstacle["_lineIndex"]
-        bs_type = obstacle["_type"]
-        depth = obstacle["_duration"]
-        width = obstacle["_width"]
+        x_position = obstacle[VERSION_KEYS[version]["_lineIndex"]]
+
+        bs_type = None
+        if version == 2:
+            bs_type = obstacle["_type"]
+        depth = obstacle[VERSION_KEYS[version]["_duration"]]
+        width = obstacle[VERSION_KEYS[version]["_width"]]
         # y_position = x_position + width
         
         if depth == 0:
             return
         
-        if bs_type == OBSTACLE_TYPE["CROUCH"]:
-            
-            if width < 4:
-                # This is a crouch wall, but its not going all the way to the end, so we are adding fall hight wall in the air to simulate
-                power_beats_vr_type = POWER_BEATS_VR_OBSTACLE_TYPES["FULL_HEIGHT"]
+        if version == 2:
+            if bs_type == OBSTACLE_TYPE["CROUCH"]:
                 
-                # Take y from normal note location and x from obstacle position
-                # Dummy 0 for now
-                # TODO make this more pretty
-                obstacle["_lineLayer"] = 0
-                position = line_index_layer_to_position(obstacle)
-                position[0], _ = obstacle_line_index_layer_to_position(obstacle)
+                if width < 4:
+                    # This is a crouch wall, but its not going all the way to the end, so we are adding fall hight wall in the air to simulate
+                    power_beats_vr_type = POWER_BEATS_VR_OBSTACLE_TYPES["FULL_HEIGHT"]
+                    
+                    # Take y from normal note location and x from obstacle position
+                    # Dummy 0 for now
+                    # TODO make this more pretty
+                    obstacle["_lineLayer"] = 0
+                    position = line_index_layer_to_position(obstacle)
+                    position[0], _ = obstacle_line_index_layer_to_position(obstacle)
+                    
+                else:
+                    # Crouch wall with fall size
+                    
+                    power_beats_vr_type = POWER_BEATS_VR_OBSTACLE_TYPES["CROUCH"]
+                    # print(current_time / 140)
+                    
+                    
+                    # Taken from level editor, not sure if there are other ways to generate
+                    # hard coded because anyway in beat saber its _lineIndex and width 4
+                    position = [0, 0.472493290901184]
                 
-            else:
-                # Crouch wall with fall size
+            elif bs_type == OBSTACLE_TYPE["FULL_HEIGHT"]:
+                power_beats_vr_type = POWER_BEATS_VR_OBSTACLE_TYPES["FULL_HEIGHT"]
                 
+                position = obstacle_line_index_layer_to_position(obstacle)
+            else:
+                print("ERROR: Unknown wall type")
+                exit(1)
+            self.add_wall(current_time, position, difficulty, beat_index, power_beats_vr_type, depth, current_beat)
+
+        elif version == 3:
+            height = obstacle[VERSION_KEYS[version]["_height"]]
+            y_position = obstacle[VERSION_KEYS[version]["_lineLayer"]]
+
+            position = line_index_layer_to_position(x_position, y_position)
+
+            if height == 1 and width > 2:
                 power_beats_vr_type = POWER_BEATS_VR_OBSTACLE_TYPES["CROUCH"]
-                # print(current_time / 140)
-                
-                
-                # Taken from level editor, not sure if there are other ways to generate
-                # hard coded because anyway in beat saber its _lineIndex and width 4
-                position = [0, 0.472493290901184]
-            
-        elif bs_type == OBSTACLE_TYPE["FULL_HEIGHT"]:
-            power_beats_vr_type = POWER_BEATS_VR_OBSTACLE_TYPES["FULL_HEIGHT"]
-            
-            position = obstacle_line_index_layer_to_position(obstacle)
-        else:
-            print("ERROR: Unknown wall type")
-            exit(1)
-            
+
+                self.add_wall(current_time, position, difficulty, beat_index, power_beats_vr_type, depth, current_beat)
+
+            elif width == 1 and height > 2:
+                power_beats_vr_type = POWER_BEATS_VR_OBSTACLE_TYPES["FULL_HEIGHT"]
+                self.add_wall(current_time, position, difficulty, beat_index, power_beats_vr_type, depth, current_beat)
+
+            else:
+                print(f"Warning: Detected wall type that is not implemented width or height larger than 1 {[width, height]} location: {[x_position, y_position]}")
+
+
+    def add_wall(self, current_time, position, difficulty, beat_index, power_beats_vr_type, depth, current_beat):
         if current_time % 1 == 0.0:
             self.data[difficulty]["beats"][beat_index]["actions"].append({
                 "position" : position,
                 "action" : "WallObstacle",
                 "type" : power_beats_vr_type,
                 "depth" : depth
                 })
@@ -165,31 +216,33 @@
                 "action" : "WallObstacle",
                 "type" : power_beats_vr_type,
                 "depth" : depth
                 })
 
         return
 
-    def add_note(self, difficulty, note):
-        current_time = note["_time"]
+    def add_note(self, difficulty, note, version=2):
+        current_time = note[VERSION_KEYS[version]["_time"]]
         current_beat = int(current_time)
         
-        # Handle intiger beat, goes in actions
+        # Handle intager beat, goes in actions
         beat_index = self.get_beat(current_beat, difficulty)
             
         if beat_index is None:
             self.add_beat(difficulty, beat_no=current_beat, actions=[], sub_beats=[])
         beat_index = self.get_beat(current_beat, difficulty)
         
         
-        # Get obstacle data
-        x_position = note["_lineIndex"]
-        bs_type = note["_type"]
+        # Get notes data
+        x_position = note[VERSION_KEYS[version]["_lineIndex"]]
+
         action = convert_action_type(note)
-        position = line_index_layer_to_position(note)
+        note_x = note[VERSION_KEYS[version]["_lineIndex"]]
+        note_y = note[VERSION_KEYS[version]["_lineLayer"]]
+        position = line_index_layer_to_position(note_x, note_y)
             
         if current_time % 1 == 0.0:
             self.data[difficulty]["beats"][beat_index]["actions"].append({
                 "position" : position,
                 "action" : action
                 })
         else:
@@ -204,26 +257,64 @@
                 self.data[difficulty]["beats"][beat_index]["subBeats"].append(subbeat)
             index_of_sub_beat = self.get_sub_beat(difficulty, beat_index, offset)
             
             self.data[difficulty]["beats"][beat_index]["subBeats"][index_of_sub_beat]["actions"].append({
                 "position" : position,
                 "action" : action
                 })
+        return
 
-        return                
+
+    def get_map_version(self, bs_note_data):
+        version = bs_note_data.get("_version", None)
+        if version is not None:
+            return version
+        version = bs_note_data.get("version", None)
+        return version
+
+    def get_powerbeatsvr_notes_v3(self, bs_note_data, level):
+        notes_bombs = merge_notes_and_bombs_v3(bs_note_data)
+
+        for note in notes_bombs:
+            self.add_note(level, note, 3)
+        return
         
-    def get_powerbeatsvr_notes(self, bs_note_data, level):
+    def get_powerbeatsvr_notes_v2(self, bs_note_data, level):
         for note in bs_note_data["_notes"]:
-            self.add_note(level, note)
+            self.add_note(level, note, 2)
         return
-    
-    def get_powerbeatsvr_obstacles(self, bs_obstacle_data, level):
+
+    def get_powerbeatsvr_obstacles_v3(self, bs_note_data, level):
+        for obstacle in bs_note_data["obstacles"]:
+            self.add_obstacle(level, obstacle, 3)
+        return
+
+    def get_powerbeatsvr_obstacles_v2(self, bs_obstacle_data, level):
         for obstacle in bs_obstacle_data["_obstacles"]:
             # print(obstacle)
-            self.add_obstacle(level, obstacle)
+            self.add_obstacle(level, obstacle, 2)
+
+
+    def get_powerbeatsvr_notes(self, bs_note_data, level):
+        if self.get_map_version(bs_note_data) == "2.0.0":
+            return self.get_powerbeatsvr_notes_v2(bs_note_data, level)
+        elif self.get_map_version(bs_note_data).startswith("3."):
+            return self.get_powerbeatsvr_notes_v3(bs_note_data, level)
+        else:
+            raise Exception("unknown map version")
+        return
+
+    def get_powerbeatsvr_obstacles(self, bs_note_data, level):
+        if self.get_map_version(bs_note_data) == "2.0.0":
+            return self.get_powerbeatsvr_obstacles_v2(bs_note_data, level)
+        elif self.get_map_version(bs_note_data).startswith("3."):
+            return self.get_powerbeatsvr_obstacles_v3(bs_note_data, level)
+        else:
+            raise Exception("unknown map version")
+        return
             
 def get_bs_info_path(folder):
     options = ["Info.dat", "info.dat"]
     for option in options:
         if os.path.isfile(os.path.join(folder, option)):
             return os.path.join(folder, option)
```

### Comparing `powerbeatsvr-0.2.0/src/powerbeatsvr.egg-info/PKG-INFO` & `powerbeatsvr-0.3.0/src/powerbeatsvr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: powerbeatsvr
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convert beats saber levels to PowerBeatsVR
 Home-page: https://github.com/guysoft/PowerBeatsVR_song_writer
 Author: Guy Sheffer
 Author-email: gusyoft@gmail.com
 License: GPLv3
 Description: # PowerBeatsVR_song_writer
         Convert a BeatSaber level in to a PowerBeatsVR level.
-        Currently does not work. Because something in the PowerBeatsVR format makes no sense.
+        Walls might be buggy, notes work perfectly.
         
         
         ## Usage
         
         ### Website
         There is a website where you can convert downloaded file, its source code is in this repository too so you can request changes:
         https://powerbeatsvr.gnethomelinux.com/
```

