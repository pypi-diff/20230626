# Comparing `tmp/villa-0.3.0.tar.gz` & `tmp/villa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.3.0.tar", max compression
+gzip compressed data, was "villa-0.4.0.tar", max compression
```

## Comparing `villa-0.3.0.tar` & `villa-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-06-16 13:41:35.807920 villa-0.3.0/LICENSE
--rw-r--r--   0        0        0     2844 2023-06-16 13:41:35.807920 villa-0.3.0/README.md
--rw-r--r--   0        0        0     1034 2023-06-16 13:41:35.807920 villa-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      285 2023-06-16 13:41:35.807920 villa-0.3.0/villa/__init__.py
--rw-r--r--   0        0        0    40237 2023-06-16 13:41:35.807920 villa-0.3.0/villa/bot.py
--rw-r--r--   0        0        0     8160 2023-06-16 13:41:35.807920 villa-0.3.0/villa/event.py
--rw-r--r--   0        0        0      473 2023-06-16 13:41:35.807920 villa-0.3.0/villa/exception.py
--rw-r--r--   0        0        0     1504 2023-06-16 13:41:35.807920 villa-0.3.0/villa/log.py
--rw-r--r--   0        0        0    16803 2023-06-16 13:41:35.807920 villa-0.3.0/villa/message.py
--rw-r--r--   0        0        0    10411 2023-06-16 13:41:35.807920 villa-0.3.0/villa/models.py
--rw-r--r--   0        0        0      935 2023-06-16 13:41:35.807920 villa-0.3.0/villa/store.py
--rw-r--r--   0        0        0      822 2023-06-16 13:41:35.807920 villa-0.3.0/villa/typing.py
--rw-r--r--   0        0        0      995 2023-06-16 13:41:35.807920 villa-0.3.0/villa/utils.py
--rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 villa-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-26 11:15:15.743545 villa-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2844 2023-06-26 11:15:15.743545 villa-0.4.0/README.md
+-rw-r--r--   0        0        0     1034 2023-06-26 11:15:15.743545 villa-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      285 2023-06-26 11:15:15.743545 villa-0.4.0/villa/__init__.py
+-rw-r--r--   0        0        0    38394 2023-06-26 11:15:15.743545 villa-0.4.0/villa/bot.py
+-rw-r--r--   0        0        0    10676 2023-06-26 11:15:15.747545 villa-0.4.0/villa/event.py
+-rw-r--r--   0        0        0      473 2023-06-26 11:15:15.747545 villa-0.4.0/villa/exception.py
+-rw-r--r--   0        0        0     1504 2023-06-26 11:15:15.747545 villa-0.4.0/villa/log.py
+-rw-r--r--   0        0        0    17127 2023-06-26 11:15:15.747545 villa-0.4.0/villa/message.py
+-rw-r--r--   0        0        0     8899 2023-06-26 11:15:15.747545 villa-0.4.0/villa/models.py
+-rw-r--r--   0        0        0      935 2023-06-26 11:15:15.747545 villa-0.4.0/villa/store.py
+-rw-r--r--   0        0        0      822 2023-06-26 11:15:15.747545 villa-0.4.0/villa/typing.py
+-rw-r--r--   0        0        0      995 2023-06-26 11:15:15.747545 villa-0.4.0/villa/utils.py
+-rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 villa-0.4.0/PKG-INFO
```

### Comparing `villa-0.3.0/LICENSE` & `villa-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.3.0/README.md` & `villa-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `villa-0.3.0/pyproject.toml` & `villa-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.3.0"
+version = "0.4.0"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.3.0/villa/bot.py` & `villa-0.4.0/villa/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import asyncio
 from itertools import product
 from typing import Any, Set, Dict, List, Type, Union, Literal, Optional
 
 import httpx
 import uvicorn
+from fastapi import FastAPI
 from pydantic import parse_obj_as
 from fastapi.responses import JSONResponse
 
 from .models import *
 from .message import Message
 from .exception import ActionFailed
 from .message import MessageSegment
@@ -20,29 +21,29 @@
 from .message import Image as ImageSegment
 from .store import get_app, get_bot, store_bot
 from .message import RoomLink as RoomLinkSegment
 from .typing import T_Func, T_Handler, EventHandler
 from .message import MentionAll as MentionAllSegment
 from .message import MentionUser as MentionUserSegment
 from .message import MentionRobot as MentionRobotSegment
-from .event import Event, SendMessageEvent, event_classes
+from .event import Event, SendMessageEvent, event_classes, pre_handle_event
 
 
 class Bot:
     """Villa Bot"""
 
     _event_handlers: List[EventHandler] = []
     _client: httpx.AsyncClient
     bot_id: str
     """机器人 Id"""
     bot_secret: str
     """机器人密钥"""
     callback_url: str
     """事件回调地址"""
-    bot_info: Optional[Robot] = None
+    _bot_info: Optional[Robot] = None
     """机器人信息"""
 
     def __init__(self, bot_id: str, bot_secret: str, callback_url: str):
         """初始化一个 Bot 实例
 
         参数:
             bot_id: 机器人 ID
@@ -56,45 +57,45 @@
             base_url="https://bbs-api.miyoushe.com/vila/api/bot/platform/"
         )
         store_bot(self)
 
     @property
     def nickname(self) -> str:
         """Bot 昵称"""
-        if self.bot_info is None:
+        if self._bot_info is None:
             raise ValueError(f"Bot {self.bot_id} not connected")
-        return self.bot_info.template.name
+        return self._bot_info.template.name
 
     @property
     def avatar_icon(self) -> str:
         """Bot 头像地址"""
-        if self.bot_info is None:
+        if self._bot_info is None:
             raise ValueError(f"Bot {self.bot_id} not connected")
-        return self.bot_info.template.icon
+        return self._bot_info.template.icon
 
     @property
-    def commands(self) -> Optional[List[RobotCommand]]:
+    def commands(self) -> Optional[List[Command]]:
         """Bot 预设命令列表"""
-        if self.bot_info is None:
+        if self._bot_info is None:
             raise ValueError(f"Bot {self.bot_id} not connected")
-        return self.bot_info.template.commands
+        return self._bot_info.template.commands
 
     @property
     def description(self) -> str:
         """Bot 介绍"""
-        if self.bot_info is None:
+        if self._bot_info is None:
             raise ValueError(f"Bot {self.bot_id} not connected")
-        return self.bot_info.template.desc
+        return self._bot_info.template.desc
 
     @property
     def current_villa_id(self) -> int:
         """Bot 最后收到的事件的大别野 ID"""
-        if self.bot_info is None:
+        if self._bot_info is None:
             raise ValueError(f"Bot {self.bot_id} not connected")
-        return self.bot_info.villa_id
+        return self._bot_info.villa_id
 
     def on_event(
         self, *event_type: Type[Event], block: bool = False, priority: int = 1
     ):
         """注册一个事件处理函数
 
         当事件属于 event_type 中的任意一个时，执行处理函数。
@@ -531,53 +532,14 @@
         await self._request(
             "POST",
             "sortGroupList",
             villa_id,
             json={"villa_id": villa_id, "group_ids": group_ids},
         )
 
-    async def create_room(
-        self,
-        villa_id: int,
-        room_name: str,
-        room_type: Union[Literal[1, 2, 3], CreateRoomType],
-        group_id: int,
-        room_default_notify_type: Union[Literal[1, 2], CreateRoomDefaultNotifyType],
-        send_msg_auth_range: SendMsgAuthRange,
-    ) -> Room:
-        """创建房间
-
-        参数:
-            villa_id: 大别野 ID
-            room_name: 房间名称
-            room_type: 房间类型
-            group_id: 分组 ID
-            room_default_notify_type: 房间默认通知类型
-            send_msg_auth_range: 房间消息发送权限范围设置
-
-        返回:
-            Room: 房间信息
-        """
-        return Room.parse_obj(
-            (
-                await self._request(
-                    "POST",
-                    "createRoom",
-                    villa_id,
-                    json={
-                        "room_name": room_name,
-                        "room_type": room_type,
-                        "group_id": group_id,
-                        "room_default_notify_type": room_default_notify_type,
-                        "send_msg_auth_range": send_msg_auth_range.dict(),
-                    },
-                )
-            )["room"]
-        )
-
     async def edit_room(self, villa_id: int, room_id: int, room_name: str) -> None:
         """编辑房间
 
         参数:
             villa_id: 大别野 ID
             room_id: 房间 ID
             room_name: 房间名称
@@ -1107,14 +1069,22 @@
 
         return MessageContentInfo(
             content=content,
             mentionedInfo=mentioned,
             quote=quote,
         )
 
+    def init_app(self, app: FastAPI):
+        logger.opt(colors=True).info(f"Initializing Bot <m>{self.bot_id}</m>...")
+        logger.opt(colors=True).debug(
+            f"With Secret: <m>{self.bot_secret}</m> and Callback URL: <m>{self.callback_url}</m>"
+        )
+        app.post(self.callback_url, status_code=200)(handle_event)
+        app.on_event("shutdown")(self._close_client)
+
     def run(
         self,
         host: str = "127.0.0.1",
         port: int = 13350,
         log_level: str = "INFO",
         **kwargs,
     ):
@@ -1151,20 +1121,15 @@
     uvicorn_kwargs = {
         k.lstrip("uvicorn_"): v for k, v in kwargs.items() if k.startswith("uvicorn_")
     }
     app = get_app()
     for key, value in fastapi_kwargs.items():
         setattr(app, key, value)
     for bot in bots:
-        logger.opt(colors=True).info(f"Initializing Bot <m>{bot.bot_id}</m>...")
-        logger.opt(colors=True).debug(
-            f"With Secret: <m>{bot.bot_secret}</m> and Callback URL: <m>{bot.callback_url}</m>"
-        )
-        app.post(bot.callback_url, status_code=200)(handle_event)
-        app.on_event("shutdown")(bot._close_client)
+        bot.init_app(app)
     uvicorn.run(
         app,
         host=host,
         port=port,
         log_config={
             "version": 1,
             "disable_existing_loggers": False,
@@ -1181,55 +1146,38 @@
                 },
             },
         },
         **uvicorn_kwargs,
     )
 
 
-async def handle_event(data: dict) -> JSONResponse:
+async def handle_event(data: Dict[str, Any]) -> JSONResponse:
     """处理事件"""
     if not (payload_data := data.get("event", None)):
         logger.warning(f"Received invalid data: {escape_tag(str(data))}")
         return JSONResponse(
             status_code=400, content={"retcode": -1, "msg": "Invalid data"}
         )
     try:
-        payload = Payload.parse_obj(payload_data)
+        event = parse_obj_as(event_classes, pre_handle_event(payload_data))
+        if (bot := get_bot(event.bot_id)) is None:
+            raise ValueError(f"Bot {event.bot_id} not found")
+        bot._bot_info = event.robot
+        logger.opt(colors=True).success(
+            f"<b><m>{bot.bot_id}</m></b> | <b><y>[{event.__class__.__name__}]</y></b>: {event.get_event_description()}"
+        )
     except Exception as e:
         logger.opt(exception=e).warning(
             f"Failed to parse payload {escape_tag(str(payload_data))}"
         )
         return JSONResponse(
             status_code=400, content={"retcode": -1, "msg": "Invalid data"}
         )
-    logger.trace(f"Received payload {escape_tag(repr(payload))}")
-    if (bot := get_bot(payload.robot.template.id)) is None:
-        raise ValueError(f"Bot {payload.robot.template.id} not found")
-    bot.bot_info = payload.robot
-    if (event_class := event_classes.get(payload.type, None)) and (
-        event_class.__type__.name in payload.extend_data["EventData"]
-    ):
-        try:
-            event = event_class.parse_obj(
-                payload.extend_data["EventData"][event_class.__type__.name]
-            )
-            logger.opt(colors=True).success(
-                f"<b><m>{bot.bot_id}</m></b> | <b><y>[{event.__class__.__name__}]</y></b>: {escape_tag(str(event.dict()))}"
-            )
-        except Exception as e:
-            logger.opt(exception=e).warning(
-                f"Failed to parse event {escape_tag(str(payload.extend_data['EventData']))} to {event_class.__name__}"
-            )
-        else:
-            asyncio.create_task(bot._handle_event(event))
     else:
-        logger.warning(
-            f"Unknown event type: {payload.type} data={escape_tag(str(payload.extend_data))}"
-        )
-
+        asyncio.create_task(bot._handle_event(event))
     return JSONResponse(status_code=200, content={"retcode": 0, "message": "success"})
 
 
 async def run_handler(handler: EventHandler, event: Event):
     """运行事件处理器"""
     try:
         if asyncio.iscoroutinefunction(handler.func):
```

