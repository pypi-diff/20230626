# Comparing `tmp/telekinesis-0.1.81.tar.gz` & `tmp/telekinesis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telekinesis-0.1.81.tar", last modified: Mon Jun 26 18:06:29 2023, max compression
+gzip compressed data, was "telekinesis-0.1.9.tar", last modified: Fri Jun 11 08:51:43 2021, max compression
```

## Comparing `telekinesis-0.1.81.tar` & `telekinesis-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:06:29.956117 telekinesis-0.1.81/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 18:06:18.000000 telekinesis-0.1.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-26 18:06:29.956117 telekinesis-0.1.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 18:06:18.000000 telekinesis-0.1.81/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:06:29.956117 telekinesis-0.1.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-26 18:06:18.000000 telekinesis-0.1.81/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:06:29.956117 telekinesis-0.1.81/telekinesis/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-26 18:06:18.000000 telekinesis-0.1.81/telekinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-06-26 18:06:18.000000 telekinesis-0.1.81/telekinesis/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26657 2023-06-26 18:06:18.000000 telekinesis-0.1.81/telekinesis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-26 18:06:18.000000 telekinesis-0.1.81/telekinesis/cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-26 18:06:18.000000 telekinesis-0.1.81/telekinesis/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    48548 2023-06-26 18:06:18.000000 telekinesis-0.1.81/telekinesis/telekinesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:06:29.956117 telekinesis-0.1.81/telekinesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-26 18:06:29.000000 telekinesis-0.1.81/telekinesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-26 18:06:29.000000 telekinesis-0.1.81/telekinesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:06:29.000000 telekinesis-0.1.81/telekinesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 18:06:29.000000 telekinesis-0.1.81/telekinesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 18:06:29.000000 telekinesis-0.1.81/telekinesis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:06:29.956117 telekinesis-0.1.81/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-26 18:06:18.000000 telekinesis-0.1.81/test/test_00_walkthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 18:06:18.000000 telekinesis-0.1.81/test/test_01_encode_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-26 18:06:18.000000 telekinesis-0.1.81/test/test_02_garbage_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-26 18:06:18.000000 telekinesis-0.1.81/test/test_03_subscribe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-26 18:06:18.000000 telekinesis-0.1.81/test/test_04_request_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-26 18:06:18.000000 telekinesis-0.1.81/test/test_05_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-26 18:06:18.000000 telekinesis-0.1.81/test/test_06_state_diffing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 08:51:43.629891 telekinesis-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-06-11 08:51:33.000000 telekinesis-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-06-11 08:51:43.629891 telekinesis-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-06-11 08:51:33.000000 telekinesis-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-11 08:51:43.629891 telekinesis-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2021-06-11 08:51:33.000000 telekinesis-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 08:51:43.625891 telekinesis-0.1.9/telekinesis/
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27480 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24725 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5045 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40593 2021-06-11 08:51:33.000000 telekinesis-0.1.9/telekinesis/telekinesis.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 08:51:43.629891 telekinesis-0.1.9/telekinesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-11 08:51:43.000000 telekinesis-0.1.9/telekinesis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 08:51:43.629891 telekinesis-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_00_walkthrough.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1148 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_01_subscribe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_02_garbage_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_03_request_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-06-11 08:51:33.000000 telekinesis-0.1.9/test/test_04_state_diffing.py
```

### Comparing `telekinesis-0.1.81/LICENSE` & `telekinesis-0.1.9/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Telekinesis, Inc.
+Copyright (c) 2020 Elias Neuman
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `telekinesis-0.1.81/PKG-INFO` & `telekinesis-0.1.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: telekinesis
-Version: 0.1.81
+Version: 0.1.9
 Summary: Open Source, End-to-End Encrypted, Anywhere-to-Anywhere, Remote Procedure Calls.
 Home-page: https://github.com/telekinesis-cloud/telekinesis
 Author: Telekinesis, Inc.
 Author-email: support@telekinesis.cloud
+License: UNKNOWN
+Description: # Telekinesis - Python Package
+        
+        See [telekinesis github repo](https://github.com/e-neuman/telekinesis)
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Telekinesis - Python Package
-
-See [telekinesis github repo](https://github.com/e-neuman/telekinesis)
```

### Comparing `telekinesis-0.1.81/setup.py` & `telekinesis-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="telekinesis",
-    version="0.1.81",
+    version="0.1.9",
     author="Telekinesis, Inc.",
     author_email="support@telekinesis.cloud",
     description="Open Source, End-to-End Encrypted, Anywhere-to-Anywhere, Remote Procedure Calls.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/telekinesis-cloud/telekinesis",
     packages=setuptools.find_packages(),
