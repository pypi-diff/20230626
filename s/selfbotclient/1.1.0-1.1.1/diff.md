# Comparing `tmp/selfbotclient-1.1.0.tar.gz` & `tmp/selfbotclient-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfbotclient-1.1.0.tar", last modified: Thu Jun 15 17:20:37 2023, max compression
+gzip compressed data, was "selfbotclient-1.1.1.tar", last modified: Mon Jun 26 20:55:49 2023, max compression
```

## Comparing `selfbotclient-1.1.0.tar` & `selfbotclient-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 17:20:37.132355 selfbotclient-1.1.0/
--rw-rw-rw-   0        0        0     1890 2023-06-15 17:20:37.132355 selfbotclient-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1286 2023-06-15 16:58:24.000000 selfbotclient-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 17:20:37.116356 selfbotclient-1.1.0/SelfBotClient/
--rw-rw-rw-   0        0        0      376 2023-06-14 23:07:30.000000 selfbotclient-1.1.0/SelfBotClient/__init__.py
--rw-rw-rw-   0        0        0      472 2023-06-09 23:04:28.000000 selfbotclient-1.1.0/SelfBotClient/__main__.py
--rw-rw-rw-   0        0        0    16059 2023-06-15 17:18:55.000000 selfbotclient-1.1.0/SelfBotClient/client.py
--rw-rw-rw-   0        0        0     1463 2023-06-15 15:43:34.000000 selfbotclient-1.1.0/SelfBotClient/enums.py
--rw-rw-rw-   0        0        0      795 2023-06-12 22:50:06.000000 selfbotclient-1.1.0/SelfBotClient/errors.py
--rw-rw-rw-   0        0        0    11687 2023-06-15 16:10:23.000000 selfbotclient-1.1.0/SelfBotClient/http.py
--rw-rw-rw-   0        0        0     1046 2023-06-12 22:50:54.000000 selfbotclient-1.1.0/SelfBotClient/logger.py
--rw-rw-rw-   0        0        0      609 2023-06-15 15:59:48.000000 selfbotclient-1.1.0/SelfBotClient/permissionbuilder.py
--rw-rw-rw-   0        0        0     2713 2023-06-15 16:38:57.000000 selfbotclient-1.1.0/SelfBotClient/thread.py
--rw-rw-rw-   0        0        0      313 2023-06-15 01:26:01.000000 selfbotclient-1.1.0/SelfBotClient/typings.py
--rw-rw-rw-   0        0        0    18892 2023-06-15 17:17:27.000000 selfbotclient-1.1.0/SelfBotClient/user.py
-drwxrwxrwx   0        0        0        0 2023-06-15 17:20:37.131355 selfbotclient-1.1.0/selfbotclient.egg-info/
--rw-rw-rw-   0        0        0     1890 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-15 17:20:37.000000 selfbotclient-1.1.0/selfbotclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 17:20:37.132355 selfbotclient-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-06-15 17:20:36.000000 selfbotclient-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:55:49.802049 selfbotclient-1.1.1/
+-rw-rw-rw-   0        0        0     1890 2023-06-26 20:55:49.801049 selfbotclient-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1286 2023-06-15 16:58:24.000000 selfbotclient-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 20:55:49.792048 selfbotclient-1.1.1/SelfBotClient/
+-rw-rw-rw-   0        0        0      376 2023-06-14 23:07:30.000000 selfbotclient-1.1.1/SelfBotClient/__init__.py
+-rw-rw-rw-   0        0        0      470 2023-06-26 18:51:57.000000 selfbotclient-1.1.1/SelfBotClient/__main__.py
+-rw-rw-rw-   0        0        0    16137 2023-06-26 20:29:08.000000 selfbotclient-1.1.1/SelfBotClient/client.py
+-rw-rw-rw-   0        0        0     1294 2023-06-26 20:40:47.000000 selfbotclient-1.1.1/SelfBotClient/enums.py
+-rw-rw-rw-   0        0        0      795 2023-06-12 22:50:06.000000 selfbotclient-1.1.1/SelfBotClient/errors.py
+-rw-rw-rw-   0        0        0     8935 2023-06-26 20:27:53.000000 selfbotclient-1.1.1/SelfBotClient/http.py
+-rw-rw-rw-   0        0        0      868 2023-06-26 20:12:17.000000 selfbotclient-1.1.1/SelfBotClient/logger.py
+-rw-rw-rw-   0        0        0      593 2023-06-26 19:03:42.000000 selfbotclient-1.1.1/SelfBotClient/permissionbuilder.py
+-rw-rw-rw-   0        0        0     2711 2023-06-26 20:51:01.000000 selfbotclient-1.1.1/SelfBotClient/tasks.py
+-rw-rw-rw-   0        0        0      313 2023-06-15 01:26:01.000000 selfbotclient-1.1.1/SelfBotClient/typings.py
+-rw-rw-rw-   0        0        0    19115 2023-06-26 20:11:10.000000 selfbotclient-1.1.1/SelfBotClient/user.py
+-rw-rw-rw-   0        0        0      294 2023-06-26 20:43:58.000000 selfbotclient-1.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-26 20:55:49.801049 selfbotclient-1.1.1/selfbotclient.egg-info/
+-rw-rw-rw-   0        0        0     1890 2023-06-26 20:55:49.000000 selfbotclient-1.1.1/selfbotclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-06-26 20:55:49.000000 selfbotclient-1.1.1/selfbotclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:55:49.000000 selfbotclient-1.1.1/selfbotclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-26 20:55:49.000000 selfbotclient-1.1.1/selfbotclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 20:55:49.000000 selfbotclient-1.1.1/selfbotclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:55:49.802049 selfbotclient-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-06-26 20:55:48.000000 selfbotclient-1.1.1/setup.py
```

### Comparing `selfbotclient-1.1.0/PKG-INFO` & `selfbotclient-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfbotclient
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library that will allow you to manage selfbots
 Author: xXenvy
 Author-email: <xpimepk01@gmail.com>
 Keywords: python,requests,discord selfbot,selfbot,discord.py,aiohttp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `selfbotclient-1.1.0/README.md` & `selfbotclient-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.1.0/SelfBotClient/client.py` & `selfbotclient-1.1.1/SelfBotClient/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 from .http import HTTPClient
 from .typings import API_VERSION, ClientResponse, RGB_COLOR
 from .enums import ChannelType
 from .permissionbuilder import PermissionBuilder
-from .thread import Thread
+from .tasks import Tasks
 
 from collections.abc import AsyncIterable
 
-from typing import Union
+from typing import Union, Optional
 from asyncio import AbstractEventLoop
 
 
 class Client(HTTPClient):
     """
     :class:`Client` supports all services of the :class:`SelfBotClient.user`.
     It has methods such as :class:`Client.send_message` which it calls in all users.
 
     :param api_version: version of the discord api used by the client
     :param loop: Set the event loop that will be used by the client
     :param logger: Enable/disable the logger
     :param request_latency: Control the rate of requests sent to discord
     :param ratelimit_additional_cooldown: Add a cooldown to the ratelimit
-    :param use_threading: Enable or disable the threading option (:class:`SelfBotClient.thread`), which for now is in beta.
+    :param use_tasks: Enable or disable the tasks option (:class:`SelfBotClient.tasks`), which for now is in beta.
 
     """
 
-    __version__: str = "1.1.0"
+    __version__: str = "1.1.1"
 
     def __init__(
             self,
             api_version: API_VERSION,
-            loop: AbstractEventLoop = None,
+            loop: Union[AbstractEventLoop, None] = None,
             logger: bool = True,
             request_latency: float = 0.1,
             ratelimit_additional_cooldown: float = 10,
             use_threading: bool = False
-    ):
+    ):  # type: ignore
 
         super().__init__(api_version, loop, logger, request_latency, ratelimit_additional_cooldown)
 
         if use_threading:
-            self.thread: Thread = Thread(client=self)
+            self.tasks: Tasks = Tasks(client=self)
 
-    def login(self, token: Union[str, list[str]]) -> None:
+    def login(self, tokens: Union[str, list[str]]) -> None:
         """
         The login function is used to check the provided tokens.
 
-        :param token: tokens to check
+        :param tokens: tokens to check
         """
 
-        if self.logger._status:
+        if self.logger._status:  # pyright: ignore
             self.logger.info("Checking the provided tokens")
 
-        self._tokens: Union[str, list[str]] = token
-        self._check_tokens()
+        self._check_tokens(tokens)
 
-    async def send_message(self, channel_id: int, message_content: str) -> Union[None, AsyncIterable[ClientResponse]]:
+    async def send_message(self, channel_id: int, message_content: str) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The send_message function sends a message to the specified channel.
 
         :param channel_id: Specify the channel to send the message to
         :param message_content: content of the message
         """
 
@@ -74,30 +73,31 @@
         """
 
         for user in self.users:
             response: ClientResponse = await user.delete_channel(channel_id)
             if response.status == 200:
                 return response
 
-    async def delete_channels(self, channel_ids: list[int]) -> Union[None, AsyncIterable[ClientResponse]]:
+    async def delete_channels(self, channel_ids: list[int]) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The delete_channels function takes a list of channel_ids and deletes them.
         It returns an AsyncIterable of ClientResponse objects, which can be used to check the status code for each request.
 
         :param channel_ids: Specify the list of channel ids that will be deleted
         """
 
         while len(channel_ids):
             for user in self.users:
                 channel_id: int = channel_ids.pop(0)
                 response: ClientResponse = await user.delete_channel(channel_id)
                 yield response
 
     async def create_channel(self, guild_id: int, name: str, channel_type: ChannelType,
-                             topic: str = None, user_limit: int = None, position: int = None, nsfw: bool = False) -> Union[None, AsyncIterable[ClientResponse]]:
+                             topic: Optional[str] = None, user_limit: Optional[int] = None,
+                             position: Optional[int] = None, nsfw: Optional[bool] = False) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The create_channel function creates a channel in the specified guild.
 
         :param guild_id: Specify the guild id of the server you want to create a channel in
         :param name: Specify the name of the channel
         :param channel_type: Specify what type of channel you want to create
         :param topic: Set the topic of the channel
@@ -106,32 +106,32 @@
         :param nsfw: Determine whether the channel is nsfw or not
         """
 
         for user in self.users:
             response: ClientResponse = await user.create_channel(guild_id, name, channel_type, topic, user_limit, position, nsfw)
             yield response
 
-    async def get_channels(self, guild_id: int) -> Union[None, AsyncIterable[ClientResponse]]:
+    async def get_channels(self, guild_id: int) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The get_channels function is a coroutine that takes in a guild_id and returns an AsyncIterable of ClientResponse objects.
         The function can return the data of all channels on the server
 
         :param guild_id: Specify the guild id of the server you want to get channels from
         """
 
         for user in self.users:
             response: ClientResponse = await user.get_channels(guild_id)
             yield response
 
     async def create_role(self,
                                 guild_id: int,
                                 name: str,
-                                color: RGB_COLOR = None,
-                                hoist: bool = False,
-                                permissions: PermissionBuilder = None) -> Union[None, AsyncIterable[ClientResponse]]:
+                                color: Optional[RGB_COLOR] = None,
+                                hoist: Optional[bool] = False,
+                                permissions: Optional[PermissionBuilder] = None) -> Optional[AsyncIterable[ClientResponse]]:
         """
         The create_role function creates a role in the specified guild.
 
         :param guild_id: Specify the guild in which you want to create a role
         :param name: Set the name of the role
         :param color: Set the color of the role
         :param hoist: Determine whether the role should be displayed separately in the user list
@@ -269,16 +269,16 @@
 
     async def kick_members(self, guild_id: int, user_ids: list[int]) -> Union[None, AsyncIterable[ClientResponse]]:
         """
         The kick_members function is a coroutine that takes in a guild_id and user_ids list.
         It then iterates through the users list, popping off the first user id from the
         user_ids list and kicking them from the specified guild. It yields each response as it goes.
 
-        :param guild_id: int: Specify which guild the user is in
-        :param user_ids: list[int]: list with id of people to kick out
+        :param guild_id: Specify which guild the user is in
+        :param user_ids: list with id of people to kick out
         """
 
         while len(user_ids):
             for user in self.users:
                 user_id: int = user_ids.pop(0)
                 response: ClientResponse = await user.kick_member(guild_id, user_id)
                 yield response
@@ -293,17 +293,17 @@
 
         for user in self.users:
             response: ClientResponse = await user.get_member(guild_id, user_id)
             if response.status == 200:
                 return response
 
     async def edit_member(self, guild_id: int, user_id: int,
-                                                                nickname: str = None,
-                                                                add_roles: list[int] = None,
-                                                                remove_roles: list[int] = None) -> Union[None, ClientResponse]:
+                                                                nickname: Optional[str] = None,
+                                                                add_roles: Optional[list[int]] = None,
+                                                                remove_roles: Optional[list[int]] = None) -> Union[None, ClientResponse]:
 
         """
         The edit_member function allows you to edit a member of a guild.
 
         :param guild_id: Specify the guild that you want to edit a member in
         :param user_id: Specify the user that you want to edit
         :param nickname: Change the nickname of a user in a guild
@@ -345,17 +345,17 @@
             if response.status == 204:
                 return response
 
     async def delete_reaction(self, channel_id: int, message_id: int, user_id: int, emoji: str) -> Union[None, ClientResponse]:
         """
         The delete_reaction function is used to delete a reaction from a message.
 
-        :param channel_id: int: Specify the channel where the message is located
-        :param message_id: int: Identify the message that you want to delete a reaction from
-        :param user_id: int: Specify the user whose reaction is to be deleted
-        :param emoji: str: Specify the emoji to be deleted
+        :param channel_id: Specify the channel where the message is located
+        :param message_id: Identify the message that you want to delete a reaction from
+        :param user_id: Specify the user whose reaction is to be deleted
+        :param emoji: Specify the emoji to be deleted
         """
 
         for user in self.users:
             response: ClientResponse = await user.delete_reaction(channel_id, message_id, user_id, emoji)
             if response.status == 204:
                 return response
```

