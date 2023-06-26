# Comparing `tmp/ailingbot-0.0.2.tar.gz` & `tmp/ailingbot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailingbot-0.0.2.tar", max compression
+gzip compressed data, was "ailingbot-0.0.3.tar", max compression
```

## Comparing `ailingbot-0.0.2.tar` & `ailingbot-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,36 @@
--rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.2/LICENSE
--rw-r--r--   0        0        0     6347 2023-06-21 10:56:08.852892 ailingbot-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.2/ailingbot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021690 ailingbot-0.0.2/ailingbot/brokers/__init__.py
--rw-r--r--   0        0        0     1940 2023-06-21 04:05:07.363931 ailingbot-0.0.2/ailingbot/brokers/broker.py
--rw-r--r--   0        0        0     4642 2023-06-21 04:29:08.996776 ailingbot-0.0.2/ailingbot/brokers/pika_broker.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.2/ailingbot/channels/__init__.py
--rw-r--r--   0        0        0     3643 2023-06-21 08:27:09.822487 ailingbot-0.0.2/ailingbot/channels/channel.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.2/ailingbot/channels/dingtalk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.2/ailingbot/channels/feishu/__init__.py
--rw-r--r--   0        0        0     5120 2023-06-21 04:20:13.833468 ailingbot-0.0.2/ailingbot/channels/feishu/agent.py
--rw-r--r--   0        0        0      736 2023-06-19 04:32:16.486131 ailingbot-0.0.2/ailingbot/channels/feishu/render.py
--rw-r--r--   0        0        0     4580 2023-06-21 04:20:13.827390 ailingbot-0.0.2/ailingbot/channels/feishu/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.2/ailingbot/channels/slack/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.2/ailingbot/channels/wechatwork/__init__.py
--rw-r--r--   0        0        0     4350 2023-06-21 04:14:09.084365 ailingbot-0.0.2/ailingbot/channels/wechatwork/agent.py
--rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.2/ailingbot/channels/wechatwork/encrypt.py
--rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.2/ailingbot/channels/wechatwork/render.py
--rw-r--r--   0        0        0     5050 2023-06-21 04:20:13.825716 ailingbot-0.0.2/ailingbot/channels/wechatwork/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.2/ailingbot/chat/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-21 08:26:56.359421 ailingbot-0.0.2/ailingbot/chat/chatbot.py
--rw-r--r--   0        0        0     3353 2023-06-19 04:12:03.268708 ailingbot-0.0.2/ailingbot/chat/messages.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.2/ailingbot/chat/policies/__init__.py
--rw-r--r--   0        0        0     1550 2023-06-21 04:13:29.677392 ailingbot-0.0.2/ailingbot/chat/policies/echo.py
--rw-r--r--   0        0        0     2390 2023-06-21 04:13:29.695901 ailingbot-0.0.2/ailingbot/chat/policies/langchain.py
--rw-r--r--   0        0        0     1761 2023-06-21 04:13:29.672032 ailingbot-0.0.2/ailingbot/chat/policy.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.2/ailingbot/cli/__init__.py
--rw-r--r--   0        0        0    12635 2023-06-21 04:30:47.588258 ailingbot-0.0.2/ailingbot/cli/cli.py
--rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.2/ailingbot/cli/options.py
--rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.2/ailingbot/cli/render.py
--rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.2/ailingbot/config.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.2/ailingbot/endpoint/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033407 ailingbot-0.0.2/ailingbot/repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033650 ailingbot-0.0.2/ailingbot/repositories/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.2/ailingbot/shared/__init__.py
--rw-r--r--   0        0        0     3953 2023-06-13 06:48:58.034885 ailingbot-0.0.2/ailingbot/shared/abc.py
--rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.2/ailingbot/shared/errors.py
--rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.2/ailingbot/shared/misc.py
--rw-r--r--   0        0        0     1068 2023-06-21 10:56:30.338610 ailingbot-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7826 1970-01-01 00:00:00.000000 ailingbot-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4761 2023-06-26 06:59:47.356194 ailingbot-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.3/ailingbot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.3/ailingbot/channels/__init__.py
+-rw-r--r--   0        0        0     2387 2023-06-26 06:57:43.397704 ailingbot-0.0.3/ailingbot/channels/channel.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.3/ailingbot/channels/dingtalk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.3/ailingbot/channels/feishu/__init__.py
+-rw-r--r--   0        0        0     5760 2023-06-26 06:57:43.398602 ailingbot-0.0.3/ailingbot/channels/feishu/agent.py
+-rw-r--r--   0        0        0      736 2023-06-19 04:32:16.486131 ailingbot-0.0.3/ailingbot/channels/feishu/render.py
+-rw-r--r--   0        0        0     6793 2023-06-26 06:57:43.399534 ailingbot-0.0.3/ailingbot/channels/feishu/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.3/ailingbot/channels/slack/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.3/ailingbot/channels/wechatwork/__init__.py
+-rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.3/ailingbot/channels/wechatwork/agent.py
+-rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.3/ailingbot/channels/wechatwork/encrypt.py
+-rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.3/ailingbot/channels/wechatwork/render.py
+-rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.3/ailingbot/channels/wechatwork/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.3/ailingbot/chat/__init__.py
+-rw-r--r--   0        0        0     2076 2023-06-26 06:57:43.401435 ailingbot-0.0.3/ailingbot/chat/chatbot.py
+-rw-r--r--   0        0        0     3487 2023-06-25 06:38:56.364334 ailingbot-0.0.3/ailingbot/chat/messages.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.3/ailingbot/chat/policies/__init__.py
+-rw-r--r--   0        0        0     5759 2023-06-25 09:11:14.559103 ailingbot-0.0.3/ailingbot/chat/policies/langchain.py
+-rw-r--r--   0        0        0     1678 2023-06-25 07:39:16.611374 ailingbot-0.0.3/ailingbot/chat/policy.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.3/ailingbot/cli/__init__.py
+-rw-r--r--   0        0        0     8659 2023-06-26 06:57:43.402052 ailingbot-0.0.3/ailingbot/cli/cli.py
+-rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.3/ailingbot/cli/options.py
+-rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.3/ailingbot/cli/render.py
+-rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.3/ailingbot/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.3/ailingbot/endpoint/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033407 ailingbot-0.0.3/ailingbot/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033650 ailingbot-0.0.3/ailingbot/repositories/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.3/ailingbot/shared/__init__.py
+-rw-r--r--   0        0        0     3953 2023-06-13 06:48:58.034885 ailingbot-0.0.3/ailingbot/shared/abc.py
+-rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.3/ailingbot/shared/errors.py
+-rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.3/ailingbot/shared/misc.py
+-rw-r--r--   0        0        0     1071 2023-06-26 06:58:18.165938 ailingbot-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6243 1970-01-01 00:00:00.000000 ailingbot-0.0.3/PKG-INFO
```

### Comparing `ailingbot-0.0.2/LICENSE` & `ailingbot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/ailingbot/channels/channel.py` & `ailingbot-0.0.3/ailingbot/channels/channel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,52 @@
 from __future__ import annotations
 
 import abc
