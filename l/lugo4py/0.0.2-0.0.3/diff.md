# Comparing `tmp/lugo4py-0.0.2.tar.gz` & `tmp/lugo4py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lugo4py-0.0.2.tar", last modified: Thu Feb 23 04:06:55 2023, max compression
+gzip compressed data, was "lugo4py-0.0.3.tar", last modified: Mon Jun 26 21:20:02 2023, max compression
```

## Comparing `lugo4py-0.0.2.tar` & `lugo4py-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 04:06:55.183717 lugo4py-0.0.2/
--rw-rw-r--   0 root         (0) root         (0)    35147 2023-02-22 23:28:00.000000 lugo4py-0.0.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     4537 2023-02-23 04:06:55.183717 lugo4py-0.0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4141 2023-02-23 02:54:11.000000 lugo4py-0.0.2/README.md
--rw-rw-r--   0 root         (0) root         (0)      373 2023-02-23 04:06:46.000000 lugo4py-0.0.2/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)      551 2023-02-23 04:06:55.183717 lugo4py-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 04:06:55.175709 lugo4py-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 04:06:55.179713 lugo4py-0.0.2/src/lugo4py/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6773 2023-02-23 02:15:54.000000 lugo4py-0.0.2/src/lugo4py/client.py
--rw-rw-r--   0 root         (0) root         (0)     1263 2023-02-23 02:15:54.000000 lugo4py-0.0.2/src/lugo4py/geo.py
--rw-rw-r--   0 root         (0) root         (0)      585 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/goal.py
--rw-rw-r--   0 root         (0) root         (0)     1661 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/loader.py
--rw-rw-r--   0 root         (0) root         (0)     3667 2023-02-23 02:15:54.000000 lugo4py-0.0.2/src/lugo4py/mapper.py
--rw-rw-r--   0 root         (0) root         (0)     1012 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/orientation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 04:06:55.183717 lugo4py-0.0.2/src/lugo4py/protos/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5182 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/broadcast_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     5946 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/broadcast_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     1860 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/health_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     3893 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/health_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     1389 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/physics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      159 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/physics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3820 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/remote_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    12109 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/remote_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     5029 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/server_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     3897 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/protos/server_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 04:06:55.183717 lugo4py-0.0.2/src/lugo4py/rl/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/rl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1848 2023-02-23 02:15:54.000000 lugo4py-0.0.2/src/lugo4py/rl/gym.py
--rw-rw-r--   0 root         (0) root         (0)     3794 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/rl/interfaces.py
--rw-rw-r--   0 root         (0) root         (0)     4218 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/rl/remote_control.py
--rw-rw-r--   0 root         (0) root         (0)     5741 2023-02-23 02:15:54.000000 lugo4py-0.0.2/src/lugo4py/rl/training_controller.py
--rw-rw-r--   0 root         (0) root         (0)     1708 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/rl/zombie.py
--rw-rw-r--   0 root         (0) root         (0)     8652 2023-02-23 02:15:54.000000 lugo4py-0.0.2/src/lugo4py/snapshot.py
--rw-rw-r--   0 root         (0) root         (0)     3821 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/specs.py
--rw-rw-r--   0 root         (0) root         (0)      955 2023-02-15 02:24:56.000000 lugo4py-0.0.2/src/lugo4py/stub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 04:06:55.179713 lugo4py-0.0.2/src/lugo4py.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     4537 2023-02-23 04:06:55.000000 lugo4py-0.0.2/src/lugo4py.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      975 2023-02-23 04:06:55.000000 lugo4py-0.0.2/src/lugo4py.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-02-23 04:06:55.000000 lugo4py-0.0.2/src/lugo4py.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)        8 2023-02-23 04:06:55.000000 lugo4py-0.0.2/src/lugo4py.egg-info/top_level.txt
+drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.184534 lugo4py-0.0.3/
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)    35147 2023-06-26 21:12:44.000000 lugo4py-0.0.3/LICENSE.txt
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     8030 2023-06-26 21:20:02.184534 lugo4py-0.0.3/PKG-INFO
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     7634 2023-06-26 21:12:44.000000 lugo4py-0.0.3/README.md
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)      373 2023-06-26 21:15:07.000000 lugo4py-0.0.3/pyproject.toml
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)      551 2023-06-26 21:20:02.184534 lugo4py-0.0.3/setup.cfg
+drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.180534 lugo4py-0.0.3/src/
+drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.180534 lugo4py-0.0.3/src/lugo4py/
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/__init__.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     6886 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/client.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     1343 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/geo.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)      629 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/goal.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     1004 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/interface.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     1604 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/loader.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     6826 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/lugo.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     3697 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/mapper.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     1012 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/orientation.py
+drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.184534 lugo4py-0.0.3/src/lugo4py/protos/
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/__init__.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)    10066 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/broadcast_pb2.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     5946 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/broadcast_pb2_grpc.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     2672 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/health_pb2.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     3893 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/health_pb2_grpc.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     2157 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/physics_pb2.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)      159 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/physics_pb2_grpc.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     7104 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/remote_pb2.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)    12109 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/remote_pb2_grpc.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     8935 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/server_pb2.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     3897 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/server_pb2_grpc.py
+drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.184534 lugo4py-0.0.3/src/lugo4py/rl/
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/__init__.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     3457 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/gym.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     2398 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/helper_bots.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     3741 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/interfaces.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     2473 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/remote_control.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     5510 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/training_controller.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     8136 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/snapshot.py
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     3821 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/specs.py
+drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.180534 lugo4py-0.0.3/src/lugo4py.egg-info/
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     8030 2023-06-26 21:20:02.000000 lugo4py-0.0.3/src/lugo4py.egg-info/PKG-INFO
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)     1005 2023-06-26 21:20:02.000000 lugo4py-0.0.3/src/lugo4py.egg-info/SOURCES.txt
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)        1 2023-06-26 21:20:02.000000 lugo4py-0.0.3/src/lugo4py.egg-info/dependency_links.txt
+-rw-rw-r--   0 aquer     (1000) aquer     (1000)        8 2023-06-26 21:20:02.000000 lugo4py-0.0.3/src/lugo4py.egg-info/top_level.txt
```

### Comparing `lugo4py-0.0.2/LICENSE.txt` & `lugo4py-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.2/setup.cfg` & `lugo4py-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.2/src/lugo4py/client.py` & `lugo4py-0.0.3/src/lugo4py/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,186 +1,172 @@
 import grpc
