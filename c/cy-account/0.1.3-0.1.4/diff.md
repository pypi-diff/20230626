# Comparing `tmp/cy_account-0.1.3.tar.gz` & `tmp/cy_account-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cy_account-0.1.3.tar", last modified: Mon Jun 26 16:17:13 2023, max compression
+gzip compressed data, was "cy_account-0.1.4.tar", last modified: Mon Jun 26 16:23:33 2023, max compression
```

## Comparing `cy_account-0.1.3.tar` & `cy_account-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:17:13.762780 cy_account-0.1.3/
--rw-rw-rw-   0        0        0      303 2023-06-26 16:17:13.761779 cy_account-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-26 16:03:11.000000 cy_account-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 16:17:13.745795 cy_account-0.1.3/cy_account/
--rw-rw-rw-   0        0        0     7962 2023-06-26 16:16:38.000000 cy_account-0.1.3/cy_account/__init__.py
--rw-rw-rw-   0        0        0     4979 2023-06-26 16:01:45.000000 cy_account-0.1.3/cy_account/account_api.py
--rw-rw-rw-   0        0        0     2415 2023-06-26 14:36:56.000000 cy_account-0.1.3/cy_account/cy_request.py
--rw-rw-rw-   0        0        0      502 2023-06-26 15:49:30.000000 cy_account-0.1.3/cy_account/test.py
--rw-rw-rw-   0        0        0      622 2023-06-26 13:51:00.000000 cy_account-0.1.3/cy_account/user_info.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:17:13.760780 cy_account-0.1.3/cy_account.egg-info/
--rw-rw-rw-   0        0        0      303 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 16:17:13.000000 cy_account-0.1.3/cy_account.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 16:17:13.762780 cy_account-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-06-26 16:17:12.000000 cy_account-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:23:33.108945 cy_account-0.1.4/
+-rw-rw-rw-   0        0        0      303 2023-06-26 16:23:33.107939 cy_account-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-26 16:03:11.000000 cy_account-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 16:23:33.082938 cy_account-0.1.4/cy_account/
+-rw-rw-rw-   0        0        0     8154 2023-06-26 16:23:24.000000 cy_account-0.1.4/cy_account/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-06-26 15:49:30.000000 cy_account-0.1.4/cy_account/test.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:23:33.105954 cy_account-0.1.4/cy_account.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-06-26 16:23:32.000000 cy_account-0.1.4/cy_account.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-06-26 16:23:33.000000 cy_account-0.1.4/cy_account.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 16:23:32.000000 cy_account-0.1.4/cy_account.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-26 16:23:32.000000 cy_account-0.1.4/cy_account.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 16:23:32.000000 cy_account-0.1.4/cy_account.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 16:23:33.108945 cy_account-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-06-26 16:23:28.000000 cy_account-0.1.4/setup.py
```

### Comparing `cy_account-0.1.3/cy_account/__init__.py` & `cy_account-0.1.4/cy_account/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,31 +165,36 @@
         if r:
             return json.loads(r)['client_secret']
         else:
             raise Exception('核心代码出现异常：无法获取到解密的client_secret')
 
 
 class ServerForRequest:
-    APP_ID = 0
+    APP_ID: str
 
     @staticmethod
-    def set_app_id(app_id: int):
+    def set_app_id(app_id: str):
         ServerForRequest.APP_ID = app_id
 
     @staticmethod
     def __get_url(server_name: str, path: str):
         if path.startswith('/'):
             url = f"http://{server_name}{path}"
         else:
             url = f"http://{server_name}/{path}"
         # print(url)
         return url
 
     @staticmethod
     def __get_header():
+
+        app_id = ServerForRequest.APP_ID
+        if not app_id:
+            raise ValueError("APP_ID 错误，请在启动的时候调用ServerForRequest.set_app_id()完成初始化")
+
         return {
             'X-APP-ID': ServerForRequest.APP_ID,
             # 'X-Request-Id': thread_local.request_id
         }
 
     @staticmethod
     def __before(response):
```

### Comparing `cy_account-0.1.3/setup.py` & `cy_account-0.1.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="cy_account",
-    version="0.1.3",
+    version="0.1.4",
     author="luyuan",
     author_email="136735431@qq.com",
     description="edited by myself",
     py_modules=["cy_account"],
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent"],
```

