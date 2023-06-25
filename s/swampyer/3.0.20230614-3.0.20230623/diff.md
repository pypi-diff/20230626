# Comparing `tmp/swampyer-3.0.20230614.tar.gz` & `tmp/swampyer-3.0.20230623.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swampyer-3.0.20230614.tar", max compression
+gzip compressed data, was "swampyer-3.0.20230623.tar", max compression
```

## Comparing `swampyer-3.0.20230614.tar` & `swampyer-3.0.20230623.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      689 2023-06-14 18:01:18.094832 swampyer-3.0.20230614/pyproject.toml
--rw-r--r--   0        0        0      168 2022-08-16 23:40:19.004711 swampyer-3.0.20230614/swampyer/__init__.py
--rw-r--r--   0        0        0    39009 2023-01-27 23:39:43.540898 swampyer-3.0.20230614/swampyer/client.py
--rw-r--r--   0        0        0     1098 2022-09-26 22:26:31.459187 swampyer-3.0.20230614/swampyer/common.py
--rw-r--r--   0        0        0      658 2022-08-16 23:40:19.004711 swampyer-3.0.20230614/swampyer/exceptions.py
--rw-r--r--   0        0        0     1014 2022-09-09 18:53:53.522720 swampyer-3.0.20230614/swampyer/fields.py
--rw-r--r--   0        0        0     7101 2022-11-23 22:28:58.618298 swampyer-3.0.20230614/swampyer/messages.py
--rw-r--r--   0        0        0    11295 2022-08-16 23:40:19.004711 swampyer-3.0.20230614/swampyer/queues.py
--rw-r--r--   0        0        0     4696 2023-06-14 18:00:00.758370 swampyer-3.0.20230614/swampyer/serializers.py
--rw-r--r--   0        0        0    17194 2022-11-22 20:12:28.152904 swampyer-3.0.20230614/swampyer/transport.py
--rw-r--r--   0        0        0       57 2022-08-16 23:40:19.004711 swampyer-3.0.20230614/swampyer/utils.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 swampyer-3.0.20230614/setup.py
--rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 swampyer-3.0.20230614/PKG-INFO
+-rw-r--r--   0        0        0      786 2023-06-25 23:27:54.599706 swampyer-3.0.20230623/pyproject.toml
+-rw-r--r--   0        0        0      168 2022-08-16 23:40:19.004711 swampyer-3.0.20230623/swampyer/__init__.py
+-rw-r--r--   0        0        0    39009 2023-06-25 20:40:07.217163 swampyer-3.0.20230623/swampyer/client.py
+-rw-r--r--   0        0        0     1098 2022-09-26 22:26:31.459187 swampyer-3.0.20230623/swampyer/common.py
+-rw-r--r--   0        0        0      658 2022-08-16 23:40:19.004711 swampyer-3.0.20230623/swampyer/exceptions.py
+-rw-r--r--   0        0        0     1014 2022-09-09 18:53:53.522720 swampyer-3.0.20230623/swampyer/fields.py
+-rw-r--r--   0        0        0     7101 2022-11-23 22:28:58.618298 swampyer-3.0.20230623/swampyer/messages.py
+-rw-r--r--   0        0        0    11295 2022-08-16 23:40:19.004711 swampyer-3.0.20230623/swampyer/queues.py
+-rw-r--r--   0        0        0     4696 2023-06-14 18:00:00.758370 swampyer-3.0.20230623/swampyer/serializers.py
+-rw-r--r--   0        0        0    24334 2023-06-25 23:30:19.640583 swampyer-3.0.20230623/swampyer/transport.py
+-rw-r--r--   0        0        0       57 2022-08-16 23:40:19.004711 swampyer-3.0.20230623/swampyer/utils.py
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 swampyer-3.0.20230623/setup.py
+-rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 swampyer-3.0.20230623/PKG-INFO
```

### Comparing `swampyer-3.0.20230614/pyproject.toml` & `swampyer-3.0.20230623/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [tool.poetry]
 name = "swampyer"
 description = "Simple WAMP library with minimal external dependencies"
