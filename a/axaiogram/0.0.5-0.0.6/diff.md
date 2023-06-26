# Comparing `tmp/axaiogram-0.0.5.tar.gz` & `tmp/axaiogram-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axaiogram-0.0.5.tar", last modified: Mon Jun 26 07:27:04 2023, max compression
+gzip compressed data, was "axaiogram-0.0.6.tar", last modified: Mon Jun 26 09:51:56 2023, max compression
```

## Comparing `axaiogram-0.0.5.tar` & `axaiogram-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.406950 axaiogram-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 07:27:04.406950 axaiogram-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-26 07:26:45.000000 axaiogram-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.398949 axaiogram-0.0.5/axaiogram/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram/db/repository/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/db/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/db/repository/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/db/repository/user.py
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/db/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram/handlers/auth/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/handlers/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/handlers/auth/email_user_auth_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/handlers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram/handlers/user/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/handlers/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/handlers/user/language_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram/middlewares/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/middlewares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram/middlewares/auth/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/middlewares/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/middlewares/template_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/middlewares/user_language_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram/settings/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/settings/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram/static/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/static/messages_group.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.406950 axaiogram-0.0.5/axaiogram/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/templates/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/templates/template_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/templates/template_group_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/templates/template_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/templates/template_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.406950 axaiogram-0.0.5/axaiogram/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5475 2023-06-26 07:26:45.000000 axaiogram-0.0.5/axaiogram/tests/test_md_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:27:04.402950 axaiogram-0.0.5/axaiogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 07:27:04.000000 axaiogram-0.0.5/axaiogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-26 07:27:04.000000 axaiogram-0.0.5/axaiogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 07:27:04.000000 axaiogram-0.0.5/axaiogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 07:27:04.000000 axaiogram-0.0.5/axaiogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 07:27:04.000000 axaiogram-0.0.5/axaiogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 07:27:04.406950 axaiogram-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-26 07:26:45.000000 axaiogram-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 09:51:56.915776 axaiogram-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-26 09:51:36.000000 axaiogram-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram/db/repository/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/repository/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/repository/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/handlers/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/auth/email_user_auth_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/handlers/user/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/user/language_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/middlewares/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/template_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/user_language_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/settings/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/static/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/static/messages_group.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/template_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/template_group_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/template_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/template_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5475 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/tests/test_md_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 09:51:56.915776 axaiogram-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-26 09:51:36.000000 axaiogram-0.0.6/setup.py
```

### Comparing `axaiogram-0.0.5/axaiogram/db/models.py` & `axaiogram-0.0.6/axaiogram/db/models.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/db/repository/user.py` & `axaiogram-0.0.6/axaiogram/db/repository/user.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/handlers/base.py` & `axaiogram-0.0.6/axaiogram/handlers/base.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/handlers/user/language_setup.py` & `axaiogram-0.0.6/axaiogram/handlers/user/language_setup.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py` & `axaiogram-0.0.6/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py` & `axaiogram-0.0.6/axaiogram/middlewares/user_language_middleware.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,29 @@
-from abc import ABC, abstractmethod
-from typing import Any, Awaitable, Callable, Dict
+from typing import Any, Awaitable, Callable, Dict, Union
 
 from aiogram import types
 from aiogram.dispatcher.middlewares.base import BaseMiddleware
 from aiogram.types import TelegramObject
 
-from axsqlalchemy.uow import UOWFactory
-from db.repository.collection import RepoCollector
+from ..handlers.user import UserLanguageSetupHandlers
 
 
-class BaseUserAuthHandlers(ABC):
-    async def require(self, chat_id: int):
-        raise NotImplementedError
-
-
-class UseHandlerUserAuthMiddleware(BaseMiddleware):
-    def __init__(
-        self,
-        uowf: UOWFactory[RepoCollector],
-        auth_handlers_group: BaseUserAuthHandlers,
-    ) -> None:
-        self.uowf = uowf
-        self.auth_handlers = auth_handlers_group
+class UserLanguageMiddleware(BaseMiddleware):
+    def __init__(self, handler: UserLanguageSetupHandlers) -> None:
+        self.handler = handler
+        super().__init__()
 
     async def __call__(
         self,
         handler: Callable[[TelegramObject, Dict[str, Any]], Awaitable[Any]],
-        event: types.Message,
+        event: Union[TelegramObject, types.Message],
         data: Dict[str, Any],
     ) -> Any:
-        if not hasattr(event, "from_user"):
-            raise NotImplementedError(
-                f"`{self.__class__.__name__}` can't handler event type of `{type(event)}`"
-            )
+        user = data.get('user')
 
-        assert event.from_user is not None
-        user_id = event.from_user.id
+        if not user:
+            raise NotImplementedError(f'`{self.__class__.__name__}` requires user auth middleware')
 
-        async with self.uowf() as uow:
-            user = await uow.repo.user.get(user_id)
+        if not user.lang_code:
+            return await self.handler._require(user.id)
 
-        if not user:
-            return await self.auth_handlers.require(user_id)
-        else:
-            return await handler(event, data)
+        return await handler(event, data)
```

### Comparing `axaiogram-0.0.5/axaiogram/middlewares/template_middleware.py` & `axaiogram-0.0.6/axaiogram/middlewares/template_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/static/messages_group.py` & `axaiogram-0.0.6/axaiogram/static/messages_group.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/templates/collection.py` & `axaiogram-0.0.6/axaiogram/templates/collection.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/templates/template_group.py` & `axaiogram-0.0.6/axaiogram/templates/template_group.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/templates/template_group_factory.py` & `axaiogram-0.0.6/axaiogram/templates/template_group_factory.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/templates/template_message.py` & `axaiogram-0.0.6/axaiogram/templates/template_message.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/templates/template_parser.py` & `axaiogram-0.0.6/axaiogram/templates/template_parser.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram/tests/test_md_parser.py` & `axaiogram-0.0.6/axaiogram/tests/test_md_parser.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/axaiogram.egg-info/SOURCES.txt` & `axaiogram-0.0.6/axaiogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.5/setup.py` & `axaiogram-0.0.6/setup.py`

 * *Files identical despite different names*