### Comparing `selfbotclient-1.1.0/SelfBotClient/enums.py` & `selfbotclient-1.1.1/SelfBotClient/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from enum import Enum
 
 
 __all__: tuple = ("ChannelType", "Permissions", "Discord")
 
 
-class Discord(Enum):
-    ENDPOINT: str = "https://discord.com/api/v{}/"
+class Discord(Enum, str):
+    ENDPOINT = "https://discord.com/api/v{}/"
 
 
-class ChannelType(Enum):
+class ChannelType(Enum, int):
 
-    TEXT_CHANNEL: int = 0
-    VOICE_CHANNEL: int = 2
-    CATEGORY_CHANNEL: int = 4
-
-
-class Permissions(Enum):
-    CREATE_INSTANT_INVITE: int = 1 << 0
-    KICK_MEMBERS: int = 1 << 1
-    BAN_MEMBERS: int = 1 << 2
-    ADMINISTRATOR: int = 1 << 3
-    MANAGE_CHANNELS: int = 1 << 4
-    MANAGE_GUILD: int = 1 << 5
-    ADD_REACTIONS: int = 1 << 6
-    VIEW_AUDIT_LOG: int = 1 << 7
-    PRIORITY_SPEAKER: int = 1 << 8
-    STREAM: int = 1 << 9
-    VIEW_CHANNEL: int = 1 << 10
-    SEND_MESSAGES: int = 1 << 11
-    SEND_TTS_MESSAGES: int = 1 << 12
-    MANAGE_MESSAGES: int = 1 << 13
-    EMBED_LINKS: int = 1 << 14
-    ATTACH_FILES: int = 1 << 15
-    READ_MESSAGE_HISTORY: int = 1 << 16
-    MENTION_EVERYONE: int = 1 << 17
-    USE_EXTERNAL_EMOJIS: int = 1 << 18
-    VIEW_GUILD_INSIGHTS: int = 1 << 19
-    CONNECT: int = 1 << 20
-    SPEAK: int = 1 << 21
-    MUTE_MEMBERS: int = 1 << 22
-    DEAFEN_MEMBERS: int = 1 << 23
-    MOVE_MEMBERS: int = 1 << 24
-    CHANGE_NICKNAME: int = 1 << 26
-    MANAGE_NICKNAMES: int = 1 << 27
-    MANAGE_ROLES: int = 1 << 28
-    MANAGE_WEBHOOKS: int = 1 << 29
-    MANAGE_THREADS: int = 1 << 34
-    CREATE_PUBLIC_THREADS: int = 1 << 35
-    CREATE_PRIVATE_THREADS: int = 1 << 36
-    MODERATE_MEMBERSL: int = 1 << 40
+    TEXT_CHANNEL = 0
+    VOICE_CHANNEL = 2
+    CATEGORY_CHANNEL = 4
+
+
+class Permissions(Enum, int):
+    CREATE_INSTANT_INVITE = 1 << 0
+    KICK_MEMBERS = 1 << 1
+    BAN_MEMBERS = 1 << 2
+    ADMINISTRATOR = 1 << 3
+    MANAGE_CHANNELS = 1 << 4
+    MANAGE_GUILD = 1 << 5
+    ADD_REACTIONS = 1 << 6
+    VIEW_AUDIT_LOG = 1 << 7
+    PRIORITY_SPEAKER = 1 << 8
+    STREAM = 1 << 9
+    VIEW_CHANNEL = 1 << 10
+    SEND_MESSAGES = 1 << 11
+    SEND_TTS_MESSAGES = 1 << 12
+    MANAGE_MESSAGES = 1 << 13
+    EMBED_LINKS = 1 << 14
+    ATTACH_FILES = 1 << 15
+    READ_MESSAGE_HISTORY = 1 << 16
+    MENTION_EVERYONE = 1 << 17
+    USE_EXTERNAL_EMOJIS = 1 << 18
+    VIEW_GUILD_INSIGHTS = 1 << 19
+    CONNECT = 1 << 20
+    SPEAK = 1 << 21
+    MUTE_MEMBERS = 1 << 22
+    DEAFEN_MEMBERS = 1 << 23
+    MOVE_MEMBERS = 1 << 24
+    CHANGE_NICKNAME = 1 << 26
+    MANAGE_NICKNAMES = 1 << 27
+    MANAGE_ROLES = 1 << 28
+    MANAGE_WEBHOOKS = 1 << 29
+    MANAGE_THREADS = 1 << 34
+    CREATE_PUBLIC_THREADS = 1 << 35
+    CREATE_PRIVATE_THREADS = 1 << 36
+    MODERATE_MEMBERS = 1 << 40
```

### Comparing `selfbotclient-1.1.0/SelfBotClient/errors.py` & `selfbotclient-1.1.1/SelfBotClient/errors.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.1.0/SelfBotClient/http.py` & `selfbotclient-1.1.1/SelfBotClient/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,90 @@
 from .typings import API_VERSION, AUTH_HEADER, METHOD
 from .errors import UnSupportedApiVersion, UnSupportedTokenType, InvalidMethodType
 from .enums import Discord
 from .logger import Logger
 from .user import UserClient
 