-import asyncio
 import typing
 
 from asgiref.typing import ASGIApplication
-from loguru import logger
 
-import ailingbot.shared.errors
-from ailingbot.brokers.broker import MessageBroker
-from ailingbot.chat.messages import ResponseMessage
-from ailingbot.config import settings
-from ailingbot.shared.abc import AbstractAsyncRunnable
+from ailingbot.shared.abc import AbstractAsyncComponent
 from ailingbot.shared.misc import get_class_dynamically
 
 
-class ChannelAgent(AbstractAsyncRunnable, abc.ABC):
+class ChannelAgent(AbstractAsyncComponent, abc.ABC):
     """Base class of channel agents."""
 
-    def __init__(self, *, num_of_tasks: int = 1):
-        super(ChannelAgent, self).__init__(num_of_tasks=num_of_tasks)
-
-        self.broker: typing.Optional[MessageBroker] = None
-
-    @abc.abstractmethod
-    async def send_message(self, message: ResponseMessage) -> None:
-        """Send message from agent to users, groups or other targets.
-
-        :param message: Message body.
-        :type message: ResponseMessage
-        """
-        raise NotImplementedError
-
-    async def _startup(self) -> None:
-        self.broker = MessageBroker.get_broker(
-            settings.broker.name,
-        )
-        await self.broker.initialize()
-
-    async def _main_task(self, *, number: int) -> None:
-        try:
-            response_message = await self.broker.consume_response()
-            await self.send_message(response_message)
-        except ailingbot.shared.errors.EmptyQueueError:
-            await asyncio.sleep(1)
-
-    async def _shutdown(self) -> None:
-        await self.broker.finalize()
+    def __init__(self):
+        super(ChannelAgent, self).__init__()
 
     @staticmethod
