# Comparing `tmp/une_ai-1.1.0.tar.gz` & `tmp/une_ai-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "une_ai-1.1.0.tar", last modified: Sun Jun 25 03:41:45 2023, max compression
+gzip compressed data, was "une_ai-1.1.1.tar", last modified: Mon Jun 26 09:12:31 2023, max compression
```

## Comparing `une_ai-1.1.0.tar` & `une_ai-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.356260 une_ai-1.1.0/
--rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-1.1.0/LICENSE
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-25 03:41:45.356094 une_ai-1.1.0/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-06-12 00:05:49.000000 une_ai-1.1.0/README.md
--rw-r--r--   0 jonathan   (501) staff       (20)      481 2023-06-25 03:39:31.000000 une_ai-1.1.0/pyproject.toml
--rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-06-25 03:41:45.356299 une_ai-1.1.0/setup.cfg
--rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-1.1.0/setup.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.347635 une_ai-1.1.0/src/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.348794 une_ai-1.1.0/src/une_ai/
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-1.1.0/src/une_ai/__init__.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.351290 une_ai-1.1.0/src/une_ai/assignments/
--rw-r--r--   0 jonathan   (501) staff       (20)      198 2023-06-17 05:23:26.000000 une_ai-1.1.0/src/une_ai/assignments/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)    12875 2023-06-25 01:46:33.000000 une_ai-1.1.0/src/une_ai/assignments/connect_four_base_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     9682 2023-06-25 02:57:40.000000 une_ai-1.1.0/src/une_ai/assignments/connect_four_game.py
--rw-r--r--   0 jonathan   (501) staff       (20)     7263 2023-06-04 07:45:17.000000 une_ai-1.1.0/src/une_ai/assignments/snake_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5982 2023-06-04 07:33:36.000000 une_ai-1.1.0/src/une_ai/assignments/snake_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.353944 une_ai-1.1.0/src/une_ai/models/
--rw-r--r--   0 jonathan   (501) staff       (20)     1323 2023-06-25 00:13:50.000000 une_ai-1.1.0/src/une_ai/models/MCTS_graph_node.py
--rw-r--r--   0 jonathan   (501) staff       (20)      254 2023-06-24 12:38:18.000000 une_ai-1.1.0/src/une_ai/models/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5409 2023-06-04 07:46:40.000000 une_ai-1.1.0/src/une_ai/models/agent.py
--rw-r--r--   0 jonathan   (501) staff       (20)      357 2023-06-04 03:18:52.000000 une_ai-1.1.0/src/une_ai/models/environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1083 2023-06-22 07:56:49.000000 une_ai-1.1.0/src/une_ai/models/game_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1312 2023-06-12 07:15:34.000000 une_ai-1.1.0/src/une_ai/models/graph_node.py
--rw-r--r--   0 jonathan   (501) staff       (20)     2198 2023-05-26 04:05:50.000000 une_ai-1.1.0/src/une_ai/models/grid_map.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5827 2023-06-24 06:33:53.000000 une_ai-1.1.0/src/une_ai/models/transposition_table.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.354700 une_ai-1.1.0/src/une_ai/tictactoe/
--rw-r--r--   0 jonathan   (501) staff       (20)       87 2023-06-25 01:53:59.000000 une_ai-1.1.0/src/une_ai/tictactoe/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1332 2023-06-25 02:53:44.000000 une_ai-1.1.0/src/une_ai/tictactoe/tictactoc_player.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5001 2023-06-25 02:58:21.000000 une_ai-1.1.0/src/une_ai/tictactoe/tictactoe_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.355699 une_ai-1.1.0/src/une_ai/vacuum/
--rw-r--r--   0 jonathan   (501) staff       (20)      186 2023-06-12 02:00:34.000000 une_ai-1.1.0/src/une_ai/vacuum/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)      910 2023-06-12 07:14:58.000000 une_ai-1.1.0/src/une_ai/vacuum/vacuum_dock_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     8119 2023-06-06 11:02:22.000000 une_ai-1.1.0/src/une_ai/vacuum/vacuum_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5938 2023-06-12 02:18:54.000000 une_ai-1.1.0/src/une_ai/vacuum/vacuum_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-25 03:41:45.349763 une_ai-1.1.0/src/une_ai.egg-info/
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)      978 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       19 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/requires.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-06-25 03:41:45.000000 une_ai-1.1.0/src/une_ai.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.260414 une_ai-1.1.1/
+-rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-1.1.1/LICENSE
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-26 09:12:31.260253 une_ai-1.1.1/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-06-12 00:05:49.000000 une_ai-1.1.1/README.md
+-rw-r--r--   0 jonathan   (501) staff       (20)      481 2023-06-26 09:11:57.000000 une_ai-1.1.1/pyproject.toml
+-rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-06-26 09:12:31.260479 une_ai-1.1.1/setup.cfg
+-rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-1.1.1/setup.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.253924 une_ai-1.1.1/src/
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.254947 une_ai-1.1.1/src/une_ai/
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-1.1.1/src/une_ai/__init__.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.256622 une_ai-1.1.1/src/une_ai/assignments/
+-rw-r--r--   0 jonathan   (501) staff       (20)      198 2023-06-17 05:23:26.000000 une_ai-1.1.1/src/une_ai/assignments/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)    12875 2023-06-25 01:46:33.000000 une_ai-1.1.1/src/une_ai/assignments/connect_four_base_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     9692 2023-06-26 09:10:11.000000 une_ai-1.1.1/src/une_ai/assignments/connect_four_game.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     7263 2023-06-04 07:45:17.000000 une_ai-1.1.1/src/une_ai/assignments/snake_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5992 2023-06-26 09:09:49.000000 une_ai-1.1.1/src/une_ai/assignments/snake_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.258732 une_ai-1.1.1/src/une_ai/models/
+-rw-r--r--   0 jonathan   (501) staff       (20)     1323 2023-06-25 00:13:50.000000 une_ai-1.1.1/src/une_ai/models/MCTS_graph_node.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      254 2023-06-24 12:38:18.000000 une_ai-1.1.1/src/une_ai/models/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5409 2023-06-04 07:46:40.000000 une_ai-1.1.1/src/une_ai/models/agent.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      357 2023-06-04 03:18:52.000000 une_ai-1.1.1/src/une_ai/models/environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1083 2023-06-22 07:56:49.000000 une_ai-1.1.1/src/une_ai/models/game_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1312 2023-06-12 07:15:34.000000 une_ai-1.1.1/src/une_ai/models/graph_node.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     2198 2023-05-26 04:05:50.000000 une_ai-1.1.1/src/une_ai/models/grid_map.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5827 2023-06-24 06:33:53.000000 une_ai-1.1.1/src/une_ai/models/transposition_table.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.259554 une_ai-1.1.1/src/une_ai/tictactoe/
+-rw-r--r--   0 jonathan   (501) staff       (20)       87 2023-06-25 01:53:59.000000 une_ai-1.1.1/src/une_ai/tictactoe/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1332 2023-06-25 02:53:44.000000 une_ai-1.1.1/src/une_ai/tictactoe/tictactoc_player.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5011 2023-06-26 09:10:25.000000 une_ai-1.1.1/src/une_ai/tictactoe/tictactoe_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.260044 une_ai-1.1.1/src/une_ai/vacuum/
+-rw-r--r--   0 jonathan   (501) staff       (20)      186 2023-06-12 02:00:34.000000 une_ai-1.1.1/src/une_ai/vacuum/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      910 2023-06-12 07:14:58.000000 une_ai-1.1.1/src/une_ai/vacuum/vacuum_dock_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     8119 2023-06-06 11:02:22.000000 une_ai-1.1.1/src/une_ai/vacuum/vacuum_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5948 2023-06-26 09:10:38.000000 une_ai-1.1.1/src/une_ai/vacuum/vacuum_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.255702 une_ai-1.1.1/src/une_ai.egg-info/
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-26 09:12:30.000000 une_ai-1.1.1/src/une_ai.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)      978 2023-06-26 09:12:31.000000 une_ai-1.1.1/src/une_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-06-26 09:12:31.000000 une_ai-1.1.1/src/une_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)       19 2023-06-26 09:12:31.000000 une_ai-1.1.1/src/une_ai.egg-info/requires.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-06-26 09:12:31.000000 une_ai-1.1.1/src/une_ai.egg-info/top_level.txt
```

### Comparing `une_ai-1.1.0/LICENSE` & `une_ai-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/PKG-INFO` & `une_ai-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une_ai
-Version: 1.1.0
+Version: 1.1.1
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `une_ai-1.1.0/README.md` & `une_ai-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/assignments/connect_four_base_environment.py` & `une_ai-1.1.1/src/une_ai/assignments/connect_four_base_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/assignments/connect_four_game.py` & `une_ai-1.1.1/src/une_ai/assignments/connect_four_game.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         for y in range(self._n_rows):
             for x in range(self._n_cols):
                 self._coordinates[y, x] = (x, y)
 
         fonts = pygame.font.get_fonts()
         self._font = fonts[0] # default to a random font
         # try to look among the most common fonts
-        test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica']
+        test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica', 'roboto']
         for font in test_fonts:
             if font in fonts:
                 self._font = font
                 break
 
         self.main()
```