-from typing import Union, Awaitable, Any
+from typing import Union, Awaitable, Any, Optional
 from aiohttp import ClientSession, ClientResponse, client_exceptions
 from asyncio import AbstractEventLoop, sleep, get_event_loop
 
-
 __all__: tuple[str, ...] = ("HTTPClient", "ClientResponse")
 
 
 class CustomSession(ClientSession):
 
     def __init__(self, logger: Logger, *args: Any, **kwargs: Any):
         """
-        The __init__ function is called when the class is instantiated.
-        It sets up all of the variables that are needed for other functions to work properly.
+        The __init__ function sets up all of the variables that are needed for other functions to work properly.
         The super() function calls __init__ from the parent class, which in this case is ClientSession.
 
-        :param self: Represent the instance of the class
-        :param logger: Logger: Pass the logger object to the class
-        :param *args: Any: Pass any additional arguments to the superclass
-        :param **kwargs: Any: Pass in additional parameters that are not explicitly defined
-        :return: None
+        :param logger: Pass the logger object to the class
+        :param *args: Pass any additional arguments to the superclass
+        :param **kwargs: Pass in additional parameters that are not explicitly defined
         """
 
         self.logger: Logger = logger
         self.logger_status = logger._status
 
-        self.request_latency: float = kwargs.get("latency")
-        self.ratelimit_additional_cooldown: float = kwargs.get("additional_cooldown")
-        self.users: list[UserClient] = kwargs.get("users")
+        self.request_latency: float = kwargs["latency"]
+        self.ratelimit_additional_cooldown: float = kwargs["additional_cooldown"]
+        self.users: Optional[list[UserClient]] = kwargs.get("users")
 
         del kwargs["latency"]
         del kwargs["users"]
         del kwargs["additional_cooldown"]
 
         super().__init__(*args, **kwargs)
 
     async def request(self, method: str, url: str, **kwargs: Any) -> ClientResponse:
         """
         The request function is a wrapper around the ClientSession.request function,
         which handles ratelimits and other exceptions that may occur during requests.
         It also adds an additional cooldown to the Retry-After header value.
 
-        :param self: Represent the instance of the class
-        :param method: str: Determine the type of request
-        :param url: str: Specify the url that you want to make a request to
-        :param **kwargs: Any: Pass in additional parameters to the request function
-        :return: A clientresponse object
+        :param method: Determine the type of request
+        :param url: Specify the url that you want to make a request to
+        :param **kwargs: Pass in additional parameters to the request function
         """
 
         response = await super().request(method=method, url=url, **kwargs)