-version = '3.0.20230614'
+version = '3.0.20230623'
 authors = ["Aki Mimoto <aki@zaber.com>"]
 packages = [
   { include = "swampyer" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4.0"
 websocket-client = ">=0.59.0"
 certifi = ">=2020.12.5"
 six = "^1.16.0"
 cbor = { version = "^1.0.0", optional = true }
 msgpack = { version = "^1.0.2", optional = true }
+websockets = { version = "^11.0.3", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = ">=4.6.11"
 
 [tool.poetry.extras]
 cbor = [ "cbor" ]
 msgpack = [ "msgpack" ]
-all = [ "cbor", "msgpack" ]
+websockets = [ "websockets" ]
+all = [ "cbor", "msgpack", "websockets" ]
 
 [tool.poetry.scripts]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `swampyer-3.0.20230614/swampyer/client.py` & `swampyer-3.0.20230623/swampyer/client.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230614/swampyer/common.py` & `swampyer-3.0.20230623/swampyer/common.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230614/swampyer/exceptions.py` & `swampyer-3.0.20230623/swampyer/exceptions.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230614/swampyer/fields.py` & `swampyer-3.0.20230623/swampyer/fields.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230614/swampyer/messages.py` & `swampyer-3.0.20230623/swampyer/messages.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230614/swampyer/queues.py` & `swampyer-3.0.20230623/swampyer/queues.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230614/swampyer/serializers.py` & `swampyer-3.0.20230623/swampyer/serializers.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20230614/swampyer/transport.py` & `swampyer-3.0.20230623/swampyer/transport.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,26 @@
 import ssl
 import stat
 import time
 import struct
 
 import socket
 import websocket
+
+HAS_ALT_WEBSOCKETS_LIBRARY = False
+if not os.getenv('SWAMPYER_DISABLE_ALT_WEBSOCKETS_LIBRARY'):
+    try:
+        import websockets.sync.client as wsc
+        HAS_ALT_WEBSOCKETS_LIBRARY = True
+    except:
+        pass
+
 import traceback
+import threading
+import logging
 import platform
 
 from .common import *
 from .messages import *
 from .utils import logger
 from .exceptions import *
 from .serializers import *
@@ -62,156 +73,314 @@
 
     def recv_data(self, control_frame=True):
         raise ExNotImplemented("recv_data is not implemented")
 
     def next(self):
         raise ExNotImplemented("next is not implemented")
 
-@register_transport('ws')
-@register_transport('wss')
-class WebsocketTransport(Transport):
-
-    loop_timeout = 1
-    protocol = 'ws'
-    ssl_origin =None
-    sslopt = None
-    subprotocols = None
-    fire_cont_frame = False
-    skip_utf8_validation = False
-    user_agent = None
-
-    def init(self, **options):
-
-        self.subprotocols = []
-        for serializer_code in self.serializers:
-            self.subprotocols.append('wamp.2.{}'.format(serializer_code))
-
-        m = re.search(r'(ws|wss)://([\w\.]+)(:?:(\d+))?',self.url)
-        if not m:
-            raise ExTransportParseError('Require ws://path or wss:// syntax for Websocket')
-        self.protocol = m.group(1).lower()
-
-        if self.protocol == 'wss':
-            origin_port = ':'+m.group(4) if m.group(4) else ''
-            self.ssl_origin = 'https://{}{}'.format(m.group(2),origin_port)
-
-        # By default if no settings are chosen we apply
-        # the looser traditional policy (makes life less
-        # secure but less excruciating on windows)
-        self.sslopt = options.get('sslopt', {
-                "cert_reqs":ssl.CERT_NONE,
-                "check_hostname": False
-            })
-
-        self.loop_timeout = options.get('loop_timeout')
-        self.fire_cont_frame = options.get('fire_cont_frame',False)
-        self.skip_utf8_validation = options.get('skip_utf8_validation',False)
-
-        self.agent = options.get('agent')
-        user_agent = options.get('user_agent')
-        if user_agent is None:
-            user_agent = "Python Swampyer v{swampyer_version} / {platform} / {python_implementation}{python_version}"
-
-        self.user_agent = user_agent.format(
-                             platform = platform.platform(),
-                             python_version = platform.python_version(),
-                             python_implementation = platform.python_implementation(),
-                             swampyer_version = version('swampyer'),
-                        )
-
-    def connect(self, **options):
-        # Handle the weird issue in websocket that the origin
-        # port will be always http://host:port even though connection is
-        # wss. This causes some origin issues with demo.crossbar.io demo
-        # so we ensure we use http or https appropriately depending on the
-        # ws or wss protocol
-
-        options.setdefault('sslopt',self.sslopt)
-        options.setdefault('subprotocols',self.subprotocols)
-
-        # Allows us to set the user agent if avaialble
-        header = options.setdefault('header', {})
-        if self.user_agent and isinstance(header, dict):
-            header.setdefault('user-agent', self.user_agent)
-
-        self.socket = websocket.WebSocket(
-                            fire_cont_frame=options.pop(
-                                  "fire_cont_frame", self.fire_cont_frame),
-                            skip_utf8_validation=options.pop(
-                                  "skip_utf8_validation", self.skip_utf8_validation),
-                            enable_multithread=True,
-                            **options)
-        self.socket.settimeout(options.get('loop_timeout',self.loop_timeout))
-        self.socket.connect(self.url, **options)
-
-        serializer_code = self.socket.subprotocol[len('wamp.2.'):]
-        self.serializer = load_serializer(serializer_code)
-
-    def settimeout(self, timeout):
-        return self.socket.settimeout(timeout)
-
-    def ping(self, last_ping_time):
-        return self.socket.ping(last_ping_time)
+if HAS_ALT_WEBSOCKETS_LIBRARY:
 
-    def send(self, payload):
-        try:
-            if self.serializer.binary:
-                self.socket.send_binary(payload)
-            else:
-                if isinstance(payload, (bytes, bytearray)):
-                    payload = payload.encode('utf8')
-                self.socket.send(payload)
-        except websocket.WebSocketConnectionClosedException:
-            raise ExWAMPConnectionError("WAMP is currently disconnected!")
-
-    def close(self):
-        return self.socket.close()
-
-    def recv_data(self, control_frame=True):
-        return self.socket.recv_data(control_frame)
-
-    def next(self):
-        """ Returns the next  buffer element
-        """
-        try:
-            opcode, data = self.recv_data(control_frame=True)
-
-            if opcode == websocket.ABNF.OPCODE_TEXT:
-                # Try to decode the data as a utf-8 string. Replace any inconvertible characters
-                # to the unicode `\uFFFD` character
-                data = data.decode('utf-8', 'replace')
+    class MyConnection(wsc.ClientConnection):
+            def __init__(
+                self,
+                socket: socket.socket,
+                protocol: wsc.ClientProtocol,
+                *,
+                close_timeout: wsc.Optional[float] = 10,
+            ) -> None:
+                self.protocol: wsc.ClientProtocol
+                self.response_rcvd = threading.Event()
+                self.socket = socket
+                self.protocol = protocol
+                self.close_timeout = close_timeout
+
+                # Inject reference to this instance in the protocol's logger.
+                self.protocol.logger = logging.LoggerAdapter(
+                    self.protocol.logger,
+                    {"websocket": self},
+                )
+
+                # Copy attributes from the protocol for convenience.
+                self.id: uuid.UUID = self.protocol.id
+                """Unique identifier of the connection. Useful in logs."""
+                self.logger: LoggerLike = self.protocol.logger
+                """Logger for this connection."""
+                self.debug = self.protocol.debug
+
+                # HTTP handshake request and response.
+                self.request: Optional[Request] = None
+                """Opening handshake request."""
+                self.response: Optional[Response] = None
+                """Opening handshake response."""
+
+                # Mutex serializing interactions with the protocol.
+                self.protocol_mutex = threading.Lock()
+
+                # Assembler turning frames into messages and serializing reads.
+                import websockets.sync.messages
+                self.recv_messages = websockets.sync.messages.Assembler()
+
+                # Whether we are busy sending a fragmented message.
+                self.send_in_progress = False
+
+                # Deadline for the closing handshake.
+                self.close_deadline: Optional[Deadline] = None
+
+                # Mapping of ping IDs to pong waiters, in chronological order.
+                self.pings: Dict[bytes, threading.Event] = {}
+
+                # Receiving events from the socket.
+                self.recv_events_thread = threading.Thread(target=self.recv_events)
+                self.recv_events_thread.daemon = True
+                self.recv_events_thread.start()
+
+                # Exception raised in recv_events, to be chained to ConnectionClosed
+                # in the user thread in order to show why the TCP connection dropped.
+                self.recv_events_exc: Optional[BaseException] = None
+
+    @register_transport('ws')
+    @register_transport('wss')
+    class WebsocketTransport(Transport):
+
+        loop_timeout = 1
+        protocol = 'ws'
+        ssl_origin =None
+        sslopt = None
+        subprotocols = None
+        user_agent = None
+
+        def init(self, **options):
+
+
+            self.subprotocols = []
+            for serializer_code in self.serializers:
+                self.subprotocols.append('wamp.2.{}'.format(serializer_code))
+
+            m = re.search(r'(ws|wss)://([\w\.]+)(:?:(\d+))?',self.url)
+            if not m:
+                raise ExTransportParseError('Require ws://path or wss2:// syntax for Websocket')
+            self.protocol = m.group(1).lower()
+
+            if self.protocol == 'wss':
+                origin_port = ':'+m.group(4) if m.group(4) else ''
+                self.ssl_origin = 'https://{}{}'.format(m.group(2),origin_port)
+
+            # By default if no settings are chosen we apply
+            # the looser traditional policy (makes life less
+            # secure but less excruciating on windows)
+            self.sslopt = options.get('sslopt', {
+                    "cert_reqs": ssl.CERT_NONE,
+                    "check_hostname": False
+                })
+
+            self.agent = options.get('agent')
+            user_agent = options.get('user_agent')
+            if user_agent is None:
+                user_agent = "Python Swampyer v{swampyer_version} / {platform} / {python_implementation}{python_version}"
+
+            self.user_agent = user_agent.format(
+                                 platform = platform.platform(),
+                                 python_version = platform.python_version(),
+                                 python_implementation = platform.python_implementation(),
+                                 swampyer_version = version('swampyer'),
+                            )
+
+        def connect(self, **options):
+            ssl_context = options.setdefault('sslopt',self.sslopt)
+            subprotocols = options.setdefault('subprotocols',self.subprotocols)
+
+            # Allows us to set the user agent if avaialble
+            header = options.setdefault('header', {})
+            if self.user_agent and isinstance(header, dict):
+                header.setdefault('user-agent', self.user_agent)
+
+            try:
+                self.socket = wsc.connect(
+                                  uri = self.url,
+                                  ssl_context = ssl_context,
+                                  subprotocols = subprotocols,
+                                  additional_headers = header,
+                                  create_connection = MyConnection,
+                              )
+                self.socket.daemon = True
+            except Exception as ex:
+                print(ex)
+                raise
+
+            serializer_code = self.socket.subprotocol[len('wamp.2.'):]
+            self.serializer = load_serializer(serializer_code)
+
+        def ping(self, last_ping_time):
+            return self.socket.ping(last_ping_time)
+
+        def close(self):
+            return self.socket.close()
+
+        def send(self, payload):
+            self.socket.send(payload)
+
+        def recv_data(self, *a, **kw):
+            return self.socket.recv()
+
+        def next(self):
+            try:
+                data = self.recv_data()
                 return self.serializer.loads(data)
-
-            if opcode == websocket.ABNF.OPCODE_BINARY:
-                return self.serializer.loads(data)
-
-            if opcode == websocket.ABNF.OPCODE_PONG:
-                duration = time.time() - float(data)
-                self._last_pong_time = time.time()
-                data = None
-                opcode = None
-                logger.debug('Received websocket ping response in %s seconds', round(duration, 3))
+            except ExWAMPConnectionError:
+                raise
+            except OSError as ex:
+                # Intended to catch Windows Socket error WSAECONNRESET (10054) which is otherwise unhandled.
+                # https://docs.microsoft.com/en-ca/windows/win32/winsock/windows-sockets-error-codes-2
+                if ex.errno == 10054:
+                    raise ExWAMPConnectionError(ex)
+                raise
+
+else:
+    @register_transport('ws')
+    @register_transport('wss')
+    class WebsocketTransport(Transport):
+
+        loop_timeout = 1
+        protocol = 'ws'
+        ssl_origin =None
+        sslopt = None
+        subprotocols = None
+        fire_cont_frame = False
+        skip_utf8_validation = False
+        user_agent = None
+
+        def init(self, **options):
+
+            self.subprotocols = []
+            for serializer_code in self.serializers:
+                self.subprotocols.append('wamp.2.{}'.format(serializer_code))
+
+            m = re.search(r'(ws|wss)://([\w\.]+)(:?:(\d+))?',self.url)
+            if not m:
+                raise ExTransportParseError('Require ws://path or wss:// syntax for Websocket')
+            self.protocol = m.group(1).lower()
+
+            if self.protocol == 'wss':
+                origin_port = ':'+m.group(4) if m.group(4) else ''
+                self.ssl_origin = 'https://{}{}'.format(m.group(2),origin_port)
+
+            # By default if no settings are chosen we apply
+            # the looser traditional policy (makes life less
+            # secure but less excruciating on windows)
+            self.sslopt = options.get('sslopt', {
+                    "cert_reqs":ssl.CERT_NONE,
+                    "check_hostname": False
+                })
+
+            self.loop_timeout = options.get('loop_timeout')
+            self.fire_cont_frame = options.get('fire_cont_frame',False)
+            self.skip_utf8_validation = options.get('skip_utf8_validation',False)
+
+            self.agent = options.get('agent')
+            user_agent = options.get('user_agent')
+            if user_agent is None:
+                user_agent = "Python Swampyer v{swampyer_version} / {platform} / {python_implementation}{python_version}"
+
+            self.user_agent = user_agent.format(
+                                 platform = platform.platform(),
+                                 python_version = platform.python_version(),
+                                 python_implementation = platform.python_implementation(),
+                                 swampyer_version = version('swampyer'),
+                            )
+
+        def connect(self, **options):
+            # Handle the weird issue in websocket that the origin
+            # port will be always http://host:port even though connection is
+            # wss. This causes some origin issues with demo.crossbar.io demo
+            # so we ensure we use http or https appropriately depending on the
+            # ws or wss protocol
+
+            options.setdefault('sslopt',self.sslopt)
+            options.setdefault('subprotocols',self.subprotocols)
+
+            # Allows us to set the user agent if avaialble
+            header = options.setdefault('header', {})
+            if self.user_agent and isinstance(header, dict):
+                header.setdefault('user-agent', self.user_agent)
+
+            self.socket = websocket.WebSocket(
+                                fire_cont_frame=options.pop(
+                                      "fire_cont_frame", self.fire_cont_frame),
+                                skip_utf8_validation=options.pop(
+                                      "skip_utf8_validation", self.skip_utf8_validation),
+                                enable_multithread=True,
+                                **options)
+            self.socket.settimeout(options.get('loop_timeout',self.loop_timeout))
+            self.socket.connect(self.url, **options)
+
+            serializer_code = self.socket.subprotocol[len('wamp.2.'):]
+            self.serializer = load_serializer(serializer_code)
+
+        def settimeout(self, timeout):
+            return self.socket.settimeout(timeout)
+
+        def ping(self, last_ping_time):
+            return self.socket.ping(last_ping_time)
+
+        def send(self, payload):
+            try:
+                if self.serializer.binary:
+                    self.socket.send_binary(payload)
+                else:
+                    if isinstance(payload, (bytes, bytearray)):
+                        payload = payload.encode('utf8')
+                    self.socket.send(payload)
+            except websocket.WebSocketConnectionClosedException:
+                raise ExWAMPConnectionError("WAMP is currently disconnected!")
+
+        def close(self):
+            return self.socket.close()
+
+        def recv_data(self, control_frame=True):
+            return self.socket.recv_data(control_frame)
+
+        def next(self):
+            """ Returns the next  buffer element
+            """
+            try:
+                opcode, data = self.recv_data(control_frame=True)
+
+                if opcode == websocket.ABNF.OPCODE_TEXT:
+                    # Try to decode the data as a utf-8 string. Replace any inconvertible characters
+                    # to the unicode `\uFFFD` character
+                    data = data.decode('utf-8', 'replace')
+                    return self.serializer.loads(data)
+
+                if opcode == websocket.ABNF.OPCODE_BINARY:
+                    return self.serializer.loads(data)
+
+                if opcode == websocket.ABNF.OPCODE_PONG:
+                    duration = time.time() - float(data)
+                    self._last_pong_time = time.time()
+                    data = None
+                    opcode = None
+                    logger.debug('Received websocket ping response in %s seconds', round(duration, 3))
+                    return
+                
+                if opcode not in (websocket.ABNF.OPCODE_TEXT, websocket.ABNF.OPCODE_BINARY):
+                    return
+            except io.BlockingIOError:
                 return
-            
-            if opcode not in (websocket.ABNF.OPCODE_TEXT, websocket.ABNF.OPCODE_BINARY):
+            except websocket.WebSocketTimeoutException:
                 return
-        except io.BlockingIOError:
-            return
-        except websocket.WebSocketTimeoutException:
-            return
-        except websocket.WebSocketConnectionClosedException as ex:
-            raise ExWAMPConnectionError(ex)
-        except OSError as ex:
-            # Intended to catch Windows Socket error WSAECONNRESET (10054) which is otherwise unhandled.
-            # https://docs.microsoft.com/en-ca/windows/win32/winsock/windows-sockets-error-codes-2
-            if ex.errno == 10054:
+            except websocket.WebSocketConnectionClosedException as ex:
                 raise ExWAMPConnectionError(ex)
-            raise
-        except ExWAMPConnectionError:
-            raise
+            except OSError as ex:
+                # Intended to catch Windows Socket error WSAECONNRESET (10054) which is otherwise unhandled.
+                # https://docs.microsoft.com/en-ca/windows/win32/winsock/windows-sockets-error-codes-2
+                if ex.errno == 10054:
+                    raise ExWAMPConnectionError(ex)
+                raise
+            except ExWAMPConnectionError:
+                raise
 
 class RawsocketTransport(Transport):
     """
     Raw Socket transport is detailed here:
 
     https://github.com/wamp-proto/wamp-proto/blob/master/rfc/text/advanced/ap_transport_rawsocket.md
     """
```