### Comparing `une_ai-1.1.0/src/une_ai/assignments/snake_environment.py` & `une_ai-1.1.1/src/une_ai/assignments/snake_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/assignments/snake_game.py` & `une_ai-1.1.1/src/une_ai/assignments/snake_game.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         # update sensors with initial state
         self._agent.sense(self._environment)
         self._tick = tick
 
         fonts = pygame.font.get_fonts()
         self._font = fonts[0] # default to a random font
         # try to look among the most common fonts
-        test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica']
+        test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica', 'roboto']
         for font in test_fonts:
             if font in fonts:
                 self._font = font
                 break
 
         self.main()
```

### Comparing `une_ai-1.1.0/src/une_ai/models/MCTS_graph_node.py` & `une_ai-1.1.1/src/une_ai/models/MCTS_graph_node.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/models/agent.py` & `une_ai-1.1.1/src/une_ai/models/agent.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/models/game_environment.py` & `une_ai-1.1.1/src/une_ai/models/game_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/models/graph_node.py` & `une_ai-1.1.1/src/une_ai/models/graph_node.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/models/grid_map.py` & `une_ai-1.1.1/src/une_ai/models/grid_map.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/models/transposition_table.py` & `une_ai-1.1.1/src/une_ai/models/transposition_table.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/tictactoe/tictactoc_player.py` & `une_ai-1.1.1/src/une_ai/tictactoe/tictactoc_player.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/tictactoe/tictactoe_game.py` & `une_ai-1.1.1/src/une_ai/tictactoe/tictactoe_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self._agents['X'] = agent_X
         self._agents['O'] = agent_O
         self._environment = environment
         
         fonts = pygame.font.get_fonts()
         self._font = fonts[0] # default to a random font
         # try to look among the most common fonts