+        headers: Optional[dict] = kwargs.get("headers")
 
-        headers: dict = kwargs.get("headers")
+        token: Optional[str] = None  # pyright: ignore
         if headers:
-            token: str = headers.get("authorization")
+            token: Optional[str] = headers.get("authorization")
 
-        if response and headers:
+        if response and token:
             try:
                 _json: dict = await response.json()
             except client_exceptions.ContentTypeError:
                 _json: dict = {}
-            if isinstance(_json, dict) and _json.get("message"):
-                if "You need to verify" in _json.get("message"):
-                    for user in self.users:
-                        if user.token == token:
-                            self.logger.error(f"It seems that your account has been blocked.\n-> Account: {user}")
-                    response.status = 901
+
+            message: Optional[str] = _json.get("message")
+            if isinstance(_json, dict) and message:
+                if "You need to verify" in message:
+                    if self.users:
+                        for user in self.users:
+                            if user.token == token:
+                                self.logger.error(f"It seems that your account has been blocked.\n-> Account: {user}")
+                        response.status = 901
 
         if response.headers.get("Retry-After"):
 
-            seconds = int(response.headers.get("Retry-After")) + self.ratelimit_additional_cooldown
+            seconds = int(response.headers.get("Retry-After")) + self.ratelimit_additional_cooldown  # pyright: ignore
             if self.logger_status:
                 self.logger.warning(f"Ratelimit has been reached. Awaiting {seconds} seconds before next request.")
 
             await sleep(seconds)
         else:
             await sleep(self.request_latency)
 
         return response
 
