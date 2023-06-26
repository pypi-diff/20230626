# Comparing `tmp/axaiogram-0.0.8.tar.gz` & `tmp/axaiogram-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axaiogram-0.0.8.tar", last modified: Mon Jun 26 11:07:32 2023, max compression
+gzip compressed data, was "axaiogram-0.0.9.tar", last modified: Mon Jun 26 11:10:32 2023, max compression
```

## Comparing `axaiogram-0.0.8.tar` & `axaiogram-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.018919 axaiogram-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 11:07:32.018919 axaiogram-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-26 11:07:06.000000 axaiogram-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.010918 axaiogram-0.0.8/axaiogram/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.010918 axaiogram-0.0.8/axaiogram/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.010918 axaiogram-0.0.8/axaiogram/db/repository/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/db/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/db/repository/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/db/repository/user.py
--rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/db/repository/user_lang.py
--rw-r--r--   0 runner    (1001) docker     (122)      367 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/db/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.014919 axaiogram-0.0.8/axaiogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.014919 axaiogram-0.0.8/axaiogram/handlers/auth/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/handlers/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/handlers/auth/email_user_auth_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      976 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/handlers/frozen_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.014919 axaiogram-0.0.8/axaiogram/handlers/user/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/handlers/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2795 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/handlers/user/language_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.014919 axaiogram-0.0.8/axaiogram/middlewares/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/middlewares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.014919 axaiogram-0.0.8/axaiogram/middlewares/auth/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/middlewares/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/middlewares/template_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/middlewares/user_language_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.014919 axaiogram-0.0.8/axaiogram/settings/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/settings/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.014919 axaiogram-0.0.8/axaiogram/static/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/static/messages_group.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.018919 axaiogram-0.0.8/axaiogram/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/templates/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/templates/template_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/templates/template_group_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/templates/template_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/templates/template_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.018919 axaiogram-0.0.8/axaiogram/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5475 2023-06-26 11:07:06.000000 axaiogram-0.0.8/axaiogram/tests/test_md_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:07:32.010918 axaiogram-0.0.8/axaiogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 11:07:31.000000 axaiogram-0.0.8/axaiogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-26 11:07:31.000000 axaiogram-0.0.8/axaiogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 11:07:31.000000 axaiogram-0.0.8/axaiogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 11:07:31.000000 axaiogram-0.0.8/axaiogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 11:07:31.000000 axaiogram-0.0.8/axaiogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 11:07:32.018919 axaiogram-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-26 11:07:06.000000 axaiogram-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.247909 axaiogram-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 11:10:32.247909 axaiogram-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-26 11:10:13.000000 axaiogram-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.239909 axaiogram-0.0.9/axaiogram/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram/db/repository/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/db/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/db/repository/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/db/repository/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/db/repository/user_lang.py
+-rw-r--r--   0 runner    (1001) docker     (122)      367 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/db/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram/handlers/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/handlers/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/handlers/auth/email_user_auth_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/handlers/frozen_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram/handlers/user/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/handlers/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2812 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/handlers/user/language_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/middlewares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram/middlewares/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/middlewares/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/middlewares/template_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/middlewares/user_language_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/settings/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram/static/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/static/messages_group.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.247909 axaiogram-0.0.9/axaiogram/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/templates/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/templates/template_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/templates/template_group_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/templates/template_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/templates/template_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.247909 axaiogram-0.0.9/axaiogram/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5475 2023-06-26 11:10:13.000000 axaiogram-0.0.9/axaiogram/tests/test_md_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:10:32.243909 axaiogram-0.0.9/axaiogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 11:10:32.000000 axaiogram-0.0.9/axaiogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-26 11:10:32.000000 axaiogram-0.0.9/axaiogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 11:10:32.000000 axaiogram-0.0.9/axaiogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 11:10:32.000000 axaiogram-0.0.9/axaiogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 11:10:32.000000 axaiogram-0.0.9/axaiogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 11:10:32.247909 axaiogram-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-26 11:10:13.000000 axaiogram-0.0.9/setup.py
```

### Comparing `axaiogram-0.0.8/axaiogram/db/models.py` & `axaiogram-0.0.9/axaiogram/db/models.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/db/repository/user.py` & `axaiogram-0.0.9/axaiogram/db/repository/user.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/handlers/base.py` & `axaiogram-0.0.9/axaiogram/handlers/base.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/handlers/frozen_handler.py` & `axaiogram-0.0.9/axaiogram/handlers/frozen_handler.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/handlers/user/language_setup.py` & `axaiogram-0.0.9/axaiogram/handlers/user/language_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Callable, Dict, Union
 
 from aiogram import Bot, Dispatcher, F, types
 from aiogram.fsm.context import FSMContext
 from aiogram.utils.keyboard import InlineKeyboardBuilder