-    def get_agent(name: str, num_of_tasks: int = 1) -> ChannelAgent:
+    def get_agent(name: str) -> ChannelAgent:
         """Gets channel agent instance.
 
         :param name: Built-in channel name or full path of agent class.
         :type name: str
-        :param num_of_tasks:
-        :type num_of_tasks:
         :return: Agent instance.
         :rtype: ChannelAgent
         """
         if name.lower() == 'wechatwork':
             from ailingbot.channels.wechatwork.agent import WechatworkAgent
 
-            instance = WechatworkAgent(num_of_tasks=num_of_tasks)
+            instance = WechatworkAgent()
         elif name.lower() == 'feishu':
             from ailingbot.channels.feishu.agent import FeishuAgent
 
-            instance = FeishuAgent(num_of_tasks=num_of_tasks)
+            instance = FeishuAgent()
         else:
-            instance = get_class_dynamically(name)(num_of_tasks=num_of_tasks)
+            instance = get_class_dynamically(name)()
 
         return instance
 
 
 class ChannelWebhookFactory(abc.ABC):
     """Base class of channel webhook factories."""
 
-    def __init__(self):
-        pass
+    def __init__(self, *, debug: bool = False):
+        self.debug = debug
 
     async def create_webhook_app(self) -> ASGIApplication | typing.Callable:
         """Creates a ASGI application.
 
         :return: ASGI application.
         :rtype: typing.Union[ASGIApplication, typing.Callable]
         """
```

### Comparing `ailingbot-0.0.2/ailingbot/channels/feishu/agent.py` & `ailingbot-0.0.3/ailingbot/channels/feishu/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,17 @@
 from ailingbot.config import settings
 from ailingbot.shared.errors import ExternalHTTPAPIError
 
 
 class FeishuAgent(ChannelAgent):
     """Feishu channel agent class."""
 
-    def __init__(
-        self,
-        *,
-        num_of_tasks: int = 1,
-    ):
+    def __init__(self):
         """Initializes class."""
-        super(FeishuAgent, self).__init__(
-            num_of_tasks=num_of_tasks,
-        )
+        super(FeishuAgent, self).__init__()
 
         self.app_id = settings.channel.app_id
         self.app_secret = settings.channel.app_secret
         self.access_token: typing.Optional[str] = None
         self.expire_in: typing.Optional[arrow.Arrow] = None
 
     async def _get_access_token(self) -> str:
@@ -139,7 +133,24 @@
             receive_id_type = 'open_id'
 
         if message.ack_uuid:
             await self._reply(ack_uuid=message.ack_uuid, body=body)
         else:
             body['receive_id'] = message.receiver_id
             await self._send(receive_id_type=receive_id_type, body=body)
+
+    async def get_resource_from_message(
+        self, message_id: str, file_key: str, resource_type: str
+    ) -> bytes:
+        """Get file or image resource from message."""
+        access_token = await self._get_access_token()
+        async with aiohttp.ClientSession() as session:
+            async with session.get(
+                f'https://open.feishu.cn/open-apis/im/v1/messages/{message_id}/resources/{file_key}',
+                headers={
+                    'Authorization': f'Bearer {access_token}',
+                },
+                params={'type': resource_type},
+            ) as response:
+                if not response.ok:
+                    response.raise_for_status()
+                return await response.content.read()
```

### Comparing `ailingbot-0.0.2/ailingbot/channels/feishu/render.py` & `ailingbot-0.0.3/ailingbot/channels/feishu/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/ailingbot/channels/wechatwork/agent.py` & `ailingbot-0.0.3/ailingbot/channels/wechatwork/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,17 @@
 from ailingbot.config import settings
 from ailingbot.shared.errors import ExternalHTTPAPIError
 
 
 class WechatworkAgent(ChannelAgent):
     """Wechatwork channel agent class."""
 
-    def __init__(
-        self,
-        *,
-        num_of_tasks: int = 1,
-    ):
+    def __init__(self):
         """Initializes class."""
