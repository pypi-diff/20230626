# Comparing `tmp/axaiogram-0.0.1.tar.gz` & `tmp/axaiogram-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axaiogram-0.0.1.tar", last modified: Mon Jun 26 07:13:45 2023, max compression
+gzip compressed data, was "axaiogram-0.0.4.tar", last modified: Mon Jun 26 07:20:11 2023, max compression
```

## Comparing `axaiogram-0.0.1.tar` & `axaiogram-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.115482 axaiogram-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 07:13:45.115482 axaiogram-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-26 07:13:24.000000 axaiogram-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram/db/repository/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/db/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/db/repository/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/db/repository/user.py
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/db/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram/handlers/auth/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/handlers/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/handlers/auth/email_user_auth_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/handlers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram/handlers/user/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/handlers/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/handlers/user/language_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram/middlewares/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/middlewares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram/middlewares/auth/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/middlewares/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/middlewares/template_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/middlewares/user_language_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram/settings/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/settings/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.115482 axaiogram-0.0.1/axaiogram/static/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/static/messages_group.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.115482 axaiogram-0.0.1/axaiogram/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/templates/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/templates/template_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/templates/template_group_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/templates/template_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/templates/template_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.115482 axaiogram-0.0.1/axaiogram/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5475 2023-06-26 07:13:24.000000 axaiogram-0.0.1/axaiogram/tests/test_md_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:13:45.111482 axaiogram-0.0.1/axaiogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 07:13:45.000000 axaiogram-0.0.1/axaiogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-26 07:13:45.000000 axaiogram-0.0.1/axaiogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 07:13:45.000000 axaiogram-0.0.1/axaiogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-26 07:13:45.000000 axaiogram-0.0.1/axaiogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 07:13:45.000000 axaiogram-0.0.1/axaiogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 07:13:45.115482 axaiogram-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-26 07:13:24.000000 axaiogram-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.690093 axaiogram-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 07:20:11.690093 axaiogram-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-26 07:19:41.000000 axaiogram-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.682093 axaiogram-0.0.4/axaiogram/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.682093 axaiogram-0.0.4/axaiogram/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.686093 axaiogram-0.0.4/axaiogram/db/repository/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/db/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/db/repository/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/db/repository/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/db/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.686093 axaiogram-0.0.4/axaiogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.686093 axaiogram-0.0.4/axaiogram/handlers/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/handlers/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/handlers/auth/email_user_auth_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/handlers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.686093 axaiogram-0.0.4/axaiogram/handlers/user/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/handlers/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/handlers/user/language_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.686093 axaiogram-0.0.4/axaiogram/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/middlewares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.686093 axaiogram-0.0.4/axaiogram/middlewares/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/middlewares/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/middlewares/template_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/middlewares/user_language_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.686093 axaiogram-0.0.4/axaiogram/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/settings/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.686093 axaiogram-0.0.4/axaiogram/static/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/static/messages_group.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.690093 axaiogram-0.0.4/axaiogram/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/templates/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/templates/template_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/templates/template_group_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/templates/template_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/templates/template_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.690093 axaiogram-0.0.4/axaiogram/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5475 2023-06-26 07:19:41.000000 axaiogram-0.0.4/axaiogram/tests/test_md_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:11.682093 axaiogram-0.0.4/axaiogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-26 07:20:11.000000 axaiogram-0.0.4/axaiogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-26 07:20:11.000000 axaiogram-0.0.4/axaiogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 07:20:11.000000 axaiogram-0.0.4/axaiogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 07:20:11.000000 axaiogram-0.0.4/axaiogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 07:20:11.000000 axaiogram-0.0.4/axaiogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 07:20:11.690093 axaiogram-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-26 07:19:41.000000 axaiogram-0.0.4/setup.py
```

### Comparing `axaiogram-0.0.1/axaiogram/db/models.py` & `axaiogram-0.0.4/axaiogram/db/models.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/db/repository/user.py` & `axaiogram-0.0.4/axaiogram/db/repository/user.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/handlers/base.py` & `axaiogram-0.0.4/axaiogram/handlers/base.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/handlers/user/language_setup.py` & `axaiogram-0.0.4/axaiogram/handlers/user/language_setup.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py` & `axaiogram-0.0.4/axaiogram/middlewares/auth/on_the_fly_user_auth_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py` & `axaiogram-0.0.4/axaiogram/middlewares/auth/use_handler_user_auth_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/middlewares/template_middleware.py` & `axaiogram-0.0.4/axaiogram/middlewares/template_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/middlewares/user_language_middleware.py` & `axaiogram-0.0.4/axaiogram/middlewares/user_language_middleware.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/static/messages_group.py` & `axaiogram-0.0.4/axaiogram/static/messages_group.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/templates/collection.py` & `axaiogram-0.0.4/axaiogram/templates/collection.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/templates/template_group.py` & `axaiogram-0.0.4/axaiogram/templates/template_group.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/templates/template_group_factory.py` & `axaiogram-0.0.4/axaiogram/templates/template_group_factory.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/templates/template_message.py` & `axaiogram-0.0.4/axaiogram/templates/template_message.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/templates/template_parser.py` & `axaiogram-0.0.4/axaiogram/templates/template_parser.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram/tests/test_md_parser.py` & `axaiogram-0.0.4/axaiogram/tests/test_md_parser.py`

 * *Files identical despite different names*

### Comparing `axaiogram-0.0.1/axaiogram.egg-info/SOURCES.txt` & `axaiogram-0.0.4/axaiogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

