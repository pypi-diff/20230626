# Comparing `tmp/axaiogram-0.0.6.tar.gz` & `tmp/axaiogram-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axaiogram-0.0.6.tar", last modified: Mon Jun 26 09:51:56 2023, max compression
+gzip compressed data, was "axaiogram-0.0.7.tar", last modified: Mon Jun 26 11:02:15 2023, max compression
```

## Comparing `axaiogram-0.0.6.tar` & `axaiogram-0.0.7.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 09:51:56.915776 axaiogram-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-26 09:51:36.000000 axaiogram-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram/db/repository/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/repository/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/repository/user.py
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/db/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/handlers/auth/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/auth/email_user_auth_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/handlers/user/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/handlers/user/language_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/middlewares/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/middlewares/auth/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/template_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/middlewares/user_language_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/settings/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/settings/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/static/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/static/messages_group.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/template_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/template_group_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/template_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/templates/template_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.915776 axaiogram-0.0.6/axaiogram/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5475 2023-06-26 09:51:36.000000 axaiogram-0.0.6/axaiogram/tests/test_md_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:51:56.911776 axaiogram-0.0.6/axaiogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 09:51:56.000000 axaiogram-0.0.6/axaiogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 09:51:56.915776 axaiogram-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-26 09:51:36.000000 axaiogram-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.513046 axaiogram-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 11:02:15.513046 axaiogram-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-26 11:01:54.000000 axaiogram-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.505046 axaiogram-0.0.7/axaiogram/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.509046 axaiogram-0.0.7/axaiogram/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.509046 axaiogram-0.0.7/axaiogram/db/repository/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/db/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/db/repository/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/db/repository/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/db/repository/user_lang.py
+-rw-r--r--   0 runner    (1001) docker     (122)      367 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/db/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.509046 axaiogram-0.0.7/axaiogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.509046 axaiogram-0.0.7/axaiogram/handlers/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/handlers/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/handlers/auth/email_user_auth_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/handlers/frozen_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.509046 axaiogram-0.0.7/axaiogram/handlers/user/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/handlers/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2795 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/handlers/user/language_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.509046 axaiogram-0.0.7/axaiogram/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/middlewares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.513046 axaiogram-0.0.7/axaiogram/middlewares/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/middlewares/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/middlewares/template_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/middlewares/user_language_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.513046 axaiogram-0.0.7/axaiogram/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/settings/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.513046 axaiogram-0.0.7/axaiogram/static/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/static/messages_group.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.513046 axaiogram-0.0.7/axaiogram/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/templates/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/templates/template_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/templates/template_group_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/templates/template_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/templates/template_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.513046 axaiogram-0.0.7/axaiogram/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5475 2023-06-26 11:01:54.000000 axaiogram-0.0.7/axaiogram/tests/test_md_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:02:15.509046 axaiogram-0.0.7/axaiogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 11:02:15.000000 axaiogram-0.0.7/axaiogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-26 11:02:15.000000 axaiogram-0.0.7/axaiogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 11:02:15.000000 axaiogram-0.0.7/axaiogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 11:02:15.000000 axaiogram-0.0.7/axaiogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 11:02:15.000000 axaiogram-0.0.7/axaiogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 11:02:15.513046 axaiogram-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-26 11:01:54.000000 axaiogram-0.0.7/setup.py
```

### Comparing `axaiogram-0.0.6/axaiogram/db/models.py` & `axaiogram-0.0.7/axaiogram/db/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import sqlalchemy as sa
-
 from axsqlalchemy.model import Base, BaseTableAt
 
 
 class AbstractUserModel(BaseTableAt):
     __abstract__ = True
 
     id = sa.Column(sa.BigInteger, primary_key=True, index=True)
     username = sa.Column(sa.String(length=256), nullable=True)
     firstname = sa.Column(sa.String(length=456), nullable=False)
     secondname = sa.Column(sa.String(length=456), nullable=True)