-import json
-import os
-import random
-import threading
-import asyncio
-import datetime
-import traceback
-from typing import Tuple, Callable, Awaitable, Any
 import time
+from concurrent.futures import ThreadPoolExecutor
+import traceback
+from typing import Callable, Iterator
+
+from . import lugo
 
-from .protos.physics_pb2 import Point, Vector
 from .protos import server_pb2
 from .protos import server_pb2_grpc as server_grpc
 
-from .stub import Bot, PLAYER_STATE
+from .interface import Bot, PLAYER_STATE
 from .loader import EnvVarLoader
-from .snapshot import defineState
+from .snapshot import define_state
+import threading
 
 PROTOCOL_VERSION = "1.0.0"
 
-RawTurnProcessor = Callable[[Any, Any], Awaitable[Any]]
+RawTurnProcessor = Callable[[lugo.OrderSet, lugo.GameSnapshot], lugo.OrderSet]
+
 
+# reference https://chromium.googlesource.com/external/github.com/grpc/grpc/+/master/examples/python/async_streaming/client.py
 class LugoClient(server_grpc.GameServicer):
 
     def __init__(self, server_add, grpc_insecure, token, teamSide, number, init_position):
-        self.callback = Callable[[server_pb2.GameSnapshot], server_pb2.OrderSet]
-        self.serverAdd = server_add
+        self._client = None
+        self.getting_ready_handler = lambda snapshot: None
+        self.callback = Callable[[lugo.GameSnapshot], lugo.OrderSet]
+        self.serverAdd = server_add + "?t=" + str(teamSide) + "-" + str(number)
         self.grpc_insecure = grpc_insecure
         self.token = token
         self.teamSide = teamSide
         self.number = number
         self.init_position = init_position
-
-        self._client = _get_client()
+        self._play_finished = threading.Event()
+        self._play_routine = None
 
     def set_client(self, client: server_grpc.GameStub):
         self._client = client
 
-    def set_initial_position(self, initial_position: Point):
+    def get_name(self):
+        return f"{'HOME' if self.teamSide == 0 else 'AWAY'}-{self.number}"
+
+    def set_initial_position(self, initial_position: lugo.Point):
         self.init_position = initial_position
 
-    def getting_ready_handler(self, snapshot : server_pb2.GameSnapshot):
-        print(f'Default getting ready handler called for {snapshot}')
+    def getting_ready_handler(self, snapshot: lugo.GameSnapshot):
+        print(f'Default getting ready handler called for ')
 
-    def setReadyHandler(self, newReadyHandler):
-        self.getting_ready_handler = newReadyHandler
+    def set_ready_handler(self, new_ready_handler):
+        self.getting_ready_handler = new_ready_handler
 
-    async def play(self, callback: Callable[[server_pb2.GameSnapshot], server_pb2.OrderSet]):
+    def play(self, executor: ThreadPoolExecutor, callback: Callable[[lugo.GameSnapshot], lugo.OrderSet],
+             on_join: Callable[[], None]) -> threading.Event:
         self.callback = callback
-        team = os.environ.get("BOT_TEAM").upper()
-        number = int(os.environ.get("BOT_NUMBER"))
-        token = os.environ.get("BOT_TOKEN")
-
-        join_request = server_pb2.JoinRequest(
-            token=token,
-            team_side=server_pb2.Team.Side.Value(team),
-            number=number,
-            init_position=self.initial_position,
-        )
-
-        retries = 3
-        for i in range(retries):
-            try:
-                await self._init( join_request)
-            except Exception as e:
-                print(e)
-                time.sleep(1)
-
-    
-    async def _init(self, join_request: server_pb2.JoinRequest) -> None:
-        for snapshot in self._client.JoinATeam(join_request):
-            try:
-                if snapshot.state == server_pb2.GameSnapshot.State.OVER:
-                    break 
-
-                elif snapshot.state == server_pb2.GameSnapshot.State.LISTENING:
-                    
-                    orders = self.callback(snapshot)
-
-                    if orders:
-                        self._client.SendOrders(orders)
-                        pass
-                    else:
-                        print(f"[turn #{snapshot.turn}] bot did not return orders")
+        log_with_time(f"{self.get_name()} Starting to play")
+        return self._bot_start(executor, callback, on_join)
 
-                elif snapshot.state == server_pb2.GameSnapshot.State.GET_READY:
-                    await self.getting_ready_handler(snapshot)
+    def play_as_bot(self, executor: ThreadPoolExecutor, bot: Bot, on_join: Callable[[], None]) -> threading.Event:
+        self.set_ready_handler(bot.getting_ready)
+        log_with_time(f"{self.get_name()} Playing as bot")
+
+        def processor(orders: lugo.OrderSet, snapshot: lugo.GameSnapshot) -> lugo.OrderSet:
+            player_state = define_state(
+                snapshot, self.number, self.teamSide)
+            if self.number == 1:
+                orders = bot.as_goalkeeper(
+                    orders, snapshot, player_state)
+            else:
+                if player_state == PLAYER_STATE.DISPUTING_THE_BALL:
+                    orders = bot.on_disputing(orders, snapshot)
+                elif player_state == PLAYER_STATE.DEFENDING:
+                    orders = bot.on_defending(orders, snapshot)
+                elif player_state == PLAYER_STATE.SUPPORTING:
+                    orders = bot.on_supporting(orders, snapshot)
+                elif player_state == PLAYER_STATE.HOLDING_THE_BALL:
+                    orders = bot.on_holding(orders, snapshot)
+            return orders
+
+        return self._bot_start(executor, processor, on_join)
+
+    def _bot_start(self, executor: ThreadPoolExecutor, processor: RawTurnProcessor,
+                   on_join: Callable[[], None]) -> threading.Event:
+        log_with_time(f"{self.get_name()} Starting bot {self.teamSide}-{self.number}")
+        if self.grpc_insecure:
+            channel = grpc.insecure_channel(self.serverAdd)
+        else:
+            channel = grpc.secure_channel(
+                self.serverAdd, grpc.ssl_channel_credentials())
+        try:
+            grpc.channel_ready_future(channel).result(timeout=5)
+        except grpc.FutureTimeoutError:
+            raise Exception(f"timed out waiting to connect to the game server ({self.serverAdd})")
 