-        super(WechatworkAgent, self).__init__(
-            num_of_tasks=num_of_tasks,
-        )
+        super(WechatworkAgent, self).__init__()
 
         self.corpid = settings.channel.corpid
         self.corpsecret = settings.channel.corpsecret
         self.agentid = settings.channel.agentid
         self.access_token: typing.Optional[str] = None
         self.expire_in: typing.Optional[arrow.Arrow] = None
```

### Comparing `ailingbot-0.0.2/ailingbot/channels/wechatwork/encrypt.py` & `ailingbot-0.0.3/ailingbot/channels/wechatwork/encrypt.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/ailingbot/channels/wechatwork/render.py` & `ailingbot-0.0.3/ailingbot/channels/wechatwork/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/ailingbot/channels/wechatwork/webhook.py` & `ailingbot-0.0.3/ailingbot/channels/wechatwork/webhook.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,66 @@
 from __future__ import annotations
 
 import typing
 from urllib import parse
 
 import xmltodict
 from asgiref.typing import ASGIApplication
-from fastapi import FastAPI, status, HTTPException
+from fastapi import FastAPI, status, HTTPException, BackgroundTasks
 from fastapi.requests import Request
 from fastapi.responses import PlainTextResponse
 
-from ailingbot.brokers.broker import MessageBroker
 from ailingbot.channels.channel import ChannelWebhookFactory
+from ailingbot.channels.wechatwork.agent import WechatworkAgent
 from ailingbot.channels.wechatwork.encrypt import signature, decrypt
-from ailingbot.chat.messages import TextRequestMessage, MessageScope
+from ailingbot.chat.chatbot import ChatBot
+from ailingbot.chat.messages import (
+    TextRequestMessage,
+    MessageScope,
+    RequestMessage,
+)
 from ailingbot.config import settings
 
 
 class WechatworkWebhookFactory(ChannelWebhookFactory):
     """Factory that creates wechatwork webhook ASGI application."""
 
-    def __init__(self):
-        super(WechatworkWebhookFactory, self).__init__()
+    def __init__(self, debug: bool = False):
+        super(WechatworkWebhookFactory, self).__init__(debug=debug)
 
         self.token = settings.channel.token
         self.aes_key = settings.channel.aes_key
 
-        self.broker: typing.Optional[MessageBroker] = None
         self.app: typing.Optional[ASGIApplication | typing.Callable] = None
+        self.agent: typing.Optional[WechatworkAgent] = None
+        self.bot: typing.Optional[ChatBot] = None
 
     async def create_webhook_app(self) -> ASGIApplication | typing.Callable:
-        self.broker = MessageBroker.get_broker(settings.broker.name)
         self.app = FastAPI()
+        self.agent = WechatworkAgent()
+        self.bot = ChatBot(debug=self.debug)
+
+        async def _chat_task(
+            conversation_id: str, message: RequestMessage
+        ) -> None:
+            """Send a request message to the bot, receive a response message, and send it back to the user."""
+            response = await self.bot.chat(
+                conversation_id=conversation_id, message=message
+            )
+            await self.agent.send_message(response)
 
         @self.app.on_event('startup')
         async def startup() -> None:
-            await self.broker.initialize()
+            await self.agent.initialize()
+            await self.bot.initialize()
 
         @self.app.on_event('shutdown')
         async def shutdown() -> None:
-            await self.broker.finalize()
+            await self.agent.finalize()
+            await self.bot.finalize()
 
         @self.app.get(
             '/webhook/wechatwork/event/',
             status_code=status.HTTP_200_OK,
             response_class=PlainTextResponse,
         )
         async def handle_challenge(
@@ -80,26 +98,32 @@
             message, _ = decrypt(key=aes_key, msg_encrypt=encrypt_message)
             return message
 
         @self.app.post(
             '/webhook/wechatwork/event/', status_code=status.HTTP_200_OK
         )
         async def handle_event(
-            msg_signature: str, timestamp: int, nonce: int, request: Request
+            msg_signature: str,
+            timestamp: int,
+            nonce: int,
+            request: Request,
+            background_tasks: BackgroundTasks,
         ) -> dict:
             """Handle the event request from Wechatwork.
 
             :param msg_signature: Message signature from challenge request.
             :type msg_signature: str
             :param timestamp: Challenge request timestamp.
             :type timestamp: int
             :param nonce: Challenge request nonce.
             :type nonce: int
             :param request: Http request.
             :type request: Request
+            :param background_tasks:
+            :type background_tasks:
             :return: Empty dict.
             :rtype: dict
             """
             token = self.token
             aes_key = self.aes_key
             body_xml = await request.body()
             body = xmltodict.parse(body_xml)
@@ -130,12 +154,14 @@
                     uuid=message_id,
                     sender_id=from_user_name,
                     scope=MessageScope.USER,
                     text=content,
                 )
 
             if req_msg:
