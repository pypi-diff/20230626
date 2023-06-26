# Comparing `tmp/nonebot_plugin_setu_now-0.6.0b1.tar.gz` & `tmp/nonebot_plugin_setu_now-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_setu_now-0.6.0b1.tar", last modified: Mon Jun 19 12:45:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_setu_now-0.6.1.tar", last modified: Mon Jun 26 06:30:51 2023, max compression
```

## Comparing `nonebot_plugin_setu_now-0.6.0b1.tar` & `nonebot_plugin_setu_now-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/LICENSE
--rw-r--r--   0        0        0     3403 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/README.md
--rwxr-xr-x   0        0        0     7447 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/__init__.py
--rw-r--r--   0        0        0      305 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/aioutils/__init__.py
--rw-r--r--   0        0        0     3922 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/aioutils/_main.py
--rw-r--r--   0        0        0     1030 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/config.py
--rw-r--r--   0        0        0     2410 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/data_source.py
--rw-r--r--   0        0        0     1123 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/database.py
--rw-r--r--   0        0        0     4274 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/img_utils.py
--rw-r--r--   0        0        0      959 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/models.py
--rw-r--r--   0        0        0      613 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/perf_timer.py
--rw-r--r--   0        0        0     1711 2023-06-19 12:45:37.655352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/r18_whitelist.py
--rw-r--r--   0        0        0     3031 2023-06-19 12:45:37.659352 nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/utils.py
--rw-r--r--   0        0        0      806 2023-06-19 12:45:51.367339 nonebot_plugin_setu_now-0.6.0b1/pyproject.toml
--rw-r--r--   0        0        0     4035 1970-01-01 00:00:00.000000 nonebot_plugin_setu_now-0.6.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3403 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/README.md
+-rwxr-xr-x   0        0        0     7467 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/aioutils/__init__.py
+-rw-r--r--   0        0        0     3922 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/aioutils/_main.py
+-rw-r--r--   0        0        0     1030 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/config.py
+-rw-r--r--   0        0        0     2340 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/data_source.py
+-rw-r--r--   0        0        0     1047 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/database.py
+-rw-r--r--   0        0        0     4262 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/img_utils.py
+-rw-r--r--   0        0        0      959 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/models.py
+-rw-r--r--   0        0        0      613 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/perf_timer.py
+-rw-r--r--   0        0        0     1640 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/r18_whitelist.py
+-rw-r--r--   0        0        0     2964 2023-06-26 06:30:41.863849 nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/utils.py
+-rw-r--r--   0        0        0      799 2023-06-26 06:30:51.727846 nonebot_plugin_setu_now-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4033 1970-01-01 00:00:00.000000 nonebot_plugin_setu_now-0.6.1/PKG-INFO
```

### Comparing `nonebot_plugin_setu_now-0.6.0b1/LICENSE` & `nonebot_plugin_setu_now-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.0b1/README.md` & `nonebot_plugin_setu_now-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/__init__.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,34 @@
+from nonebot import require
+
+require("nonebot_plugin_localstore")
+require("nonebot_plugin_tortoise_orm")
+
 import asyncio
 from re import I, sub
 from typing import Any, Union, Annotated
 from pathlib import Path
 
 from PIL import UnidentifiedImageError
 from nonebot import on_regex, on_command
 from nonebot.log import logger
 from nonebot.params import Depends, RegexGroup
-from nonebot.plugin import PluginMetadata, require
+from nonebot.plugin import PluginMetadata
 from nonebot.exception import ActionFailed
 from nonebot.adapters.onebot.v11 import (
     GROUP,
     PRIVATE_FRIEND,
     Bot,
     Message,
     MessageEvent,
     MessageSegment,
     GroupMessageEvent,
     PrivateMessageEvent,
 )
+from nonebot_plugin_tortoise_orm import add_model
 from nonebot.adapters.onebot.v11.helpers import (
     Cooldown,
     CooldownIsolateLevel,
     autorevoke_send,
 )
 
 from .utils import SpeedLimiter
@@ -41,17 +47,14 @@
     description="另一个色图插件",
     usage=usage_msg,
     type="application",
     config=Config,
     extra={},
 )
 