-            except Exception as e:
-                print("internal error processing turn", e)
-                traceback.print_exc()
+        self.channel = channel
+        self._client = server_grpc.GameStub(channel)
 
+        join_request = server_pb2.JoinRequest(
+            token=self.token,
+            team_side=self.teamSide,
+            number=self.number,
+            init_position=self.init_position,
+        )
 
-    async def play_as_bot(self, bot: Bot):
-        join_request = server_pb2.JoinRequest(token = self.token, team_side = self.teamSide, number = self.number, init_position = self.init_position)
-        # join_request = server_pb2.JoinRequest({'token':self.token,  'team_side' : self.teamSide, 'number' : self.number, 'init_position': self.init_position})
-        print(join_request)
-
-        retries = 3
-        for i in range(retries):
-            try:
-                await self._bot_start(bot, join_request)
-            except Exception as e:
-                print(e)
-                traceback.print_exc()
-                time.sleep(1)
-
-
-
-    async def _bot_start(self, bot: Bot, join_request: server_pb2.JoinRequest) -> None:
-        print("Bot Starting")
-        for snapshot in self._client.JoinATeam(join_request):
-            try:
-                if snapshot.state == server_pb2.GameSnapshot.State.OVER:
-                    break 
-
-                elif snapshot.state == server_pb2.GameSnapshot.State.LISTENING:
-
-                    playerState = defineState(snapshot, self.number, self.teamSide)
+        response_iterator = self._client.JoinATeam(join_request)
+        on_join()
+        self._play_routine = executor.submit(self._response_watcher, response_iterator, processor)
+        return self._play_finished
+
+    def stop(self):
+        log_with_time(
+            f"{self.get_name()} stopping bot - you may need to kill the process if there is no messages coming from "
+            f"the server")
+        self._play_routine.cancel()
+        self._play_finished.set()
+
+    def wait(self):
+        self._play_finished.wait(timeout=None)
+
+    def _response_watcher(
+            self,
+            response_iterator: Iterator[lugo.GameSnapshot],
+            # snapshot,
+            processor: RawTurnProcessor) -> None:
+        try:
+            for snapshot in response_iterator:
+                if snapshot.state == lugo.State.OVER:
+                    log_with_time(
+                        f"{self.get_name()} All done! {lugo.State.OVER}")
+                    break
+                elif self._play_finished.is_set():
+                    break
+                elif snapshot.state == lugo.State.LISTENING:
                     orders = server_pb2.OrderSet()
-
-                    if (self.number == 1):
-                        orders = bot.asGoalkeeper(orders, snapshot, playerState)
-
-                    else:
-                        if playerState == PLAYER_STATE.DISPUTING_THE_BALL:
-                            # print(f"[turn #{snapshot.turn}] will call disputing")
-                            orders = bot.onDisputing(orders, snapshot)
-                        elif playerState == PLAYER_STATE.DEFENDING:
-                            # print(f"[turn #{snapshot.turn}] will call defending")
-                            orders = bot.onDefending(orders, snapshot)
-                        elif playerState == PLAYER_STATE.SUPPORTING:
-                            # print(f"[turn #{snapshot.turn}] will call supporting")
-                            orders = bot.onSupporting(orders, snapshot)
-                        elif playerState == PLAYER_STATE.HOLDING_THE_BALL:
-                            # print(f"[turn #{snapshot.turn}] will call holding")
-                            orders = bot.onHolding(orders, snapshot)
+                    orders.turn = snapshot.turn
+                    try:
+                        orders = processor(orders, snapshot)
+                    except Exception as e:
+                        traceback.print_exc()
+                        log_with_time(f"{self.get_name()}bot processor error: {e}")
 
                     if orders:
                         self._client.SendOrders(orders)
-
                     else:
-                        print(f"[turn #{snapshot.turn}] bot did not return orders")
+                        log_with_time(
+                            f"{self.get_name()} [turn #{snapshot.turn}] bot {self.teamSide}-{self.number} did not return orders")
+                elif snapshot.state == lugo.State.GET_READY:
+                    self.getting_ready_handler(snapshot)
+
+            self._play_finished.set()
+        except grpc.RpcError as e:
+            if grpc.StatusCode.INVALID_ARGUMENT == e.code():
+                log_with_time(f"{self.get_name()} did not connect {e.details()}")
+        except Exception as e:
+            log_with_time(f"{self.get_name()} internal error processing turn: {e}")
+            traceback.print_exc()
 
-                elif snapshot.state == server_pb2.GameSnapshot.State.GET_READY:
-                    await bot.gettingReady(snapshot)
 
-            except Exception as e:
-                print("internal error processing turn", e)
-                traceback.print_exc()
-
-    @classmethod
-    def new_client(cls, initial_position: Point) -> 'LugoClient':
-        instance = cls()
-        instance.set_initial_position(initial_position)
-        client = _get_client()
-        instance.set_client(client)
-        return instance
-
-def NewClientFromConfig(config: EnvVarLoader, initialPosition: Point) -> LugoClient:
+def NewClientFromConfig(config: EnvVarLoader, initialPosition: lugo.Point) -> LugoClient:
     return LugoClient(
-        config.getGrpcUrl(),
-        config.getGrpcInsecure(),
-        config.getBotToken(),
-        config.getBotTeamSide(),
-        config.getBotNumber(),
+        config.get_grpc_url(),
+        config.get_grpc_insecure(),
+        config.get_bot_token(),
+        config.get_bot_team_side(),
+        config.get_bot_number(),
         initialPosition,
     )
 
