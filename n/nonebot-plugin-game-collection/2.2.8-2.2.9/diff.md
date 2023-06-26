# Comparing `tmp/nonebot_plugin_game_collection-2.2.8.tar.gz` & `tmp/nonebot_plugin_game_collection-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.2.8.tar", last modified: Sat Jun 24 17:04:14 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.2.9.tar", last modified: Sat Jun 24 22:56:07 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.2.8.tar` & `nonebot_plugin_game_collection-2.2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.189350 nonebot_plugin_game_collection-2.2.8/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.8/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-24 17:04:14.188849 nonebot_plugin_game_collection-2.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.125795 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    19529 2023-06-24 16:29:41.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    60126 2023-06-22 17:20:27.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.144312 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9182 2023-06-20 12:33:55.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    13713 2023-06-23 11:42:31.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    19332 2023-06-23 14:22:48.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    23191 2023-06-24 16:59:38.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    29223 2023-06-23 14:03:04.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/config.py
--rw-rw-rw-   0        0        0     5586 2023-06-20 12:48:06.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/data.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.151318 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.176339 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5335 2023-06-24 06:35:42.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.178341 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2278 2023-06-20 13:08:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.186848 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0    16012 2023-06-24 16:57:10.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1141 2023-06-23 21:24:50.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.135303 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-24 17:04:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1947 2023-06-24 17:04:14.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 17:04:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-24 17:04:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-24 17:04:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 17:04:14.189851 nonebot_plugin_game_collection-2.2.8/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-06-24 17:04:09.000000 nonebot_plugin_game_collection-2.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.588432 nonebot_plugin_game_collection-2.2.9/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.9/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-24 22:56:07.585929 nonebot_plugin_game_collection-2.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.525602 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    19529 2023-06-24 16:29:41.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    60126 2023-06-22 17:20:27.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.544118 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-20 12:33:55.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    13713 2023-06-23 11:42:31.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    19306 2023-06-24 22:54:29.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    23183 2023-06-24 22:54:29.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    29223 2023-06-23 14:03:04.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0     5586 2023-06-20 12:48:06.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.551124 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.577055 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5335 2023-06-24 06:35:42.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.579057 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-20 13:08:13.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.583927 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    16012 2023-06-24 16:57:10.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-23 21:24:50.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 22:56:07.535610 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1947 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-24 22:56:07.000000 nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 22:56:07.588432 nonebot_plugin_game_collection-2.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-06-24 22:56:02.000000 nonebot_plugin_game_collection-2.2.9/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.2.8/LICENSE` & `nonebot_plugin_game_collection-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/README.md` & `nonebot_plugin_game_collection-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Market.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from turtle import width
 from typing import Tuple
 from PIL import Image
 from nonebot.adapters.onebot.v11 import (
     Bot,
     MessageEvent,
     GroupMessageEvent,
     MessageSegment
```

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/Prop.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import random
 
 from .utils.utils import get_message_at
 from .utils.chart import linecard_to_png
 from .data import props_library, props_index, element_library
 from .config import bot_name, sign_gold, revolt_gold, max_bet_gold, gacha_gold
 
-from .Manager import data,BG_path
+from .Manager import data
 from . import Manager
 
 user_data = data.user
 group_data = data.group
```

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/data.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.2.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.8/setup.py` & `nonebot_plugin_game_collection-2.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.2.8',
+version='2.2.9',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