-    install_requires=["websockets", "cryptography", "bson", "ujson", "packaging"],
+    install_requires=["websockets", "cryptography", "makefun", "bson", "ujson", "packaging"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

### Comparing `telekinesis-0.1.81/telekinesis/__init__.py` & `telekinesis-0.1.9/telekinesis/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from .client import Session, Connection, Channel, Route
 from .broker import Broker
-from .telekinesis import Telekinesis, inject_first_arg, block_arg_evaluation, State
+from .telekinesis import Telekinesis, inject_first_arg, State
 from .helpers import Entrypoint, authenticate, create_entrypoint
-from .cryptography import PrivateKey, PublicKey, SharedKey, Token
-from . import cryptography
 
 from pkg_resources import get_distribution
 
 __version__ = get_distribution(__name__).version
 
 __all__ = [
     "__version__",
@@ -17,11 +15,9 @@
     "authenticate",
     "create_entrypoint",
     "Session",
     "Connection",
     "Channel",
     "Route",
     "inject_first_arg",
-    "block_arg_evaluation",
     "State",
-    "cryptography",
 ]
```

### Comparing `telekinesis-0.1.81/telekinesis/broker.py` & `telekinesis-0.1.9/telekinesis/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,555 +1,633 @@
+import base64
 import logging
+import time
 import os
 import asyncio
-import time
-from packaging import version
-import re
+import bson
+import zlib
+from collections import deque, OrderedDict
 from pkg_resources import get_distribution
+import hashlib
 
-import ujson
 import websockets
+import ujson
 
-from .cryptography import PrivateKey, PublicKey, Token, InvalidSignature
-from .client import Route
+from .cryptography import PrivateKey, PublicKey, SharedKey, Token, InvalidSignature
 
 
 class Connection:
-    def __init__(self, websocket):
-        self.MIN_CLIENT_VERSION = "0.1.59"
-        self.websocket = websocket
+    def __init__(self, session, url="ws://localhost:8776"):
+        self.RESEND_TIMEOUT = 2  # sec
+        self.MAX_SEND_RETRIES = 3
+
+        self.session = session
+        self.url = url
         self.logger = logging.getLogger(__name__)
-        self.session = None
-        self.channels = set()
-        self.tasks = set()
+        self.websocket = None
+        self.t_offset = 0
+        self.broker_id = None
+        self.entrypoint = None
 
-    async def handshake(self, sessions, broker_key, entrypoint, peers):
-        challenge = os.urandom(32) + int(time.time()).to_bytes(4, "big")
+        self.is_connecting_lock = asyncio.Event()
+        self.awaiting_ack = OrderedDict()
 
-        await self.websocket.send(challenge)
-        m = await asyncio.wait_for(self.websocket.recv(), 15)
+        session.connections.add(self)
 
-        signature, session_id, client_challenge, metadata_raw = m[:64], m[64:152].decode(), m[152:184], m[184:]
-        metadata = ujson.loads(metadata_raw.decode())
+        self.listener = asyncio.get_event_loop().create_task(self.listen())
 
-        if version.parse(metadata["version"]) < version.parse(self.MIN_CLIENT_VERSION):
-            err_message = f'Incompatible version {metadata["version"]} < {self.MIN_CLIENT_VERSION}'
-            await self.websocket.send(err_message.encode())
-            raise Exception(err_message)
+    async def reconnect(self):
+        if self.is_connecting_lock.is_set():
+            self.is_connecting_lock.clear()
+            if self.listener:
+                self.listener.cancel()
 
-        PublicKey(session_id).verify(signature, challenge)
+            self.listener = asyncio.get_event_loop().create_task(self.listen())
 
-        await self.websocket.send(
-            broker_key.sign(client_challenge)
-            + broker_key.public_serial().encode()
-            + ujson.dumps({
-                "entrypoint": entrypoint and entrypoint.to_dict(),
-                "peers": peers,
-            }, escape_forward_slashes=False).encode()
-        )
+        await self.is_connecting_lock.wait()
 
-        if session_id not in sessions:
-            sessions[session_id] = Session(session_id)
+    async def _connect(self):
+        self.logger.info("%s connecting", self.session.session_key.public_serial()[:4])
+        if self.websocket:
+            await self.websocket.close()
 
-        self.session = sessions[session_id]
-        self.session.connections.add(self)
+        self.websocket = await websockets.connect(self.url)
 
-        return self
+        challenge = await self.websocket.recv()
+        t_broker = int.from_bytes(challenge[-4:], "big")
 
-    async def close(self, sessions, remove=True):
-        try:
-            await self.websocket.close()
-            for channel in self.channels:
-                if self in channel.connections:
-                    channel.connections.remove(self)
-                if not channel.connections:
-                    self.session.channels.pop(channel.channel_id, None)
-
-            if remove:
-                if self in self.session.connections:
-                    self.session.connections.remove(self)
-
-                self.session.broker_connections.pop(self, None)
-
-                if not self.session.channels and not self.session.broker_connections and not self.session.connections:
-                    sessions.pop(self.session.session_id, None)
-
-                await asyncio.gather(*(x for x in self.tasks if x.done()))
-                # print([x for x in self.tasks if not x.done()])
-                [x.cancel() for x in self.tasks if not x.done()]
-        except Exception:
-            self.logger.error("Exception when closing %s", self.session.session_id[:4], exc_info=True)
+        self.t_offset = int(time.time()) - t_broker
+        signature = self.session.session_key.sign(challenge)
 
+        pk = self.session.session_key.public_serial().encode()
 
-class Session:
-    def __init__(self, session_id):
-        self.session_id = session_id
-        self.channels = {}
-        self.expecting_channels = {}
-        self.connections = set()
-        self.broker_connections = {}
-        self.cached_tokens = {}
-
-    async def expect_channel(self, channel_id):
-        if channel_id not in self.channels:
-            list(self.connections)[0].logger.info("awaiting channel %s", channel_id[:4])
-            event = asyncio.Event()
-            self.expecting_channels[channel_id] = event
-            try:
-                await asyncio.wait_for(event.wait(), 2)
-                self.expecting_channels.pop(channel_id, None)
-            except asyncio.exceptions.TimeoutError:
-                pass
-        return self.channels.get(channel_id)
+        sent_challenge = os.urandom(32)
+        sent_metadata = {"version": get_distribution(__name__.split(".")[0]).version}
+        await self.websocket.send(
+            signature + pk + sent_challenge + ujson.dumps(sent_metadata, escape_forward_slashes=False).encode()
+        )
 
+        m = await asyncio.wait_for(self.websocket.recv(), 15)
 
-class Channel:
-    def __init__(self, session, channel_id, is_public):
-        self.session = session
-        self.channel_id = channel_id
-        self.is_public = is_public
-        self.connections = set()
+        if m[: len("Incompatible")] == b"Incompatible":
+            raise Exception(m.decode())
 
-    def close(self):
-        for connection in self.connections:
-            connection.channels.remove(self)
+        broker_signature, broker_id, metadata = m[:64], m[64:152].decode(), ujson.loads(m[152:].decode())
+        PublicKey(broker_id).verify(broker_signature, sent_challenge)
 
-        self.session.channels.pop(self.channel_id)
+        self.broker_id = broker_id
+        self.entrypoint = Route(**metadata.get("entrypoint")) if metadata.get("entrypoint") else None
 
-    async def validate_token_chain(self, source_id, tokens, broker):
-        if (source_id == self.session.session_id) or self.is_public:
-            return True
+        headers = []
+        for token, prev_token in self.session.issued_tokens.values():
+            headers.append(("token", ("issue", token.encode(), prev_token and prev_token.encode())))
+        for channel in self.session.channels.values():
+            listen_dict = channel.route.to_dict()
+            listen_dict["is_public"] = channel.is_public
+            listen_dict.pop("tokens")
+            headers.append(("listen", listen_dict))
+        await self.send(headers)
 
-        if not tokens:
-            broker.logger.info("||| no tokens")
-            return False
+        self.is_connecting_lock.set()
 
-        asset = self.channel_id
-        last_receiver = self.session.session_id
-        max_depth = None
+        return self
 
-        for depth, enc_token in enumerate(tokens):
-            token = Token.decode(enc_token, False)
-            if await broker.check_token(token):
-                if (token.asset == asset) and (token.issuer == last_receiver):
-                    max_depth = (max_depth and min(max_depth, (token.max_depth or max_depth) + depth)) or token.max_depth
-                    if depth >= (max_depth or (depth + 1)):
-                        return False
-                    if token.receiver == source_id:
-                        return True
-                    last_receiver = token.receiver
-                    asset = token.signature
+    async def send(self, header, payload=b"", bundle_id=None, ack_message_id=None):
+        self.logger.info(
+            "%s sending: %s %s",
+            self.session.session_key.public_serial()[:4],
+            " ".join(h[0] for h in header),
+            len(payload),
+        )
 
-            else:
-                broker.logger.info("||| token failed broker.check_token %s", token.signature[:4])
-        return False
+        def encode(header, payload, message_id, retry):
+            h = ujson.dumps(header, escape_forward_slashes=False).encode()
+            r = (retry).to_bytes(1, "big") + (message_id or b"0" * 64)
+            p = hashlib.sha256(payload).digest()
+            m = len(h).to_bytes(2, "big") + len(r + p + payload).to_bytes(3, "big") + h + r + p
+            t = int(time.time() - self.t_offset).to_bytes(4, "big")
+            s = self.session.session_key.sign(t + m)
+            return s, t + m + payload
+
+        s, mm = encode(header, payload, ack_message_id, 255 if ack_message_id else 0)
+        message_id = s
+
+        expect_ack = "send" in set(a for a, _ in header) and not ack_message_id
+        if expect_ack:
+            while True:  # Clearing old messages
+                if self.awaiting_ack:
+                    target = list(self.awaiting_ack.values())[0]
+                    if target[3] < (time.time() - (1 + self.MAX_SEND_RETRIES) * self.RESEND_TIMEOUT):
+                        self.clear(target[1])
+                        continue
+                break
+            lock = asyncio.Event()
+            if not self.awaiting_ack:
+                lock.set()
+            self.awaiting_ack[message_id or s] = (header, bundle_id, lock, time.time())
+
+        for retry in range(self.MAX_SEND_RETRIES + 1):
+            if not self.websocket or self.websocket.closed:
+                self.logger.info("%s reconnecting during send retry %d", self.session.session_key.public_serial()[:4], retry)
+                if self.is_connecting_lock.is_set():
+                    await self.reconnect()
+                else:
+                    await self.is_connecting_lock.wait()
 
+            try:
+                await self.websocket.send(s + mm)
+            except Exception:
+                self.logger.info("%s Connection.send", self.session.session_key.public_serial()[:4], exc_info=True)
+                continue
 
-class Broker:
-    def __init__(self, broker_key_file=None, broker_key_pass=None):
-        self.sessions = {}
-        self.servers = {}
-        self.entrypoint = None
-        self.broker_key = PrivateKey(broker_key_file, broker_key_pass)
-        self.logger = logging.getLogger(__name__)
-        self.seen_messages = [set(), set(), 0]
-        self.topology_cache = {0: {}}
+            if not expect_ack or await self.expect_ack(message_id, lock):
+                return
 
-    async def handle_connection(self, websocket, _):
-        connection = None
+            if retry < (self.MAX_SEND_RETRIES):
+                s, mm = encode(header, payload, message_id, retry + 1)
+                self.logger.info("%s retrying send %d", self.session.session_key.public_serial()[:4], retry)
+
+        raise Exception("%s Max send retries reached" % self.session.session_key.public_serial()[:4])
+
+    async def expect_ack(self, message_id, lock):
+        await lock.wait()
+        if message_id not in self.awaiting_ack:
+            return True
+        lock.clear()
         try:
-            connection = await Connection(websocket).handshake(self.sessions, self.broker_key, self.entrypoint, list(self.topology_cache[0]))
-            self.logger.info("%s: new connection %s", self.broker_key.public_serial()[:4], connection.session.session_id[:4])
+            await asyncio.wait_for(lock.wait(), self.RESEND_TIMEOUT)
+        except asyncio.TimeoutError:
+            lock.set()
+        if message_id not in self.awaiting_ack:
+            return True
 
-            async for message in websocket:
-                if self.check_no_repeat(message):
-                    await asyncio.gather(*(x for x in connection.tasks if x.done()))
-                    connection.tasks = set(x for x in connection.tasks if not x.done())
-                    connection.tasks.add(asyncio.get_event_loop().create_task(self.handle_message(connection, message)))
-
-        except Exception:
-            if connection:
-                self.logger.error(
-                    "%s: %s .handle_connection",
-                    self.broker_key.public_serial()[:4],
-                    connection.session.session_id[:4],
-                    exc_info=True,
-                )
-            else:
-                self.logger.error("%s: Handshake error", self.broker_key.public_serial(), exc_info=True)
+        return False
 
-        finally:
-            if connection:
-                self.logger.info("%s: %s disconnected", self.broker_key.public_serial()[:4], connection.session.session_id[:4])
-                await connection.close(self.sessions)
+    def clear(self, bundle_id):
+        if bundle_id:
+            self.logger.info("%s clearing %s", self.session.session_key.public_serial()[:4], bundle_id[:4])
+            ks = []
+            for k, v in self.awaiting_ack.items():
+                if v[1] == bundle_id:
+                    ks.append(k)
+            for k in ks:
+                self.awaiting_ack.pop(k)
 
-    async def handle_message(self, connection, message):
-        try:
-            headers = self.decode_header(message)
-            for action, args in headers:
-                if action == "listen":
-                    self.handle_listen(connection, **args)
-                if action == "broker":
-                    await self.handle_broker_action(connection, *args)
-                if action == "send":
-                    await self.handle_send(connection, message, **args)
-                if action == "close":
-                    self.handle_close(connection, **args)
-
-        except Exception:
-            self.logger.error(
-                "%s: %s .handle_message",
-                self.broker_key.public_serial()[:4],
-                connection.session.session_id[:4],
-                exc_info=True,
-            )
-            self.logger.info("%s: %s disconnected", self.broker_key.public_serial()[:4], connection.session.session_id[:4])
-            await connection.close(self.sessions)
+    async def listen(self):
+        n_tries = 0
+        while True:
+            try:
+                await self._connect()
+                while True:
+                    await self.recv()
+                    n_tries = 0
+            except Exception:
+                self.logger.warning("%s Connection.listen", self.session.session_key.public_serial()[:4], exc_info=True)
 
-    async def handle_send(self, connection, message, source, destination):
-        # self.logger.info(
-        #     "%s: send %s %s ??? %s ??? %s %s",
-        #     self.broker_key.public_serial()[:4],
-        #     source["session"][0][:4],
-        #     source["channel"][:4],
-        #     str(len(message) // 2 ** 10),
-        #     destination["session"][0][:4],
-        #     destination["channel"][:4],
-        # )
-        s = Route(**source)
-        d = Route(**destination)
-
-        if d.brokers and self.broker_key.public_serial() in d.brokers:
-            dest_session = self.sessions.get(d.session[0])
-            if dest_session:
-                dest_channel = await dest_session.expect_channel(d.channel)
-
-                if dest_session.channels.get(d.channel):
-                    if await dest_channel.validate_token_chain(s.session[0], d.tokens, self):
-                        if connection.session.session_id != s.session[0]:
-                            try:
-                                len_h = int.from_bytes(message[68:70], "big")
-                                PublicKey(s.session[0]).verify(message[:64], message[64 : 73 + len_h + 65 + 32])
-                            except InvalidSignature:
-                                self.logger.info(
-                                    'Invalid forwarded message signature - source: %s connection: %s',
-                                    s.session[0][:4],
-                                    connection.session.session_id[:4]
-                                )
-                                return
-                        self.logger.info(
-                            "%s: send %s %s >>> %s >>> %s %s",
-                            self.broker_key.public_serial()[:4],
-                            source["session"][0][:4],
-                            source["channel"][:4],
-                            str(len(message) // 2 ** 10),
-                            destination["session"][0][:4],
-                            destination["channel"][:4],
-                        )
-
-                        for connection in dest_channel.connections:
-                            await connection.websocket.send(message)
-                        return
-                    else:
-                        # print('|||||', [Token.decode(t) for t in s.tokens], [Token.decode(t) for t in d.tokens])
-                        self.logger.info(
-                            "%s: send %s %s ||| %s ||| %s %s",
-                            self.broker_key.public_serial()[:4],
-                            source["session"][0][:4],
-                            source["channel"][:4],
-                            str(len(message) // 2 ** 10),
-                            destination["session"][0][:4],
-                            destination["channel"][:4],
-                        )
-                else:
-                    if self.broker_key.public_serial() in (d.brokers or []):
-                        return
+            self.is_connecting_lock.clear()
+            await asyncio.sleep(1)
 
-        if d.brokers:
-            for depth in sorted(self.topology_cache):
-                brokers = set(d.brokers).intersection(set(self.topology_cache[depth].keys()))
-                if brokers:
-                    for broker_id in brokers:
-                        for broker_connection in self.topology_cache[depth][broker_id]:
-                            if broker_connection.websocket.closed == False:
-                                await broker_connection.websocket.send(message)
-                                self.logger.info(
-                                    "%s: send %s %s ))) %s ))) %s %s (%s)",
-                                    self.broker_key.public_serial()[:4],
-                                    source["session"][0][:4],
-                                    source["channel"][:4],
-                                    str(len(message) // 2 ** 10),
-                                    destination["session"][0][:4],
-                                    destination["channel"][:4],
-                                    broker_id[:4],
-                                )
-                    return
-            for peer in set().union(*self.topology_cache[0].values()):
-                await peer.send(
-                    [
-                        (
-                            "broker",
-                            (
-                                "topology_update",
-                                {"source": self.broker_key.public_serial(), "destinations": d.brokers, "counter": 0},
-                            ),
-                        )
-                    ]
-                )
+            if n_tries > self.MAX_SEND_RETRIES:
+                self.is_connecting_lock.set()
+                raise Exception("%s Max tries reached" % self.session.session_key.public_serial()[:4])
+            n_tries += 1
+
+    async def recv(self):
+        if not self.websocket or self.websocket.closed:
+            if self.is_connecting_lock.is_set():
+                await self.reconnect()
+            else:
+                await self.is_connecting_lock.wait()
 
-    def handle_listen(self, connection, session, channel, brokers, is_public=False):
-        if session[0] == connection.session.session_id:
-            self.logger.info(
-                "%s: listen %s %s %s",
-                self.broker_key.public_serial()[:4],
-                str(connection.session.session_id[:4]),
-                str(channel[:4]),
-                str(is_public),
-            )
+        message = await self.websocket.recv()
 
-            if channel not in connection.session.channels:
-                connection.session.channels[channel] = Channel(connection.session, channel, is_public)
+        signature, timestamp = message[:64], int.from_bytes(message[64:68], "big")
 
-            channel_obj = connection.session.channels[channel]
-            channel_obj.connections.add(connection)
-            connection.channels.add(channel_obj)
-
-            event = connection.session.expecting_channels.pop(channel, None)
-            if event:
-                event.set()
+        if self.session.check_no_repeat(signature, timestamp + self.t_offset):
 
-    def handle_close(self, connection, session, channel, **kwargs):
-        if session[0] == connection.session.session_id:
+            len_h, len_p = [int.from_bytes(x, "big") for x in [message[68:70], message[70:73]]]
+            header = ujson.loads(message[73 : 73 + len_h])
+            full_payload = message[73 + len_h : 73 + len_h + len_p]
             self.logger.info(
-                "%s: close %s %s",
-                self.broker_key.public_serial()[:4],
-                str(connection.session.session_id[:4]),
-                str(channel[:4]),
+                "%s received: %s %s",
+                self.session.session_key.public_serial()[:4],
+                " ".join(h[0] for h in header),
+                len(full_payload),
             )
+            for action, content in header:
+                if action == "send":
+                    source, destination = Route(**content["source"]), Route(**content["destination"])
+                    PublicKey(source.session[0]).verify(signature, message[64 : 73 + len_h + 65 + 32])
+                    if self.session.channels.get(destination.channel):
+                        channel = self.session.channels.get(destination.channel)
+                        if full_payload[0] == 255:
+                            self.ack(source.session[0], full_payload[1:65])
+                        else:
+                            ret_signature = signature if (full_payload[0] == 0) else full_payload[1:65]
+                            payload = full_payload[65 + 32 :]
+                            await self.send(
+                                (("send", {"destination": content["source"], "source": content["destination"]}),),
+                                b"",
+                                None,
+                                ret_signature,
+                            )
+                            # print(self.session.session_key.public_serial()[:4], 'sent ack', ret_signature[:4])
+                            if hashlib.sha256(payload).digest() == full_payload[65 : 65 + 32]:
+                                if (ret_signature == signature) or self.session.check_no_repeat(
+                                    ret_signature, timestamp + self.t_offset
+                                ):
+                                    channel.handle_message(source, destination, payload, message[: 73 + len_h + 65 + 32])
+                            else:
+                                raise Exception("Authentication Error: message payload does not match signed hash")
+
+    def ack(self, source_id, message_id):
+        # print(self.session.session_key.public_serial()[:4], 'received ack', message_id[:4], 'from', source_id[:4])
+        header = self.awaiting_ack.get(message_id, [[]])[0]
+        for action, content in header:
+            if action == "send":
+                if content["destination"]["session"][0] == source_id:
+                    t = self.awaiting_ack.pop(message_id)
+                    t[2].set()
+                    if self.awaiting_ack:
+                        self.awaiting_ack[list(self.awaiting_ack.keys())[0]][2].set()
 
-            if connection.session.channels.get(channel):
-                channel_obj = connection.session.channels.get(channel)
-                connection.channels.remove(channel_obj)
-                channel_obj.connections.remove(connection)
-                if not channel_obj.connections:
-                    channel_obj.close()
-
-    async def handle_broker_action(self, connection, action, params=None):
-        if action == "open":
-            peer = Peer(connection.websocket, self)
-            session_id = connection.session.session_id
-            connection.session.broker_connections[connection] = peer
-            self.topology_cache[0][session_id] = (self.topology_cache[0].get(session_id) or set()).union([peer])
-        if action == "close":
-            connection.session.broker_sessions.pop(connection, None)
-        if action == "topology_update" and params:
-            self.logger.info("%s: topology %s", self.broker_key.public_serial()[:4], str(params))
-            # if self.check_no_repeat...
-            peer = connection.session.broker_connections[connection]
-            if self.broker_key.public_serial() == params["source"]:
-                # if check signature
-                for reply in params["replies"]:
-                    peer_set = self.topology_cache[params["replies"][reply]].get(reply) or set()
-                    peer_set = peer_set.union([peer])
-                    self.topology_cache[params["replies"][reply]][reply] = peer_set
-            elif "replies" in params:
-                for reply in params["replies"]:
-                    params["replies"][reply] += 1
-                for depth in self.topology_cache:
-                    source_set = self.topology_cache[depth].get(params["source"])
-                    if source_set:
-                        for conn in source_set:
-                            await conn.send([("broker", ("topology_update", params))])
-                        return
-            else:
-                destination_set = set(params["destinations"]).intersection(set(self.topology_cache[0].keys()))
-                if destination_set:
-                    params["replies"] = {d: 0 for d in destination_set}
-                    await peer.send([("broker", ("topology_update", params))])
-                    return
-                params["counter"] += 1
-                source_set = self.topology_cache[params["counter"]].get(params["source"]) or set()
-                self.topology_cache[params["counter"]][params["source"]] = source_set.union([peer])
-
-                for forwarded in set().union(self.topology_cache[0].values()):
-                    await peer.send([("broker", ("topology_update", params))])
-
-    async def add_broker(self, url, inherit_entrypoint=False):
-        peer = Peer(None, self)
-        if re.sub(r"(?![\w\d]+:\/\/[\w\d.]+):[\d]+", "", url) == url:
-            i = len(re.findall(r"[\w\d]+:\/\/[\w\d.]+", url)[0])
-            url = url[:i] + ":8776" + url[i:]
-
-        await peer.connect(url, inherit_entrypoint)  # This already adds the peer to self.sessions
-
-    async def check_token(self, token):
-        session = self.sessions.get(token.issuer)
-        if session:
-            if token.signature in session.cached_tokens:
-                return token.encode() == session.cached_tokens.get(token.signature).encode()
+    def __await__(self):
+        async def await_lock():
+            if self.listener:
+                await self.is_connecting_lock.wait()
+                if self.listener.done():
+                    old_listener = self.listener
+                    self.listener = None
+                    await old_listener
             else:
-                if token.verify(token.signature):
-                    session.cached_tokens[token.signature] = token
-                    return True
-                else:
-                    return False
+                await self.reconnect()
 
-        else:
-            return token.verify(token.signature)
+            return self
 
-    def check_no_repeat(self, message):
-        signature, timestamp = message[:64], int.from_bytes(message[64:68], "big")
+        return await_lock().__await__()
+
+
+class Session:
+    def __init__(self, session_key_file=None):
+        self.session_key = PrivateKey(session_key_file)
+        self.instance_id = base64.b64encode(os.urandom(6)).decode()
+        self.channels = {}
+        self.targets = {}
+        self.routes = {}
+        self.connections = set()
+        self.seen_messages = [set(), set(), 0]
+        self.issued_tokens = {}
+        self.pending_tasks = set()
+
+    def check_no_repeat(self, signature, timestamp):
         now = int(time.time())
 
         lead = now // 60
         if self.seen_messages[2] != lead:
             self.seen_messages[lead % 2].clear()
             self.seen_messages[2] = lead
 
         if (now - 60 + 4) <= timestamp <= now + 4:
             if signature not in self.seen_messages[0].union(self.seen_messages[1]):
                 self.seen_messages[lead % 2].add(signature)
                 return True
-
         return False
 
-    def decode_header(self, m):
-        header = ujson.loads(m[73 : 73 + int.from_bytes(m[68:70], "big")])
-        return header
-
-    async def serve(self, host="127.0.0.1", port=8776, **kwargs):
-        if "compression" not in kwargs:
-            kwargs["compression"] = None
-        server = await websockets.serve(self.handle_connection, host, port, **kwargs)
-        self.servers[(host, port)] = server
+    def issue_token(self, target, receiver, max_depth=None):
+        if isinstance(target, Token):
+            token_type = "extension"
+            prev_token = target
+            asset = target.signature
+        else:
+            token_type = "root"
+            prev_token = None
+            asset = target
+
+        for token, prev_token_tmp in self.issued_tokens.values():
+            if (
+                token.asset == asset
+                and token.receiver == receiver
+                and token.token_type == token_type
+                and token.max_depth == max_depth
+                and all([x.broker_id in token.brokers for x in self.connections])
+            ):
+                prev_token = prev_token_tmp
+                break
+        else:
+            token = Token(
+                self.session_key.public_serial(),
+                [x.broker_id for x in self.connections],
+                receiver,
+                asset,
+                token_type,
+                max_depth,
+            )
+            signature = token.sign(self.session_key)
+
+            self.issued_tokens[signature] = token, prev_token
 
-        return self
+        return ("token", ("issue", token.encode(), prev_token and prev_token.encode()))
 
-    async def close(self, host=None, port=None):
-        keys = set(self.servers.keys())
-        for server_host, server_port in keys:
-            if not host or server_host == host:
-                if not port or server_port == port:
-                    self.servers.pop((server_host, server_port)).close()
+    def revoke_tokens(self, asset):
+        children = [tid for tid, t in self.issued_tokens.items() if t[0].asset == asset]
+        headers = [h for hs in [self.revoke_tokens(tid) for tid in children] for h in hs]
 
+        tokens = self.issued_tokens.pop(asset, None)
+        if tokens:
+            return [("token", ("revoke", tokens[0].signature))] + headers
+        return headers
 
-class Peer(Connection):
-    def __init__(self, websocket, broker):
-        super().__init__(websocket)
-        self.broker = broker
-        self.t_offset = 0
-        self.listener = None
-        self.url = None
+    def extend_route(self, route, receiver, max_depth=None):
+
+        if route.session[0] == self.session_key.public_serial():
+            token_header = self.issue_token(route.channel, receiver, max_depth)
+            route.tokens = [token_header[1][1]]
+            return token_header
+
+        for i, enc_token in enumerate(route.tokens):
+            token = Token.decode(enc_token)
+            if token.receiver == self.session_key.public_serial():
+                route.tokens = route.tokens[: i + 1]
+
+        token = Token.decode(route.tokens[-1], False)
+        token_header = self.issue_token(token, receiver, max_depth)
+        route.tokens.append(token_header[1][1])
+        return token_header
+
+    def clear(self, bundle_id):
+        for connection in self.connections:
+            connection.clear(bundle_id)
+
+    async def send(self, header, payload=b"", bundle_id=None):
+        for connection in self.connections:
+            await connection.send(header, payload, bundle_id)
+
+    def __repr__(self):
+        return "Session %s %s" % (
+            self.session_key.public_serial()[:4],
+            self.instance_id[:2],
+        )
+
+
+class Channel:
+    def __init__(self, session, channel_key_file=None, is_public=False):
+        self.MAX_PAYLOAD_LEN = 2 ** 19
+        self.MAX_COMPRESSION_LEN = 2 ** 19
+        self.MAX_OUTBOX = 2 ** 4
+
+        self.session = session
+        self.channel_key = PrivateKey(channel_key_file)
+        self.is_public = is_public
+        self.route = Route(
+            list(set(c.broker_id for c in self.session.connections)),
+            (self.session.session_key.public_serial(), self.session.instance_id),
+            self.channel_key.public_serial(),
+        )
+        self.header_buffer = []
+        self.chunks = {}
+        self.messages = deque()
         self.lock = asyncio.Event()
-        self.exception = None
+        session.channels[self.channel_key.public_serial()] = self
 
-    def connect(self, url, inherit_entrypoint):
-        self.url = url
-        self.listener = asyncio.get_event_loop().create_task(self.listen(inherit_entrypoint))
+        self.telekinesis = None
+
+    def handle_message(self, source, destination, raw_payload, proof):
+        if self.validate_token_chain(source.session[0], destination.tokens):
+            message_tuple = None
+            shared_key = SharedKey(self.channel_key, PublicKey(source.channel))
+            payload = shared_key.decrypt(raw_payload[16:], raw_payload[:16])
+            metadata = RequestMetadata(
+                self.session, source, [{"raw_payload": raw_payload, "shared_key": shared_key.key, "proof": proof}]
+            )
+
+            if payload[:4] == b"\x00" * 4:
+                if payload[4] == 0:
+                    message_tuple = (metadata, bson.loads(payload[5:]))
+                elif payload[4] == 255:
+                    message_tuple = (metadata, bson.loads(zlib.decompress(payload[5:])))
+                else:
+                    raise Exception("Received message with different encoding")
+            else:
+                ir, nr, mmid, chunk = payload[:2], payload[2:4], payload[4:8], payload[8:]
+                i, n = int.from_bytes(ir, "big"), int.from_bytes(nr, "big")
+
+                mid = source.session[0].encode() + mmid
+                if mid not in self.chunks:
+                    self.chunks[mid] = {}
+                self.chunks[mid][i] = (chunk, metadata)
+
+                if len(self.chunks[mid]) == n:
+                    chunks = self.chunks.pop(mid)
+                    payload = b"".join(chunks[ii][0] for ii in range(n))
+
+                    combined_metadata = RequestMetadata(
+                        metadata._session, metadata.caller, [chunks[ii][1].raw_messages[0] for ii in range(n)]
+                    )
+                    if payload[0] == 0:
+                        message_tuple = (combined_metadata, bson.loads(payload[1:]))
+                    elif payload[0] == 255:
+                        message_tuple = (combined_metadata, bson.loads(zlib.decompress(payload[1:])))
+                    else:
+                        raise Exception("Received message with different encoding")
+
+            if message_tuple:
+                # print('<<<', source, destination, {k: v is None for k, v in message_tuple[1].items()})
+                if not self.telekinesis:
+                    self.messages.appendleft(message_tuple)
+                    self.lock.set()
+                else:
+                    asyncio.get_event_loop().create_task(self.telekinesis._handle_request(self, *message_tuple))
+        else:
+            self.session.logger.error(
+                "Invalid Tokens: %s %s -> %s %s [%s]",
+                source.session[0][:4],
+                source.channel[:4],
+                destination.session[0][:4],
+                destination.channel[:4],
+                destination.tokens,
+            )
+
+    async def recv(self):
+        if not self.messages:
+            self.lock.clear()
+            await self.lock.wait()
+
+        return self.messages.pop()
+
+    def listen(self):
+        listen_dict = self.route.to_dict()
+        listen_dict["is_public"] = self.is_public
+        listen_dict.pop("tokens")
+        self.header_buffer.append(("listen", listen_dict))
 
         return self
 
-    async def reconnect(self):
-        if self.websocket:
-            await self.websocket.close()
+    async def send(self, destination, payload_obj):
+        # if payload_obj:
+        # print('>>>', self.route, destination, {k: v is None for k, v in payload_obj.items()})
+        def encrypt_slice(payload, max_payload, shared_key, mid, n, i):
+            if i < n:
+                if n == 1:
+                    chunk = b"\x00" * 4 + payload
+                else:
+                    if n > 2 ** 16:
+                        raise Exception(f"Payload size {len(payload)/2**20} MiB is too large")
+                    chunk = i.to_bytes(2, "big") + n.to_bytes(2, "big") + mid + payload[i * max_payload : (i + 1) * max_payload]
+
+                nonce = os.urandom(16)
+                yield nonce + shared_key.encrypt(chunk, nonce)
+                yield from encrypt_slice(payload, max_payload, shared_key, mid, n, i + 1)
+
+        async def execute(header, encrypted_slice_generator, mid):
+            for encrypted_slice in encrypted_slice_generator:
+                await self.execute(header, encrypted_slice, mid)
+
+        source_route = self.route.clone()
+        self.header_buffer.append(self.session.extend_route(source_route, destination.session[0]))
+        self.listen()
 
-        self.websocket = await websockets.connect(self.url)
+        payload = bson.dumps(payload_obj)
 
-        challenge = await self.websocket.recv()
-        t_broker = int.from_bytes(challenge[-4:], "big")
+        if len(payload) < self.MAX_COMPRESSION_LEN:
+            payload = b"\xff" + zlib.compress(payload)
+        else:
+            payload = b"\x00" + payload
 
-        self.t_offset = int(time.time()) - t_broker
-        signature = self.broker.broker_key.sign(challenge)
+        mid = os.urandom(4)
+        shared_key = SharedKey(self.channel_key, PublicKey(destination.channel))
 
-        pk = self.broker.broker_key.public_serial().encode()
+        header = ("send", {"source": source_route.to_dict(), "destination": destination.to_dict()})
 
-        sent_challenge = os.urandom(32)
-        sent_metadata = {"version": get_distribution(__name__.split(".")[0]).version}
-        await self.websocket.send(signature + pk + sent_challenge + ujson.dumps(sent_metadata).encode())
+        n = (len(payload) - 1) // self.MAX_PAYLOAD_LEN + 1
+        n_tasks = min(n, self.MAX_OUTBOX)
+        gen = encrypt_slice(payload, self.MAX_PAYLOAD_LEN, shared_key, mid, n, 0)
 
-        m = await asyncio.wait_for(self.websocket.recv(), 15)
+        try:
+            await asyncio.gather(*(execute(header, gen, mid) for _ in range(n_tasks)))
+        except asyncio.CancelledError:
+            self.session.clear(mid)
+            raise asyncio.CancelledError
+        finally:
+            self.session.clear(mid)
 
-        if m[: len("Incompatible")] == b"Incompatible":
-            raise Exception(m.decode())
+        return self
 
-        signature, session_id, metadata = m[:64], m[64:152].decode(), ujson.loads(m[152:].decode())
-        PublicKey(session_id).verify(signature, sent_challenge)
+    async def execute(self, header=None, payload=b"", bundle_id=None):
+        await self.session.send([h for h in (self.header_buffer + [header]) if h], payload, bundle_id)
+        self.header_buffer = []
 
-        entrypoint = Route(**metadata.get("entrypoint")) if metadata.get("entrypoint") else None
+        return self
 
-        await self.send([("broker", ("open",))])
+    def __await__(self):
+        return self.execute().__await__()
 
-        return session_id, entrypoint
+    def close(self):
+        self.header_buffer.append(("close", self.route.to_dict()))
+        self.header_buffer += self.session.revoke_tokens(self.channel_key.public_serial())
 
-    async def send(self, header):
-        h = ujson.dumps(header).encode()
-        m = len(h).to_bytes(2, "big") + (0).to_bytes(3, "big") + h
-        t = int(time.time() - self.t_offset - 4).to_bytes(4, "big")
-        s = self.broker.broker_key.sign(
-            t + m,
-        )
+        self.session.channels.pop(self.channel_key.public_serial(), None)
 
-        await self.websocket.send(s + t + m)
+        return self
 
-    async def listen(self, inherit_entrypoint):
-        n_tries = 0
-        while True:
+    def validate_token_chain(self, source_id, tokens):
+        if self.is_public or (source_id == self.session.session_key.public_serial()):
+            return True
+        if not tokens:
+            return False
+
+        asset = self.channel_key.public_serial()
+        last_receiver = self.session.session_key.public_serial()
+        max_depth = None
+
+        for depth, token_string in enumerate(tokens):
             try:
-                self.lock.clear()
-                session_id, entrypoint = await self.reconnect()
+                token = Token.decode(token_string)
+            except InvalidSignature:
+                return False
+            if (token.asset == asset) and (token.issuer == last_receiver):
+                if token.issuer == self.session.session_key.public_serial():
+                    if token.signature not in self.session.issued_tokens:
+                        return False
+                if token.max_depth:
+                    if not max_depth or (token.max_depth + depth) < max_depth:
+                        max_depth = token.max_depth + depth
+                if not max_depth or depth < max_depth:
+                    last_receiver = token.receiver
+                    asset = token.signature
+                    if last_receiver == source_id:
+                        return True
+                    continue
+            return False
+        return False
 
-                if not (-15 < self.t_offset < 2):
-                    raise IncompatibleBrokerException(f"Unix time difference too large: {self.t_offset} seconds.")
-                self.lock.set()
-
-                if session_id not in self.broker.sessions:
-                    self.broker.sessions[session_id] = Session(session_id)
-
-                if inherit_entrypoint:
-                    self.broker.entrypoint = entrypoint
-
-                self.session = self.broker.sessions[session_id]
-                self.session.connections.add(self)
-                self.session.broker_connections[self] = self
-                self.broker.topology_cache[0][session_id] = (self.broker.topology_cache[0].get(session_id) or set()).union(
-                    [self]
-                )
+    def __repr__(self):
+        return "Channel %s %s - %s: %s" % (
+            self.session.session_key.public_serial()[:4],
+            self.session.instance_id[:2],
+            self.channel_key.public_serial()[:4],
+            self.telekinesis,
+        )
 
-                n_tries = 0
-                while True:
-                    message = await self.websocket.recv()
-                    self.tasks.add(asyncio.get_event_loop().create_task(self.broker.handle_message(self, message)))
+    async def __aenter__(self):
+        return self.listen()
 
-                    # await asyncio.gather(*(x for x in self.tasks if x.done() and not x.exception()), return_exceptions=True)
-                    self.tasks = set(x for x in self.tasks if not x.done())
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.close()
 
-            except IncompatibleBrokerException as e:
-                self.logger.error("Peer.listen", exc_info=True)
-                self.exception = e
-                await self.close(self.broker.sessions, False)
-                self.lock.set()
-                return
+        return isinstance(exc_type, Exception)
 
-            except Exception:
-                self.logger.error("Peer.listen", exc_info=True)
-                await self.close(self.broker.sessions, False)
-                self.lock.set()
-
-                if n_tries > 10:
-                    self.logger.error("Peer.listen: Max connection retries reached", exc_info=True)
-                    return
 
-                await asyncio.sleep(1)
-                n_tries += 1
-                continue
+class Route:
+    def __init__(self, brokers, session, channel, tokens=None, parent_channel=None):
+        self.brokers = brokers
+        self.session = tuple(session)
+        self.channel = channel
+        self.tokens = tokens or []
+        self._parent_channel = parent_channel
+
+    def to_dict(self):
+        return {"brokers": self.brokers, "session": self.session, "channel": self.channel, "tokens": self.tokens}
+
+    def clone(self):
+        return Route(**self.to_dict())
+
+    def validate_token_chain(self, receiver):
+        if self.session[0] != receiver:
+            assert len(self.tokens) > 0
+            prev_token = None
+            for i, raw_token in enumerate(self.tokens):
+                token = Token.decode(raw_token)
+                if i == 0:
+                    assert token.asset == self.channel
+                    assert token.issuer == self.session[0]
+                    assert token.token_type == "root"
+                else:
+                    assert token.asset == prev_token.signature
+                    assert token.issuer == prev_token.receiver
+                    assert token.token_type == "extension"
+                if token.receiver == receiver:
+                    break
+                prev_token = token
+            else:
+                return False
+        return True
 
-    def __await__(self):
-        async def wait_lock():
-            await self.lock.wait()
-            if self.exception:
-                raise self.exception
+    def __repr__(self):
+        return f"Route {self.session[0][:4]} {self.session[1][:2]} - {self.channel[:4]}"
 
-        return wait_lock().__await__()
+    def __eq__(self, route):
+        return self.to_dict() == route.to_dict()
+
+    def __await__(self):
+        async def await_parent_channel():
+            await self._parent_channel
+            return self
+
+        return self._parent_channel and await_parent_channel().__await__()
 
 
-class IncompatibleBrokerException(Exception):
-    pass
+class RequestMetadata:
+    def __init__(self, session, caller, raw_messages):
+        self._session = session
+        self.session_public_key = session.session_key.public_serial()
+        self.caller = caller
+        self.raw_messages = raw_messages
```

### Comparing `telekinesis-0.1.81/telekinesis/client.py` & `telekinesis-0.1.9/telekinesis/broker.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,685 +1,659 @@
-import base64
 import logging
-import time
 import os
 import asyncio
-import bson
-import zlib
-from collections import deque, OrderedDict
+import time
+from packaging import version
+import re
 from pkg_resources import get_distribution
-import hashlib
 
-import websockets
 import ujson
+import websockets
 
-from .cryptography import PrivateKey, PublicKey, SharedKey, Token, InvalidSignature
+from .cryptography import PrivateKey, PublicKey, Token, InvalidSignature
+from .client import Route
 
 
 class Connection:
-    def __init__(self, session, url="ws://localhost:8776"):
-        self.RESEND_TIMEOUT = 2  # sec
-        self.MAX_SEND_RETRIES = 3
-
-        self.session = session
-        self.url = url
+    def __init__(self, websocket):
+        self.MIN_CLIENT_VERSION = "0.1.4"
+        self.websocket = websocket
         self.logger = logging.getLogger(__name__)
-        self.websocket = None
-        self.t_offset = 0
-        self.broker_id = None
-        self.entrypoint = None
-        self.broker_peers = []
+        self.session = None
+        self.channels = set()
+        self.tasks = set()
 
-        self.is_connecting_lock = asyncio.Event()
-        self.awaiting_ack = OrderedDict()
+    async def handshake(self, sessions, broker_key, entrypoint):
+        challenge = os.urandom(32) + int(time.time()).to_bytes(4, "big")
 
-        if 'connections' not in dir(session):
-            session.connections = set()
+        await self.websocket.send(challenge)
+        m = await asyncio.wait_for(self.websocket.recv(), 15)
 
-        session.connections.add(self)
+        signature, session_id, client_challenge, metadata_raw = m[:64], m[64:152].decode(), m[152:184], m[184:]
+        metadata = ujson.loads(metadata_raw.decode())
 
-        self.listener = asyncio.get_event_loop().create_task(self.listen())
+        if version.parse(metadata["version"]) < version.parse(self.MIN_CLIENT_VERSION):
+            err_message = f'Incompatible version {metadata["version"]} < {self.MIN_CLIENT_VERSION}'
+            await self.websocket.send(err_message.encode())
+            raise Exception(err_message)
 
-    async def reconnect(self):
-        if self.is_connecting_lock.is_set():
-            self.is_connecting_lock.clear()
-            if self.listener:
-                self.listener.cancel()
+        PublicKey(session_id).verify(signature, challenge)
 
-            self.listener = asyncio.get_event_loop().create_task(self.listen())
+        await self.websocket.send(
+            broker_key.sign(client_challenge)
+            + broker_key.public_serial().encode()
+            + ujson.dumps({"entrypoint": entrypoint and entrypoint.to_dict()}, escape_forward_slashes=False).encode()
+        )
 
-        await self.is_connecting_lock.wait()
+        if session_id not in sessions:
+            sessions[session_id] = Session(session_id)
 
-    async def _connect(self):
-        self.logger.info("%s connecting", self.session.session_key.public_serial(False)[:4])
-        if self.websocket:
+        self.session = sessions[session_id]
+        self.session.connections.add(self)
+
+        return self
+
+    async def close(self, sessions, remove=True):
+        try:
             await self.websocket.close()
+            for channel in self.channels:
+                if self in channel.connections:
+                    channel.connections.remove(self)
+                if not channel.connections:
+                    self.session.channels.pop(channel.channel_id, None)
+
+            if remove:
+                if self in self.session.connections:
+                    self.session.connections.remove(self)
+
+                self.session.broker_connections.pop(self, None)
+
+                if not self.session.channels and not self.session.broker_connections and not self.session.connections:
+                    sessions.pop(self.session.session_id, None)
+
+                await asyncio.gather(*(x for x in self.tasks if x.done()))
+                # print([x for x in self.tasks if not x.done()])
+                [x.cancel() for x in self.tasks if not x.done()]
+        except Exception:
+            self.logger.error("Exception when closing %s", self.session.session_id[:4], exc_info=True)
 
-        self.websocket = await websockets.connect(self.url)
 
-        challenge = await self.websocket.recv()
-        t_broker = int.from_bytes(challenge[-4:], "big")
+class Session:
+    def __init__(self, session_id):
+        self.session_id = session_id
+        self.channels = {}
+        self.expecting_channels = {}
+        self.connections = set()
+        self.broker_connections = {}
+        self.active_tokens = {}
+        self.cached_tokens = {}
+        self.expecting_tokens = {}
+        self.tasks = set()
+
+    async def validate_peer_token(self, token, event):
+        if token.signature in self.cached_tokens and token.encode() == self.cached_tokens[token.signature].encode():
+            event.set()
+            return True
+        self.expecting_tokens[token.signature] = (event, token)
+        for broker in self.broker_connections.values():
+            await broker.send((("token", ("validate", token.encode())),))
+        self.tasks.add(asyncio.get_event_loop().create_task(self.clean_expecting_token(token)))
 
-        self.t_offset = int(time.time()) - t_broker
-        signature = self.session.session_key.sign(challenge)
+        return False
 
-        pk = self.session.session_key.public_serial(False).encode()
+    async def clean_expecting_token(self, token):
+        await asyncio.sleep(2)
+        self.expecting_tokens.pop(token.signature, None)
+
+    async def timeout_cached_token(self, token):
+        await asyncio.sleep(15)
+        self.cached_tokens.pop(token.signature, None)
+
+    def approve_token(self, token):
+        self.tasks = set(x for x in self.tasks if not x.done())
+        if token.issuer == self.session_id:
+            self.active_tokens[token.signature] = token
+        else:
+            self.cached_tokens[token.signature] = token
+            self.tasks.add(asyncio.get_event_loop().create_task(self.timeout_cached_token(token)))
 
-        sent_challenge = os.urandom(32)
-        sent_metadata = {"version": get_distribution(__name__.split(".")[0]).version}
-        await self.websocket.send(
-            signature + pk + sent_challenge + ujson.dumps(sent_metadata, escape_forward_slashes=False).encode()
-        )
+        event, expected_token = self.expecting_tokens.get(token.signature, (None, None))
+        if expected_token and expected_token.encode() == token.encode():
+            self.expecting_tokens.pop(token.signature, None)
+            event.set()
+
+    async def expect_channel(self, channel_id):
+        if channel_id not in self.channels:
+            list(self.connections)[0].logger.info("awaiting channel %s", channel_id[:4])
+            event = asyncio.Event()
+            self.expecting_channels[channel_id] = event
+            try:
+                await asyncio.wait_for(event.wait(), 2)
+                self.expecting_channels.pop(channel_id, None)
+            except asyncio.exceptions.TimeoutError:
+                pass
+        return self.channels.get(channel_id)
 
-        m = await asyncio.wait_for(self.websocket.recv(), 15)
 
-        if m[: len("Incompatible")] == b"Incompatible":
-            raise Exception(m.decode())
+class Channel:
+    def __init__(self, session, channel_id, is_public):
+        self.session = session
+        self.channel_id = channel_id
+        self.is_public = is_public
+        self.connections = set()
 
-        broker_signature, broker_id, metadata = m[:64], m[64:152].decode(), ujson.loads(m[152:].decode())
-        PublicKey(broker_id).verify(broker_signature, sent_challenge)
+    def close(self):
+        for connection in self.connections:
+            connection.channels.remove(self)
 
-        self.broker_id = broker_id
-        self.entrypoint = Route(**metadata.get("entrypoint")) if metadata.get("entrypoint") else None
-        self.broker_peers = metadata.get("peers", [])
-
-        headers = []
-        for channel in self.session.channels.values():
-            listen_dict = channel.route.to_dict()
-            listen_dict["is_public"] = channel.is_public
-            listen_dict.pop("tokens")
-            headers.append(("listen", listen_dict))
-
-        lens = tuple((len(ujson.dumps(h, escape_forward_slashes=False)), h) for h in headers)
-
-        groups = [[]]
-        acc_len = 1
-        for l, h in lens:
-            if acc_len + l + 1 < 256**2:
-                groups[-1].append(h)
-                acc_len += l + 1
-            else:
-                groups.append([h])
-                acc_len = l + 2
+        self.session.channels.pop(self.channel_id)
 
-        for group in groups:
-            await self.send(group)
+    async def validate_token_chain(self, source_id, tokens, broker):
+        if (source_id == self.session.session_id) or self.is_public:
+            return True
 
-        self.is_connecting_lock.set()
+        if not tokens:
+            broker.logger.info("||| no tokens")
+            return False
 
-        return self
+        asset = self.channel_id
+        last_receiver = self.session.session_id
+        max_depth = None
 
-    async def send(self, header, payload=b"", bundle_id=None, ack_message_id=None):
-        if not ack_message_id:
-            self.logger.info(
-                "%s sending: %s %s",
-                self.session.session_key.public_serial(False)[:4],
-                " ".join(h[0] for h in header),
-                len(payload),
-            )
+        for depth, enc_token in enumerate(tokens):
+            token = Token.decode(enc_token, False)
+            if await broker.check_token(token):
+                if (token.asset == asset) and (token.issuer == last_receiver):
+                    max_depth = (max_depth and min(max_depth, (token.max_depth or max_depth) + depth)) or token.max_depth
+                    if depth >= (max_depth or (depth + 1)):
+                        return False
+                    if token.receiver == source_id:
+                        return True
+                    last_receiver = token.receiver
+                    asset = token.signature
 
-        def encode(header, payload, message_id, retry):
-            h = ujson.dumps(header, escape_forward_slashes=False).encode()
-            r = (retry).to_bytes(1, "big") + (message_id or b"0" * 64)
-            p = hashlib.sha256(payload).digest()
-            m = len(h).to_bytes(2, "big") + len(r + p + payload).to_bytes(3, "big") + h + r + p
-            t = int(time.time() - self.t_offset).to_bytes(4, "big")
-            s = self.session.session_key.sign(t + m)
-            return s, t + m + payload
-
-        s, mm = encode(header, payload, ack_message_id, 255 if ack_message_id else 0)
-        message_id = s
-
-        expect_ack = "send" in set(a for a, _ in header) and not ack_message_id
-        if expect_ack:
-            while True:  # Clearing old messages
-                if self.awaiting_ack:
-                    target = list(self.awaiting_ack.values())[0]
-                    if target[3] < (time.time() - (1 + self.MAX_SEND_RETRIES) * self.RESEND_TIMEOUT):
-                        self.clear(target[1])
-                        continue
-                break
-            lock = asyncio.Event()
-            if not self.awaiting_ack:
-                lock.set()
-            self.awaiting_ack[message_id or s] = (header, bundle_id, lock, time.time())
-
-        for retry in range(self.MAX_SEND_RETRIES + 1):
-            if not self.websocket or self.websocket.closed:
-                self.logger.info("%s reconnecting during send retry %d", self.session.session_key.public_serial(False)[:4], retry)
-                if self.is_connecting_lock.is_set():
-                    await self.reconnect()
-                else:
-                    await self.is_connecting_lock.wait()
+            else:
+                broker.logger.info("||| token failed broker.check_token ")
+        return False
 
-            try:
-                await self.websocket.send(s + mm)
-            except Exception:
-                self.logger.info("%s Connection.send", self.session.session_key.public_serial(False)[:4], exc_info=True)
-                continue
 
-            if not expect_ack or await self.expect_ack(message_id, lock):
-                return
+class Broker:
+    def __init__(self, broker_key_file=None):
+        self.sessions = {}
+        self.servers = {}
+        self.entrypoint = None
+        self.broker_key = PrivateKey(broker_key_file)
+        self.logger = logging.getLogger(__name__)
+        self.seen_messages = [set(), set(), 0]
+        self.topology_cache = {0: {}}
 
-            if retry < (self.MAX_SEND_RETRIES):
-                s, mm = encode(header, payload, message_id, retry + 1)
-                self.logger.info("%s retrying send %d", self.session.session_key.public_serial(False)[:4], retry)
-
-        raise ConnectionError(["%s send %s %s - %s max retries reached" % (
-            self.session.session_key.public_serial(False)[:4],
-            h['destination']['session'][0][:4], 
-            h['destination']['session'][1][:2],
-            h['destination']['channel'][:4],
-            ) for a, h in header if a == 'send'][0])
-
-    async def expect_ack(self, message_id, lock):
-        await lock.wait()
-        if message_id not in self.awaiting_ack:
-            return True
-        lock.clear()
+    async def handle_connection(self, websocket, _):
+        connection = None
         try:
-            await asyncio.wait_for(lock.wait(), self.RESEND_TIMEOUT)
-        except asyncio.TimeoutError:
-            lock.set()
-        if message_id not in self.awaiting_ack:
-            return True
+            connection = await Connection(websocket).handshake(self.sessions, self.broker_key, self.entrypoint)
+            self.logger.info("%s: new connection %s", self.broker_key.public_serial()[:4], connection.session.session_id[:4])
 
-        return False
+            async for message in websocket:
+                if self.check_no_repeat(message):
+                    await asyncio.gather(*(x for x in connection.tasks if x.done()))
+                    connection.tasks = set(x for x in connection.tasks if not x.done())
+                    connection.tasks.add(asyncio.get_event_loop().create_task(self.handle_message(connection, message)))
+
+        except Exception:
+            if connection:
+                self.logger.error(
+                    "%s: %s .handle_connection",
+                    self.broker_key.public_serial()[:4],
+                    connection.session.session_id[:4],
+                    exc_info=True,
+                )
+            else:
+                self.logger.error("%s: Handshake error", self.broker_key.public_serial(), exc_info=True)
 
-    def clear(self, bundle_id):
-        if bundle_id:
-            self.logger.info("%s clearing %s", self.session.session_key.public_serial(False)[:4], bundle_id[:4])
-            ks = []
-            for k, v in self.awaiting_ack.items():
-                if v[1] == bundle_id:
-                    ks.append(k)
-            for k in ks:
-                self.awaiting_ack.pop(k)
+        finally:
+            if connection:
+                self.logger.info("%s: %s disconnected", self.broker_key.public_serial()[:4], connection.session.session_id[:4])
+                await connection.close(self.sessions)
 
-    async def listen(self):
-        n_tries = 0
-        while True:
-            try:
-                await self._connect()
-                while True:
-                    await self.recv()
-                    n_tries = 0
-            except Exception:
-                self.logger.warning("%s Connection.listen", self.session.session_key.public_serial(False)[:4], exc_info=True)
+    async def handle_message(self, connection, message):
+        try:
+            headers = self.decode_header(message)
+            for action, args in headers:
+                if action == "listen":
+                    self.handle_listen(connection, **args)
+                if action == "token":
+                    await self.handle_tokens(connection, *args)
+                if action == "broker":
+                    await self.handle_broker_action(connection, *args)
+                if action == "send":
+                    await self.handle_send(connection, message, **args)
+                if action == "close":
+                    self.handle_close(connection, **args)
+
+        except Exception:
+            self.logger.error(
+                "%s: %s .handle_message",
+                self.broker_key.public_serial()[:4],
+                connection.session.session_id[:4],
+                exc_info=True,
+            )
+            self.logger.info("%s: %s disconnected", self.broker_key.public_serial()[:4], connection.session.session_id[:4])
+            await connection.close(self.sessions)
 
-            self.is_connecting_lock.clear()
-            await asyncio.sleep(1)
+    async def handle_send(self, connection, message, source, destination):
+        self.logger.info(
+            "%s: send %s %s ??? %s ??? %s %s",
+            self.broker_key.public_serial()[:4],
+            source["session"][0][:4],
+            source["channel"][:4],
+            str(len(message) // 2 ** 10),
+            destination["session"][0][:4],
+            destination["channel"][:4],
+        )
+        s = Route(**source)
+        d = Route(**destination)
 
-            if n_tries > self.MAX_SEND_RETRIES:
-                self.is_connecting_lock.set()
-                raise ConnectionError("%s Max tries reached" % self.session.session_key.public_serial(False)[:4])
-            n_tries += 1
-
-    async def recv(self):
-        if not self.websocket or self.websocket.closed:
-            if self.is_connecting_lock.is_set():
-                await self.reconnect()
+        dest_session = self.sessions.get(d.session[0])
+        if dest_session:
+            dest_channel = await dest_session.expect_channel(d.channel)
+
+            if dest_session.channels.get(d.channel):
+                if await dest_channel.validate_token_chain(s.session[0], d.tokens, self):
+                    self.logger.info(
+                        "%s: send %s %s >>> %s >>> %s %s",
+                        self.broker_key.public_serial()[:4],
+                        source["session"][0][:4],
+                        source["channel"][:4],
+                        str(len(message) // 2 ** 10),
+                        destination["session"][0][:4],
+                        destination["channel"][:4],
+                    )
+                    if connection.session.session_id != s.session[0]:
+                        try:
+                            len_h = int.from_bytes(message[68:70], "big")
+                            PublicKey(s.session[0]).verify(message[:64], message[64 : 73 + len_h + 65 + 32])
+                        except InvalidSignature:
+                            return
+
+                    for connection in dest_channel.connections:
+                        await connection.websocket.send(message)
+                    return
+                else:
+                    # print('|||||', [Token.decode(t) for t in s.tokens], [Token.decode(t) for t in d.tokens])
+                    self.logger.info(
+                        "%s: send %s %s ||| %s ||| %s %s",
+                        self.broker_key.public_serial()[:4],
+                        source["session"][0][:4],
+                        source["channel"][:4],
+                        str(len(message) // 2 ** 10),
+                        destination["session"][0][:4],
+                        destination["channel"][:4],
+                    )
             else:
-                await self.is_connecting_lock.wait()
+                if self.broker_key.public_serial() in (d.brokers or []):
+                    return
 
-        message = await self.websocket.recv()
+        if d.brokers:
+            for depth in sorted(self.topology_cache):
+                brokers = set(d.brokers).intersection(set(self.topology_cache[depth].keys()))
+                if brokers:
+                    for broker_id in brokers:
+                        for broker_connection in self.topology_cache[depth][broker_id]:
+                            for enc_token in d.tokens:
+                                token = Token.decode(enc_token, False)
+                                if (
+                                    self.broker_key.public_serial() in token.brokers
+                                    and token.issuer in self.sessions
+                                    and token.signature in self.sessions[token.issuer].active_tokens
+                                    and enc_token == self.sessions[token.issuer].active_tokens.get(token.signature).encode()
+                                ):
+                                    await broker_connection.send((("token", ("approve", enc_token)),))
+                            await broker_connection.websocket.send(message)
+                            self.logger.info(
+                                "%s: send %s %s ))) %s ))) %s %s (%s)",
+                                self.broker_key.public_serial()[:4],
+                                source["session"][0][:4],
+                                source["channel"][:4],
+                                str(len(message) // 2 ** 10),
+                                destination["session"][0][:4],
+                                destination["channel"][:4],
+                                broker_id[:4],
+                            )
+                    return
+            for peer in set().union(*self.topology_cache[0].values()):
+                await peer.send(
+                    [
+                        (
+                            "broker",
+                            (
+                                "topology_update",
+                                {"source": self.broker_key.public_serial(), "destinations": d.brokers, "counter": 0},
+                            ),
+                        )
+                    ]
+                )
 
-        signature, timestamp = message[:64], int.from_bytes(message[64:68], "big")
+    def handle_listen(self, connection, session, channel, brokers, is_public=False):
+        if session[0] == connection.session.session_id:
+            self.logger.info(
+                "%s: listen %s %s %s",
+                self.broker_key.public_serial()[:4],
+                str(connection.session.session_id[:4]),
+                str(channel[:4]),
+                str(is_public),
+            )
+
+            if channel not in connection.session.channels:
+                connection.session.channels[channel] = Channel(connection.session, channel, is_public)
 
-        if self.session.check_no_repeat(signature, timestamp + self.t_offset):
+            channel_obj = connection.session.channels[channel]
+            channel_obj.connections.add(connection)
+            connection.channels.add(channel_obj)
+
+            event = connection.session.expecting_channels.pop(channel, None)
+            if event:
+                event.set()
 
-            len_h, len_p = [int.from_bytes(x, "big") for x in [message[68:70], message[70:73]]]
-            header = ujson.loads(message[73 : 73 + len_h])
-            full_payload = message[73 + len_h : 73 + len_h + len_p]
+    def handle_close(self, connection, session, channel, **kwargs):
+        if session[0] == connection.session.session_id:
             self.logger.info(
-                "%s received: %s %s",
-                self.session.session_key.public_serial(False)[:4],
-                " ".join(h[0] for h in header),
-                len(full_payload),
+                "%s: close %s %s",
+                self.broker_key.public_serial()[:4],
+                str(connection.session.session_id[:4]),
+                str(channel[:4]),
             )
-            for action, content in header:
-                if action == "send":
-                    source, destination = Route(**content["source"]), Route(**content["destination"])
-                    PublicKey(source.session[0]).verify(signature, message[64 : 73 + len_h + 65 + 32])
-                    if self.session.channels.get(destination.channel):
-                        channel = self.session.channels.get(destination.channel)
-                        if full_payload[0] == 255:
-                            self.ack(source.session[0], full_payload[1:65])
-                        else:
-                            ret_signature = signature if (full_payload[0] == 0) else full_payload[1:65]
-                            payload = full_payload[65 + 32 :]
-                            await self.send(
-                                (("send", {"destination": content["source"], "source": content["destination"]}),),
-                                b"",
-                                None,
-                                ret_signature,
-                            )
-                            # print(self.session.session_key.public_serial(False)[:4], 'sent ack', ret_signature[:4])
-                            if hashlib.sha256(payload).digest() == full_payload[65 : 65 + 32]:
-                                if (ret_signature == signature) or self.session.check_no_repeat(
-                                    ret_signature, timestamp + self.t_offset
-                                ):
-                                    channel.handle_message(source, destination, payload, message[: 73 + len_h + 65 + 32])
-                            else:
-                                raise AssertionError("Message payload does not match signed hash")
-
-    def ack(self, source_id, message_id):
-        # print(self.session.session_key.public_serial(False)[:4], 'received ack', message_id[:4], 'from', source_id[:4])
-        header = self.awaiting_ack.get(message_id, [[]])[0]
-        for action, content in header:
-            if action == "send":
-                if content["destination"]["session"][0] == source_id:
-                    t = self.awaiting_ack.pop(message_id)
-                    t[2].set()
-                    if self.awaiting_ack:
-                        self.awaiting_ack[list(self.awaiting_ack.keys())[0]][2].set()
-
-    def __await__(self):
-        async def await_lock():
-            if self.listener:
-                await self.is_connecting_lock.wait()
-                if self.listener.done():
-                    old_listener = self.listener
-                    self.listener = None
-                    await old_listener
-            else:
-                await self.reconnect()
 
-            return self
+            if connection.session.channels.get(channel):
+                channel_obj = connection.session.channels.get(channel)
+                connection.channels.remove(channel_obj)
+                channel_obj.connections.remove(connection)
+                if not channel_obj.connections:
+                    channel_obj.close()
+
+    async def handle_tokens(self, connection, action, *args):
+        if action == "issue":
+            tokens = [Token.decode(x) for x in args if x]
+            token = tokens[0]
+            if connection.session.session_id == token.issuer:
+                self.logger.info(
+                    "%s: tokens %s %s -> %s: %s (%s)",
+                    self.broker_key.public_serial()[:4],
+                    token.issuer[:4],
+                    action,
+                    token.signature[:4],
+                    str(token.receiver[:4]),
+                    token.asset[:4],
+                )
+                if token.token_type == "root":
+                    connection.session.active_tokens[token.signature] = token
+                elif token.token_type == "extension":
+                    prev_token = tokens[1]
+                    if await self.check_token(prev_token):
+                        connection.session.approve_token(token)
+
+        if action == "revoke":
+            token = connection.session.active_tokens.get(args[0])
+            if token:
+                self.logger.info(
+                    "%s: tokens %s %s %s",
+                    self.broker_key.public_serial()[:4],
+                    str(token.issuer[:4]),
+                    action,
+                    str(token.signature[:4]),
+                )
+                connection.session.active_tokens.pop(token.signature, None)
+
+        if action == "validate":
+            token = Token.decode(args[0], False)
+            if token.issuer in self.sessions:
+                if await self.check_token(token):
+                    broker_connection = connection.session.broker_connections.get(connection)
+                    if broker_connection:
+                        self.logger.info(
+                            "%s: tokens %s %s %s",
+                            self.broker_key.public_serial()[:4],
+                            str(token.issuer[:4]),
+                            action,
+                            str(token.signature[:4]),
+                        )
+                        await broker_connection.send((("token", ("approve", token.encode())),))
 
-        return await_lock().__await__()
+        if action == "approve":
+            token = Token.decode(args[0])
+            self.logger.info(
+                "%s: tokens %s %s %s",
+                self.broker_key.public_serial()[:4],
+                str(token.issuer[:4]),
+                action,
+                str(token.signature[:4]),
+            )
+            connection.session.approve_token(token)
 
+    async def handle_broker_action(self, connection, action, params=None):
+        if action == "open":
+            peer = Peer(connection.websocket, self)
+            session_id = connection.session.session_id
+            connection.session.broker_connections[connection] = peer
+            self.topology_cache[0][session_id] = (self.topology_cache[0].get(session_id) or set()).union([peer])
+        if action == "close":
+            connection.session.broker_sessions.pop(connection, None)
+        if action == "topology_update" and params:
+            self.logger.info("%s: topology %s", self.broker_key.public_serial()[:4], str(params))
+            # if self.check_no_repeat...
+            peer = connection.session.broker_connections[connection]
+            if self.broker_key.public_serial() == params["source"]:
+                # if check signature
+                for reply in params["replies"]:
+                    peer_set = self.topology_cache[params["replies"][reply]].get(reply) or set()
+                    peer_set = peer_set.union([peer])
+                    self.topology_cache[params["replies"][reply]][reply] = peer_set
+            elif "replies" in params:
+                for reply in params["replies"]:
+                    params["replies"][reply] += 1
+                for depth in self.topology_cache:
+                    source_set = self.topology_cache[depth].get(params["source"])
+                    if source_set:
+                        for conn in source_set:
+                            await conn.send([("broker", ("topology_update", params))])
+                        return
+            else:
+                destination_set = set(params["destinations"]).intersection(set(self.topology_cache[0].keys()))
+                if destination_set:
+                    params["replies"] = {d: 0 for d in destination_set}
+                    await peer.send([("broker", ("topology_update", params))])
+                    return
+                params["counter"] += 1
+                source_set = self.topology_cache[params["counter"]].get(params["source"]) or set()
+                self.topology_cache[params["counter"]][params["source"]] = source_set.union([peer])
+
+                for forwarded in set().union(self.topology_cache[0].values()):
+                    await peer.send([("broker", ("topology_update", params))])
+
+    async def add_broker(self, url, inherit_entrypoint=False):
+        peer = Peer(None, self)
+        if re.sub(r"(?![\w\d]+:\/\/[\w\d.]+):[\d]+", "", url) == url:
+            i = len(re.findall(r"[\w\d]+:\/\/[\w\d.]+", url)[0])
+            url = url[:i] + ":8776" + url[i:]
+
+        await peer.connect(url, inherit_entrypoint)  # This already adds the peer to self.sessions
+
+    async def check_token(self, token):
+        session = self.sessions.get(token.issuer)
+        if session:
+            if token.signature in session.active_tokens:
+                return token.encode() == session.active_tokens.get(token.signature).encode()
+            else:
+                event = asyncio.Event()
+                session.expecting_tokens[token.signature] = (event, token)
+                session.tasks.add(asyncio.get_event_loop().create_task(session.clean_expecting_token(token)))
+                await asyncio.wait_for(event.wait(), 2)
 
-class Session:
-    def __init__(self, session_key=None, session_key_pass=None):
-        self.session_key = session_key if isinstance(session_key, PrivateKey) else PrivateKey(session_key, session_key_pass)
-        self.instance_id = base64.b64encode(os.urandom(6)).decode()
-        self.channels = {}
-        self.targets = {}
-        self.routes = {}
-        self.connections = set()
-        self.seen_messages = [set(), set(), 0]
-        self.issued_tokens = {}
-        self.pending_tasks = set()
-        self.message_listener = None
-        self.logger = logging.getLogger(__name__)
+                return True
+        else:
+            event = asyncio.Event()
+            for broker in token.brokers:
+                if broker in self.sessions and await self.sessions[broker].validate_peer_token(token, event):
+                    break
+            else:
+                try:
+                    await asyncio.wait_for(event.wait(), 2)
+                except asyncio.exceptions.TimeoutError:
+                    return False
+            return True
 
-    def check_no_repeat(self, signature, timestamp):
+    def check_no_repeat(self, message):
+        signature, timestamp = message[:64], int.from_bytes(message[64:68], "big")
         now = int(time.time())
 
         lead = now // 60
         if self.seen_messages[2] != lead:
             self.seen_messages[lead % 2].clear()
             self.seen_messages[2] = lead
 
         if (now - 60 + 4) <= timestamp <= now + 4:
             if signature not in self.seen_messages[0].union(self.seen_messages[1]):
                 self.seen_messages[lead % 2].add(signature)
                 return True
-        return False
-
-    def issue_token(self, target, receiver, max_depth=None):
-        if isinstance(target, Token):
-            token_type = "extension"
-            prev_token = target
-            asset = target.signature
-        else:
-            token_type = "root"
-            prev_token = None
-            asset = target
-
-        for token, prev_token_tmp in self.issued_tokens.values():
-            if (
-                token.asset == asset
-                and token.receiver == receiver
-                and token.token_type == token_type
-                and token.max_depth == max_depth
-                and all([x.broker_id in token.brokers for x in self.connections])
-            ):
-                prev_token = prev_token_tmp
-                break
-        else:
-            token = Token(
-                self.session_key.public_serial(False),
-                [x.broker_id for x in self.connections],
-                receiver,
-                asset,
-                token_type,
-                max_depth,
-            )
-            signature = token.sign(self.session_key)
 
-            self.issued_tokens[signature] = token, prev_token
-
-        return ("token", ("issue", token.encode(), prev_token and prev_token.encode()))
-
-    def revoke_tokens(self, asset):
-        children = [tid for tid, t in self.issued_tokens.items() if t[0].asset == asset]
-        [self.revoke_tokens(tid) for tid in children]
-        self.issued_tokens.pop(asset, None)
-
-    def extend_route(self, route, receiver, max_depth=None):
-
-        if route.session[0] == self.session_key.public_serial(False):
-            token_header = self.issue_token(route.channel, receiver, max_depth)
-            route.tokens = [token_header[1][1]]
-            return token_header
-
-        for i, enc_token in enumerate(route.tokens):
-            token = Token.decode(enc_token)
-            if token.receiver == self.session_key.public_serial(False):
-                route.tokens = route.tokens[: i + 1]
-
-        token = Token.decode(route.tokens[-1], False)
-        token_header = self.issue_token(token, receiver, max_depth)
-        route.tokens.append(token_header[1][1])
-
-    def clear(self, bundle_id):
-        for connection in self.connections:
-            connection.clear(bundle_id)
+        return False
 
-    async def send(self, header, payload=b"", bundle_id=None):
-        for connection in self.connections:
-            await connection.send(header, payload, bundle_id)
+    def decode_header(self, m):
+        header = ujson.loads(m[73 : 73 + int.from_bytes(m[68:70], "big")])
+        return header
+
+    async def serve(self, host="127.0.0.1", port=8776, **kwargs):
+        if "compression" not in kwargs:
+            kwargs["compression"] = None
+        server = await websockets.serve(self.handle_connection, host, port, **kwargs)
+        self.servers[(host, port)] = server
 
-    def __repr__(self):
-        return "Session %s %s" % (
-            self.session_key.public_serial(False)[:4],
-            self.instance_id[:2],
-        )
+        return self
 
+    async def close(self, host=None, port=None):
+        keys = set(self.servers.keys())
+        for server_host, server_port in keys:
+            if not host or server_host == host:
+                if not port or server_port == port:
+                    self.servers.pop((server_host, server_port)).close()
 
-class Channel:
-    def __init__(self, session, channel_key=None, channel_key_pass=None, is_public=False):
-        self.MAX_PAYLOAD_LEN = 2 ** 19
-        self.MAX_COMPRESSION_LEN = 2 ** 19
-        self.MAX_OUTBOX = 2 ** 4
 
-        self.session = session
-        self.channel_key = channel_key if isinstance(channel_key, PrivateKey) else PrivateKey(channel_key, channel_key_pass)
-        self.is_public = is_public
-        self.route = Route(
-            list(set(c.broker_id for c in self.session.connections)),
-            (self.session.session_key.public_serial(False), self.session.instance_id),
-            self.channel_key.public_serial(False),
-        )
-        self.header_buffer = []
-        self.chunks = {}
-        self.messages = deque()
+class Peer(Connection):
+    def __init__(self, websocket, broker):
+        super().__init__(websocket)
+        self.broker = broker
+        self.t_offset = 0
+        self.listener = None
+        self.url = None
         self.lock = asyncio.Event()
-        session.channels[self.channel_key.public_serial(False)] = self
-
-        self.telekinesis = None
+        self.exception = None
 
-    def handle_message(self, source, destination, raw_payload, proof):
-        if self.validate_token_chain(source.session[0], destination.tokens):
-            message_tuple = None
-            shared_key = SharedKey(self.channel_key, PublicKey(source.channel))
-            payload = shared_key.decrypt(raw_payload[16:], raw_payload[:16])
-            metadata = RequestMetadata(
-                self.session, source, [{"raw_payload": raw_payload, "shared_key": shared_key.key, "proof": proof}]
-            )
-
-            if payload[:4] == b"\x00" * 4:
-                if payload[4] == 0:
-                    message_tuple = (metadata, bson.loads(payload[5:]))
-                elif payload[4] == 255:
-                    message_tuple = (metadata, bson.loads(zlib.decompress(payload[5:])))
-                else:
-                    raise BufferError("Received message with different encoding")
-            else:
-                ir, nr, mmid, chunk = payload[:2], payload[2:4], payload[4:8], payload[8:]
-                i, n = int.from_bytes(ir, "big"), int.from_bytes(nr, "big")
-
-                mid = source.session[0].encode() + mmid
-                if mid not in self.chunks:
-                    self.chunks[mid] = {}
-                self.chunks[mid][i] = (chunk, metadata)
-
-                if len(self.chunks[mid]) == n:
-                    chunks = self.chunks.pop(mid)
-                    payload = b"".join(chunks[ii][0] for ii in range(n))
-
-                    combined_metadata = RequestMetadata(
-                        metadata._session, metadata.caller, [chunks[ii][1].raw_messages[0] for ii in range(n)]
-                    )
-                    if payload[0] == 0:
-                        message_tuple = (combined_metadata, bson.loads(payload[1:]))
-                    elif payload[0] == 255:
-                        message_tuple = (combined_metadata, bson.loads(zlib.decompress(payload[1:])))
-                    else:
-                        raise BufferError("Received message with different encoding")
-
-            if message_tuple:
-                if self.session.message_listener:
-                    self.session.message_listener(message_tuple[0])
-                # print('<<<', source, destination, {k: v is None for k, v in message_tuple[1].items()})
-                if not self.telekinesis:
-                    self.messages.appendleft(message_tuple)
-                    self.lock.set()
-                else:
-                    asyncio.get_event_loop().create_task(self.telekinesis._handle_request(self, *message_tuple))
-        else:
-            self.session.logger.error(
-                "Invalid Tokens: %s %s -> %s %s [%s]",
-                source.session[0][:4],
-                source.channel[:4],
-                destination.session[0][:4],
-                destination.channel[:4],
-                destination.tokens,
-            )
-
-    async def recv(self):
-        if not self.messages:
-            self.lock.clear()
-            await self.lock.wait()
-
-        return self.messages.pop()
-
-    def listen(self):
-        listen_dict = self.route.to_dict()
-        listen_dict["is_public"] = self.is_public
-        listen_dict.pop("tokens")
-        self.header_buffer.append(("listen", listen_dict))
+    def connect(self, url, inherit_entrypoint):
+        self.url = url
+        self.listener = asyncio.get_event_loop().create_task(self.listen(inherit_entrypoint))
 
         return self
 
-    async def send(self, destination, payload_obj):
-        # if payload_obj:
-        # print('>>>', self.route, destination, {k: v is None for k, v in payload_obj.items()})
-        def encrypt_slice(payload, max_payload, shared_key, message_id, n, i):
-            if i < n:
-                if n == 1:
-                    chunk = b"\x00" * 4 + payload
-                else:
-                    if n > 2 ** 16:
-                        raise MemoryError(f"Payload size {len(payload)/2**20} MiB is too large")
-                    chunk = i.to_bytes(2, "big") + n.to_bytes(2, "big") + message_id + payload[i * max_payload : (i + 1) * max_payload]
-
-                nonce = os.urandom(16)
-                yield nonce + shared_key.encrypt(chunk, nonce)
-                yield from encrypt_slice(payload, max_payload, shared_key, message_id, n, i + 1)
-
-        async def execute(header, encrypted_slice_generator, message_id):
-            for encrypted_slice in encrypted_slice_generator:
-                await self.execute(header, encrypted_slice, message_id)
-
-        source_route = self.route.clone()
-        self.session.extend_route(source_route, destination.session[0])
-        self.listen()
-
-        payload = bson.dumps(payload_obj)
-
-        if len(payload) < self.MAX_COMPRESSION_LEN:
-            payload = b"\xff" + zlib.compress(payload)
-        else:
-            payload = b"\x00" + payload
-
-        message_id = os.urandom(4)
-        shared_key = SharedKey(self.channel_key, PublicKey(destination.channel))
-
-        header = ("send", {"source": source_route.to_dict(), "destination": destination.to_dict()})
-
-        n = (len(payload) - 1) // self.MAX_PAYLOAD_LEN + 1
-        n_tasks = min(n, self.MAX_OUTBOX)
-        gen = encrypt_slice(payload, self.MAX_PAYLOAD_LEN, shared_key, message_id, n, 0)
-
-        try:
-            await asyncio.gather(*(execute(header, gen, message_id) for _ in range(n_tasks)))
-        except asyncio.CancelledError:
-            self.session.clear(message_id)
-            raise asyncio.CancelledError
-        finally:
-            self.session.clear(message_id)
+    async def reconnect(self):
+        if self.websocket:
+            await self.websocket.close()
 
-        return self
+        self.websocket = await websockets.connect(self.url)
 
-    async def execute(self, header=None, payload=b"", bundle_id=None):
-        all_headers = [h for h in self.header_buffer + [header] if h]
-        lens = tuple((len(ujson.dumps(h, escape_forward_slashes=False)), h) for h in all_headers)
-
-        groups = [[]]
-        acc_len = 1
-        for l, h in lens:
-            if acc_len + l + 1 < 256**2:
-                groups[-1].append(h)
-                acc_len += l + 1
-            else:
-                groups.append([h])
-                acc_len = l + 2
+        challenge = await self.websocket.recv()
+        t_broker = int.from_bytes(challenge[-4:], "big")
 
-        for group in groups:
-            await self.session.send(group, payload if 'send' in set(h[0] for h in group) else b'', bundle_id)
-        self.header_buffer = []
+        self.t_offset = int(time.time()) - t_broker
+        signature = self.broker.broker_key.sign(challenge)
 
-        return self
+        pk = self.broker.broker_key.public_serial().encode()
 
-    def __await__(self):
-        return self.execute().__await__()
+        sent_challenge = os.urandom(32)
+        sent_metadata = {"version": get_distribution(__name__.split(".")[0]).version}
+        await self.websocket.send(signature + pk + sent_challenge + ujson.dumps(sent_metadata).encode())
 
-    def close(self):
-        self.header_buffer.append(("close", self.route.to_dict()))
-        self.session.revoke_tokens(self.channel_key.public_serial(False))
+        m = await asyncio.wait_for(self.websocket.recv(), 15)
 
-        self.session.channels.pop(self.channel_key.public_serial(False), None)
+        if m[: len("Incompatible")] == b"Incompatible":
+            raise Exception(m.decode())
 
-        return self
+        signature, session_id, metadata = m[:64], m[64:152].decode(), ujson.loads(m[152:].decode())
+        PublicKey(session_id).verify(signature, sent_challenge)
 
-    def validate_token_chain(self, source_id, tokens):
-        if self.is_public or (source_id == self.session.session_key.public_serial(False)):
-            return True
-        if not tokens:
-            return False
+        entrypoint = Route(**metadata.get("entrypoint")) if metadata.get("entrypoint") else None
 
-        asset = self.channel_key.public_serial(False)
-        last_receiver = self.session.session_key.public_serial(False)
-        max_depth = None
+        await self.send([("broker", ("open",))])
 
-        for depth, token_string in enumerate(tokens):
-            try:
-                token = Token.decode(token_string)
-            except InvalidSignature:
-                return False
-            if (token.asset == asset) and (token.issuer == last_receiver):
-                if token.issuer == self.session.session_key.public_serial(False):
-                    if token.signature not in self.session.issued_tokens:
-                        return False
-                if token.max_depth:
-                    if not max_depth or (token.max_depth + depth) < max_depth:
-                        max_depth = token.max_depth + depth
-                if not max_depth or depth < max_depth:
-                    last_receiver = token.receiver
-                    asset = token.signature
-                    if last_receiver == source_id:
-                        return True
-                    continue
-            return False
-        return False
+        return session_id, entrypoint
 
-    def __repr__(self):
-        return "Channel %s %s - %s: %s" % (
-            self.session.session_key.public_serial(False)[:4],
-            self.session.instance_id[:2],
-            self.channel_key.public_serial(False)[:4],
-            self.telekinesis,
+    async def send(self, header):
+        h = ujson.dumps(header).encode()
+        m = len(h).to_bytes(2, "big") + (0).to_bytes(3, "big") + h
+        t = int(time.time() - self.t_offset - 4).to_bytes(4, "big")
+        s = self.broker.broker_key.sign(
+            t + m,
         )
 
-    async def __aenter__(self):
-        return self#.listen()
+        await self.websocket.send(s + t + m)
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self.close()
-
-        return isinstance(exc_type, Exception)
-
-    def __getstate__(self):
-        out = self.__dict__
-        out['lock'] = None
-        return out
+    async def listen(self, inherit_entrypoint):
+        n_tries = 0
+        while True:
+            try:
+                self.lock.clear()
+                session_id, entrypoint = await self.reconnect()
 
-    def __setstate__(self, state):
-        self.__dict__.update(state)
-        self.lock = asyncio.Event()
-        if self.telekinesis:
-            self.telekinesis._session = self.session
+                if not (-15 < self.t_offset < 2):
+                    raise IncompatibleBrokerException(f"Unix time difference too large: {self.t_offset} seconds.")
+                self.lock.set()
+
+                if session_id not in self.broker.sessions:
+                    self.broker.sessions[session_id] = Session(session_id)
+
+                if inherit_entrypoint:
+                    self.broker.entrypoint = entrypoint
+
+                self.session = self.broker.sessions[session_id]
+                self.session.connections.add(self)
+                self.session.broker_connections[self] = self
+                self.broker.topology_cache[0][session_id] = (self.broker.topology_cache[0].get(session_id) or set()).union(
+                    [self]
+                )
 
+                n_tries = 0
+                while True:
+                    message = await self.websocket.recv()
+                    self.tasks.add(asyncio.get_event_loop().create_task(self.broker.handle_message(self, message)))
 
-class Route:
-    def __init__(self, brokers, session, channel, tokens=None, parent_channel=None, **_):
-        self.brokers = brokers
-        self.session = tuple(session)
-        self.channel = channel
-        self.tokens = tokens or []
-        self._parent_channel = parent_channel
-
-    def to_dict(self):
-        return {"brokers": self.brokers, "session": self.session, "channel": self.channel, "tokens": self.tokens }
-
-    def clone(self):
-        return Route(**self.to_dict())
-
-    def validate_token_chain(self, receiver):
-        if self.session[0] != receiver:
-            assert len(self.tokens) > 0
-            prev_token = None
-            for i, raw_token in enumerate(self.tokens):
-                token = Token.decode(raw_token)
-                if i == 0:
-                    assert token.asset == self.channel
-                    assert token.issuer == self.session[0]
-                    assert token.token_type == "root"
-                else:
-                    assert token.asset == prev_token.signature
-                    assert token.issuer == prev_token.receiver
-                    assert token.token_type == "extension"
-                if token.receiver == receiver:
-                    break
-                prev_token = token
-            else:
-                return False
-        return True
+                    # await asyncio.gather(*(x for x in self.tasks if x.done() and not x.exception()), return_exceptions=True)
+                    self.tasks = set(x for x in self.tasks if not x.done())
 
-    def __repr__(self):
-        return f"Route {self.session[0][:4]} {self.session[1][:2]} - {self.channel[:4]}"
+            except IncompatibleBrokerException as e:
+                self.logger.error("Peer.listen", exc_info=True)
+                self.exception = e
+                await self.close(self.broker.sessions, False)
+                self.lock.set()
+                return
 
-    def __eq__(self, route):
-        return self.to_dict() == route.to_dict()
+            except Exception:
+                self.logger.error("Peer.listen", exc_info=True)
+                await self.close(self.broker.sessions, False)
+                self.lock.set()
+
+                if n_tries > 10:
+                    self.logger.error("Peer.listen: Max connection retries reached", exc_info=True)
+                    return
 
-    def __hash__(self):
-        return ujson.dumps(self.to_dict()).__hash__()
+                await asyncio.sleep(1)
+                n_tries += 1
+                continue
 
     def __await__(self):
-        async def await_parent_channel():
-            await self._parent_channel
-            return self
-
-        return self._parent_channel and await_parent_channel().__await__()
+        async def wait_lock():
+            await self.lock.wait()
+            if self.exception:
+                raise self.exception
+
+        return wait_lock().__await__()
 
 
-class RequestMetadata:
-    def __init__(self, session, caller, raw_messages):
-        self._session = session
-        self.session_public_key = session.session_key.public_serial(False)
-        self.caller = caller
-        self.raw_messages = raw_messages
-        self.reply_to = None
-        self.pipeline = None
+class IncompatibleBrokerException(Exception):
+    pass
```

### Comparing `telekinesis-0.1.81/telekinesis/cryptography.py` & `telekinesis-0.1.9/telekinesis/cryptography.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,73 +7,52 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.exceptions import InvalidSignature
 
 
 class PrivateKey:
-    def __init__(self, key_file=None, password=None, name=None):
-        self._public_serial_cache = None
-        self.name = name
+    def __init__(self, key_file=None, password=None):
         if key_file and os.path.exists(key_file):
-            with open(key_file, "r") as kf:
+            with open(key_file, "rb") as kf:
                 data = kf.read()
-            pk = PrivateKey.from_private_serial(data, password)
-            self.key = pk.key
-            self.name = pk.name
+            self.key = serialization.load_pem_private_key(
+                data, None if password is None else password.encode(), default_backend()
+            )
             return
 
         self.key = ec.generate_private_key(curve=ec.SECP256R1, backend=default_backend())
 
         if key_file:
-            self.save_key_file(key_file, password)
+            with open(key_file, "wb") as kf:
+                enc = (
+                    serialization.NoEncryption()
+                    if password is None
+                    else serialization.BestAvailableEncryption(password.encode())
+                )
+                data = self.key.private_bytes(
+                    encoding=serialization.Encoding.PEM,
+                    format=serialization.PrivateFormat.PKCS8,
+                    encryption_algorithm=enc,
+                )
+                kf.write(data)
 
     def sign(self, m):
         signature = self.key.sign(m, ec.ECDSA(hashes.SHA256()))
         r, s = utils.decode_dss_signature(signature)
         return b"".join([x.to_bytes(32, "big") for x in (r, s)])
 
-    def public_serial(self, show_name=True):
-        if not self._public_serial_cache:
-            Q = self.key.public_key().public_numbers()
-            self._public_serial_cache = base64.b64encode(b"".join([x.to_bytes(32, "big") for x in (Q.x, Q.y)])).decode()
-        return (f'{self.name}.' if self.name and show_name else '') + self._public_serial_cache
-
-    def private_serial(self, password=None):
-        enc = (
-            serialization.NoEncryption()
-            if password is None
-            else serialization.BestAvailableEncryption(password.encode())
-        )
-        return self.key.private_bytes(
-            encoding=serialization.Encoding.PEM, format=serialization.PrivateFormat.PKCS8, encryption_algorithm=enc,
-        ).decode() + (f'\n{self.name}' if self.name else '')
-
-    def save_key_file(self, key_file, password=None):
-        with open(key_file, "w") as kf:
-            kf.write(self.private_serial(password))
-
-    @staticmethod
-    def from_private_serial(data, password=None):
-        out = PrivateKey()
-        end = '-----END PRIVATE KEY-----' if '-----END PRIVATE KEY-----' in data else '-----END ENCRYPTED PRIVATE KEY-----'
-        serial, *name = data.split(end)
-        out.name = end.join(name).replace('\n', '') if name else None
-        serial += end
-        out.key = serialization.load_pem_private_key(
-            data.encode(), None if password is None else password.encode(), default_backend()
-        )
-        return out
+    def public_serial(self):
+        Q = self.key.public_key().public_numbers()
+        return base64.b64encode(b"".join([x.to_bytes(32, "big") for x in (Q.x, Q.y)])).decode()
 
 
 class PublicKey:
     def __init__(self, public_serial):
-        self.public_serial = public_serial
-        self.key = ec.EllipticCurvePublicKey.from_encoded_point(ec.SECP256R1(), b"\x04" + base64.b64decode(public_serial.split('.')[-1]))
-        self.name = '.'.join(public_serial.split('.')[:-1])
+        self.key = ec.EllipticCurvePublicKey.from_encoded_point(ec.SECP256R1(), b"\x04" + base64.b64decode(public_serial))
 
     def verify(self, raw_signature, message):
         r = int.from_bytes(raw_signature[:32], "big")
         s = int.from_bytes(raw_signature[32:], "big")
 
         signature = utils.encode_dss_signature(r, s)
 
@@ -102,25 +81,27 @@
         brokers,
         receiver,
         asset,
         token_type,
         max_depth=None,
         valid_from=None,
         valid_until=None,
+        fail_mode="CLOSED",
         metadata=None,
     ):
         self.issuer = issuer
         self.brokers = brokers
         self.receiver = receiver
         self.asset = asset
         self.token_type = token_type
         self.max_depth = max_depth
         self.valid_from = valid_from or time.time()
         self.valid_until = valid_until
         self.metadata = metadata or {}
+        self.fail_mode = fail_mode
         self.signature = None
 
     def verify(self, signature):
         try:
             PublicKey(self.issuer).verify(base64.b64decode(signature.encode()), self._to_string().encode())
             self.signature = signature
             return True
@@ -135,24 +116,25 @@
                 "brokers",
                 "receiver",
                 "asset",
                 "token_type",
                 "max_depth",
                 "valid_from",
                 "valid_until",
+                "fail_mode",
                 "metadata",
             ]
         }
 
     def _to_string(self):
         return ujson.dumps(self._to_dict(), escape_forward_slashes=False)
 
     def encode(self):
         if not self.signature:
-            raise RuntimeError("You need to sign the token before encoding it")
+            raise Exception("You need to sign the token before encoding it")
         return self.signature + "." + self._to_string()
 
     def sign(self, signing_key):
         self.signature = base64.b64encode(signing_key.sign(self._to_string().encode())).decode()
         return self.signature
 
     def __repr__(self):
```

### Comparing `telekinesis-0.1.81/telekinesis/telekinesis.py` & `telekinesis-0.1.9/telekinesis/telekinesis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,198 +1,169 @@
-import asyncio
 import sys
+import io
+import time
+import asyncio
 import inspect
-import types
 import traceback
 import logging
+from functools import partialmethod
+
 import re
+import makefun
 
-from .client import Route, Channel, RequestMetadata
+from .client import Route, Channel
 
 
 class State:
-    def __init__(self, attributes=None, methods=None, repr=None, doc=None, name=None, pipeline=None):
-        self.attributes = {} if attributes is None else (set(attributes) if isinstance(attributes, list) else attributes) 
+    def __init__(self, attributes=None, methods=None, repr=None, doc=None, pipeline=None):
+        self.attributes = (set(attributes) if isinstance(attributes, list) else attributes) or {}
         self.methods = methods or {}
         self.pipeline = pipeline or []
         self.repr = repr or ""
         self.doc = doc
-        self.name = name
         self._pending_changes = {}
         self._history_offset = 0
         self._history = []
 
     def to_dict(self, mask=None, cache_attributes=False):
         mask = mask or set()
         return {
             "attributes": {k: v for k, v in self.attributes.items() if k not in mask}
             if cache_attributes and isinstance(self.attributes, dict)
             else [k for k in self.attributes if k not in mask],
             "methods": {k: v for k, v in self.methods.items() if k not in mask},
             "pipeline": self.pipeline,
             "repr": self.repr,
             "doc": self.doc,
-            "name": self.name,
         }
 
     def clone(self):
         out = State(**self.to_dict(None, True))
         out._history = self._history.copy()
         out._history_offset = self._history_offset
         return out
 
     def get_diffs(self, last_version=0, mask=None, cache_attributes=False):
-        if last_version < self._history_offset:
+        if last_version < self._history_offset and last_version >= 0:
             return self._history_offset + len(self._history), self.to_dict(mask, cache_attributes)
         out = {}
-        for i, diff in enumerate(self._history[last_version - self._history_offset :]):
-            filtered = {}
-            if "attributes" in diff:
-                if cache_attributes:
-                    x = {k: v for k, v in diff["attributes"][1].items() if k not in (mask or set())}
-                else:
-                    x = {
-                        k: v[0] for k, v in diff["attributes"][1].items() if k not in (mask or set()) and v[0] in ["c", "d"]
-                    }
-                if x:
-                    filtered["attributes"] = (diff["attributes"][0], x)
-            if "methods" in diff:
-                x = {k: v for k, v in diff["methods"][1].items() if k not in (mask or set())}
-                if x:
-                    filtered["methods"] = (diff['methods'][0], x)
-            if "repr" in diff:
-                filtered["repr"] = diff["repr"]
-            if "doc" in diff:
-                filtered["doc"] = diff["doc"]
-            if "name" in diff:
-                filtered["name"] = diff["name"]
-            out[i + last_version + 1] = filtered
+        if last_version >= 0:
+            for i, diff in enumerate(self._history[last_version - self._history_offset :]):
+                filtered = {}
+                if "attributes" in diff:
+                    if cache_attributes:
+                        x = {k: v for k, v in diff["attributes"][1].items() if k not in (mask or set())}
+                    else:
+                        x = {
+                            k: v[0] for k, v in diff["attributes"][1].items() if k not in (mask or set()) and v[0] in ["c", "d"]
+                        }
+                    if x:
+                        filtered["attributes"] = (diff["attributes"][0], x)
+                if "methods" in diff:
+                    x = {k: v for k, v in diff["methods"].items() if k not in (mask or set())}
+                    if x:
+                        filtered["methods"] = x
+                if "repr" in diff:
+                    filtered["repr"] = diff["repr"]
+                if "doc" in diff:
+                    filtered["doc"] = diff["doc"]
+                out[i + last_version + 1] = filtered
         out["pipeline"] = self.pipeline
         return 0, out
 
     def update_from_target(self, target):
         logger = logging.getLogger(__name__)
 
         attributes, methods, repr_ = {}, {}, ""
 
         for attribute_name in dir(target):
             if attribute_name[0] != "_" or attribute_name in [
                 "__call__",
                 "__init__",
                 "__getitem__",
                 "__setitem__",
-                "__aiter__",
-                "__anext__",
                 "__add__",
                 "__mul__",
             ]:
                 try:
                     if isinstance(target, type):
-                        try:
-                            target_attribute = target.__getattribute__(target, attribute_name)
-                        except AttributeError:
-                            target_attribute = target.__getattr__(target, attribute_name)
+                        target_attribute = target.__getattribute__(target, attribute_name)
                     else:
-                        try:
-                            try:
-                                if attribute_name in dir(type(target)) and isinstance(type(target).__getattribute__(type(target), attribute_name), types.GetSetDescriptorType):
-                                    # Hack to avoid duplicating memory usage with numpy arrays
-                                    target_attribute = None
-                                else:
-                                    target_attribute = target.__getattribute__(attribute_name)
-                            except (AttributeError, TypeError):
-                                target_attribute = target.__getattribute__(attribute_name)
-                        except AttributeError:
-                            target_attribute = target.__getattr__(attribute_name)
+                        target_attribute = target.__getattribute__(attribute_name)
 
-                    if "__call__" in dir(target_attribute) and not isinstance(target_attribute, Telekinesis):
+                    if "__call__" in dir(target_attribute):
                         if attribute_name == "__call__" or (isinstance(target, type) and attribute_name == "__init__"):
                             target_attribute = target
                         signature = None
                         try:
                             signature = str(inspect.signature(target_attribute))
 
                             if "_tk_inject_first_arg" in dir(target_attribute) and target_attribute._tk_inject_first_arg:
                                 signature = (
                                     re.sub(r"[a-zA-Z0-9=\_\s]+(?=[\)\,])", "", signature, 1)
                                     .replace("(,", "(", 1)
                                     .replace("( ", "(", 1)
                                 )
-                        except Exception as e:
-                            logger.debug("Could not obtain signature from %s.%s: %s", target, attribute_name, e)
+                        except Exception:
+                            logger.debug("Could not obtain signature from %s.%s", target, attribute_name)
 
-                        if attribute_name == "__init__":
-                            if isinstance(target, type):
-                                methods["__call__"] = (signature, target.__init__.__doc__)
-                        elif attribute_name == '__call__':
-                            methods[attribute_name] = (
-                                signature, 
-                                (target_attribute.__call__.__doc__ or '')
-                            )
+                        if attribute_name == "__init__" and isinstance(target, type):
+                            methods["__call__"] = (signature, target.__init__.__doc__)
                         else:
-                            methods[attribute_name] = (signature, str(target_attribute.__doc__))
+                            methods[attribute_name] = (signature, target_attribute.__doc__)
                     else:
-                        if asyncio.iscoroutine(target_attribute):
-                            target_attribute.close()
-                            target_attribute = None
                         attributes[attribute_name] = target_attribute.copy() if type(target_attribute) in [dict, list, set] else target_attribute 
 
                 except Exception as e:
                     logger.error("Could not obtain handle for %s.%s: %s", target, attribute_name, e)
-        try:
-            name = target.__name__
-        except:
-            name = None
 
         if isinstance(target, type):
             repr_ = str(type(target))
             doc = target.__doc__
         else:
-            doc = target.__doc__
+            doc = None
             repr_ = target.__repr__()
 
         if self._history_offset == 0:
             self._history_offset = 1
             self.attributes = attributes
             self.methods = methods
             self.repr = repr_
             self.doc = doc
-            self.name = name
             return self
         diff = {}
         cmp = {
             "attributes": (self.attributes, attributes),
             "methods": (self.methods, methods),
             "repr": (self.repr, repr_),
             "doc": (self.doc, doc),
-            "name": (self.name, name)
         }
         for k in cmp:
             x = self.calc_diff(*cmp[k])
             if x:
                 diff[k] = x
 
         if diff:
             return self.update_from_diffs(0, {self._history_offset + len(self._history) + 1: diff})
         return self
 
     def update_from_diffs(self, last_version, diffs):
-        ks = ["attributes", "methods", "repr", "doc", "name"]
+        ks = ["attributes", "methods", "repr", "doc"]
         if last_version:
             self._history = []
             self._history_offset = last_version
             self._pending_changes = {}
             new_state = State(**diffs)
             for k in ks:
                 self.__dict__[k] = new_state.__dict__[k]
         else:
             next_version = self._history_offset + len(self._history) + 1
             diffs_int = {int(k): v for k, v in diffs.items() if k != "pipeline"}
             if next_version in diffs_int:
-                for i in range(len(diffs_int)-next_version+min(diffs_int.keys())):
+                for i in range(len(diffs_int)):
                     self._history.append(diffs_int[i + next_version])
                     for k in ks:
                         if k in diffs_int[i + next_version]:
                             self.__dict__[k] = self.apply_diff(self.__dict__[k], diffs_int[i + next_version][k])
 
                 for i in sorted(self._pending_changes):
                     if i < (self._history_offset + len(self._history) + 1):
@@ -216,18 +187,16 @@
         return "State<attributes: %s |methods: %s>" % (
             ", ".join(x for x in self.attributes or {}),
             ", ".join(x for x in self.methods or {}),
         )
 
     @staticmethod
     def calc_diff(obj0, obj1, max_depth=10):
-        try:
-            if obj0 == obj1:
-                return
-        except Exception: pass
+        if obj0 == obj1:
+            return
         if max_depth > 0:
             if type(obj0) == type(obj1) == dict:
                 changes = {}
                 for key in obj0:
                     if key in obj1:
                         changes[key] = State.calc_diff(obj0[key], obj1[key], max_depth - 1)
                     else:
@@ -268,92 +237,76 @@
                 for key, code in diff[1].items():
                     if code == "c":
                         obj1.add(key)
                     if code == "d":
                         obj1.discard(key)
                 return obj1
 
-    def __getstate__(self):
-        return {'channel': self.channel, 'coro_callback': self.coro_callback}
-
-    def __setstate__(self, state):
-        self.channel = state['channel']
-        self.set_callback(state['coro_callback'])
-
 
 class Telekinesis:
     def __init__(
         self,
         target,
         session,
         mask=None,
         expose_tb=True,
         max_delegation_depth=None,
-        block_gc=False,
+        compile_signatures=True,
         parent=None,
     ):
         self._logger = logging.getLogger(__name__)
         self._target = target
         self._session = session
-        self._mask = [mask] if isinstance(mask, str) else mask or []
+        self._mask = mask or []
         self._expose_tb = expose_tb
         self._max_delegation_depth = max_delegation_depth
-        self._block_gc = block_gc
+        self._compile_signatures = compile_signatures
         self._parent = parent
         self._channel = None
         self._clients = {}
-        self._requests = {}
         self._on_update_callback = None
         self._subscription = None
         self._subscribers = set()
         self._state = State()
-        self._last_magic = None
-        self._magic_history = []
 
         if isinstance(target, Route):
             if parent is None:
                 if (target.session, target.channel) not in session.routes:
                     session.routes[(target.session, target.channel)] = {"refcount": 0, "delegations": set(), "state": State()}
                 session.routes[(target.session, target.channel)]["refcount"] += 1
 
         elif not asyncio.iscoroutine(target) and not parent:
             session.targets[id(target)] = (session.targets.get(id(target)) or set()).union(set((self,)))
             self._state.update_from_target(target)
             self._update_state()
 
-    def __getattribute__(self, attr, override=False):
-        if attr[0] == "_" and not override:
+    def __getattribute__(self, attr):
+        if attr[0] == "_":
             return super().__getattribute__(attr)
 
-        if isinstance(self._state.attributes, dict) and isinstance(self._state.attributes.get(attr), Telekinesis) and not self._state.pipeline:
-            state = self._state.attributes[attr]._state.clone()
-            target = self._state.attributes[attr]
-        else: 
-            state = self._state.clone()
-            state.pipeline.append(("get", attr))
-            target = self
+        state = self._state.clone()
+        state.pipeline.append(("get", attr))
 
         return Telekinesis._from_state(
             state,
-            target._target,
-            target._session,
-            target._mask,
-            target._expose_tb,
-            target._max_delegation_depth,
-            target._block_gc,
-            target,
+            self._target,
+            self._session,
+            self._mask,
+            self._expose_tb,
+            self._max_delegation_depth,
+            self._compile_signatures,
+            self,
         )
 
     def _get_root_parent(self):
         if self._parent:
             return self._parent._get_root_parent()
         return self
 
-    @property
-    def _last_value(self):
+    def _last(self):
         if (
             (len(self._state.pipeline) == 1)
             and (self._state.pipeline[0][0] == "get")
             and (isinstance(self._state.attributes, dict))
         ):
             return self._state.attributes[self._state.pipeline[0][1]]
 
@@ -371,37 +324,25 @@
         for attribute_name in self._state.attributes:
             if attribute_name[0] != "_":
                 super().__setattr__(attribute_name, None)
 
         if self._on_update_callback:
             self._on_update_callback(self)
 
-        gets = [g for g in self._state.pipeline if g[0] == 'get']
-        if gets:
-            self.__doc__ = '\n'.join([s or '' for s in self._state.methods.get(gets[-1][1]) or ['', '']])
-        else:
-            self.__doc__ = ((self._state.doc and (self._state.doc + "\n")) or "") + '\n'.join([s or '' for s in self._state.methods.get('__call__') or ['', '']])
-
-
-
         return self
 
     def _delegate(self, receiver, parent_channel=None):
         token_header = []
         extend_route = True
 
         if isinstance(self._target, Route):
             route = self._target.clone()
             max_delegation_depth = None
             if isinstance(receiver, str) and receiver == "*":
-                raise PermissionError("Cannot delegate remote Channel to public.")
-            if not route.tokens:
-                extend_route = False
-            if receiver == self._session.session_key.public_serial(False):
-                extend_route = False
+                raise Exception("Cannot delegate remote Channel to public.")
 
         else:
             if not self._channel:
                 self._channel = Channel(self._session, is_public=isinstance(receiver, str) and receiver == "*")
                 self._channel.telekinesis = self
                 self._channel.listen()
                 token_header += [self._channel.header_buffer.pop()]
@@ -412,15 +353,17 @@
             route = self._channel.route
             if isinstance(receiver, str) and receiver == "*" and not self._channel.is_public:
                 self._channel.is_public = True
                 self._channel.listen()
                 token_header += [self._channel.header_buffer.pop()]
 
         if extend_route:
-            self._session.extend_route(route, receiver[0] if isinstance(receiver, tuple) else receiver, max_delegation_depth)
+            token_header += [
+                self._session.extend_route(route, receiver[0] if isinstance(receiver, tuple) else receiver, max_delegation_depth)
+            ]
             if (route.session, route.channel) in self._session.routes:
                 self._session.routes[(route.session, route.channel)]["delegations"].add(
                     receiver if isinstance(receiver, tuple) else (receiver, None)
                 )
 
         route._parent_channel = parent_channel or self._channel
         [route._parent_channel.header_buffer.append(th) for th in token_header]
@@ -436,15 +379,15 @@
         self._on_update_callback = callback
         self._subscription = Telekinesis(
             subscription_callback,
             self._session,
             None,
             self._expose_tb,
             self._max_delegation_depth,
-            self._block_gc,
+            self._compile_signatures,
         )
         self._state.pipeline.append(("subscribe", self._subscription))
 
         return self
 
     async def _handle_request(self, channel, metadata, payload):
         pipeline = None
@@ -463,121 +406,75 @@
                         if delegation[1] is not None:
                             self._clients.pop((delegation[0], None), None)
                 if not self._clients and not self._channel.is_public:
                     await self._close()
             elif "ping" in payload:
                 await channel.channel.send(metadata.caller, {"pong": True})
             elif "pipeline" in payload:
-                self._requests[metadata.caller] = {'metadata': metadata, 'payload': payload, 'channel': channel}
                 pipeline = self._decode(payload.get("pipeline"), metadata.caller.session[0])
-                self._logger.info("%s %s called %s %s", metadata.caller.session[0][:4], metadata.caller.session[1][:2], self, len(pipeline))
-                # print('...', self._requests.keys())
+                self._logger.info("%s called %s", metadata.caller.session, len(pipeline))
                 if payload.get("reply_to"):
                     reply_to = Route(**payload["reply_to"])
-                    reply_to.validate_token_chain(self._session.session_key.public_serial(False))
-                    metadata.reply_to = reply_to
-                ret = await self._execute(metadata, pipeline, True)
-                await self._respond_request(metadata.caller, ret, False)
-
-        except (Exception, KeyboardInterrupt) as e:
-            if not isinstance(e, StopAsyncIteration):
-                if pipeline is None:
-                    self._logger.error("Telekinesis request error with payload %s", payload, exc_info=True)
-                else:
-                    self._logger.error("Telekinesis request error with pipeline %s", pipeline, exc_info=True)
-
-            self._state.pipeline.clear()
-
-            if self._expose_tb:
-                if callable(self._expose_tb):
-                    err_message = self._expose_tb(e)
-                else:
-                    _, _, exc_traceback = sys.exc_info()
-                    tb = traceback.extract_tb(exc_traceback)
+                    reply_to.validate_token_chain(self._session.session_key.public_serial())
 
-                    adjusted_tb = tb[2:]
-
-                    # Format the modified traceback and include it in the exception message
-                    err_message = str(e) + '\n'
-                    for frame in adjusted_tb:
-                        err_message += f'  File "{frame.filename}" in {frame.name}, line {frame.lineno}\n'
-                        err_message += f'    {frame.line}\n'
-            else:
-                err_message = ''
+                ret = await self._execute(metadata, pipeline, True)
 
-            err_dict = {
-                "error": err_message, 
-                "error_type": type(e).__name__
-            }
-            await self._respond_request(metadata.caller, err_dict, True)
-
-    async def _respond_request(self, caller, return_object, error):
-        # print('here')
-        if caller in self._requests:
-            # print('here 1')
-            metadata = self._requests[caller]['metadata']
-            payload = self._requests[caller]['payload']
-            channel = self._requests[caller]['channel']
-            reply_to = metadata.reply_to
-            self._requests.pop(caller)
-            if not error:
                 if (
-                    isinstance(return_object, Telekinesis)
-                    and isinstance(return_object._target, Route)
-                    and return_object._state.pipeline
-                    and return_object._target.session != (self._session.session_key.public_serial(False), self._session.instance_id)
-                    and self.__on_same_network(return_object._session)
+                    isinstance(ret, Telekinesis)
+                    and isinstance(ret._target, Route)
+                    and ret._state.pipeline
+                    and (
+                        ret._target.session != self._session.session_key.public_serial()
+                        or ret._target._channel not in self._session.channels
+                    )
                 ):
-                    await return_object._forward(
-                        return_object._state.pipeline,
+                    await ret._forward(
+                        ret._state.pipeline,
                         reply_to or metadata.caller,
-                        self._session if return_object._session.session_key.public_serial(False) != self._session.session_key.public_serial(False) else None,
                         root_parent=payload.get("root_parent") if reply_to else (self, metadata.caller.session),
                     )
                 else:
-                    try:
-                        if reply_to:
-                            async with Channel(self._session) as new_channel:
-                                await new_channel.send(
-                                    reply_to,
-                                    {
-                                        "return": self._encode(return_object, reply_to.session, new_channel),
-                                        "root_parent": payload.get("root_parent"),
-                                    },
-                                )
-                        else:
-                            await channel.send(
-                                metadata.caller,
+                    if reply_to:
+                        async with Channel(self._session) as new_channel:
+                            await new_channel.send(
+                                reply_to,
                                 {
-                                    "return": self._encode(return_object, metadata.caller.session),
-                                    "root_parent": None if return_object is self else self._encode(self, metadata.caller.session, channel),
+                                    "return": self._encode(ret, reply_to.session, new_channel),
+                                    "root_parent": payload.get("root_parent"),
                                 },
                             )
-                    except ConnectionError:
-                        pass
-            else:
-                try:
-                    if reply_to:
-                        async with Channel(self._session) as new_channel:
-                            await new_channel.send(reply_to, return_object)
                     else:
-                        await channel.send(metadata.caller, return_object)
-                except Exception as e:
-                    print(e)
-                finally:
-                    pass
+                        await channel.send(
+                            metadata.caller,
+                            {
+                                "return": self._encode(ret, metadata.caller.session),
+                                "root_parent": None if ret is self else self._encode(self, metadata.caller.session, channel),
+                            },
+                        )
+
+        except Exception:
+            if pipeline is None:
+                self._logger.error("Telekinesis request error with payload %s", payload, exc_info=True)
+            else:
+                self._logger.error("Telekinesis request error with pipeline %s", pipeline, exc_info=True)
+
+            self._state.pipeline.clear()
+            try:
+                err_message = {"error": traceback.format_exc() if self._expose_tb else ""}
+                if reply_to:
+                    async with Channel(self._session) as new_channel:
+                        await new_channel.send(reply_to, err_message)
+                else:
+                    await channel.send(metadata.caller, err_message)
+            finally:
+                pass
 
     async def _execute(self, metadata=None, pipeline=None, break_on_telekinesis=False):
         if asyncio.iscoroutine(self._target):
-            target = await self._target
-            x = self
-            while x:
-                x._target = target
-                x = x._parent
-
+            self._target = await self._target
             if isinstance(self._target, Route):
                 if (self._target.session, self._target.channel) not in self._session.routes:
                     self._session.routes[(self._target.session, self._target.channel)] = {
                         "refcount": 0,
                         "delegations": set(),
                         "state": State(),
                     }
@@ -589,152 +486,98 @@
 
         if not pipeline:
             pipeline = []
 
         pipeline = self._state.pipeline + pipeline
         self._state.pipeline.clear()
 
-        if not metadata:
-            metadata = RequestMetadata(self._session, None, None)
-
         if isinstance(self._target, Route):
-            try:
-                return await self._forward(pipeline)
-            except Exception:
-                exc_type, exc_value, exc_traceback = sys.exc_info()
-                tb = traceback.extract_tb(exc_traceback)
-
-                adjusted_tb = tb[2:]
-
-                new_message = str(exc_value) + '\n'
-                for _ in adjusted_tb:
-                    new_message += f'  Remote exception on Telekinesis object "\u2248\033 {self._state.repr}", {self._session}, {str(self._target)}\n'
-
-                # Raise a new exception with the error message forwarded from the remote telekinesis object
-                raise exc_type(new_message) from None
+            return await self._forward(pipeline)
 
         async def exc(x):
             if isinstance(x, Telekinesis) and x._state.pipeline:
                 return await x._execute(metadata)
             return x
 
         target = self._target
 
         touched = self._session.targets.get(id(target))
-        break_var = False
         for i, (action, arg) in enumerate(pipeline):
-            check_pipeline = False
             if (
                 break_on_telekinesis
                 and isinstance(target, Telekinesis)
                 and isinstance(target._target, Route)
                 and (
-                    target._target.session != (self._session.session_key.public_serial(False), self._session.instance_id)
+                    target._target.session != self._session.session_key.public_serial()
                     or target._target.channel not in self._session.channels
                 )
             ):
                 new_state = target._state.clone()
                 target = Telekinesis(
                     target._target,
                     target._session,
                     target._mask,
                     target._expose_tb,
                     target._max_delegation_depth,
-                    target._block_gc,
+                    target._compile_signatures,
                     target._parent,
                 )
                 target._state = new_state
                 target._state.pipeline += pipeline[i:]
-                if not self.__on_same_network(target._session):
-                    target = await target
                 break
 
             if action == "get":
                 self._logger.info("%s %s %s", action, arg, target)
                 if (
-                    (arg[0] == "_" and arg not in ["__getitem__", "__setitem__", "__aiter__", "__anext__", "__add__", "__mul__"])
+                    (arg[0] == "_" and arg not in ["__getitem__", "__setitem__", "__add__", "__mul__"])
                     or arg in (self._mask or [])
+                    or (type(target) == dict)
                 ):
-                    raise PermissionError("Private attributes and methods (those starting with _) cannot be accessed remotely")
-                elif type(target) in (dict, list, set) and arg not in (
-                    'get', 'index', 'count', '__getitem__', 'copy', 'difference', 'intersection', 'isdisjoint', 'issubset', 'issuperset', 
-                    'symmetric_difference', 'union' 
-                ):
-                    raise PermissionError("dicts, lists and sets cannot be modified remotely")
+                    raise Exception("Unauthorized!")
                 if isinstance(target, type):
-                    try:
-                        target = target.__getattribute__(target, arg)
-                    except AttributeError as ae:
-                        try:
-                            target = target.__getattr__(target, arg)
-                        except AttributeError:
-                            raise ae
+                    target = target.__getattribute__(target, arg)
                 else:
-                    try:
-                        target = target.__getattribute__(arg)
-                    except AttributeError as ae:
-                        try:
-                            target = target.__getattr__(arg)
-                        except AttributeError:
-                            raise ae
-                if asyncio.iscoroutine(target):
-                    target = await target
-                
+                    target = target.__getattribute__(arg)
             if action == "call":
                 self._logger.info("%s %s", action, target)
                 ar, kw = arg
-                if "_tk_block_arg_evaluation" in dir(target) and target._tk_block_arg_evaluation:
-                    args, kwargs = [ar, kw]
-                else:
-                    args, kwargs = [await exc(x) for x in ar], {x: await exc(kw[x]) for x in kw}
+                args, kwargs = [await exc(x) for x in ar], {x: await exc(kw[x]) for x in kw}
 
-                if (
-                    "_tk_inject_first_arg" in dir(target) and target._tk_inject_first_arg or
-                    isinstance(target, type) and "_tk_inject_first_arg" in dir(target.__init__) and target.__init__._tk_inject_first_arg
-                ):
-                    metadata.pipeline = pipeline[i+1:]
-                    check_pipeline = True
+                if "_tk_inject_first_arg" in dir(target) and target._tk_inject_first_arg:
                     target = target(metadata, *args, **kwargs)
                 else:
                     target = target(*args, **kwargs)
                 if asyncio.iscoroutine(target):
                     target = await target
-
-                if check_pipeline and not metadata.pipeline:
-                    break_var = True
+                if (
+                    isinstance(target, Telekinesis)
+                    and isinstance(target._target, Route)
+                    and target._state.pipeline
+                    and not break_on_telekinesis
+                ):
+                    target = await target._execute()
             if action == "subscribe":
                 if arg._target.validate_token_chain(metadata.caller.session[0]):
                     tk = Telekinesis._reuse(
                         target,
                         self._session,
                         self._mask,
                         self._expose_tb,
                         self._max_delegation_depth,
-                        self._block_gc,
+                        self._compile_signatures,
                         None,
                     )
                     if arg._target.session not in tk._clients:
                         tk._clients[arg._target.session] = {"last_state": 0, "cache_attributes": True}
                         tk._clients.pop((arg._target.session[0], None), None)
                     if tk._clients[arg._target.session]["cache_attributes"] != True:
                         tk._clients[arg._target.session]["last_state"] = 0
                     tk._clients[arg._target.session]["cache_attributes"] = True
                     tk._subscribers.add(arg)
-            if (
-                isinstance(target, Telekinesis)
-                and not (
-                    break_on_telekinesis
-                    and isinstance(target._target, Route) 
-                    # and target._state.pipeline
-                    )
-                ):
-                target = await target._execute()
             touched = touched.union((self._session.targets.get(id(target))) or set())
-            if break_var:
-                break
 
         for tk in touched:
             tk._state.update_from_target(tk._target)
             tk._update_state()
             if tk and tk._subscribers:
                 for s in tk._subscribers:
                     asyncio.create_task(s(tk)._execute())
@@ -756,128 +599,79 @@
 
             if response.get("root_parent"):
                 root = self._get_root_parent()
                 diffs = root._decode(response["root_parent"], metadata.caller.session[0])._state.get_diffs(0, None, True)
                 root._update_state(diffs)
 
             if "error" in response:
-                if response.get("error_type") == "PermissionError":
-                    raise PermissionError(response["error"])
-                if response.get("error_type") == "StopAsyncIteration":
-                    raise StopAsyncIteration(response["error"])
-                else:
-                    raise Exception(response["error"])
+                raise Exception(response["error"])
 
             if "return" in response:
                 ret = self._decode(response["return"], metadata.caller.session[0])
                 return ret
 
     async def _close(self):
         try:
             if isinstance(self._target, Route):
                 self._session.routes[(self._target.session, self._target.channel)]["refcount"] -= 1
                 if self._session.routes[(self._target.session, self._target.channel)]["refcount"] <= 0:
                     o = self._session.routes.pop((self._target.session, self._target.channel))
                     async with Channel(self._session) as new_channel:
                         await new_channel.send(self._target, {"close": list(o["delegations"])})
             else:
-                # print('closing', id(self._target), self._session.targets.get(id(self._target)))
-                if id(self._target) in self._session.targets:
-                    self._session.targets[id(self._target)].discard(self)
-                    if not self._session.targets[id(self._target)]:
-                        self._session.targets.pop(id(self._target))
-                    self._channel and await self._channel.close()
-        except ConnectionError:
-            self._session.logger.info("Error closing Telekinesis Object: %s", self._target, exc_info=True)
+                self._session.targets[id(self._target)].remove(self)
+                if not self._session.targets[id(self._target)]:
+                    self._session.targets.pop(id(self._target))
+                self._channel and await self._channel.close()
         except Exception:
-            self._session.logger.error("Error closing Telekinesis Object: %s", self._target, exc_info=True)
+            self._session.logger("Error closing Telekinesis Object: %s", self._target, exc_info=True)
 
-    async def _forward(self, pipeline, reply_to=None, session=None, **kwargs):
+    async def _forward(self, pipeline, reply_to=None, **kwargs):
         async with Channel(self._session) as new_channel:
             if reply_to:
-                if session:
-                    session.extend_route(reply_to, self._session.session_key.public_serial(False))
-                self._session.extend_route(reply_to, self._target.session[0])
+                token_header = self._session.extend_route(reply_to, self._target.session[0])
+                new_channel.header_buffer.append(token_header)
             for key, value in kwargs.items():
                 if isinstance(value, tuple) and isinstance(value[0], Telekinesis):
                     kwargs[key] = value[0]._encode(value[0], value[1], new_channel)
             return await self._send_request(
                 new_channel,
                 reply_to=reply_to and reply_to.to_dict(),
                 pipeline=self._encode(pipeline, self._target.session, new_channel),
                 **kwargs,
             )
 
-    def _register_magic(self, ipython, name=None):
-        self_name =[ k for k,v in ipython.ns_table['user_global'].items() 
-            if v is self and k != '_'][0]
-        
-        name = name or self_name
-
-        def inject_code(line, cell):
-            args, kwargs = [], {}
-            method, *rest = line.split('(')
-            eval(
-                "(lambda *a, **kw: _tkj_args.extend(a) or _tkj_kwargs.update(kw))"+'('.join(['', *rest]),
-                {**ipython.ns_table['user_global'], '_tkj_args': args, '_tkj_kwargs': kwargs}
-            )
-            f = eval(self_name+method.strip(), ipython.ns_table['user_global'])
-            t = asyncio.create_task(f(cell, *args, **kwargs)._execute())
-            
-            self._last_magic = t
-            self._magic_history.append(t)
-        
-        ipython.register_magic_function(inject_code, 'cell', name)
-
     def __call__(self, *args, **kwargs):
         state = self._state.clone()
         state.pipeline.append(("call", (args, kwargs)))
 
         return Telekinesis._from_state(
             state,
             self._target,
             self._session,
             self._mask,
             self._expose_tb,
             self._max_delegation_depth,
-            self._block_gc,
+            self._compile_signatures,
             self,
         )
 
     def __setattr__(self, attribute, value):
         if attribute[0] != "_":
-            raise PermissionError("Attributes for Telekinesis objects cannot be set directly")
+            raise Exception("Attributes for Telekinesis objects cannot be set directy")
         super().__setattr__(attribute, value)
 
-    def __getitem__(self, key):
-        return self.__getattribute__('__getitem__', True)(key)
-
-    def __setitem__(self, key, val):
-        return asyncio.create_task(self.__getattribute__('__setitem__', True)(key, val)._execute())
- 
-    def __aiter__(self):
-        return self.__getattribute__('__aiter__', True)()
-
-    def __anext__(self):
-        return self.__getattribute__('__anext__', True)()
-
-    def __add__(self, val):
-        return self.__getattribute__('__add__', True)(val)
-
-    def __mul__(self, val):
-        return self.__getattribute__('__mul__', True)(val)
-
     def __await__(self):
         return self._execute().__await__()
 
     def __repr__(self):
         return "\033[92m\u2248\033[0m " + str(self._state.repr)
 
     def __del__(self):
-        if self._parent is None and not self._block_gc:
+        if self._parent is None:
             self._session.pending_tasks.add(asyncio.get_event_loop().create_task(self._close()))
 
     def _encode(self, target, receiver=None, channel=None, traversal_stack=None, block_recursion=False):
         if traversal_stack is None:
             i = 0
             traversal_stack = {}
         else:
@@ -885,72 +679,63 @@
                 return str(traversal_stack[id(target)][0])
             i = len(traversal_stack)
 
         traversal_stack[id(target)] = [i, None, target]
         # ..  keep a copy of the target so it doesn't get garbage collected - which messes up the id()
 
         if receiver is None:
-            receiver = (self._session.session_key.public_serial(False), self._session.instance_id)
+            receiver = (self._session.session_key.public_serial(), self._session.instance_id)
 
-
-        if type(target) in (str, bytes, bool, type(None)):
+        if type(target) in (int, float, str, bytes, bool, type(None)):
             tup = (type(target).__name__, target)
-        elif isinstance(target, float):
-            tup = ('float', target)
-        elif isinstance(target, int) or re.match(r'<class \'numpy\.[\w]*int', str(type(target))):
-            tup = ('int', int(target))
         elif type(target) in (range, slice):
             tup = (type(target).__name__, (target.start, target.stop, target.step))
-        elif type(target) in (list, dict) and is_bson_encodable(target):
-            tup = ('raw_'+type(target).__name__, target)
         elif type(target) in (list, tuple, set):
             tup = (
                 type(target).__name__,
                 [self._encode(v, receiver, channel, traversal_stack, block_recursion) for v in target],
             )
         elif type(target) == dict:
             tup = (
                 "dict",
-                [(
-                    self._encode(x, receiver, channel, traversal_stack, block_recursion),
-                    self._encode(target[x], receiver, channel, traversal_stack, block_recursion) 
-                ) for x in target],
+                {x: self._encode(target[x], receiver, channel, traversal_stack, block_recursion) for x in target},
             )
         elif isinstance(target, Route):
             tup = ("route", target.to_dict())
         else:
-            if isinstance(target, Telekinesis) and (not isinstance(target._target, Route) or self.__on_same_network(target._session)):
+            if isinstance(target, Telekinesis):
                 obj = target
             else:
                 obj = Telekinesis._reuse(
                     target,
                     self._session,
                     self._mask,
                     self._expose_tb,
                     self._max_delegation_depth,
-                    self._block_gc,
+                    self._compile_signatures,
                 )
             if not isinstance(obj._target, Route):
                 if receiver not in obj._clients:
                     obj._clients[receiver] = {"last_state": 0, "cache_attributes": None}
                     if receiver[1] is not None:
                         obj._clients.pop((receiver[0], None), None)
 
             route = obj._delegate(receiver[0], channel or self._channel)
-            diffs = obj._state.get_diffs(
-                obj._clients[receiver]["last_state"] if receiver in obj._clients else 0,
-                self._mask,
-                obj._clients.get(receiver) and obj._clients[receiver]["cache_attributes"] and not block_recursion,
-            ) if receiver != route.session else [0, {"pipeline": obj._state.pipeline}]
             tup = (
                 "obj",
                 (
                     route.to_dict(),
                     self._encode(
-                        diffs,
+                        obj._state.get_diffs(
+                            obj._clients[receiver]["last_state"] if receiver in obj._clients else 0,
+                            self._mask,
+                            obj._clients.get(receiver) and obj._clients[receiver]["cache_attributes"] and not block_recursion,
+                        )
+                        if receiver != route.session
+                        else [0, {"pipeline": obj._state.pipeline}],
                         receiver,
                         channel,
                         traversal_stack,
                         block_recursion=True,
                     ),
                 ),
             )
@@ -968,15 +753,15 @@
         if root is None:
             root = "0"
             output_stack = {}
         if root in output_stack:
             return output_stack[root]
 
         typ, obj = input_stack[root]
-        if typ in ("int", "float", "str", "bytes", "bool", "NoneType", "raw_list", "raw_dict"):
+        if typ in ("int", "float", "str", "bytes", "bool", "NoneType"):
             out = obj
         elif typ in ("range", "slice"):
             out = {"range": range, "slice": slice}[typ](*obj)
         elif typ == "list":
             out = [None] * len(obj)
             output_stack[root] = out
             for k, v in enumerate(obj):
@@ -987,47 +772,45 @@
             for v in obj:
                 out.add(self._decode(input_stack, caller_id, v, output_stack))
         elif typ == "tuple":
             out = tuple(self._decode(input_stack, caller_id, v, output_stack) for v in obj)
         elif typ == "dict":
             out = {}
             output_stack[root] = out
-            for k, v in obj:
-                out[self._decode(input_stack, caller_id, k, output_stack)] = self._decode(input_stack, caller_id, v, output_stack)
+            for k, v in obj.items():
+                out[k] = self._decode(input_stack, caller_id, v, output_stack)
         elif typ == "route":
             out = Route(**obj)
         else:
             route = Route(**obj[0])
             state_diff = self._decode(input_stack, caller_id, obj[1], output_stack)
 
-            if route.session == (self._session.session_key.public_serial(False), self._session.instance_id) and route.channel in self._session.channels:
+            if route.session == (self._session.session_key.public_serial(), self._session.instance_id) and route.channel in self._session.channels:
                 channel = self._session.channels.get(route.channel)
                 if channel.validate_token_chain(caller_id, route.tokens):
 
                     if state_diff[1].get('pipeline'):
-                        
                         return Telekinesis._from_state(
                             channel.telekinesis._state.clone().update_from_diffs(*state_diff),
                             channel.telekinesis._target,
                             self._session,
                             self._mask,
                             self._expose_tb,
                             self._max_delegation_depth,
-                            self._block_gc,
+                            self._compile_signatures,
                             channel.telekinesis,
                         )
                     out = channel.telekinesis._target
                 else:
-                    raise PermissionError(f"Unauthorized! {caller_id} {route} {route.tokens}")
-            # elif self._parent and (
-            #     ("__call__" not in self._state.methods)
-            #     or ("methods" not in state_diff[1])
-            #     or ("__call__" not in state_diff[1]["methods"])
-            # ):
-            elif self._parent and root == '0':
+                    raise Exception(f"Unauthorized! {caller_id} {route.tokens}")
+            elif self._parent and (
+                ("__call__" not in self._state.methods)
+                or ("methods" not in state_diff[1])
+                or ("__call__" not in state_diff[1]["methods"])
+            ):
                 self._target = route
                 self._parent = None
                 if (self._target.session, self._target.channel) not in self._session.routes:
                     self._session.routes[(self._target.session, self._target.channel)] = {
                         "refcount": 0,
                         "delegations": set(),
                         "state": State(),
@@ -1059,88 +842,149 @@
                 out = Telekinesis._from_state(
                     self._session.routes[(route.session, route.channel)]["state"].clone(),
                     route,
                     self._session,
                     self._mask,
                     self._expose_tb,
                     self._max_delegation_depth,
-                    self._block_gc,
+                    self._compile_signatures,
                 )
 
         output_stack[root] = out
         return out
 
-    def __on_same_network(self, session):
-        for c in self._session.connections:
-            for cc in session.connections:
-                if set([c.broker_id, *c.broker_peers]).intersection([cc.broker_id, *cc.broker_peers]):
-                    return True
-        return False
-
     @property
     def __signature__(self):
         gets = [g for g in self._state.pipeline if g[0] == 'get']
         if gets:
             return (self._state.methods.get(gets[-1][1]) or [None])[0]
         return (self._state.methods.get('__call__') or [None])[0]
 
-    # @property
-    # def __doc__(self):
-    #     gets = [g for g in self._state.pipeline if g[0] == 'get']
-    #     if gets:
-    #         return '\n'.join([s or '' for s in self._state.methods.get(gets[-1][1]) or ['', '']])
-    #     return ((self._state.doc and self._state.doc + "\n") or "") + '\n'.join([s or '' for s in self._state.methods.get('__call__') or ['', '']])
+    @property
+    def __doc__(self):
+        gets = [g for g in self._state.pipeline if g[0] == 'get']
+        if gets:
+            return (self._state.methods.get(gets[-1][1]) or [None, None])[1]
+        return ((self._state.doc and self._state.doc + "\n") or "") + ((self._state.methods.get('__call__') or [None, None])[1] or "") or None
 
     @staticmethod
     def _from_state(
         state,
         target,
         session,
         mask=None,
         expose_tb=True,
         max_delegation_depth=None,
-        block_gc=True,
+        compile_signatures=True,
         parent=None,
     ):
-        out = Telekinesis(target, session, mask, expose_tb, max_delegation_depth, block_gc, parent)
+        def signatured_subclass(signature, method_name, docstring):
+            class Telekinesis_(Telekinesis):
+                @makefun.with_signature(
+                    signature,
+                    func_name=method_name,
+                    doc=docstring if method_name == "__call__" else None,
+                    module_name="telekinesis.telekinesis",
+                )
+                def __call__(self, *args, **kwargs):
+                    return Telekinesis.__call__(self, *args, **kwargs)
+
+            return Telekinesis_
+
+        method_name = state.pipeline[-1][1] if state.pipeline and state.pipeline[-1][0] == "get" else "__call__"
+
+        reset = "call" in [x[0] for x in state.pipeline[:-1]]
+        if method_name in state.methods or reset:
+            signature, docstring = (not reset and state.methods.get(method_name)) or (None, None)
+            signature = signature or "(*args, **kwargs)"
+            signature = signature.replace("(", "(self, ")
+
+            stderr = sys.stderr
+            sys.stderr = io.StringIO()
+
+            try:
+                if compile_signatures and check_signature(signature):
+                    Telekinesis_ = signatured_subclass(signature, method_name, docstring)
+                else:
+                    Telekinesis_ = signatured_subclass("(self, *args, **kwargs)", method_name, docstring)
+            except Exception:
+                Telekinesis_ = signatured_subclass("(self, *args, **kwargs)", method_name, docstring)
+
+            sys.stderr = stderr
+
+        else:
+            Telekinesis_ = Telekinesis
+            docstring = None
+
+        if method_name == "__call__":
+
+            def dundermethod(self, method, key):
+                state = self._state.clone()
+                state.pipeline.append(("get", method))
+                state.pipeline.append(("call", ((key,), {})))
+                return Telekinesis._from_state(
+                    state,
+                    self._target,
+                    self._session,
+                    self._mask,
+                    self._expose_tb,
+                    self._max_delegation_depth,
+                    self._compile_signatures,
+                    self,
+                )
+
+            def setitem(self, key, value):
+                state = self._state
+                state.pipeline.append(("get", "__setitem__"))
+                state.pipeline.append(("call", ((key, value), {})))
+                return Telekinesis._from_state(
+                    state,
+                    self._target,
+                    self._session,
+                    self._mask,
+                    self._expose_tb,
+                    self._max_delegation_depth,
+                    self._compile_signatures,
+                    self,
+                )
+
+            if "__getitem__" in state.methods:
+                Telekinesis_.__getitem__ = partialmethod(dundermethod, "__getitem__")
+            if "__add__" in state.methods:
+                Telekinesis_.__add__ = partialmethod(dundermethod, "__add__")
+            if "__mul__" in state.methods:
+                Telekinesis_.__mul__ = partialmethod(dundermethod, "__mul__")
+            if "__setitem__" in state.methods:
+                Telekinesis_.__setitem__ = setitem
+
+        out = Telekinesis_(target, session, mask, expose_tb, max_delegation_depth, compile_signatures, parent)
         out._state = state
         out._update_state()
+        # out.__doc__ = state.doc if method_name == "__call__" else docstring
 
         return out
 
     @staticmethod
     def _reuse(
         target,
         session,
         mask=None,
         expose_tb=True,
         max_delegation_depth=None,
-        block_gc=True,
+        compile_signatures=True,
         parent=None,
     ):
         kwargs = locals()
 
         for tk in session.targets.get(id(target)) or []:
             if all((kwargs[x] == tk.__getattribute__("_" + x) for x in kwargs)):
                 return tk
         return Telekinesis(**kwargs)
 
 
-def inject_first_arg(func):
-    func._tk_inject_first_arg = True
-    return func
+def check_signature(signature):
+    return not ("\n" in signature or (signature != re.sub(r"(?:[^A-Za-z0-9_])lambda(?=[\)\s\:])", "", signature)))
 
 
-def block_arg_evaluation(func):
-    func._tk_block_arg_evaluation = True
+def inject_first_arg(func):
+    func._tk_inject_first_arg = True
     return func
-
-def is_bson_encodable(target, depth=0):
-    if depth > 300:
-        return False
-    elif type(target) in (str, bytes, bool, type(None), float, int):
-        return True
-    elif type(target) == list:
-        return all(is_bson_encodable(x, depth+1) for x in target)
-    elif type(target) == dict:
-        return all(isinstance(k, str) and is_bson_encodable(x, depth+1) for k, x in target.items())
-    return False
```

### Comparing `telekinesis-0.1.81/telekinesis.egg-info/PKG-INFO` & `telekinesis-0.1.9/telekinesis.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: telekinesis
-Version: 0.1.81
+Version: 0.1.9
 Summary: Open Source, End-to-End Encrypted, Anywhere-to-Anywhere, Remote Procedure Calls.
 Home-page: https://github.com/telekinesis-cloud/telekinesis
 Author: Telekinesis, Inc.
 Author-email: support@telekinesis.cloud
+License: UNKNOWN
+Description: # Telekinesis - Python Package
+        
+        See [telekinesis github repo](https://github.com/e-neuman/telekinesis)
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Telekinesis - Python Package
-
-See [telekinesis github repo](https://github.com/e-neuman/telekinesis)
```

### Comparing `telekinesis-0.1.81/test/test_00_walkthrough.py` & `telekinesis-0.1.9/test/test_00_walkthrough.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from telekinesis import Broker, Telekinesis, Connection, Session, Channel, PrivateKey
+from telekinesis import Broker, Telekinesis, Connection, Session, Channel
 import random
 import asyncio
 import pytest
 import os
 
 pytestmark = pytest.mark.asyncio
 random.seed(42)
@@ -12,22 +12,22 @@
 def event_loop():  # This avoids 'Task was destroyed but it is pending!' message
     yield asyncio.get_event_loop()
 
 
 async def test_walkthrough():
     class FaultyBroker(Broker):  # Telekinesis should survive broker errors
         async def handle_send(self, *args, **kwargs):
-            if random.random() < 0.01:
+            if random.random() < 0.005:
                 self.logger.error("Gotcha!!!")
                 kwargs["message"] = Exception("Random Fault Injection")
             await super().handle_send(*args, **kwargs)
 
     broker_0 = await FaultyBroker().serve(port=8777)
 
-    conn_0 = await Connection(Session(PrivateKey(name='demo')), "ws://localhost:8777")
+    conn_0 = await Connection(Session(), "ws://localhost:8777")
     conn_0.RESEND_TIMEOUT = 1
 
     broker_0.entrypoint = await Telekinesis(lambda x: (lambda y: x + y), conn_0.session)._delegate("*")
 
     broker_1 = await FaultyBroker().serve(port=8778)  # Telekinesis works with clusters of Brokers
     await broker_1.add_broker("ws://localhost:8777", True)
 
@@ -79,25 +79,23 @@
         conn_1.session.session_key.public_serial()
     )  # << Max delegation depth!
 
     counter = await Telekinesis(route_counter, conn_1.session)()._timeout(4)
 
     assert await counter.increment().increment().value._timeout(4) == 2
 
-    assert 'to_be_masked' not in counter._state.methods
-
-    with pytest.raises(PermissionError):
+    with pytest.raises(Exception, match=r".*Unauthorized.*"):
         await counter.to_be_masked()
 
-    with pytest.raises(PermissionError):
+    with pytest.raises(Exception, match=r".*Unauthorized.*"):
         c = counter.increment()
         c._state.pipeline[0] = ("get", "to_be_masked")
         await c
 
-    with pytest.raises(PermissionError):
+    with pytest.raises(Exception, match=r".*Unauthorized.*"):
         c = counter.increment()
         c._state.pipeline[0] = ("get", "_private")
         await c
 
     # Try to delegate
     counter_delegator_route = await Telekinesis(lambda: counter, conn_1.session)._delegate(
         conn_2.session.session_key.public_serial()
```

### Comparing `telekinesis-0.1.81/test/test_01_encode_decode.py` & `telekinesis-0.1.9/test/test_01_subscribe.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 from telekinesis import Broker, Telekinesis, Connection, Session, Entrypoint
 import asyncio
 import pytest
+import os
+
 from telekinesis.helpers import create_entrypoint
 
 pytestmark = pytest.mark.asyncio
 
 
 @pytest.fixture
 def event_loop():  # This avoids 'Task was destroyed but it is pending!' message
     yield asyncio.get_event_loop()
 
 
-async def test_encode_decode():
-
-    bro = await Broker().serve(port=8784)
+async def test_subscribe():
+    bro = await Broker().serve(port=8780)
 
     class Registry(dict):
         pass
 
-    bro.entrypoint, _ = await create_entrypoint(Registry(), "ws://localhost:8784")
+    bro.entrypoint, _ = await create_entrypoint(Registry(), "ws://localhost:8780")
+
+    class Counter:
+        def __init__(self, initial_value=0):
+            self.value = initial_value
+
+        def increment(self, amount=1):
+            self.value += amount
+            return self
 
+    registry = await Entrypoint("ws://localhost:8780")
+    await registry.update({"counter": Counter(2)})
 
-    registry = await Entrypoint("ws://localhost:8784")
-    await registry.update({"echo_type": lambda x: type(x).__name__})
-    echo_type = await Entrypoint("ws://localhost:8784").get("echo_type")
+    counter0 = await Entrypoint("ws://localhost:8780").get("counter")
+    counter1 = await Entrypoint("ws://localhost:8780").get("counter")._subscribe()
 
-    assert await echo_type(1) == 'int'
-    assert await echo_type(1.0) == 'float'
-    assert await echo_type('one') == 'str'
+    assert counter1.value._last() == 2
 
-    await registry.update({"echo_key_type": lambda obj: type(list(obj.keys())[0]).__name__})
-    echo_key_type = await Entrypoint("ws://localhost:8784").get("echo_key_type")
+    await counter0.increment(3).increment(1)
 
-    assert await echo_key_type({(1, 2): '123'}) == 'tuple'
+    await asyncio.sleep(0.1)
+    assert counter1.value._last() == 6
```

### Comparing `telekinesis-0.1.81/test/test_02_garbage_collection.py` & `telekinesis-0.1.9/test/test_02_garbage_collection.py`

 * *Files identical despite different names*

### Comparing `telekinesis-0.1.81/test/test_03_subscribe.py` & `telekinesis-0.1.9/test/test_03_request_forwarding.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 from telekinesis import Broker, Telekinesis, Connection, Session, Entrypoint
 import asyncio
 import pytest
-import os
-
 from telekinesis.helpers import create_entrypoint
 
 pytestmark = pytest.mark.asyncio
 
 
 @pytest.fixture
 def event_loop():  # This avoids 'Task was destroyed but it is pending!' message
     yield asyncio.get_event_loop()
 
 
-async def test_subscribe():
-    bro = await Broker().serve(port=8780)
-
-    class Registry(dict):
-        pass
+async def test_forwarding():
+    count = {"count": 0}
 
-    bro.entrypoint, _ = await create_entrypoint(Registry(), "ws://localhost:8780")
+    class CountedBroker(Broker):
+        async def handle_send(self, *args, **kwargs):
+            count["count"] += 1
+            return await super().handle_send(*args, **kwargs)
 
-    class Counter:
-        def __init__(self, initial_value=0):
-            self.value = initial_value
+    bro = await CountedBroker().serve(port=8782)
 
-        def increment(self, amount=1):
-            self.value += amount
-            return self
-
-    registry = await Entrypoint("ws://localhost:8780")
-    await registry.update({"counter": Counter(2)})
+    class Registry(dict):
+        pass
 
-    counter0 = await Entrypoint("ws://localhost:8780").get("counter")
-    counter1 = await Entrypoint("ws://localhost:8780").get("counter")._subscribe()
+    bro.entrypoint, _ = await create_entrypoint(Registry(), "ws://localhost:8782")
 
-    assert counter1.value._last_value == 2
+    echo = lambda x: x
 
-    await counter0.increment(3).increment(1)
+    registry = await Entrypoint("ws://localhost:8782")
+    await registry.update({"echo": echo})
 
-    await asyncio.sleep(0.1)
-    assert counter1.value._last_value == 6
+    count["count"] = 0
+    assert await Entrypoint("ws://localhost:8782").get("echo")("hello") == "hello"
+    assert count["count"] == 2 * 3
```

### Comparing `telekinesis-0.1.81/test/test_06_state_diffing.py` & `telekinesis-0.1.9/test/test_04_state_diffing.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,33 +23,25 @@
             return await super().handle_send(connection, message, source, destination)
 
     bro = await MeasuredBroker().serve(port=8783)
 
     class Container:
         def set(self, attr, val):
             self.__setattr__(attr, val)
-        def add_method(self, doc):
-            self.method = lambda x: x
-            self.method.__doc__ = doc
 
     bro.entrypoint, container = await create_entrypoint(Container(), "ws://localhost:8783")
 
     registry = await Entrypoint("ws://localhost:8783")._subscribe()
 
     assert measures["size_kb"] < 2 ** 10
 
     await container.set("x", os.urandom(2 ** 20))
 
     await registry
     assert 2 ** 10 < measures["size_kb"] < 1.1 * 2 ** 10
-    assert registry.x._last_value == container.x._last_value
+    assert registry.x._last() == container.x._last()
 
     await container.set("y", os.urandom(2 ** 20))
 
     await registry
     assert 2 ** 11 < measures["size_kb"] < 1.1 * 2 ** 11
-    assert registry.y._last_value == container.y._last_value
-
-    await container.add_method("some docstring")
-    
-    await registry
-    assert registry._state.methods.get('method')[1] == "some docstring"
+    assert registry.y._last() == container.y._last()
```