-def _get_config() -> Tuple[str, bool]:
-    url = os.environ.get("BOT_GRPC_URL")
-    if url is None:
-        raise Exception("BOT_GRPC_URL is not set")
-    insecure = os.environ.get("BOT_GRPC_INSECURE", "false").lower() == "true"
-    return url, insecure
-
-
-def _get_client() -> server_grpc.GameStub:
-    url, insecure = _get_config()
-    if insecure:
-        channel = grpc.insecure_channel(url)
-    else:
-        channel = grpc.secure_channel(url, grpc.ssl_channel_credentials())
-    return server_grpc.GameStub(channel)
 
+def log_with_time(msg):
+    current_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
+    print(f"{current_time}: {msg}")
```

### Comparing `lugo4py-0.0.2/src/lugo4py/loader.py` & `lugo4py-0.0.3/src/lugo4py/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,49 @@
-from .protos import server_pb2_grpc
-from .protos import server_pb2
+import os
 
 from . import specs
+from .protos import server_pb2
 
-import os
 
 class EnvVarLoader:
 
     def __init__(self):
         self._grpcUrl = ""
         self._grpcInsecure = True
         self._botTeamSide = None
         self._botNumber = None
         self._botToken = ""
 
         if "BOT_TEAM" not in os.environ:
             raise SystemError("missing BOT_TEAM env value")
-        
 
         if "BOT_NUMBER" not in os.environ:
             raise SystemError("missing BOT_NUMBER env value")
 
         # the Lugo address
-        self._grpcUrl = os.environ["BOT_GRPC_URL"] if "BOT_GRPC_URL" in os.environ else 'localhost:5000'
-        if "BOT_GRPC_INSECURE" in os.environ:
-            self._grpcUrl = bool(os.environ["BOT_GRPC_INSECURE"])
-        
+        self._grpcUrl = os.environ.get('BOT_GRPC_URL', 'localhost:5000')
+        self._grpcInsecure = bool(os.environ.get('BOT_GRPC_INSECURE', 'false'))
+
         # defining bot side
-        self._botTeamSide = server_pb2.Team.Side.HOME if os.environ["BOT_TEAM"].upper() == 'HOME' else server_pb2.Team.Side.AWAY
+        self._botTeamSide = server_pb2.Team.Side.HOME if os.environ[
+                                                             "BOT_TEAM"].upper() == 'HOME' else server_pb2.Team.Side.AWAY
         self._botNumber = int(os.environ["BOT_NUMBER"])
-        if (self._botNumber < 1 or self._botNumber > specs.MAX_PLAYERS):
-            raise  SystemError('invalid bot number {self._botNumber}, must be between 1 and {specs.MAX_PLAYERS}')
+        if self._botNumber < 1 or self._botNumber > specs.MAX_PLAYERS:
+            raise SystemError('invalid bot number {self._botNumber}, must be between 1 and {specs.MAX_PLAYERS}')
 
         # // the token is mandatory in official matches, but you may ignore in local games
         self._botToken = os.environ["BOT_TOKEN"] if "BOT_TOKEN" in os.environ else ''
-    
 
-    def getGrpcUrl(self):
+    def get_grpc_url(self):
         return self._grpcUrl
 
-    def getGrpcInsecure(self):
+    def get_grpc_insecure(self):
         return self._grpcInsecure
-    
-    def getBotTeamSide(self):
+
+    def get_bot_team_side(self):
         return self._botTeamSide
 
-    def getBotNumber(self):
+    def get_bot_number(self):
         return self._botNumber
 
-    def getBotToken(self):
+    def get_bot_token(self):
         return self._botToken
-
```

### Comparing `lugo4py-0.0.2/src/lugo4py/mapper.py` & `lugo4py-0.0.3/src/lugo4py/mapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,119 +2,121 @@
 from .protos import server_pb2
 
 from . import specs
 
 from math import floor
 
 # ErrMinCols defines an error for invalid number of cols
-ErrMinCols = AttributeError("number of cols lower the minimum")
+ERR_MIN_COLS = AttributeError("number of cols lower the minimum")
 # ErrMaxCols defines an error for invalid number of cols
-ErrMaxCols = AttributeError("number of cols higher the maximum")
+ERR_MAX_COLS = AttributeError("number of cols higher the maximum")
 # ErrMinRows defines an error for invalid number of rows
-ErrMinRows = AttributeError("number of rows lower the minimum")
+ERR_MIN_ROWS = AttributeError("number of rows lower the minimum")
 # ErrMaxRows defines an error for invalid number of rows
-ErrMaxRows = AttributeError("number of rows higher the maximum")
-
+ERR_MAX_ROWS = AttributeError("number of rows higher the maximum")
 
 # MinCols Define the min number of cols allowed on the field division by the Mapper
-MinCols = 4
+MIN_COLS = 4
 # MinRows Define the min number of rows allowed on the field division by the Mapper
-MinRows = 2
+MIN_ROWS = 2
 # MaxCols Define the max number of cols allowed on the field division by the Mapper
-MaxCols = 200
+MAX_COLS = 200
 # MaxRows Define the max number of rows allowed on the field division by the Mapper
-MaxRows = 100
+MAX_ROWS = 100
 
 
-def mirrorCoordsToAway(center):
+def mirror_coords_to_away(center):
     mirrored = physics_pb2.Point()
     mirrored.x = (specs.MAX_X_COORDINATE - center.x)
     mirrored.y = (specs.MAX_Y_COORDINATE - center.y)
     return mirrored
 