### Comparing `villa-0.3.0/villa/log.py` & `villa-0.4.0/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.3.0/villa/message.py` & `villa-0.4.0/villa/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,81 +84,81 @@
     def __iadd__(self, other: Union[str, "MessageSegment", "Message"]) -> "Message":
         return self.__add__(other)
 
 
 class Text(MessageSegment):
     """文本消息段"""
 
-    type: Literal["text"] = "text"
+    type: Literal["text"] = Field(default="text", repr=False)
     content: str
 
 
 class MentionRobot(MessageSegment):
     """@机器人消息段"""
 
-    type: Literal["mention_robot"] = "mention_robot"
+    type: Literal["mention_robot"] = Field(default="mention_robot", repr=False)
     bot_id: str
     bot_name: str
 
 
 class MentionUser(MessageSegment):
     """@用户消息段"""
 
-    type: Literal["mention_user"] = "mention_user"
+    type: Literal["mention_user"] = Field(default="mention_user", repr=False)
     villa_id: int
     user_id: int
 
 
 class MentionAll(MessageSegment):
     """@全体成员消息段"""
 
-    type: Literal["mention_all"] = "mention_all"
+    type: Literal["mention_all"] = Field(default="mention_all", repr=False)
     show_text: str = "全体成员"
 
 
 class RoomLink(MessageSegment):
     """房间链接消息段"""
 