-    async def get(self, url: str, *, allow_redirects: bool = True, **kwargs: Any) -> ClientResponse:
-        """
-        The get function is a wrapper for the get function in the ClientSession class.
-        It allows us to use asyncio's await syntax, which makes it easier to write asynchronous code.
-        The get function takes a url and returns an object of type ClientResponse.
-
-        :param self: Represent the instance of the class
-        :param url: str: Specify the url to be requested
-        :param *: Unpack the tuple and the ** parameter is used to unpack the dictionary
-        :param allow_redirects: bool: Determine whether the client will follow redirects
-        :param **kwargs: Any: Pass in any additional parameters that are not specified
-        :return: A clientresponse object
-        """
-
-        response = await super().get(url=url, allow_redirects=allow_redirects, **kwargs)
-        return response
-
 
 class HTTPClient:
     """
     HTTPClient handles all requests related to the client.
     It also has methods from checking tokens or creating a new session.
 
     :param api_version: version of the discord api used by the client
@@ -112,153 +93,125 @@
     :param request_latency: Control the rate of requests sent to discord
     :param ratelimit_additional_cooldown: Add a cooldown to the ratelimit
     """
 
     def __init__(
             self,
             api_version: API_VERSION,
-            loop: AbstractEventLoop = None,
-            logger: bool = True,
-            request_latency: float = 0.1,
-            ratelimit_additional_cooldown: float = 10
+            loop: Union[AbstractEventLoop, None],
+            logger: bool,
+            request_latency: float,
+            ratelimit_additional_cooldown: float
 
     ):
 
         if api_version not in (9, 10):
             raise UnSupportedApiVersion
 
         self.request_latency: float = request_latency
         self.ratelimit_additional_cooldown: float = ratelimit_additional_cooldown
 
         self.api_version: int = api_version
         self.endpoint: str = Discord.ENDPOINT.value.format(self.api_version)