+
+class Region:
+    def __init__(self, col: int, row: int, side: server_pb2.Team.Side, center: physics_pb2.Point, mapper):
+        self.col = col
+        self.row = row
+        self.side = side
+        self.center = center
+        self.positioner = mapper
+
+    def eq(self, region):
+        return region.get_col() == self.col and region.side == self.side and region.get_row() == self.row
+
+    def get_col(self):
+        return self.col
+
+    def get_row(self):
+        return self.row
+
+    def get_center(self):
+        return self.center
+
+    def to_string(self):
+        return f"{{{self.col}, {self.row}}}"
+
+    def front(self):
+        return self.positioner.get_region(max(self.col + 1, 0), self.row)
+
+    def back(self):
+        return self.positioner.get_region(max(self.col - 1, 0), self.row)
+
+    def left(self):
+        return self.positioner.get_region(self.col, max(self.row + 1, 0))
+
+    def right(self):
+        return self.positioner.get_region(self.col, max(self.row - 1, 0))
+
+
 class Mapper:
     def __init__(self, cols: int, rows: int, side: server_pb2.Team.Side):
-        if (cols < MinCols):
-            raise ErrMinCols
+        if cols < MIN_COLS:
+            raise ERR_MIN_COLS
 
-        if (cols > MaxCols):
-            raise ErrMaxCols
+        if cols > MAX_COLS:
+            raise ERR_MAX_COLS
 
-        if (rows < MinRows):
-            raise ErrMinRows
+        if rows < MIN_ROWS:
+            raise ERR_MIN_ROWS
 
-        if (rows > MaxRows):
-            raise ErrMaxRows
+        if rows > MAX_ROWS:
+            raise ERR_MAX_ROWS
 
         self.cols = cols
         self.rows = rows
         self.side = side
         self.regionWidth = specs.MAX_X_COORDINATE / cols
         self.regionHeight = specs.MAX_Y_COORDINATE / rows
 
-    def getRegion(self, col: int, row: int): 
+    def get_region(self, col: int, row: int) -> Region:
         col = max(0, col)
         col = min(self.cols - 1, col)
 
         row = max(0, row)
         row = min(self.rows - 1, row)
 
         center = physics_pb2.Point()
         center.x = (round((col * self.regionWidth) + (self.regionWidth / 2)))
         center.y = (round((row * self.regionHeight) + (self.regionHeight / 2)))
 
-        if (self.side == server_pb2.Team.Side.AWAY):
-            center = mirrorCoordsToAway(center)
+        if self.side == server_pb2.Team.Side.AWAY:
+            center = mirror_coords_to_away(center)
 
         return Region(
             col,
             row,
             self.side,
             center,
             self,
         )
 
-    def getRegionFromPoint(self, point: physics_pb2.Point):
-        if (self.side == server_pb2.Team.Side.AWAY):
-            point = mirrorCoordsToAway(point)
+    def get_region_from_point(self, point: physics_pb2.Point):
+        if self.side == server_pb2.Team.Side.AWAY:
+            point = mirror_coords_to_away(point)
 
         cx = floor(point.x / self.regionWidth)
         cy = floor(point.y / self.regionHeight)
         col = min(cx, self.cols - 1)
         row = min(cy, self.rows - 1)
-        return self.getRegion(col, row)
-
-class Region:
-    def __init__(self, col:int , row:int, side:server_pb2.Team.Side, center:physics_pb2.Point, positioner:Mapper):
-        self.col = col
-        self.row = row
-        self.side = side
-        self.center = center
-        self.positioner = positioner
-
-    def eq(self, region): 
-        return region.getCol() == self.col and region.side == self.side and region.getRow() == self.row
-
-    def getCol(self):
-        return self.col
-
-    def getRow(self):
-        return self.row
-
-    def getCenter(self):
-        return self.center
-
-    def toString(self):
-        return "{"+self.col+","+self.row+"}"
-
-    def front(self):
-        return self.positioner.getRegion(max(self.col + 1, 0), self.row)
-
-    def back(self): 
-        return self.positioner.getRegion(max(self.col - 1, 0), self.row)
-
-    def left(self): 
-        return self.positioner.getRegion(self.col, max(self.row + 1, 0))
+        return self.get_region(col, row)
 
-    def sright(self): 
-        return self.positioner.getRegion(self.col, max(self.row - 1, 0))
```

### Comparing `lugo4py-0.0.2/src/lugo4py/orientation.py` & `lugo4py-0.0.3/src/lugo4py/orientation.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.2/src/lugo4py/protos/broadcast_pb2_grpc.py` & `lugo4py-0.0.3/src/lugo4py/protos/broadcast_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.2/src/lugo4py/protos/health_pb2.py` & `lugo4py-0.0.3/src/lugo4py/protos/health_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,45 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: health.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0chealth.proto\x12\x0egrpc.health.v1\"%\n\x12HealthCheckRequest\x12\x0f\n\x07service\x18\x01 \x01(\t\"\xa9\x01\n\x13HealthCheckResponse\x12\x41\n\x06status\x18\x01 \x01(\x0e\x32\x31.grpc.health.v1.HealthCheckResponse.ServingStatus\"O\n\rServingStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVING\x10\x01\x12\x0f\n\x0bNOT_SERVING\x10\x02\x12\x13\n\x0fSERVICE_UNKNOWN\x10\x03\x32\xae\x01\n\x06Health\x12P\n\x05\x43heck\x12\".grpc.health.v1.HealthCheckRequest\x1a#.grpc.health.v1.HealthCheckResponse\x12R\n\x05Watch\x12\".grpc.health.v1.HealthCheckRequest\x1a#.grpc.health.v1.HealthCheckResponse0\x01\x42#Z!github.com/lugobots/lugo4go/protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'health_pb2', globals())
+
+
+_HEALTHCHECKREQUEST = DESCRIPTOR.message_types_by_name['HealthCheckRequest']
+_HEALTHCHECKRESPONSE = DESCRIPTOR.message_types_by_name['HealthCheckResponse']
+_HEALTHCHECKRESPONSE_SERVINGSTATUS = _HEALTHCHECKRESPONSE.enum_types_by_name['ServingStatus']
+HealthCheckRequest = _reflection.GeneratedProtocolMessageType('HealthCheckRequest', (_message.Message,), {
+  'DESCRIPTOR' : _HEALTHCHECKREQUEST,
+  '__module__' : 'health_pb2'
+  # @@protoc_insertion_point(class_scope:grpc.health.v1.HealthCheckRequest)
+  })
+_sym_db.RegisterMessage(HealthCheckRequest)
+
+HealthCheckResponse = _reflection.GeneratedProtocolMessageType('HealthCheckResponse', (_message.Message,), {
+  'DESCRIPTOR' : _HEALTHCHECKRESPONSE,
+  '__module__' : 'health_pb2'
+  # @@protoc_insertion_point(class_scope:grpc.health.v1.HealthCheckResponse)
+  })
+_sym_db.RegisterMessage(HealthCheckResponse)
+
+_HEALTH = DESCRIPTOR.services_by_name['Health']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z!github.com/lugobots/lugo4go/proto'
   _HEALTHCHECKREQUEST._serialized_start=32
   _HEALTHCHECKREQUEST._serialized_end=69
   _HEALTHCHECKRESPONSE._serialized_start=72