-require("nonebot_plugin_localstore")
-require("nonebot_plugin_tortoise_orm")
-from nonebot_plugin_tortoise_orm import add_model
 
 add_model("nonebot_plugin_setu_now.database")
 
 global_speedlimiter = SpeedLimiter()
 
 setu_matcher = on_regex(
     r"^(setu|色图|涩图|来点色色|色色|涩涩|来点色图)\s?([x|✖️|×|X|*]?\d+[张|个|份]?)?\s?(r18)?\s?\s?(tag)?\s?(.*)?",
@@ -201,15 +204,14 @@
 
     if message_info := await MessageInfo.get_or_none(message_id=reply_message_id):
         message_pid = message_info.pid
     else:
         await setuinfo_matcher.finish("未找到该插画相关信息")
 
     if setu_info := await SetuInfo.get_or_none(pid=message_pid):
-
         info_message = MessageSegment.text(f"标题：{setu_info.title}\n")
         info_message += MessageSegment.text(f"画师：{setu_info.author}\n")
         info_message += MessageSegment.text(f"PID：{setu_info.pid}")
 
         await setu_matcher.finish(MessageSegment.reply(reply_message_id) + info_message)
     else:
         await setuinfo_matcher.finish("该插画相关信息已被移除")
```

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/aioutils/_main.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/aioutils/_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/config.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/data_source.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 from typing import List, Callable
 from asyncio import gather
 from pathlib import Path
 
 import nonebot_plugin_localstore as store
 from httpx import AsyncClient
-
-from nonebot import require
 from nonebot.log import logger
 
 from .utils import download_pic
 from .config import PROXY, API_URL, SETU_SIZE, REVERSE_PROXY
 from .models import Setu, SetuApiData, SetuNotFindError
 
-
-require("nonebot_plugin_tortoise_orm")
-
 CACHE_PATH = Path(store.get_cache_dir("nonebot_plugin_setu_now"))
 if not CACHE_PATH.exists():
     logger.info("Creating setu cache floder")
     CACHE_PATH.mkdir(parents=True, exist_ok=True)
 
 
 class SetuHandler:
```

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/database.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from tortoise import fields
-
-from nonebot.plugin import require
 from tortoise.models import Model
 
 from .data_source import SETU_SIZE, Setu
 
-require("nonebot_plugin_tortoise_orm")
-
 
 class SetuInfo(Model):
     pid = fields.IntField(pk=True)
     author = fields.CharField(max_length=50)
     title = fields.CharField(max_length=50)
     url = fields.TextField()
```

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/img_utils.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/img_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import time
 from io import BytesIO
 from pathlib import Path
 from random import choice, randint
 from typing import Union
 
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot.log import logger
```

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/models.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/perf_timer.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/perf_timer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/r18_whitelist.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/r18_whitelist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-from nonebot import require
-
-
 from nonebot.log import logger
 
 from nonebot.plugin.on import on_command
 from nonebot.permission import SUPERUSER
 from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent
 
 from .database import GroupWhiteListRecord
 
-require("nonebot_plugin_tortoise_orm")
-
 
 async def get_group_white_list_record(
     event: MessageEvent,
 ) -> GroupWhiteListRecord | None:
     if isinstance(event, GroupMessageEvent):
         res = await GroupWhiteListRecord.get_or_none(group_id=event.group_id)
         logger.debug(f"Database white list record: {res}")
@@ -24,15 +19,14 @@
 r18_activate_matcher = on_command(
     "开启涩涩", aliases={"可以涩涩", "开启色色", "可以色色", "r18开启"}, permission=SUPERUSER
 )
 
 
 @r18_activate_matcher.handle()
 async def _(event: GroupMessageEvent):
-
     if _ := await GroupWhiteListRecord.get_or_none(group_id=event.group_id):
         logger.debug("已有白名单记录")
 
     else:
         logger.debug(f"添加白名单 {event.group_id}")
         await GroupWhiteListRecord.create(
             group_id=event.group_id, operator_user_id=event.user_id
```

### Comparing `nonebot_plugin_setu_now-0.6.0b1/nonebot_plugin_setu_now/utils.py` & `nonebot_plugin_setu_now-0.6.1/nonebot_plugin_setu_now/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import time
 import asyncio
 from typing import List, Optional
 from pathlib import Path
 
+import nonebot_plugin_localstore as store
 from httpx import AsyncClient
-from nonebot import require
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11 import Bot, Message, GroupMessageEvent
 
 from .config import SETU_PATH, SEND_INTERVAL
 from .perf_timer import PerfTimer
 
-require("nonebot_plugin_localstore")
-
-import nonebot_plugin_localstore as store
-
 
 async def download_pic(
     url: str, proxies: Optional[str] = None, file_mode=False, file_name=""
 ) -> Optional[Path]:
     headers = {
         "Referer": "https://accounts.pixiv.net/login?lang=zh&source=pc&view_type=page&ref=wwwtop_accounts_index",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) "
```

### Comparing `nonebot_plugin_setu_now-0.6.0b1/pyproject.toml` & `nonebot_plugin_setu_now-0.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-setu-now"
-version = "0.6.0.beta.1"
+version = "0.6.1"
 description = "另一个色图插件"
 authors = [
     { name = "kexue", email = "xana278@foxmail.com" },
 ]
 dependencies = [
     "httpx<1.0.0,>=0.18.0",
     "nonebot2>=2.0.0",
```

### Comparing `nonebot_plugin_setu_now-0.6.0b1/PKG-INFO` & `nonebot_plugin_setu_now-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-setu-now
-Version: 0.6.0b1
+Version: 0.6.1
 Summary: 另一个色图插件
 Home-page: https://github.com/kexue-z/nonebot-plugin-setu-now
 Author-Email: kexue <xana278@foxmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/kexue-z/nonebot-plugin-setu-now
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx<1.0.0,>=0.18.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-setu-now Version: 0.6.0b1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-setu-now Version: 0.6.1 Summary:
 å¦ä¸ä¸ªè²å¾æä»¶ Home-page: https://github.com/kexue-z/nonebot-plugin-
 setu-now Author-Email: kexue
 foxmail.com> License: MIT Project-URL: Homepage, https://github.com/kexue-z/
 nonebot-plugin-setu-now Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx<1.0.0,>=0.18.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-
 adapter-onebot>=2.0.0 Requires-Dist: pydantic>=1.5.0 Requires-Dist:
 pillow>=8.0.0 Requires-Dist: nonebot-plugin-tortoise-orm>=0.0.1a3 Requires-
```

