# Comparing `tmp/cy-account-0.1.0.tar.gz` & `tmp/cy_account-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cy-account-0.1.0.tar", last modified: Mon Jun 26 15:49:08 2023, max compression
+gzip compressed data, was "cy_account-0.1.1.tar", last modified: Mon Jun 26 16:02:35 2023, max compression
```

## Comparing `cy-account-0.1.0.tar` & `cy_account-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 15:49:08.158986 cy-account-0.1.0/
--rw-rw-rw-   0        0        0      303 2023-06-26 15:49:08.157990 cy-account-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-06-26 15:48:42.000000 cy-account-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 15:49:08.129988 cy-account-0.1.0/cy-account/
--rw-rw-rw-   0        0        0        0 2023-06-26 13:46:14.000000 cy-account-0.1.0/cy-account/__init__.py
--rw-rw-rw-   0        0        0     4979 2023-06-26 15:39:46.000000 cy-account-0.1.0/cy-account/account_api.py
--rw-rw-rw-   0        0        0     2415 2023-06-26 14:36:56.000000 cy-account-0.1.0/cy-account/cy_request.py
--rw-rw-rw-   0        0        0      476 2023-06-26 15:46:28.000000 cy-account-0.1.0/cy-account/test.py
--rw-rw-rw-   0        0        0      622 2023-06-26 13:51:00.000000 cy-account-0.1.0/cy-account/user_info.py
-drwxrwxrwx   0        0        0        0 2023-06-26 15:49:08.155994 cy-account-0.1.0/cy_account.egg-info/
--rw-rw-rw-   0        0        0      303 2023-06-26 15:49:08.000000 cy-account-0.1.0/cy_account.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-06-26 15:49:08.000000 cy-account-0.1.0/cy_account.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 15:49:08.000000 cy-account-0.1.0/cy_account.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-26 15:49:08.000000 cy-account-0.1.0/cy_account.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 15:49:08.000000 cy-account-0.1.0/cy_account.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 15:49:08.158986 cy-account-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      644 2023-06-26 15:47:43.000000 cy-account-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:02:35.615801 cy_account-0.1.1/
+-rw-rw-rw-   0        0        0      303 2023-06-26 16:02:35.613809 cy_account-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-26 15:56:06.000000 cy_account-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 16:02:35.584820 cy_account-0.1.1/cy_account/
+-rw-rw-rw-   0        0        0       54 2023-06-26 16:02:18.000000 cy_account-0.1.1/cy_account/__init__.py
+-rw-rw-rw-   0        0        0     4979 2023-06-26 16:01:45.000000 cy_account-0.1.1/cy_account/account_api.py
+-rw-rw-rw-   0        0        0     2415 2023-06-26 14:36:56.000000 cy_account-0.1.1/cy_account/cy_request.py
+-rw-rw-rw-   0        0        0      502 2023-06-26 15:49:30.000000 cy_account-0.1.1/cy_account/test.py
+-rw-rw-rw-   0        0        0      622 2023-06-26 13:51:00.000000 cy_account-0.1.1/cy_account/user_info.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:02:35.612820 cy_account-0.1.1/cy_account.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-06-26 16:02:35.000000 cy_account-0.1.1/cy_account.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-26 16:02:35.000000 cy_account-0.1.1/cy_account.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 16:02:35.000000 cy_account-0.1.1/cy_account.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-26 16:02:35.000000 cy_account-0.1.1/cy_account.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 16:02:35.000000 cy_account-0.1.1/cy_account.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 16:02:35.615801 cy_account-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-26 16:02:24.000000 cy_account-0.1.1/setup.py
```

### Comparing `cy-account-0.1.0/cy-account/account_api.py` & `cy_account-0.1.1/cy_account/account_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 import redis as redis
 from fastapi import HTTPException
 from cy_request import ServerForRequest
 from user_info import UserInfo
 
-USER_INFO_CACHE_KEY = 'cy-account-user-info-for-core'
+USER_INFO_CACHE_KEY = 'cy_account-user-info-for-core'
 CLIENT_AUTH_KEY = 'account-api-client-auth-hash'
 
 
 class AccountAPI:
 
     def __init__(self, redis_cli: redis.Redis):
         """
```

### Comparing `cy-account-0.1.0/cy-account/cy_request.py` & `cy_account-0.1.1/cy_account/cy_request.py`

 * *Files identical despite different names*

### Comparing `cy-account-0.1.0/cy-account/user_info.py` & `cy_account-0.1.1/cy_account/user_info.py`

 * *Files identical despite different names*

### Comparing `cy-account-0.1.0/setup.py` & `cy_account-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 setuptools.setup(
-    name="cy-account",
-    version="0.1.0",
+    name="cy_account",
+    version="0.1.01",
     author="luyuan",
     author_email="136735431@qq.com",
     description="edited by myself",
-    py_modules=["cy-account.account_api", "cy-account.cy_request", "cy-account.user_info", ],
+    py_modules=["cy_account.account_api", "cy_account.cy_request", "cy_account.user_info", ],
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent"],
     # 自动找到项目中导入的模块
     packages=setuptools.find_packages(),
     # 依赖模块
     install_requires=['pydantic', 'fastapi', 'redis'],
```