```

### Comparing `lugo4py-0.0.2/src/lugo4py/protos/health_pb2_grpc.py` & `lugo4py-0.0.3/src/lugo4py/protos/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.2/src/lugo4py/protos/remote_pb2_grpc.py` & `lugo4py-0.0.3/src/lugo4py/protos/remote_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.2/src/lugo4py/protos/server_pb2_grpc.py` & `lugo4py-0.0.3/src/lugo4py/protos/server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.2/src/lugo4py/rl/interfaces.py` & `lugo4py-0.0.3/src/lugo4py/rl/interfaces.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,82 @@
-from ..protos.server_pb2 import GameSnapshot, OrderSet
-from  abc import ABC, abstractmethod
-import asyncio
-from typing import Tuple, Callable, Awaitable, Any
+from abc import ABC, abstractmethod
+from typing import Callable, Any
+
+from .. import lugo
+
 
 #
 # The TrainingController is passed to your Training function to give you control of the game flow.
 #
+
+
 class TrainingController(ABC):
     #
-    #This method should be called whenever your need to reset the game to an initial state.
+    # This method should be called whenever your need to reset the game to an initial state.
     #
     @abstractmethod
-    async def setRandomState(self):
+    def set_environment(self, data):
         pass
 
     #
     # Use this method to get the inputs that will be used by your model. E.g. if you are using tensor flow, you may
     # return the tensors used to feed your network.
     #
     @abstractmethod
-    async def getInputs(self):
+    def get_state(self):
         pass
 
     #
     # Use this method to pass that action picked by you model. It will return the reward and `done` values got from
     # your BotTrainer.
     # @param action
     # @returns {Promise<{reward: number, done: boolean}>}
     #
     @abstractmethod
-    async def update(self, action):
+    def update(self, action):
         pass
+
     #
     # Stops the training
     #
+
     @abstractmethod
-    async def stop(self):
+    def stop(self):
         pass
+
+
 #
 # The BotTrainer is used by the Gym class to play the game as a bot and to control the game state when needed.
 # It is NOT your learning agent!
 #
+
+
 class BotTrainer(ABC):
 
     #
     # createNewInitialState should create the initial scenario for each game.
     #
     # IMPORTANT!! Note that this method should define the new state directly on the game server. So you MUST
     # use the remote control client to change the game elements' position/state
     #
     @abstractmethod
-    async def createNewInitialState(self):
+    def set_environment(self, data):
         pass
 
     #
     # getInputs is called in each training step.
     # The training function will call this method to receive whatever inputs you want to use in your neural network.
     # Example, if you have 3 sensors, or 3 tensors, etc.
     #
     # This method must read the game snapshot and define input values and return it
     #
     # @param {GameSnapshot} snapshot - The current game state
     #
     @abstractmethod
-    async def getInputs (self, snapshot: GameSnapshot):
+    def get_state(self, snapshot: lugo.GameSnapshot):
         pass
 
     #
     # play define the orders that will be sent to the game server based on the `action` sent by your training function.
     #
     # IMPORTANT:
     # Do not confuse this method role with an agent! Your agent will define the `action` inside your training function.
@@ -76,28 +85,27 @@
     # @param {OrderSet} orderSet - used to define the orders that will be sent to the server. Your bot should set the orders
     #                     and return it to the server.
     # @param {GameSnapshot} snapshot - The current game state
     # @param {any} action - Value passed by your training function to the TrainingController `update` method
     #
     #
     @abstractmethod
-    async def play(self, orderSet: OrderSet, snapshot: GameSnapshot, action):
+    def play(self, order_set: lugo.OrderSet, snapshot: lugo.GameSnapshot, action) -> lugo.OrderSet:
         pass
 
     #
     # This method is called by the TrainingController right after your bot play a turn of the game.
     # It must compare the two states and return the reward and a boolean `done` to indicate that the game each the end.
     #
     # Your bot may evaluate turn by turn, or comparing the final game state to the initial state.
     # However, if you want to compare with the initial state, your bot trainer will have to store the initial
     # state when the method `createNewInitialState` is called.
     #
     # @param {GameSnapshot} previousSnapshot - The current game state
     # @param {GameSnapshot} newSnapshot - The current game state
     #
     @abstractmethod
-    async def evaluate(previousSnapshot: GameSnapshot, newSnapshot: GameSnapshot):
+    def evaluate(self, previous_snapshot: lugo.GameSnapshot, new_snapshot: lugo.GameSnapshot) -> Any:
         pass
 
 
-
-# TrainingFunction = Callable[TrainingController, Awaitable[None]]
+TrainingFunction = Callable[[TrainingController], None]
```

### Comparing `lugo4py-0.0.2/src/lugo4py/rl/training_controller.py` & `lugo4py-0.0.3/src/lugo4py/rl/training_controller.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,150 +1,149 @@
 import asyncio