-        self.loop: AbstractEventLoop = loop if loop else get_event_loop()
+
+        if not loop:
+            self.loop: AbstractEventLoop = get_event_loop()
+        else:
+            self.loop: AbstractEventLoop = loop
 
         self._tokens: Union[str, list, None] = None
         self._logger_status: bool = logger
 
-        self.logger: Logger = Logger().logger
+        self.logger: Logger.logger = Logger().logger  # pyright: ignore
         self.logger._status = self._logger_status
-        self.session: Union[CustomSession, None] = None
+        self.session: Union[CustomSession, None] = None  # pyright: ignore
 
         self.users: list[UserClient] = []
         self.loop.run_until_complete(self.create_session())
 
     async def create_session(self) -> None:
         """
-        The create_session function is used to create a new session for the bot.
-        This function is called when the bot starts up, and also when it needs to reconnect.
-        The session object contains all of the information about how many requests have been made,
-        and how long until more can be made.
-
-        :param self: Refer to the current instance of a class
-        :return: None
+        The create_session function is used to create a new session for the Client.
+        The session object contains all of the information that we need in order to connect with Discord's API.
         """
 
         self.session: CustomSession = CustomSession(self.logger,
                                                     latency=self.request_latency,
                                                     additional_cooldown=self.ratelimit_additional_cooldown,
                                                     users=self.users)
 
-    def _check_tokens(self) -> None:
+    def _check_tokens(self, tokens: Union[list[str], str]) -> None:  # pyright: ignore
         """
         The _check_tokens function is used to check if the tokens provided are valid.
-        If a token is invalid, it will be removed from the list of tokens and not be used in any future requests.
-        The function also creates UserClient objects for each valid token.
+        If they are, then it will add them to the users list. If not, then it will delete them from the list.
 
-        :param self: Represent the instance of the class
-        :return: None
+        :param tokens: Tokens to check
         """
 
-        async def _check(_type: Union[type[list], type[str]]) -> None:
+        async def _check() -> None:
             _url: str = self.endpoint + "users/@me"
-            if _type == str:
-                header: AUTH_HEADER = AUTH_HEADER(authorization=self._tokens)
+            for token in tokens:
+                header: AUTH_HEADER = AUTH_HEADER(authorization=token)
                 response: ClientResponse = await self.session.get(_url, headers=header)
                 if response.status != 200:
                     if self._logger_status:
                         self.logger.warning(
-                            f"An invalid token has been provided: {self._tokens} | The token will be automatically deleted")
+                            f"An invalid token has been provided: {token} | The token will be automatically deleted")
+
                 else:
-                    data = await response.json()
-                    data["token"] = self._tokens
+                    data: dict = await response.json()
+                    data["token"] = token
                     data["endpoint"] = self.endpoint
-                    self.users.append(UserClient(data, self.session))
-
-                    self._tokens = [self._tokens]
 
-            elif _type == list:
-                for token in self._tokens:
-
-                    header: AUTH_HEADER = AUTH_HEADER(authorization=token)
-                    response: ClientResponse = await self.session.get(_url, headers=header)
-                    if response.status != 200:
-                        if self._logger_status:
-                            self.logger.warning(
-                                f"An invalid token has been provided: {token} | The token will be automatically deleted")
-
-                    else:
-                        data = await response.json()
-                        data["token"] = token
-                        data["endpoint"] = self.endpoint
-
-                        self.users.append(UserClient(data, self.session))
+                    self.users.append(UserClient(data, self.session))
 
             if self._logger_status:
                 self.logger.info(f"Checking of tokens successfully completed | Loaded ({len(self.users)}) tokens\n")
 
-        if not isinstance(self._tokens, list) and not isinstance(self._tokens, str):
+        if not isinstance(tokens, list) and not isinstance(tokens, str):
             raise UnSupportedTokenType
 
-        self.loop.run_until_complete(_check(type(self._tokens)))
+        if isinstance(tokens, str):
+            tokens: list[str] = [tokens]  # pyright: ignore
 
-    def __del__(self) -> None:
-        """
-        The __del__ function is called when the object is garbage collected.
-        The __del__ function can be used to clean up resources that are not managed by Python, such as file handles or network connections.
-        If you have a class with an open file handle, and you want to make sure that the file gets closed when the object gets deleted,
-        you can implement __del__ for this purpose.
+        self.loop.run_until_complete(_check())
 
-        :param self: Represent the instance of the class
-        :return: None
-        """
+    def __del__(self) -> None:
         try:
             self.loop.run_until_complete(self.session.close())
         except AttributeError:
             pass
 
     def run_async(self, function: Awaitable) -> None:
         """
         The run_async function is a helper function that allows you to run an asyncio coroutine in the background.
         It takes a single argument, which must be an awaitable object (such as a coroutine). It runs the event loop until
-        the awaitable completes and then returns. This is useful for running tasks in parallel with other code.
+        the awaitable completes. This is useful for running tasks in parallel with other code.
 
-        :param self: Access the attributes and methods of a class
-        :param function: Awaitable: Specify the type of the parameter function
-        :return: None
+        :param function: Specify the coroutine
         """
+
         self.loop.run_until_complete(function)
 