-                await self.broker.produce_request(req_msg)
+                background_tasks.add_task(
+                    _chat_task, req_msg.sender_id, req_msg
+                )
 
             return {}
 
         return self.app
```

### Comparing `ailingbot-0.0.2/ailingbot/chat/messages.py` & `ailingbot-0.0.3/ailingbot/chat/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,22 @@
 
 class TextRequestMessage(RequestMessage):
     """Plain text request message."""
 
     text: str = ''
 
 
+class FileRequestMessage(RequestMessage):
+    """File request message."""
+
+    content: bytes
+    file_type: str
+    file_name: str
+
+
 class InputRequestMessage(RequestMessage):
     """Input request message."""
 
     value: typing.Any = None
 
 
 class ResponseMessage(BaseModel, abc.ABC):
```

### Comparing `ailingbot-0.0.2/ailingbot/chat/policies/langchain.py` & `ailingbot-0.0.3/ailingbot/chat/chatbot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,72 @@
+from __future__ import annotations
+
+import asyncio
+import typing
 import uuid
 
-from langchain import ConversationChain
-from langchain.chains.base import Chain
-from langchain.chains.loading import load_chain_from_config
-from langchain.llms.loading import load_llm_from_config
-from langchain.memory import ConversationBufferMemory
+from loguru import logger
 
 from ailingbot.chat.messages import (
     RequestMessage,
-    ResponseMessage,
-    TextRequestMessage,
-    TextResponseMessage,
     FallbackResponseMessage,
+    ResponseMessage,
 )
 from ailingbot.chat.policy import ChatPolicy
 from ailingbot.config import settings
+from ailingbot.shared.abc import AbstractAsyncComponent
 
 
-class LCChainChatPolicy(ChatPolicy):
-    """Load LangChain chain and use the chain as chat policy"""
+class ChatBot(AbstractAsyncComponent):
+    """ChatBot is core component that responsible for retrieve request and make response."""
 
     def __init__(
         self,
         *,
         debug: bool = False,
     ):
-        super(LCChainChatPolicy, self).__init__(debug=debug)
+        super(ChatBot, self).__init__()
 
-        self.chain: dict[str, Chain] = {}
+        self.debug = debug
 
-    async def _load_chain(self) -> Chain:
-        config = {
-            '_type': settings.policy._type,
-            'llm': settings.policy.llm,
-            'prompt': settings.policy.prompt,
-        }
-        if self.debug:
-            config['verbose'] = True
-        return load_chain_from_config(config)
+        self.locks: dict[str, asyncio.Lock] = {}
+        self.policy: typing.Optional[ChatPolicy] = None
 