-from remote_control import RemoteControl
-# from ..protos.remote_pb2_grpc import RemoteStub
+from .remote_control import RemoteControl
 from .interfaces import TrainingController, BotTrainer, TrainingFunction
 from ..protos.server_pb2 import GameSnapshot, OrderSet
+import threading
+from concurrent.futures import ThreadPoolExecutor
+import time
 
-delay = lambda ms : asyncio.sleep(ms)
 
-class TrainingCrl(TrainingController):
 
-    def __init__(self, remoteControl: RemoteControl, bot: BotTrainer, onReadyCallback: TrainingFunction):
-        self.remoteControl = remoteControl
-        self.trainingHasStarted = False
-        self.lastSnapshot = GameSnapshot()
 
-        self.waitingForAction = False
+class TrainingCrl(TrainingController):
 
+    def __init__(self, executor: ThreadPoolExecutor, remoteControl: RemoteControl, bot: BotTrainer, onReadyCallback: TrainingFunction):
+        self._gotNextState = lambda snapshot: print("got first snapshot")
+        self.logger = lambda msg: print(f'set debugger')
+        self.previousState = None
+        self.remoteControl = remoteControl  # type: RemoteControl
+        self.onReady = onReadyCallback
+        self.trainingHasStarted = False
+        self.lastSnapshot = None  # type: GameSnapshot
+        self.onListeningMode = False
+        self.OrderSet = None
         self.cycleSeq = 0
-        
-        self.debugging_log = True
-        self.stopRequested = False
+        self.bot = bot  # type: BotTrainer
+        self.debugging_log = False
+        self.stopRequested = threading.Event()
+        self.trainingExecutor = executor
+        self.resumeListeningPhase = lambda action: print(
+            'resumeListeningPhase not defined yet - should wait the initialise it on the first "update" call')
 
-        #self.gotNewAction = async print('gotNewAction not defined yet - should wait the initialise it on the first "update" call')
+    def set_environment(self, data):
+        self.logger('Reset state')
+        try:
+            self.lastSnapshot = self.bot.set_environment(data)
+            return self.bot.get_state(self.lastSnapshot)
+        except Exception as e:
+            print('bot trainer failed to create initial state: ', e)
+            raise e
 
-        self.onReady = onReadyCallback
-        self.bot = bot
-        self.remoteControl = remoteControl
+    def get_state(self):
+        try:
+            self.cycleSeq = self.cycleSeq + 1
+            self.logger('get state')
+            return self.bot.get_state(self.lastSnapshot)
+        except Exception as e:
+            print('bot trainer failed to return inputs from a particular state', e)
+            raise e
+
+    def update(self, action: any):
+        self.logger('received action from training bot')
+        if not self.onListeningMode:
+            raise ValueError('faulty synchrony - got a new action when was still processing the last one')
 
-    async def setRandomState(self):
-        self._debug('Reset state')
         try:
-            self.lastSnapshot = await self.bot.createNewInitialState()
+            previousState = self.lastSnapshot
+            self.OrderSet.turn = self.lastSnapshot.turn
+            updatedOrderSet = self.bot.play(self.OrderSet, self.lastSnapshot, action)
 
-        except Exception as e: 
-            print('bot trainer failed to create initial state', e)
-            raise e
+            self.logger('got order set, passing down')
 
-    def getInputs(self):
-        try: 
-            self.cycleSeq = self.cycleSeq + 1 
-            self._debug('get state')
-            return self.bot.getInputs(self.lastSnapshot)
-        except Exception as e: 
-            print('bot trainer failed to return inputs from a particular state', e)
+            self.resumeListeningPhase(updatedOrderSet)
+            #time.sleep(2.4)  # before calling next turn, let's wait just a bit to ensure the server got our order
+            self.lastSnapshot = self.wait_until_next_listening_state()
+
+            self.logger('got new snapshot after order has been sent')
+
+            if self.stopRequested.is_set():
+                return None
+
+            # TODO: if I want to skip the net N turns? I should be able too
+            self.logger(f"update finished (turn {self.lastSnapshot.turn} waiting for next action)")
+        except Exception as e:
+            print('failed send new action to the server: ', e)
             raise e
-        
-    
 
-    #  return Promise< reward: number done: boolean > 
-    async def update(self, action: any):
-        self._debug('UPDATE')
-        if not self.waitingForAction:
-            raise RuntimeError("faulty synchrony - got a new action when was still processing the last one")
-        
-
-        self.previousState = self.lastSnapshot
-        self._debug('got action for turn $self.lastSnapshot.getTurn()')
-        self.lastSnapshot = await self.gotNewAction(action)
-        self._debug('got new snapshot after order has been sent')
-
-        if (self.stopRequested):
-            return {'done': True, 'reward': 0}
-        
-
-        # TODO: if I want to skip the net N turns? I should be able too
-        self._debug('update finished (turn $self.lastSnapshot.getTurn() waiting for next action')
-        try: 
-            returnDict = await self.bot.evaluate(self.previousState, self.lastSnapshot)
-            return returnDict
-        except Exception as e: 
+        try:
+            return self.bot.evaluate(previousState, self.lastSnapshot)
+        except Exception as e:
             print('bot trainer failed to evaluate game state', e)
             raise e
 
-    def _gotNextState (self, newState: GameSnapshot): 
-        self._debug('No one waiting for the next state')
-    
-
-    async def gameTurnHandler(self, orderSet, snapshot):
-        self._debug('new turn')
-        if (self.waitingForAction): 
-            raise RuntimeError("faulty synchrony - got new turn while waiting for order (check the lugo 'timer-mode')")
-        
+    def gameTurnHandler(self, order_set, snapshot):
+        if self.stopRequested.is_set():
+            self.logger('skipping turn handler because the stop request')
+            return None
+        self.logger('new turn')
+        if self.onListeningMode:
+            raise RuntimeError(
+                "faulty synchrony - got new turn while waiting for order (check the lugo 'timer-mode')")
+
         self._gotNextState(snapshot)