-        test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica']
+        test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica', 'roboto']
         for font in test_fonts:
             if font in fonts:
                 self._font = font
                 break
 
         self.main()
```

### Comparing `une_ai-1.1.0/src/une_ai/vacuum/vacuum_dock_environment.py` & `une_ai-1.1.1/src/une_ai/vacuum/vacuum_dock_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/vacuum/vacuum_environment.py` & `une_ai-1.1.1/src/une_ai/vacuum/vacuum_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.0/src/une_ai/vacuum/vacuum_game.py` & `une_ai-1.1.1/src/une_ai/vacuum/vacuum_game.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         # updating the sensors based on initial environment state
         self._agent.sense(self._environment)
 
         fonts = pygame.font.get_fonts()
         self._font = fonts[0] # default to a random font
         # try to look among the most common fonts
-        test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica']
+        test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica', 'roboto']
         for font in test_fonts:
             if font in fonts:
                 self._font = font
                 break
 
         self.main()
```

### Comparing `une_ai-1.1.0/src/une_ai.egg-info/PKG-INFO` & `une_ai-1.1.1/src/une_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une-ai
-Version: 1.1.0
+Version: 1.1.1
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `une_ai-1.1.0/src/une_ai.egg-info/SOURCES.txt` & `une_ai-1.1.1/src/une_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

