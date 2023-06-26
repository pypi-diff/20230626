# Comparing `tmp/cgsubmit-1.2.0.tar.gz` & `tmp/cgsubmit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgsubmit-1.2.0.tar", last modified: Sun Jun 11 08:06:01 2023, max compression
+gzip compressed data, was "cgsubmit-1.2.1.tar", last modified: Mon Jun 26 16:39:19 2023, max compression
```

## Comparing `cgsubmit-1.2.0.tar` & `cgsubmit-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:06:01.984577 cgsubmit-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-11 08:06:01.984577 cgsubmit-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:06:01.984577 cgsubmit-1.2.0/cgsubmit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/cgsubmit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/cgsubmit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:06:01.984577 cgsubmit-1.2.0/cgsubmit/api/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/cgsubmit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/cgsubmit/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:06:01.984577 cgsubmit-1.2.0/cgsubmit/games/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/cgsubmit/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/cgsubmit/games/games.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:06:01.984577 cgsubmit-1.2.0/cgsubmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-11 08:06:01.000000 cgsubmit-1.2.0/cgsubmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-11 08:06:01.000000 cgsubmit-1.2.0/cgsubmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 08:06:01.000000 cgsubmit-1.2.0/cgsubmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-11 08:06:01.000000 cgsubmit-1.2.0/cgsubmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 08:06:01.000000 cgsubmit-1.2.0/cgsubmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 08:06:01.988577 cgsubmit-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-11 08:05:48.000000 cgsubmit-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:39:19.202005 cgsubmit-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-26 16:39:19.202005 cgsubmit-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:39:19.198005 cgsubmit-1.2.1/cgsubmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/cgsubmit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/cgsubmit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:39:19.198005 cgsubmit-1.2.1/cgsubmit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/cgsubmit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/cgsubmit/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:39:19.198005 cgsubmit-1.2.1/cgsubmit/games/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/cgsubmit/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/cgsubmit/games/games.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:39:19.198005 cgsubmit-1.2.1/cgsubmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-26 16:39:19.000000 cgsubmit-1.2.1/cgsubmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 16:39:19.000000 cgsubmit-1.2.1/cgsubmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:39:19.000000 cgsubmit-1.2.1/cgsubmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 16:39:19.000000 cgsubmit-1.2.1/cgsubmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 16:39:19.000000 cgsubmit-1.2.1/cgsubmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:39:19.202005 cgsubmit-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 16:39:00.000000 cgsubmit-1.2.1/setup.py
```

### Comparing `cgsubmit-1.2.0/LICENSE` & `cgsubmit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.2.0/PKG-INFO` & `cgsubmit-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.2.0
+Version: 1.2.1
 Summary: Analyse your submit in codingame competitions.
-Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
-Author: FrequentlyMissedDeadlines
-Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
+Author-email: FrequentlyMissedDeadlines <FrequentlyMissedDeadlines+cgsubmit@gmail.com>
+Project-URL: Homepage, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
+Keywords: CodinGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build](https://github.com/FrequentlyMissedDeadlines/cgsubmit/actions/workflows/python-package.yml/badge.svg)](https://github.com/FrequentlyMissedDeadlines/cgsubmit/actions/workflows/python-package.yml)
 [![Publish](https://github.com/FrequentlyMissedDeadlines/cgsubmit/actions/workflows/python-publish.yml/badge.svg)](https://github.com/FrequentlyMissedDeadlines/cgsubmit/actions/workflows/python-publish.yml)
 [![Version](https://img.shields.io/pypi/v/cgsubmit)](https://pypi.org/project/cgsubmit)
 [![Version](https://img.shields.io/pypi/pyversions/cgsubmit)](https://pypi.org/project/cgsubmit)
```

### Comparing `cgsubmit-1.2.0/README.md` & `cgsubmit-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.2.0/cgsubmit/games/games.py` & `cgsubmit-1.2.1/cgsubmit/games/games.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,72 @@
 class Games:
     def __init__(self, games):
         self.games = games
         self.pseudo = self.find_pseudo(games)
         self.number_by_id = self.find_game_by_id(games)
         self.win, self.lost = self.get_win_and_lost(games, self.pseudo)
-    
+
     def find_pseudo(self, games) -> str:
-        player1 = ''
-        player2 = ''
+        player1 = ""
+        player2 = ""
 
         i = 0
         while i < len(games):
-            if len(games[i]['players']) <= 1:
+            if len(games[i]["players"]) <= 1:
                 i = i + 1
                 continue
-            if player1 == '':
-                player1 = games[i]['players'][0]['nickname']
-                player2 = games[i]['players'][1]['nickname']
+            if player1 == "":
+                player1 = games[i]["players"][0]["nickname"]
+                player2 = games[i]["players"][1]["nickname"]
             else:
-                if player1 == games[i]['players'][0]['nickname'] and player2 != games[i]['players'][1]['nickname'] or \
-                    player1 == games[i]['players'][1]['nickname'] and player2 != games[i]['players'][0]['nickname']:
+                if (
+                    player1 == games[i]["players"][0]["nickname"]
+                    and player2 != games[i]["players"][1]["nickname"]
+                    or player1 == games[i]["players"][1]["nickname"]
+                    and player2 != games[i]["players"][0]["nickname"]
+                ):
                     return player1
-                if player1 != games[i]['players'][0]['nickname'] and player2 == games[i]['players'][1]['nickname'] or \
-                    player1 != games[i]['players'][1]['nickname'] and player2 == games[i]['players'][0]['nickname']:
+                if (
+                    player1 != games[i]["players"][0]["nickname"]
+                    and player2 == games[i]["players"][1]["nickname"]
+                    or player1 != games[i]["players"][1]["nickname"]
+                    and player2 == games[i]["players"][0]["nickname"]
+                ):
                     return player2
             i = i + 1
-        
-        raise Exception('Not enough games played to guess who is the right player. You must play against at least 2 different opponents.')
-    
+
+        raise Exception(
+            "Not enough games played to guess who is the right player. You must play against at least 2 different opponents."
+        )
+
     def find_game_by_id(self, games) -> dict:
         number_by_id = {}
 
         for i in range(len(games)):
-            number_by_id[games[i]['gameId']] = len(games) - i
-        
+            number_by_id[games[i]["gameId"]] = len(games) - i
+
         return number_by_id
-    
+
     def get_win_and_lost(self, games, pseudo):
-        wins = [a for a in games if ('nickname' in a['players'][0] and a['players'][0]['nickname'] == pseudo and a['players'][0]['position'] == 0) or \
-                (len(a['players']) > 1 and 'nickname' in a['players'][1] and a['players'][1]['nickname'] == pseudo and a['players'][1]['position'] == 0)]
-        losts = [a['gameId'] for a in games if a not in wins]
+        wins = [
+            a
+            for a in games
+            if (
+                "nickname" in a["players"][0]
+                and a["players"][0]["nickname"] == pseudo
+                and a["players"][0]["position"] == 0
+            )
+            or (
+                len(a["players"]) > 1
+                and "nickname" in a["players"][1]
+                and a["players"][1]["nickname"] == pseudo
+                and a["players"][1]["position"] == 0
+            )
+        ]
+        losts = [a["gameId"] for a in games if a not in wins]
         return (wins, losts)
-    
+
     def get_timeouts(self, lost_games):
-        self.timeouts = [a for a in lost_games if a['scores'][0] == -1 or a['scores'][1] == -1]
-        return self.timeouts
+        self.timeouts = [
+            a for a in lost_games if a["scores"][0] == -1 or a["scores"][1] == -1
+        ]
+        return self.timeouts
```

### Comparing `cgsubmit-1.2.0/cgsubmit.egg-info/PKG-INFO` & `cgsubmit-1.2.1/cgsubmit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.2.0
+Version: 1.2.1
 Summary: Analyse your submit in codingame competitions.
-Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
-Author: FrequentlyMissedDeadlines
-Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
+Author-email: FrequentlyMissedDeadlines <FrequentlyMissedDeadlines+cgsubmit@gmail.com>
+Project-URL: Homepage, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
+Keywords: CodinGame
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build](https://github.com/FrequentlyMissedDeadlines/cgsubmit/actions/workflows/python-package.yml/badge.svg)](https://github.com/FrequentlyMissedDeadlines/cgsubmit/actions/workflows/python-package.yml)
 [![Publish](https://github.com/FrequentlyMissedDeadlines/cgsubmit/actions/workflows/python-publish.yml/badge.svg)](https://github.com/FrequentlyMissedDeadlines/cgsubmit/actions/workflows/python-publish.yml)
 [![Version](https://img.shields.io/pypi/v/cgsubmit)](https://pypi.org/project/cgsubmit)
 [![Version](https://img.shields.io/pypi/pyversions/cgsubmit)](https://pypi.org/project/cgsubmit)
```