+        self.OrderSet = order_set
+
+        waiter = threading.Event()
+        new_order_set = None
+
+        def resume(updated_order_set):
+            nonlocal new_order_set
+            new_order_set = updated_order_set
+            waiter.set()
+            self.logger(f'Sending new action')
+
+        self.resumeListeningPhase = resume
+        self.onListeningMode = True
+        if self.trainingHasStarted is False:
+            self.trainingExecutor.submit(self.onReady, self, self.stopRequested)
+            self.trainingHasStarted = True
+            self.logger(f'the training has started')
+
+        self.logger(f'Waiting get new update!')
+        waiter.wait(timeout=5)
+        self.logger(f'order sent to the game server')
+        return new_order_set
+
+    def wait_until_next_listening_state(self) -> GameSnapshot:
+        try:
+            self.onListeningMode = False
+            waiter = threading.Event()
+
+            new_snapshot = None
+            def resume(newGameSnapshot):
+                nonlocal new_snapshot
+                new_snapshot = newGameSnapshot
+                waiter.set()
+
+            self._gotNextState = resume
+
+
+            waiterResumeListening = threading.Event()
+            self.trainingExecutor.submit(self.remoteControl.resume_listening, waiterResumeListening)
+            waiterResumeListening.wait()
+
+            waiter.wait(timeout=3)
+            if new_snapshot is None:
+                raise RuntimeError(
+                    "timed out waiting for the next listening state - check the training controller")
+
+            self.logger(f'resume_listening: {new_snapshot.turn}')
+
+            return new_snapshot
+        except Exception as e:
+            self.logger(f'failed to send the orders to the server {e}')
+            raise
+
+    def stop(self):
+        self.stopRequested.set()
+
 
-        return await new Promise(async (resolve, reject) => 
-            const maxWait = setTimeout(() => 
-                if (self.stopRequested) 
-                    return resolve(orderSet)
-                
-                console.error('max wait for a new action')
-                reject()
-            , 5000)
-            if (self.stopRequested) 
-                self._debug('stop requested - will not defined call back for new actions')
-                resolve(orderSet)
-                clearTimeout(maxWait)
-                return null
-            
-
-            self.gotNewAction = async (newAction) => 
-                self._debug('sending new action')
-                clearTimeout(maxWait)
-                return new Promise<GameSnapshot>((resolveTurn, rejectTurn) => 
-                    try 
-                        self.waitingForAction = false
-                        self._gotNextState = (newState) => 
-                            self._debug('Returning result for new action (snapshot of turn $newState.getTurn())')
-                            resolveTurn(newState)
-                        
-                        self._debug('sending order for turn $snapshot.getTurn() based on action')
-                        orderSet.setTurn(self.lastSnapshot.getTurn())
-                        self.bot.play(orderSet, snapshot, newAction).then((orderSet) => 
-                            resolve(orderSet)// sending the orders wh
-                            self._debug('order sent, calling next turn')
-                            return delay(80)// why? ensure the server got the order?
-                        ).then(() => 
-                            self._debug('RESUME NOW!')
-                            return self.remoteControl.resumeListening()
-                        ).then(() => 
-                            self._debug('listening resumed')
-                        )
-                     catch (e) 
-                        reject()
-                        rejectTurn()
-                        console.error('failed to send the orders to the server', e)
-                    
-                )
-            
-            self.waitingForAction = true
-            self._debug('gotNewAction defined, waiting for action (has started: $self.trainingHasStarted)')
-            if (!self.trainingHasStarted) 
-                self.onReady(this)
-                self.trainingHasStarted = true
-                self._debug('the training has started')
-            
-
-        )
-    
-
-    async stop() 
-        self.stopRequested = true
-    
-
-    _debug(msg) 
-        if (self.debugging_log) 
-            console.log('[$self.cycleSeq] $msg')
-            
-async def asyncToSync(asyncOriginalFunc):
-    const result = await asyncOriginalFunc()
-    return  result
```

### Comparing `lugo4py-0.0.2/src/lugo4py/specs.py` & `lugo4py-0.0.3/src/lugo4py/specs.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.2/src/lugo4py.egg-info/SOURCES.txt` & `lugo4py-0.0.3/src/lugo4py.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 README.md
 pyproject.toml
 setup.cfg
 src/lugo4py/__init__.py
 src/lugo4py/client.py
 src/lugo4py/geo.py
 src/lugo4py/goal.py
+src/lugo4py/interface.py
 src/lugo4py/loader.py
+src/lugo4py/lugo.py
 src/lugo4py/mapper.py
 src/lugo4py/orientation.py
 src/lugo4py/snapshot.py
 src/lugo4py/specs.py
-src/lugo4py/stub.py
 src/lugo4py.egg-info/PKG-INFO
 src/lugo4py.egg-info/SOURCES.txt
 src/lugo4py.egg-info/dependency_links.txt
 src/lugo4py.egg-info/top_level.txt
 src/lugo4py/protos/__init__.py
 src/lugo4py/protos/broadcast_pb2.py
 src/lugo4py/protos/broadcast_pb2_grpc.py
@@ -25,11 +26,11 @@
 src/lugo4py/protos/physics_pb2_grpc.py
 src/lugo4py/protos/remote_pb2.py
 src/lugo4py/protos/remote_pb2_grpc.py
 src/lugo4py/protos/server_pb2.py
 src/lugo4py/protos/server_pb2_grpc.py
 src/lugo4py/rl/__init__.py
 src/lugo4py/rl/gym.py
+src/lugo4py/rl/helper_bots.py
 src/lugo4py/rl/interfaces.py
 src/lugo4py/rl/remote_control.py
-src/lugo4py/rl/training_controller.py
-src/lugo4py/rl/zombie.py
+src/lugo4py/rl/training_controller.py
```