-from axsqlalchemy.uow import UOWFactory
+from axsqlalchemy.uow import UOWFactory, TRepoCollector
 
 from axaiogram.db.repository.collection import RepoCollector
 from axaiogram.handlers.frozen_handler import FrozenHandler
 
 from ..base import BaseHandlersGroup
 from ..base import proxy_router as _router
 
 
 class UserLanguageSetupHandlers(BaseHandlersGroup):
     def __init__(
         self,
         bot: Bot,
         dp: Dispatcher,
-        uowf: UOWFactory[RepoCollector],
+        uowf: UOWFactory[TRepoCollector],
         languages: Union[Dict[str, str], None] = None,
         start_handler: Union[Callable, None] = None,
     ) -> None:
         super().__init__(bot, dp, uowf)
         self.uowf = uowf
 
         if not languages:
```

### Comparing `axaiogram-0.0.8/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py` & `axaiogram-0.0.9/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py` & `axaiogram-0.0.9/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/middlewares/template_middleware.py` & `axaiogram-0.0.9/axaiogram/middlewares/template_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/middlewares/user_language_middleware.py` & `axaiogram-0.0.9/axaiogram/middlewares/user_language_middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any, Awaitable, Callable, Dict, Union
 
 from aiogram import types
 from aiogram.dispatcher.middlewares.base import BaseMiddleware
 from aiogram.types import TelegramObject
-from axsqlalchemy.uow import UOWFactory
+from axsqlalchemy.uow import UOWFactory, TRepoCollector
 
 from axaiogram.db.repository.collection import RepoCollector
 from axaiogram.handlers.frozen_handler import FrozenHandler
 
 from ..handlers.user import UserLanguageSetupHandlers
 
 
 class UserLanguageMiddleware(BaseMiddleware):
     def __init__(
-        self, uowf: UOWFactory[RepoCollector], handler: UserLanguageSetupHandlers
+        self, uowf: UOWFactory[TRepoCollector], handler: UserLanguageSetupHandlers
     ) -> None:
         self.handler = handler
         self.uowf = uowf
         super().__init__()
 
     async def __call__(
         self,
```

### Comparing `axaiogram-0.0.8/axaiogram/static/messages_group.py` & `axaiogram-0.0.9/axaiogram/static/messages_group.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/templates/collection.py` & `axaiogram-0.0.9/axaiogram/templates/collection.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/templates/template_group.py` & `axaiogram-0.0.9/axaiogram/templates/template_group.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/templates/template_group_factory.py` & `axaiogram-0.0.9/axaiogram/templates/template_group_factory.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/templates/template_message.py` & `axaiogram-0.0.9/axaiogram/templates/template_message.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/templates/template_parser.py` & `axaiogram-0.0.9/axaiogram/templates/template_parser.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram/tests/test_md_parser.py` & `axaiogram-0.0.9/axaiogram/tests/test_md_parser.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/axaiogram.egg-info/SOURCES.txt` & `axaiogram-0.0.9/axaiogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.8/setup.py` & `axaiogram-0.0.9/setup.py`

 * *Files identical despite different names*

