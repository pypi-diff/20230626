# Comparing `tmp/cy_account-0.1.2.tar.gz` & `tmp/cy_account-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cy_account-0.1.2.tar", last modified: Mon Jun 26 16:14:13 2023, max compression
+gzip compressed data, was "cy_account-0.1.3.tar", last modified: Mon Jun 26 16:17:13 2023, max compression
```

## Comparing `cy_account-0.1.2.tar` & `cy_account-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:14:13.938775 cy_account-0.1.2/
--rw-rw-rw-   0        0        0      303 2023-06-26 16:14:13.937771 cy_account-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-26 16:03:11.000000 cy_account-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 16:14:13.916766 cy_account-0.1.2/cy_account/
--rw-rw-rw-   0        0        0     7918 2023-06-26 16:14:09.000000 cy_account-0.1.2/cy_account/__init__.py
--rw-rw-rw-   0        0        0     4979 2023-06-26 16:01:45.000000 cy_account-0.1.2/cy_account/account_api.py
--rw-rw-rw-   0        0        0     2415 2023-06-26 14:36:56.000000 cy_account-0.1.2/cy_account/cy_request.py
--rw-rw-rw-   0        0        0      502 2023-06-26 15:49:30.000000 cy_account-0.1.2/cy_account/test.py
--rw-rw-rw-   0        0        0      622 2023-06-26 13:51:00.000000 cy_account-0.1.2/cy_account/user_info.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:14:13.935768 cy_account-0.1.2/cy_account.egg-info/
--rw-rw-rw-   0        0        0      303 2023-06-26 16:14:13.000000 cy_account-0.1.2/cy_account.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-06-26 16:14:13.000000 cy_account-0.1.2/cy_account.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:14:13.000000 cy_account-0.1.2/cy_account.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-26 16:14:13.000000 cy_account-0.1.2/cy_account.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 16:14:13.000000 cy_account-0.1.2/cy_account.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 16:14:13.939768 cy_account-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-06-26 16:14:09.000000 cy_account-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:17:13.762780 cy_account-0.1.3/
+-rw-rw-rw-   0        0        0      303 2023-06-26 16:17:13.761779 cy_account-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-26 16:03:11.000000 cy_account-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 16:17:13.745795 cy_account-0.1.3/cy_account/
+-rw-rw-rw-   0        0        0     7962 2023-06-26 16:16:38.000000 cy_account-0.1.3/cy_account/__init__.py
+-rw-rw-rw-   0        0        0     4979 2023-06-26 16:01:45.000000 cy_account-0.1.3/cy_account/account_api.py
+-rw-rw-rw-   0        0        0     2415 2023-06-26 14:36:56.000000 cy_account-0.1.3/cy_account/cy_request.py
+-rw-rw-rw-   0        0        0      502 2023-06-26 15:49:30.000000 cy_account-0.1.3/cy_account/test.py
+-rw-rw-rw-   0        0        0      622 2023-06-26 13:51:00.000000 cy_account-0.1.3/cy_account/user_info.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:17:13.760780 cy_account-0.1.3/cy_account.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 16:17:13.762780 cy_account-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-06-26 16:17:12.000000 cy_account-0.1.3/setup.py
```

### Comparing `cy_account-0.1.2/cy_account/__init__.py` & `cy_account-0.1.3/cy_account/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = []
+__all__ = ["UserInfo", "AccountAPI", "ServerForRequest"]
 
 from typing import Optional
 from pydantic import BaseModel, ValidationError
 
 import json
 import requests
 import redis as redis
```

### Comparing `cy_account-0.1.2/cy_account/account_api.py` & `cy_account-0.1.3/cy_account/account_api.py`

 * *Files identical despite different names*

### Comparing `cy_account-0.1.2/cy_account/cy_request.py` & `cy_account-0.1.3/cy_account/cy_request.py`

 * *Files identical despite different names*

### Comparing `cy_account-0.1.2/cy_account/user_info.py` & `cy_account-0.1.3/cy_account/user_info.py`

 * *Files identical despite different names*

### Comparing `cy_account-0.1.2/setup.py` & `cy_account-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="cy_account",
-    version="0.1.2",
+    version="0.1.3",
     author="luyuan",
     author_email="136735431@qq.com",
     description="edited by myself",
     py_modules=["cy_account"],
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent"],
```

