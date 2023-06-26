# Comparing `tmp/nonebot_adapter_villa-0.2.1.tar.gz` & `tmp/nonebot_adapter_villa-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.3.0.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.2.1.tar` & `nonebot_adapter_villa-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1062 2023-06-17 08:49:37.971137 nonebot_adapter_villa-0.2.1/LICENSE
--rw-r--r--   0        0        0     5070 2023-06-17 08:49:37.971137 nonebot_adapter_villa-0.2.1/README.md
--rw-r--r--   0        0        0      235 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0     5056 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     2905 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     3714 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    12434 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0    10411 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    12230 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      263 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0     8936 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     6704 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-06-17 08:49:37.975137 nonebot_adapter_villa-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5070 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/README.md
+-rw-r--r--   0        0        0      235 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0     4633 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     2905 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     3714 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    12434 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     8899 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    12220 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      263 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    11641 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     6704 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0       76 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-06-26 13:03:15.079872 nonebot_adapter_villa-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.3.0/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.2.1/LICENSE` & `nonebot_adapter_villa-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.1/README.md` & `nonebot_adapter_villa-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import asyncio
 from typing import Any, cast
 
+from pydantic import parse_obj_as
 from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 from nonebot.drivers import (
     URL,
     Driver,
     Request,
     Response,
@@ -15,17 +16,17 @@
 )
 
 from nonebot.adapters import Adapter as BaseAdapter
 
 from .bot import Bot
 from .utils import log
 from .config import Config
-from .event import event_classes
-from .api import API_HANDLERS, Payload
+from .api import API_HANDLERS
 from .exception import ApiNotAvailable
+from .event import event_classes, pre_handle_event
 
 
 class Adapter(BaseAdapter):
     @overrides(BaseAdapter)
     def __init__(self, driver: Driver, **kwargs: Any):
         super().__init__(driver, **kwargs)
         self.villa_config: Config = Config(**self.config.dict())
@@ -57,64 +58,52 @@
             )
             self.setup_http_server(http_setup)
 
     async def _handle_http(self, request: Request) -> Response:
         if data := request.content:
             json_data = json.loads(data)
             if payload_data := json_data.get("event"):
-                payload = Payload.parse_obj(payload_data)
-                bot_id = payload.robot.template.id
-                if (bot := self.bots.get(bot_id, None)) is None:
-                    if (
-                        bot_secret := next(
-                            (
-                                bot.bot_secret
-                                for bot in self.villa_config.villa_bots
-                                if bot.bot_id == bot_id
-                            ),
-                            None,
-                        )
-                    ) is not None:
-                        bot = Bot(self, bot_id, payload.robot, bot_secret=bot_secret)
-                        self.bot_connect(bot)
-                        log("INFO", f"<y>Bot {bot.self_id} connected</y>")
-                    else:
-                        log(
-                            "WARNING",
-                            f"<r>Missing bot secret for bot {bot_id}</r>, event will not be handle",
-                        )
-                        return Response(
-                            200,
-                            content=json.dumps(
-                                {"retcode": 0, "message": "NoneBot2 Get it!"}
-                            ),
-                        )
-                bot = cast(Bot, bot)
-                bot._bot_info = payload.robot
-
-                if (event_class := event_classes.get(payload.type, None)) and (
-                    event_class.__type__.name in payload.extend_data["EventData"]
-                ):
-                    try:
-                        event = event_class.parse_obj(
-                            payload.extend_data["EventData"][event_class.__type__.name]
-                        )
-                    except Exception as e:
-                        log(
-                            "WARNING",
-                            f"Failed to parse event {escape_tag(repr(payload))}",
-                            e,
-                        )
-                    else:
-                        asyncio.create_task(bot.handle_event(event))
-                else:
+                try:
+                    event = parse_obj_as(event_classes, pre_handle_event(payload_data))
+                    bot_id = event.bot_id
+                    if (bot := self.bots.get(bot_id, None)) is None:
+                        if (
+                            bot_secret := next(
+                                (
+                                    bot.bot_secret
+                                    for bot in self.villa_config.villa_bots
+                                    if bot.bot_id == bot_id
+                                ),
+                                None,
+                            )
+                        ) is not None:
+                            bot = Bot(self, bot_id, event.robot, bot_secret=bot_secret)
+                            self.bot_connect(bot)
+                            log("INFO", f"<y>Bot {bot.self_id} connected</y>")
+                        else:
+                            log(
+                                "WARNING",
+                                f"<r>Missing bot secret for bot {bot_id}</r>, event will not be handle",
+                            )
+                            return Response(
+                                200,
+                                content=json.dumps(
+                                    {"retcode": 0, "message": "NoneBot2 Get it!"}
+                                ),
+                            )
+                    bot = cast(Bot, bot)
+                    bot._bot_info = event.robot
+                except Exception as e:
                     log(
-                        "INFO",
-                        f"Unknown event type: {payload.type} data={escape_tag(str(payload.extend_data))}",
+                        "WARNING",
+                        f"Failed to parse event {escape_tag(str(payload_data))}",
+                        e,
                     )
+                else:
+                    asyncio.create_task(bot.handle_event(event))
                 # (Path().cwd() / f'test_event_{payload.created_at}.json').write_text(json.dumps(json_data, indent=4, ensure_ascii=False), encoding='utf-8')
                 return Response(
                     200,
                     content=json.dumps({"retcode": 0, "message": "NoneBot2 Get it!"}),
                 )
             return Response(400, content="Invalid Request Body")
         return Response(400, content="Invalid Request Body")
```

### Comparing `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/cilent.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/models.py`

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

### Comparing `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from .utils import log
 from .event import Event, SendMessageEvent
 from .message import Message, MessageSegment
 from .api import (
     Link,
     Image,
     Robot,
+    Command,
     ApiClient,
     ImageSize,
     QuoteInfo,
     TextEntity,
     MentionType,
     MentionedAll,
-    RobotCommand,
     MentionedInfo,
     MentionedUser,
     VillaRoomLink,
     MentionedRobot,
     MessageContentInfo,
     PostMessageContent,
     TextMessageContent,
@@ -119,15 +119,15 @@
 
     @property
     def nickname(self) -> str:
         """Bot 昵称"""
         return self._bot_info.template.name
 
     @property
-    def commands(self) -> Optional[List[RobotCommand]]:
+    def commands(self) -> Optional[List[Command]]:
         """Bot 命令预设命令列表"""
         return self._bot_info.template.commands
 
     @property
     def description(self) -> str:
         """Bot 介绍描述"""
         return self._bot_info.template.desc
```

### Comparing `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.1/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.2.1/pyproject.toml` & `nonebot_adapter_villa-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.2.1"
+version = "0.3.0"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.2.1/PKG-INFO` & `nonebot_adapter_villa-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.2.1
+Version: 0.3.0
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.3.0 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