-    lang_code = sa.Column(sa.String(length=256), nullable=True)
     is_active = sa.Column(sa.Boolean, nullable=False, default=True)
 
 
+class AbstractUserLanguageModel(BaseTableAt):
+    id = sa.Column(sa.BigInteger, primary_key=True, index=True)
+    lang_code = sa.Column(sa.String(length=256), nullable=True)
+
+
 class AbstractUserWithEmailModel(AbstractUserModel):
     __abstract__ = True
 
     email = sa.Column(sa.String, nullable=False)
 
 
 __all__ = [
```

### Comparing `axaiogram-0.0.6/axaiogram/db/repository/user.py` & `axaiogram-0.0.7/axaiogram/db/repository/user.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/handlers/base.py` & `axaiogram-0.0.7/axaiogram/handlers/base.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/handlers/user/language_setup.py` & `axaiogram-0.0.7/axaiogram/handlers/user/language_setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from typing import Callable, Dict, Union
 
 from aiogram import Bot, Dispatcher, F, types
+from aiogram.fsm.context import FSMContext
 from aiogram.utils.keyboard import InlineKeyboardBuilder
+from axsqlalchemy.uow import UOWFactory
+
+from axaiogram.db.repository.collection import RepoCollector
+from axaiogram.handlers.frozen_handler import FrozenHandler
 
 from ..base import BaseHandlersGroup
 from ..base import proxy_router as _router
 
 
 class UserLanguageSetupHandlers(BaseHandlersGroup):
     def __init__(
         self,
         bot: Bot,
         dp: Dispatcher,
-        uowf,
+        uowf: UOWFactory[RepoCollector],
         languages: Union[Dict[str, str], None] = None,
         start_handler: Union[Callable, None] = None,
     ) -> None:
         super().__init__(bot, dp, uowf)
         self.uowf = uowf
 
         if not languages:
@@ -55,24 +60,30 @@
 
     @_router.message(F.text.strip().startswith("🌍"))
     async def handle_list(self, message: types.Message):
         assert message.from_user is not None
         return await self._require(message.from_user.id)
 
     @_router.callback_query(F.data.startswith("chlang:"))
-    async def handle_choosen(self, cq: types.CallbackQuery):
+    async def handle_choosen(self, cq: types.CallbackQuery, state: FSMContext):
         assert cq.data is not None
         assert cq.from_user is not None
 
         if cq.message:
             await cq.message.delete()
 
         _, lang_code = cq.data.split(":")
 
         async with self.uowf() as uow:
-            user = await uow.repo.user.get(cq.from_user.id)
-            user.lang_code = lang_code
-
-            await uow.repo.user.update(user)
+            await uow.repo.user_lang.add(
+                uow.repo.user_lang.IModel(
+                    id=cq.from_user.id,
+                    lang_code=lang_code,
+                )
+            )
+
+        if fhandler := await FrozenHandler.get(state):
+            await fhandler.delete(state)
+            return await fhandler.handler(fhandler.event, fhandler.data)
 
         if self.start_handler is not None:
             await self.start_handler(cq.from_user.id)
```

### Comparing `axaiogram-0.0.6/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py` & `axaiogram-0.0.7/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py` & `axaiogram-0.0.7/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,25 @@
         if not hasattr(event, "from_user"):
             raise NotImplementedError(
                 f"`{self.__class__.__name__}` can't handler event type of `{type(event)}`"
             )
 
         assert event.from_user is not None
         user_id = event.from_user.id
+        data["user_id"] = user_id
 
         async with self.uowf() as uow:
             user = await uow.repo.user.get(user_id)
 
         if not user:
             state: FSMContext = data["state"]
 
             current_state = await state.get_state()
             print(f"{current_state=}")
             print(
                 f"state in auth states group: {current_state in self.auth_states_group.__states__}"
             )
 
             if current_state not in self.auth_states_group.__states__:
-                return await self.auth_handlers.require(user_id, state)
+                return await self.auth_handlers.require(event, data)
 
         return await handler(event, data)
```

### Comparing `axaiogram-0.0.6/axaiogram/middlewares/template_middleware.py` & `axaiogram-0.0.7/axaiogram/middlewares/template_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/middlewares/user_language_middleware.py` & `axaiogram-0.0.7/axaiogram/middlewares/user_language_middleware.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 from typing import Any, Awaitable, Callable, Dict, Union
 
 from aiogram import types
 from aiogram.dispatcher.middlewares.base import BaseMiddleware
 from aiogram.types import TelegramObject
+from axsqlalchemy.uow import UOWFactory
+
+from axaiogram.db.repository.collection import RepoCollector
+from axaiogram.handlers.frozen_handler import FrozenHandler
 
 from ..handlers.user import UserLanguageSetupHandlers
 
 
 class UserLanguageMiddleware(BaseMiddleware):
-    def __init__(self, handler: UserLanguageSetupHandlers) -> None:
+    def __init__(
+        self, uowf: UOWFactory[RepoCollector], handler: UserLanguageSetupHandlers
+    ) -> None:
         self.handler = handler
+        self.uowf = uowf
         super().__init__()
 
     async def __call__(
         self,
         handler: Callable[[TelegramObject, Dict[str, Any]], Awaitable[Any]],
         event: Union[TelegramObject, types.Message],
         data: Dict[str, Any],
     ) -> Any:
-        user = data.get('user')
+        user_data: types.User = data["event_from_user"]
+        user_id = user_data.id
+
+        async with self.uowf() as uow:
+            user_lang_data = await uow.repo.user_lang.get(user_id)
+
+        if not user_lang_data:
+            state = data["state"]
+
+            await FrozenHandler(handler, event, data).freeze(state)
 
-        if not user:
-            raise NotImplementedError(f'`{self.__class__.__name__}` requires user auth middleware')
+            return await self.handler._require(user_id)
 
-        if not user.lang_code:
-            return await self.handler._require(user.id)
+        data["user_lang_data"] = user_lang_data
 
         return await handler(event, data)
```

### Comparing `axaiogram-0.0.6/axaiogram/static/messages_group.py` & `axaiogram-0.0.7/axaiogram/static/messages_group.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/templates/collection.py` & `axaiogram-0.0.7/axaiogram/templates/collection.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/templates/template_group.py` & `axaiogram-0.0.7/axaiogram/templates/template_group.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/templates/template_group_factory.py` & `axaiogram-0.0.7/axaiogram/templates/template_group_factory.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/templates/template_message.py` & `axaiogram-0.0.7/axaiogram/templates/template_message.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/templates/template_parser.py` & `axaiogram-0.0.7/axaiogram/templates/template_parser.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram/tests/test_md_parser.py` & `axaiogram-0.0.7/axaiogram/tests/test_md_parser.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.6/axaiogram.egg-info/SOURCES.txt` & `axaiogram-0.0.7/axaiogram.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 axaiogram.egg-info/top_level.txt
 axaiogram/db/__init__.py
 axaiogram/db/models.py
 axaiogram/db/schemas.py
 axaiogram/db/repository/__init__.py
 axaiogram/db/repository/collection.py
 axaiogram/db/repository/user.py
+axaiogram/db/repository/user_lang.py
 axaiogram/handlers/__init__.py
 axaiogram/handlers/base.py
+axaiogram/handlers/frozen_handler.py
 axaiogram/handlers/auth/__init__.py
 axaiogram/handlers/auth/email_user_auth_handlers.py
 axaiogram/handlers/user/__init__.py
 axaiogram/handlers/user/language_setup.py
 axaiogram/middlewares/__init__.py
 axaiogram/middlewares/template_middleware.py
 axaiogram/middlewares/user_language_middleware.py
```

### Comparing `axaiogram-0.0.6/setup.py` & `axaiogram-0.0.7/setup.py`

 * *Files identical despite different names*