-    async def request(self, url: str, method: METHOD, headers: dict = None, data: dict = None) -> ClientResponse:
+    async def request(self, url: str, method: METHOD, headers: Optional[dict] = None,
+                      data: Optional[dict] = None) -> ClientResponse:
         """
         The request function is used to send a request to the API.
 
-        :param self: Represent the instance of the class
-        :param url: str: Specify the url of the request
-        :param method: METHOD: Specify the type of request being sent
-        :param headers: dict: Pass in a dictionary of headers to be sent with the request
-        :param data: dict: Send data to the server
-        :return: A clientresponse object
+        :param url: Specify the url of the request
+        :param method: Specify the type of request being sent
+        :param headers: Pass in a dictionary of headers to be sent with the request
+        :param data: Send data to the api
         """
 
         if method not in ("POST", "GET", "DELETE", "PATCH", "PUT"):
             raise InvalidMethodType(method)
 
-        url: str = self.endpoint + url
+        _url: str = self.endpoint + url
 
         if self._logger_status:
-            self.logger.debug(f"Sending request: {method} -> {url}")
+            self.logger.debug(f"Sending request: {method} -> {_url}")
 
         response: ClientResponse = await self.session.request(method=method, url=url, headers=headers, json=data)
         response.raise_for_status()
 
         return response
```

### Comparing `selfbotclient-1.1.0/SelfBotClient/permissionbuilder.py` & `selfbotclient-1.1.1/SelfBotClient/permissionbuilder.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class PermissionBuilder:
     """
     PermissionBuilder takes a Permissions type and then adds them all to a value.
     Methods using PermissionBuilder acquire this value.
 
-    :param args: Accept a variable number of arguments
+    :param args: PermissionType values
     """
 
     __slots__ = ("value",)
 
     def __init__(self, *args: Permissions) -> None:
 
         self.value: int = 0
```

### Comparing `selfbotclient-1.1.0/SelfBotClient/thread.py` & `selfbotclient-1.1.1/SelfBotClient/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     from .client import Client
 
 from asyncio import Task
 import threading
 from time import sleep
 
 
-class Thread:
+class Tasks:
     """
-    :class:`Thread` Allows you to run several methods simultaneously with tasks.
+    :class:`Tasks` Allows you to run several methods simultaneously with tasks.
 
     :param client: Client object to obtain main program loop
     """
 
     def __init__(self, client: Client) -> None:
         self._client: Client = client
         self._loop = client.loop
```

### Comparing `selfbotclient-1.1.0/SelfBotClient/user.py` & `selfbotclient-1.1.1/SelfBotClient/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union, Optional
 
 if TYPE_CHECKING:
     from .http import CustomSession
 
 from .typings import AUTH_HEADER, RGB_COLOR
 from .logger import Logger
 from .enums import ChannelType
@@ -22,22 +22,22 @@
 
     :param data: Dict with account data - such as token, name, id.
     :param session: Session to send requests in methods
     """
 
     def __init__(self, data: dict, session: CustomSession):
         self._session: CustomSession = session
-        self._logger: Logger = getLogger("Logger")
+        self._logger: Logger = getLogger("Logger")  # pyright: ignore
 
         self.data: dict = data
-        self._endpoint: str = self.data.get("endpoint")
-        self.token: str = self.data.get("token")
-        self.name: str = self.data.get("username")
-        self.discriminator: str = f"#{self.data.get('discriminator')}"
-        self.id: int = self.data.get("id")
+        self._endpoint: str = self.data["endpoint"]
+        self.token: str = self.data["token"]
+        self.name: str = self.data["name"]
+        self.discriminator: str = f"#{self.data['discriminator']}"
+        self.id: int = self.data["id"]
 
         self._auth_header: AUTH_HEADER = AUTH_HEADER(
             authorization=self.token
         )
 
     def __repr__(self):
         return f"<UserClient(name={self.name}, discriminator={self.discriminator}, id={self.id})>"
@@ -86,15 +86,16 @@
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
                 f"Request DELETE channels/{channel_id} failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def create_channel(self, guild_id: int, name: str, channel_type: ChannelType,
-                             topic: str = None, user_limit: int = None, position: int = None, nsfw: bool = False) -> ClientResponse:
+                             topic: Optional[str] = None, user_limit: Optional[int] = None,
+                             position: Optional[int] = None, nsfw: Optional[bool] = False) -> ClientResponse:
         """
         The create_channel function creates a channel in the specified guild.
 
         :param guild_id: Specify the guild id of the server you want to create a channel in
         :param name: Specify the name of the channel
         :param channel_type: Specify what type of channel you want to create
         :param topic: Set the topic of the channel