-    type: Literal["room_link"] = "room_link"
+    type: Literal["room_link"] = Field(default="room_link", repr=False)
     villa_id: int
     room_id: int
 
 
 class Link(MessageSegment):
     """链接消息段"""
 
-    type: Literal["link"] = "link"
+    type: Literal["link"] = Field(default="link", repr=False)
     url: str
     show_text: str
 
 
 class Image(MessageSegment):
     """图片消息段"""
 
-    type: Literal["image"] = "image"
+    type: Literal["image"] = Field(default="image", repr=False)
     url: str
     width: Optional[int] = None
     height: Optional[int] = None
     file_size: Optional[int] = None
 
 
 class Quote(MessageSegment):
     """引用消息段"""
 
-    type: Literal["quote"] = "quote"
+    type: Literal["quote"] = Field(default="quote", repr=False)
     quoted_message_id: str
     quoted_message_send_time: int
     original_message_id: str
     original_message_send_time: int
 
 
 class Post(MessageSegment):
     """帖子消息段"""
 
-    type: Literal["post"] = "post"
+    type: Literal["post"] = Field(default="post", repr=False)
     post_id: str
 
 
 class Message(BaseModel):
     __root__: List[MessageSegment] = Field(default_factory=list)
 
     def __init__(
@@ -387,14 +387,17 @@
         else:
             raise TypeError(f"unsupported type: {type(other)}")
         return self
 
     def __iter__(self) -> Iterator[MessageSegment]:
         return iter(self.__root__)
 
+    def __repr__(self) -> str:
+        return f"Message({repr(self.__root__)})"
+
     def has_segment_type(self, segment_type: MessageType) -> bool:
         """判断消息是否包含指定类型的消息段
 
         参数:
             segment_type: 消息段类型
 
         返回:
```

### Comparing `villa-0.3.0/villa/models.py` & `villa-0.4.0/villa/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import json
 import inspect
 from enum import Enum, IntEnum
 from typing import Any, List, Union, Literal, Optional
 
-from pydantic import Field, BaseModel, validator, root_validator
+from pydantic import Field, BaseModel, validator
 
 
 class ApiResponse(BaseModel):
     retcode: int
     message: str
     data: Any
 
@@ -16,69 +16,30 @@
 class BotAuth(BaseModel):
     bot_id: str
     bot_secret: str
 
 
 # http事件回调部分
 # see https://webstatic.mihoyo.com/vila/bot/doc/callback.html
-class RobotCommand(BaseModel):
+class Command(BaseModel):
     name: str
     desc: str
 
 
-class RobotTemplate(BaseModel):
+class Template(BaseModel):
     id: str
     name: str
     desc: str
     icon: str
-    commands: Optional[List[RobotCommand]] = None
+    commands: Optional[List[Command]] = None
 
 
 class Robot(BaseModel):
     villa_id: int
-    template: RobotTemplate
-
-
-class Payload(BaseModel):
-    robot: Robot
-    type: int
-    id: str
-    created_at: int
-    send_at: int
-    extend_data: dict
-
-    @root_validator(pre=True)
-    def _add_villa_id_to_extend_data(cls, values: dict):
-        """把villa_id和bot_id添加到extend_data中，方便使用"""
-        if values.get("type") == 2 and "SendMessage" in values.get(
-            "extend_data", {}
-        ).get("EventData", {}):
-            if isinstance(
-                values["extend_data"]["EventData"]["SendMessage"]["content"], str
-            ):
-                values["extend_data"]["EventData"]["SendMessage"][
-                    "content"
-                ] = json.loads(
-                    values["extend_data"]["EventData"]["SendMessage"]["content"]
-                )
-            if (
-                "villa_id" in values.get("robot", {})
-                and "villa_id" not in values["extend_data"]["EventData"]["SendMessage"]
-            ):
-                values["extend_data"]["EventData"]["SendMessage"]["villa_id"] = values[
-                    "robot"
-                ]["villa_id"]
-            if (
-                "id" in values.get("robot", {}).get("template", {})
-                and "bot_id" not in values["extend_data"]["EventData"]["SendMessage"]
-            ):
-                values["extend_data"]["EventData"]["SendMessage"]["bot_id"] = values[
-                    "robot"
-                ]["template"]["id"]
-        return values
+    template: Template
 
 
 ## 鉴权部分
 ## see https://webstatic.mihoyo.com/vila/bot/doc/auth_api/
 class BotMemberAccessInfo(BaseModel):
     uid: int
     villa_id: int
@@ -418,18 +379,17 @@
     if inspect.isclass(obj) and issubclass(obj, BaseModel):
         obj.update_forward_refs()
 
 
 __all__ = [
     "ApiResponse",
     "BotAuth",
-    "RobotCommand",
-    "RobotTemplate",
+    "Command",
+    "Template",
     "Robot",
-    "Payload",
     "BotMemberAccessInfo",
     "CheckMemberBotAccessTokenReturn",
     "Villa",
     "MemberBasic",
     "Member",
     "MemberListReturn",
     "MentionType",
```

### Comparing `villa-0.3.0/villa/store.py` & `villa-0.4.0/villa/store.py`

 * *Files identical despite different names*

### Comparing `villa-0.3.0/villa/typing.py` & `villa-0.4.0/villa/typing.py`

 * *Files identical despite different names*

### Comparing `villa-0.3.0/villa/utils.py` & `villa-0.4.0/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.3.0/PKG-INFO` & `villa-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.3.0
+Version: 0.4.0
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