-    async def respond(
+    async def chat(
         self, *, conversation_id: str, message: RequestMessage
     ) -> ResponseMessage:
-        if not isinstance(message, TextRequestMessage):
-            response = FallbackResponseMessage()
-            response.reason = 'LCChainChatPolicy can only handle messages of type TextRequestMessage.'
-        else:
-            if conversation_id not in self.chain:
-                self.chain[conversation_id] = await self._load_chain()
-            r = await self.chain[conversation_id].arun(message.text)
-            response = TextResponseMessage()
-            response.text = r
-        response.uuid = str(uuid.uuid4())
-        response.ack_uuid = message.uuid
-        response.receiver_id = message.sender_id
-        response.scope = message.scope
-        response.echo = message.echo
+        """Run chat pipeline, and replies messages to sender.
 
-        return response
-
-
-class LCConversationChain(LCChainChatPolicy):
-    def __init__(
-        self,
-        *,
-        debug: bool = False,
-    ):
-        super(LCConversationChain, self).__init__(
-            debug=debug,
+        :param conversation_id: Conversation id.
+        :type conversation_id: str
+        :param message: Reqeust message.
+        :type message: RequestMessage
+        """
+        if conversation_id not in self.locks:
+            self.locks[conversation_id] = asyncio.Lock()
+        lock = self.locks[conversation_id]
+
+        async with lock:
+            try:
+                return await self.policy.respond(
+                    conversation_id=conversation_id, message=message
+                )
+            except Exception as e:
+                logger.error(e)
+                return FallbackResponseMessage(
+                    uuid=str(uuid.uuid4()),
+                    ack_uuid=message.uuid,
+                    receiver_id=message.sender_id,
+                    scope=message.scope,
+                    echo=message.echo,
+                    reason=str(e),
+                )
+
+    async def _initialize(self) -> None:
+        self.policy = ChatPolicy.get_policy(
+            name=settings.policy.name,
+            debug=self.debug,
         )
+        await self.policy.initialize()
 
-    async def _load_chain(self) -> Chain:
-        llm = load_llm_from_config(settings.policy.llm)
-        return ConversationChain(
-            llm=llm,
-            memory=ConversationBufferMemory(),
-            verbose=self.debug,
-        )
+    async def _finalize(self):
+        await self.policy.finalize()
```

### Comparing `ailingbot-0.0.2/ailingbot/chat/policy.py` & `ailingbot-0.0.3/ailingbot/chat/policy.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,23 +35,23 @@
         :param name: Built-in policy name or full path of policy class.
         :type name: str
         :param debug:
         :type debug:
         :return: Policy instance.
         :rtype: ChatPolicy
         """
-        if name.lower() == 'echo':
-            from ailingbot.chat.policies.echo import EchoChatPolicy
+        if name.lower() == 'lc_conversation':
+            from ailingbot.chat.policies.langchain import (
+                LCConversationChatPolicy,
+            )
 
-            instance = EchoChatPolicy(debug=debug)
-        elif name.lower() == 'lc_llm_chain':
-            from ailingbot.chat.policies.langchain import LCChainChatPolicy
+            instance = LCConversationChatPolicy(debug=debug)
+        elif name.lower() == 'lc_document_qa':
+            from ailingbot.chat.policies.langchain import (
+                LCDocumentQAPolicy,
+            )
 
-            instance = LCChainChatPolicy(debug=debug)
-        elif name.lower() == 'lc_conversation_chain':
-            from ailingbot.chat.policies.langchain import LCConversationChain
-
-            instance = LCConversationChain(debug=debug)
+            instance = LCDocumentQAPolicy(debug=debug)
         else:
             instance = get_class_dynamically(name)(debug=debug)
 
         return instance
```

### Comparing `ailingbot-0.0.2/ailingbot/cli/options.py` & `ailingbot-0.0.3/ailingbot/cli/options.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/ailingbot/cli/render.py` & `ailingbot-0.0.3/ailingbot/cli/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/ailingbot/config.py` & `ailingbot-0.0.3/ailingbot/config.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/ailingbot/shared/abc.py` & `ailingbot-0.0.3/ailingbot/shared/abc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/ailingbot/shared/errors.py` & `ailingbot-0.0.3/ailingbot/shared/errors.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/ailingbot/shared/misc.py` & `ailingbot-0.0.3/ailingbot/shared/misc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.2/pyproject.toml` & `ailingbot-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ailingbot"
-version = "0.0.2"
+version = "0.0.3"
 description = "An all-in-one solution to empower your IM bot with LLM."
 authors = ["ericzhang-cn <ericzhang.buaa@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
@@ -12,29 +12,29 @@
 cryptography = "^38.0.3"
 arrow = "^1.2.3"
 dynaconf = "^3.1.11"
 fastapi = "^0.86.0"
 xmltodict = "^0.13.0"
 uvicorn = "^0.19.0"
 loguru = "^0.6.0"
-pika = "^1.3.1"
-aio-pika = "^8.2.4"
 aiohttp = { version = "^3.8.3", extras = ["speedups"] }
-aioredis = "^2.0.1"
 tomli = "^2.0.1"
 babel = "^2.11.0"
 click = "^8.1.3"
 asgiref = "^3.5.2"
 tabulate = { version = "^0.9.0", extras = ["widechars"] }
 emoji = "^2.2.0"
 prompt-toolkit = "^3.0.33"
-langchain = "^0.0.192"
+langchain = "^0.0.214"
 openai = "^0.27.8"
 rich = "^13.4.2"
 tomlkit = "^0.11.8"
+chromadb = "^0.3.26"
+pypdf = "^3.11.0"
+tiktoken = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 sphinx = "^5.3.0"
 pytest-asyncio = "^0.20.1"
 blue = "^0.9.1"
```