@@ -147,17 +148,17 @@
                 f"Request GET guilds/{guild_id}/channels failed.\n -> {self} {await response.json()}.")
 
         return response
 
     async def create_role(self,
                                 guild_id: int,
                                 name: str,
-                                color: RGB_COLOR = None,
-                                hoist: bool = False,
-                                permissions: PermissionBuilder = None) -> ClientResponse:
+                                color: Optional[RGB_COLOR] = None,
+                                hoist: Optional[bool] = False,
+                                permissions: Union[PermissionBuilder, int, None] = None) -> ClientResponse:
 
         """
         The create_role function creates a role in the specified guild.
 
         :param guild_id: Specify the guild in which you want to create a role
         :param name: Set the name of the role
         :param color: Set the color of the role
@@ -168,28 +169,28 @@
         _url = self._endpoint + f"guilds/{guild_id}/roles"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: POST -> {_url}")
 
         if color:
             r, g, b = color.values()
-            color = (r << 16) + (g << 8) + b
+            _color = (r << 16) + (g << 8) + b  # pyright: ignore
         else:
-            color = 0
+            _color: int = 0  # pyright: ignore
 
         if not permissions:
-            permissions = 0
+            _permissions: int = 0
         else:
-            permissions = permissions.value
+            _permissions: int = permissions.value  # pyright: ignore
 
         json: dict = {
             "name": name,
             "hoist": hoist,
-            "color": color,
-            "permissions": permissions
+            "color": _color,
+            "permissions": _permissions
         }
 
         response: ClientResponse = await self._session.request(
             method="POST", url=_url, headers=self._auth_header, json=json)
 
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
@@ -218,16 +219,16 @@
 
         return response
 
     async def delete_role(self, guild_id: int, role_id: int) -> ClientResponse:
         """
         The delete_role function deletes a role from the guild.
 
-        :param guild_id: int: Specify the guild that you want to delete a role from
-        :param role_id: int: Specify the role_id to be deleted
+        :param guild_id: Specify the guild that you want to delete a role from
+        :param role_id: Specify the role_id to be deleted
         """
 
         _url = self._endpoint + f"guilds/{guild_id}/roles/{role_id}"
 
         if self._logger._status:
             self._logger.debug(f"Sending request: DELETE -> {_url}")
 
@@ -346,17 +347,17 @@
         if response.status not in (200, 429) and self._logger._status:
             self._logger.error(
                 f"Request GET guilds/{guild_id}/members/{user_id} failed.\n -> {self} {await response.json()}")
 
         return response
 
     async def edit_member(self, guild_id: int, user_id: int,
-                          nickname: str = None,
-                          add_roles: list[int] = None,
-                          remove_roles: list[int] = None) -> ClientResponse:
+                          nickname: Optional[str] = None,
+                          add_roles: Optional[list[int]] = None,
+                          remove_roles: Optional[list[int]] = None) -> ClientResponse:
 
         """
         The edit_member function allows you to edit a member of a guild.
 
         :param guild_id: Specify the guild that you want to edit a member in
         :param user_id: Specify the user that you want to edit
         :param nickname: Change the nickname of a user in a guild
@@ -366,25 +367,26 @@
 
         json: dict = {}
 
         if add_roles or remove_roles:
             user_response: ClientResponse = await self.get_member(guild_id, user_id)
             user_data: dict = await user_response.json()
 
-            roles: list[str] = user_data.get("roles")
-            if not roles:
-                roles: list[str] = []
+            roles: Union[None, list[str]] = user_data.get("roles")
+
+            roles_list: list[str] = [] if not roles else roles
 
             if add_roles:
                 for _role in add_roles:
-                    roles.append(str(_role))
+                    roles_list.append(str(_role))
+
             if remove_roles:
                 for _role in remove_roles:
                     try:
-                        roles.remove(str(_role))
+                        roles_list.remove(str(_role))
                     except ValueError:
                         pass
             json["roles"] = roles
 
         if nickname:
             json["nick"] = nickname
 
@@ -454,18 +456,18 @@
 
         return response
 
     async def delete_reaction(self, channel_id: int, message_id: int, user_id: int, emoji: str) -> ClientResponse:
         """
         The delete_reaction function is used to delete a reaction from a message.
 
-        :param channel_id: int: Specify the channel where the message is located
-        :param message_id: int: Identify the message that you want to delete a reaction from
-        :param user_id: int: Specify the user whose reaction is to be deleted
-        :param emoji: str: Specify the emoji to be deleted
+        :param channel_id: Specify the channel where the message is located
+        :param message_id: Identify the message that you want to delete a reaction from
+        :param user_id: Specify the user whose reaction is to be deleted
+        :param emoji: Specify the emoji to be deleted
         """
 
         emoji = quote(emoji)
 
         _url = self._endpoint + f"channels/{channel_id}/messages/{message_id}/reactions/{emoji}/{user_id}"
 
         if self._logger._status:
```

### Comparing `selfbotclient-1.1.0/selfbotclient.egg-info/PKG-INFO` & `selfbotclient-1.1.1/selfbotclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfbotclient
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library that will allow you to manage selfbots
 Author: xXenvy
 Author-email: <xpimepk01@gmail.com>
 Keywords: python,requests,discord selfbot,selfbot,discord.py,aiohttp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `selfbotclient-1.1.0/setup.py` & `selfbotclient-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 DESCRIPTION = 'Library that will allow you to manage selfbots'
 LONG_DESCRIPTION = 'The library logs into your account thanks to the entered tokens and can manage them. ' \
                    'such as sending messages, deleting roles, etc.'
 
 # Setting up
 setup(
     name="selfbotclient",
```

