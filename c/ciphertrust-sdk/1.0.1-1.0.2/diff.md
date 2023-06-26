# Comparing `tmp/ciphertrust-sdk-1.0.1.tar.gz` & `tmp/ciphertrust-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciphertrust-sdk-1.0.1.tar", last modified: Tue Jun  6 14:06:13 2023, max compression
+gzip compressed data, was "ciphertrust-sdk-1.0.2.tar", last modified: Mon Jun 26 14:00:25 2023, max compression
```

## Comparing `ciphertrust-sdk-1.0.1.tar` & `ciphertrust-sdk-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-06 14:06:13.812700 ciphertrust-sdk-1.0.1/
--rw-rw-r--   0 adamt      (501) staff       (20)     1064 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/LICENSE
--rw-r--r--   0 adamt      (501) staff       (20)     3179 2023-06-06 14:06:13.812222 ciphertrust-sdk-1.0.1/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)     1495 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/README.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-06 14:06:13.805147 ciphertrust-sdk-1.0.1/ciphertrust_sdk.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)     3179 2023-06-06 14:06:13.000000 ciphertrust-sdk-1.0.1/ciphertrust_sdk.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      492 2023-06-06 14:06:13.000000 ciphertrust-sdk-1.0.1/ciphertrust_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-06-06 14:06:13.000000 ciphertrust-sdk-1.0.1/ciphertrust_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       80 2023-06-06 14:06:13.000000 ciphertrust-sdk-1.0.1/ciphertrust_sdk.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)       12 2023-06-06 14:06:13.000000 ciphertrust-sdk-1.0.1/ciphertrust_sdk.egg-info/top_level.txt
--rw-rw-r--   0 adamt      (501) staff       (20)     1034 2023-06-06 14:06:01.000000 ciphertrust-sdk-1.0.1/pyproject.toml
--rw-r--r--   0 adamt      (501) staff       (20)       38 2023-06-06 14:06:13.812861 ciphertrust-sdk-1.0.1/setup.cfg
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-06 14:06:13.801808 ciphertrust-sdk-1.0.1/src/
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-06 14:06:13.811431 ciphertrust-sdk-1.0.1/src/ciphertrust/
--rw-rw-r--   0 adamt      (501) staff       (20)      134 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/_version.py
--rw-rw-r--   0 adamt      (501) staff       (20)     5441 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/api.py
--rw-rw-r--   0 adamt      (501) staff       (20)     7290 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/auth.py
--rw-rw-r--   0 adamt      (501) staff       (20)      248 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/config.py
--rw-rw-r--   0 adamt      (501) staff       (20)      471 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/exceptions.py
--rw-rw-r--   0 adamt      (501) staff       (20)     3719 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/models.py
--rw-rw-r--   0 adamt      (501) staff       (20)     3972 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/requestapi.py
--rw-rw-r--   0 adamt      (501) staff       (20)      244 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/static.py
--rw-rw-r--   0 adamt      (501) staff       (20)     6291 2023-06-06 13:48:10.000000 ciphertrust-sdk-1.0.1/src/ciphertrust/utils.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-26 14:00:25.462445 ciphertrust-sdk-1.0.2/
+-rw-rw-r--   0 adamt      (501) staff       (20)     1064 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/LICENSE
+-rw-r--r--   0 adamt      (501) staff       (20)     4532 2023-06-26 14:00:25.462011 ciphertrust-sdk-1.0.2/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)     2849 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/README.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-26 14:00:25.457085 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)     4532 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      492 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       94 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       12 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)     1054 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/pyproject.toml
+-rw-r--r--   0 adamt      (501) staff       (20)       38 2023-06-26 14:00:25.462564 ciphertrust-sdk-1.0.2/setup.cfg
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-26 14:00:25.454062 ciphertrust-sdk-1.0.2/src/
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-26 14:00:25.461502 ciphertrust-sdk-1.0.2/src/ciphertrust/
+-rw-rw-r--   0 adamt      (501) staff       (20)      134 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/_version.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     6353 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/api.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     8075 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/auth.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      248 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/config.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      471 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/exceptions.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     3721 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/models.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     9785 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/requestapi.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      417 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/static.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     6720 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/utils.py
```

### Comparing `ciphertrust-sdk-1.0.1/LICENSE` & `ciphertrust-sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.1/PKG-INFO` & `ciphertrust-sdk-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciphertrust-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thales CipherTrust SDK RestAPI
 Author-email: atav928 <dev@tavnets.com>
 License: MIT License
         
         Copyright (c) 2023 atav928
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -99,7 +99,49 @@
         "algorithm": "",
         "size": 0,
         "muid": ""
       }
     ]
 }
 ```
+
+## Version
+
+| Version | Build | Changes |
+| ------- | ----- | ------- |
+| **0.0.1** | **final** | Test Relese; basic functionality |
+| **1.0.1** | **final** | Available Release with API and Auth functionality |
+| **1.0.2** | **a1** | Removed print |
+| **1.0.2** | **a2** | Added metrics in calls and additional awaits to call on mutliple calls |
+| **1.0.2** | **final** | See notes below |
+
+### Known Bugs/Futue Features
+
+__TODO:__
+
+* &#9745; Create a metrics fucntion to return
+* &#9745; Delete all private aand passwords being printed
+* &#9744; Add logging or streaming or none
+* &#9744; Add own metrics
+  * &#9744; Generic metrics wrapper
+  * &#9744; Logging metrics wrapper
+* &#9745; Create an average, mean, total time depending on calls being made for when you want to do a full list of keys
+* &#9745; Missing delete https action
+
+#### Release Notes
+
+#### v1.0.2
+
+* Added Generic Metrics to each call with additional statistics that can be used.
+* Added async to handle multle requests; still need to take advantage of it.
+* Removed disclosure of secrets in debug prints.
+
+__Known Bugs:__
+
+* Too many calls cause crash or non-responsive requests leading to time out.
+
+#### v1.0.1
+
+Initial usable release
+
+* Allows ability to run get functions in a wrapper.
+* Supply all changes and updates with the standard get request using the api.get() call.
```

### Comparing `ciphertrust-sdk-1.0.1/ciphertrust_sdk.egg-info/PKG-INFO` & `ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciphertrust-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thales CipherTrust SDK RestAPI
 Author-email: atav928 <dev@tavnets.com>
 License: MIT License
         
         Copyright (c) 2023 atav928
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -99,7 +99,49 @@
         "algorithm": "",
         "size": 0,
         "muid": ""
       }
     ]
 }
 ```
+
+## Version
+
+| Version | Build | Changes |
+| ------- | ----- | ------- |
+| **0.0.1** | **final** | Test Relese; basic functionality |
+| **1.0.1** | **final** | Available Release with API and Auth functionality |
+| **1.0.2** | **a1** | Removed print |
+| **1.0.2** | **a2** | Added metrics in calls and additional awaits to call on mutliple calls |
+| **1.0.2** | **final** | See notes below |
+
+### Known Bugs/Futue Features
+
+__TODO:__
+
+* &#9745; Create a metrics fucntion to return
+* &#9745; Delete all private aand passwords being printed
+* &#9744; Add logging or streaming or none
+* &#9744; Add own metrics
+  * &#9744; Generic metrics wrapper
+  * &#9744; Logging metrics wrapper
+* &#9745; Create an average, mean, total time depending on calls being made for when you want to do a full list of keys
+* &#9745; Missing delete https action
+
+#### Release Notes
+
+#### v1.0.2
+
+* Added Generic Metrics to each call with additional statistics that can be used.
+* Added async to handle multle requests; still need to take advantage of it.
+* Removed disclosure of secrets in debug prints.
+
+__Known Bugs:__
+
+* Too many calls cause crash or non-responsive requests leading to time out.
+
+#### v1.0.1
+
+Initial usable release
+
+* Allows ability to run get functions in a wrapper.
+* Supply all changes and updates with the standard get request using the api.get() call.
```

### Comparing `ciphertrust-sdk-1.0.1/pyproject.toml` & `ciphertrust-sdk-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 ]
 dynamic = ["version", "readme"]
 dependencies = [
     "orjson==3.8.*",
     "PyJWT==2.7.*",
     "requests==2.31.*",
     "dataclasses==0.6",
-    "validators==0.20.*"
+    "validators==0.20.*",
+    "httpx==0.24.*"
 ]
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"], content-type = "text/markdown"}
 version = {attr = "ciphertrust.__version__"}
 
 [tool.setuptools.packages.find]
@@ -35,8 +36,8 @@
 exclude = ["*.xml"]
 namespaces = true
 
 [tool.coverage.run]
 source = ["src"]
 
 [tool.pylint]
-max-line-length = 101
+max-line-length = 101
```

### Comparing `ciphertrust-sdk-1.0.1/src/ciphertrust/api.py` & `ciphertrust-sdk-1.0.2/src/ciphertrust/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,44 +2,57 @@
 """API"""
 
 from typing import Any, Dict
 import orjson
 
 from ciphertrust import config
 from ciphertrust.auth import Auth
-from ciphertrust.requestapi import ctm_request
+from ciphertrust.requestapi import (ctm_request, asyn_get_all)
 from ciphertrust.static import ENCODE
 
 
 class API:
     """CipherTrust Manager API"""
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any):
         self.auth = Auth(**kwargs)
 
         # Bind API method classes to this object
-        subclasses = self._subclass_container()
-        self.get = subclasses['get']()
+        subclasses: dict[str, Any] = self._subclass_container()
+        self.get = subclasses["get"]()
+        self.post = subclasses["post"]()
+        self.patch = subclasses["patch"]()
+        self.delete = subclasses["delete"]()
 
-    def _subclass_container(self):
+    def _subclass_container(self) -> dict[str,Any]:
         _parent_class = self
-        return_object = {}
+        return_object: dict[str,Any] = {}
 
         class GetWrapper(Get):
-            def __init__(self):
+            def __init__(self) -> None:
                 self._parent_class = _parent_class
         return_object["get"] = GetWrapper
 
         class PostWrapper(Post):
-            def __init__(self):
+            def __init__(self) -> None:
                 self._parent_class = _parent_class
         return_object["post"] = PostWrapper
+
+        class PatchWrapper(Patch):
+            def __init__(self) -> None:
+                self._parent_class = _parent_class
+        return_object["patch"] = PatchWrapper
+
+        class DeleteWrapper(Delete):
+            def __init__(self) -> None:
+                self._parent_class = _parent_class
+        return_object["delete"] = DeleteWrapper
         return return_object
 
-    def convert_to_string(self, query: dict) -> str:
+    def convert_to_string(self, query: dict[str,Any]) -> str:
         """convert json to string
 
         :param query: _description_
         :type query: dict
         :return: _description_
         :rtype: str
         """
@@ -51,92 +64,96 @@
 
     :return: _description_
     :rtype: _type_
     """
     _parent_class = None
     method = "GET"
 
-    def call(self, url_path: str, **kwargs) -> dict[str, Any]:
+    def call(self, url_path: str, **kwargs: Any) -> dict[str, Any]:
         """Generic Call Method
 
         :param url_path: _description_
         :type url_path: str
         :return: _description_
         :rtype: dict[str, Any]
         """
-        url: str = config.API_URL.format(self._parent_class.auth.hostname, url_path)
-        params: dict = kwargs.pop("params", {})
-        response: dict[str, Any] = ctm_request(auth=self._parent_class.auth,
-                                               url=url,
-                                               method=self.method,
-                                               params=params,
-                                               timeout=self._parent_class.auth.timeout,
-                                               verify=self._parent_class.auth.verify)
-        print(f"{response=}")
+        url: str = config.API_URL.format(self._parent_class.auth.hostname, # type: ignore
+                                         url_path)
+        params: dict[str,Any] = kwargs.pop("params", {})
+        calls = {
+            "standard": ctm_request,
+            "list_all": asyn_get_all
+        }
+        get_all = "list_all" if kwargs.get("get_all", False) else "standard"
+        response: dict[str,Any] = calls[get_all](auth=self._parent_class.auth, # type: ignore
+                                                 url=url,
+                                                 method=self.method, # type: ignore
+                                                 params=params,
+                                                 timeout=self._parent_class.auth.timeout, # type: ignore
+                                                 verify=self._parent_class.auth.verify) # type: ignore
         return response
 
 
 class Post:
     """Calls generic POST requests for CipherTrust Manager
 
     :return: _description_
     :rtype: _type_
     """
     _parent_class = None
     method: str = "POST"
 
-    def call(self, url_path: str, **kwargs) -> Dict[str, Any]:
+    def call(self, url_path: str, **kwargs: Any) -> Dict[str, Any]:
         """POST call for CipherTrust Manager
 
         :param url_path: _description_
         :type url_path: str
         """
-        url: str = config.API_URL.format(self._parent_class.auth.hostname, url_path)
-        params: dict = kwargs.pop("params", {})
-        data: str = self._parent_class.convert_to_string(
+        url: str = config.API_URL.format(self._parent_class.auth.hostname, url_path) # type: ignore
+        params: dict[str,Any] = kwargs.pop("params", {})
+        data: str = self._parent_class.convert_to_string( # type: ignore
             query=kwargs.pop("query")) if kwargs.get("query") else ""
-        response: dict[str, Any] = ctm_request(auth=self._parent_class.auth,
+        response: dict[str, Any] = ctm_request(auth=self._parent_class.auth, # type: ignore
                                                method=self.method,
                                                url=url,
                                                params=params,
                                                data=data,
                                                timeout=self._parent_class.auth.timeout,
                                                verify=self._parent_class.auth.verify)
-        print(f"{response=}")
         return response
 
 
 class Delete:
     """DELETE API Calls"""
     _parent_class = None
     method: str = "DELETE"
 
-    def call(self, url_path: str, **kwargs) -> dict[str, Any]:
+    def call(self, url_path: str, **kwargs: Any) -> dict[str, Any]:
         """DELETE call for CipherTrust Manager
 
         :param url_path: _description_
         :type url_path: str
         :return: _description_
         :rtype: dict[str, Any]
         """
         url: str = config.API_URL.format(self._parent_class.auth.hostname, url_path)
         response: dict[str, Any] = ctm_request(auth=self._parent_class.auth,
                                                url=url,
                                                method=self.method,
                                                timeout=self._parent_class.auth.timeout,
                                                verify=self._parent_class.auth.verify)
-        print(f"{response=}")
+        # print(f"{response=}")
         return response
 
 
 class Patch:
     _parent_class = None
     method: str = "PATCH"
 
-    def call(self, url_path, **kwargs) -> Dict[str, Any]:
+    def call(self, url_path: str, **kwargs: Any) -> Dict[str, Any]:
         """CipherTrust API Patch calls
 
         :param url_path: _description_
         :type url_path: _type_
         :return: _description_
         :rtype: Dict[str,Any]
         """
@@ -147,9 +164,9 @@
         response: dict[str, Any] = ctm_request(auth=self._parent_class.auth,
                                                url=url,
                                                method=self.method,
                                                params=params,
                                                data=data,
                                                timeout=self._parent_class.auth.timeout,
                                                verify=self._parent_class.auth.verify)
-        print(f"{response=}")
+        # print(f"{response=}")
         return response
```

### Comparing `ciphertrust-sdk-1.0.1/src/ciphertrust/auth.py` & `ciphertrust-sdk-1.0.2/src/ciphertrust/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=missing-function-docstring,raise-missing-from
 """Authorization"""
 
 from typing import Dict, Any
 import time
+import statistics
 # from urllib.parse import urlparse
 
 import jwt
 import requests
 from requests import HTTPError, Response
 import orjson
 
@@ -34,49 +35,53 @@
     expiration: int
     refresh_token_id: str
     refresh_token: str
     token: str
     token_type: str
     refresh_authparams: AuthParams
     auth_response: Dict[str, Any] = {}
-    refresh_token_expires_in: int = 0
-    duration: int = 300
+    exec_time_elapsed: list[float] = []
+    exec_time_stdev: float = 0.0
+    exec_time_min: float = 0.0
+    exec_time_max: float = 0.0
+    exec_time: float = 0.0
+    duration: int = 240
     refresh_params: Dict[str, Any] = {}
 
     def __init__(self, **kwargs: Dict[str, Any]) -> None:
         authparams: Dict[str, Any] = AuthParams(**kwargs).asdict()  # type: ignore
-        print(f"{authparams=}")
+        # print(f"{authparams=}")
         try:
             self.hostname: str = authparams.pop("hostname")
             self.timeout: int = authparams.pop("timeout")
             self.verify: Any = authparams.pop("verify")
             self.headers: Dict[str, Any] = authparams.pop("headers")
             self.__renew_refresh_token: bool = authparams.pop("renew_refresh_token", False)
         except KeyError as err:
             error: str = reformat_exception(err)
             raise CipherValueError(f"Invalid value: {error}")
         self.payload: Dict[str, Any] = self._create_payload(authparams)
         self.url: str = config.AUTH.format(self.hostname)
-        print(f"{self.url}")
+        # print(f"{self.url}")
         self.gen_token()
 
     @property
     def renew_refresh_token(self):
         return self.__renew_refresh_token
 
     @renew_refresh_token.setter
     def renew_refresh_token(self, value: bool):
         if not isinstance(value, bool):
             raise CipherValueError(f"Invalid value for renew_refresh_token: {value}")
         self.__renew_refresh_token = value
 
     def _create_payload(self, payload: Dict[str, Any]) -> Dict[str, Any]:
-        print(f"{payload=}")
+        # print(f"{payload=}")
         response: Dict[str, Any] = default_payload(**payload)
-        print(f"createdpayload={response}")
+        # print(f"createdpayload={response}")
         return response
 
     def _jwt_decode(self, jwt_token: str) -> Dict[str, Any]:
         jwt_decrypted: dict[str, Any] = jwt.decode(jwt_token,  # type: ignore
                                                    options={"verify_signature": False})
         self.expiration = jwt_decrypted["exp"]
         return jwt_decrypted
@@ -84,42 +89,58 @@
     def gen_token(self) -> None:
         """_summary_
 
         :return: _description_
         :rtype: Dict[str,Any]
         """
         data: str = orjson.dumps(self.payload).decode(ENCODE)  # pylint: disable=no-member
-        print(
-            f"method={self.method}|url={self.url}|data={data}|timeout={self.timeout}|verify={self.verify}|headers={self.headers}")
+        # print(f"method={self.method}|url={self.url}|data={data}|timeout={self.timeout}|verify={self.verify}|headers={self.headers}")
         response: Response = self._request(data=data)
-        print(f"response={response.json()}|code={response.status_code}")
+        # print(f"response={response.json()}|code={response.status_code}")
         self.api_raise_error(response)
         try:
             jwt_decode: Dict[str, Any] = self._jwt_decode(response.json()["jwt"])
         except KeyError:
             raise CipherAPIError("No token in response")
+        self._update_exec_time(response.elapsed.total_seconds())
         response_json: Dict[str, Any] = response.json()
         response_json["jwt_decode"] = jwt_decode
-        print(f"{response_json=}")
+        # print(f"{response_json=}")
         self._update_token_info(response_json=response_json)
 
     def gen_refresh_token(self) -> None:
         payload: Dict[str, Any] = self._create_payload(self.refresh_authparams.asdict())
         data: str = orjson.dumps(payload).decode(ENCODE)  # pylint: disable=no-member
         response: Response = self._request(data=data)
-        print(f"response_code{response.status_code}|response={response.json()}")
+        # print(f"response_code{response.status_code}|response={response.json()}")
         self.api_raise_error(response=response)
         try:
             jwt_decode: Dict[str, Any] = self._jwt_decode(response.json()["jwt"])
         except KeyError:
             raise CipherAPIError("No token in response")
+        self._update_exec_time(response.elapsed.total_seconds())
         response_json: Dict[str, Any] = response.json()
         response_json["jwt_decode"] = jwt_decode
         self._update_token_info(response_json=response_json)
 
+    def _update_exec_time(self, exec_time: float) -> None:
+        """Updates Execution Times to track 
+
+        :param exec_time: _description_
+        :type exec_time: float
+        """
+        self.exec_time = exec_time
+        self.exec_time_elapsed.append(exec_time)
+        self.exec_time_min = min(self.exec_time_elapsed)
+        self.exec_time_max = max(self.exec_time_elapsed)
+        self.exec_time_stdev = 0.0 if len(
+            self.exec_time_elapsed) <= 1 else statistics.stdev(
+            self.exec_time_elapsed)
+    
+
     def _update_token_info(self, response_json: Dict[str, Any]):
         self.expiration = response_json["jwt_decode"]["exp"]
         self.issued_at = response_json["jwt_decode"]["iat"]
         self.refresh_token = response_json["refresh_token"]
         self.token = response_json["jwt"]
         self.token_type: str = response_json["token_type"]
         self.refresh_token_id = response_json["refresh_token_id"]
@@ -148,17 +169,14 @@
         """Raises error if response not what was expected
 
         :param response: Request Response
         :type response: Response
         :raises CipherAuthError: Authorization Error
         :raises CipherAPIError: Generic API Error
         """
-        # if response.status_code == 403:
-        #    message = response.json().get("message", "Permission Denied")
-        #    raise CipherAuthError(message)
         try:
             response.raise_for_status()
         except HTTPError as err:
             error: str = reformat_exception(err)
             raise CipherAPIError(f"{error=}|response={response.text}")
         if not (response.status_code >= 200 or response.status_code < 299):
             raise CipherAPIError(response.json())
@@ -166,11 +184,13 @@
 
 # refersh token decorator
 def refresh_token(decorated):  # type: ignore
     def wrapper(auth: Auth, **kwargs: Dict[str, Any]) -> Any:
         try:
             if time.time() >= auth.expiration:
                 auth.gen_refresh_token()
+                # print("Generatinga new token|auth.expiration=",
+                #       f"{auth.expiration}|issued={auth.issued_at}")
         except KeyError:
             raise CipherAuthError(f"Invalid Authorization {auth}")
         return decorated(auth, **kwargs)
     return wrapper
```

### Comparing `ciphertrust-sdk-1.0.1/src/ciphertrust/models.py` & `ciphertrust-sdk-1.0.2/src/ciphertrust/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,8 +104,8 @@
         "headers": {
             "Content-Type": "application/json",
             "Accept": "application/json"
         },
         "ext": "value"
     }
     authparam: dict[str, Any] = AuthParams(**sample).asdict()
-    print(f"{authparam=}")
+    # print(f"{authparam=}")
```

### Comparing `ciphertrust-sdk-1.0.1/src/ciphertrust/utils.py` & `ciphertrust-sdk-1.0.2/src/ciphertrust/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 """Utilities"""
 
+import time
 from typing import Dict, Any
 
 import validators
 
 from ciphertrust.exceptions import CipherValueError
 
+def concat_resources(dict1, dict2) -> list[dict[str,Any]]:
+    """Use reduce to generate a list of resources
+
+    :param dict1: _description_
+    :type dict1: _type_
+    :param dict2: _description_
+    :type dict2: _type_
+    :return: _description_
+    :rtype: list[dict[str,Any]]
+    """
+    for key in dict2:
+        if key in dict1 and key == "resources":
+            dict1[key] += dict2[key]
+    return dict1
 
 def reformat_exception(error: Exception) -> str:
     """Reformates Exception to print out as a string pass for logging
 
     Args:
         error (Exception): _description_
 
@@ -190,11 +205,11 @@
     except KeyError as err:
         error: str = reformat_exception(err)
         raise CipherValueError(f"Invalid value: {error}")
 
 
 if __name__ == "__main__":
     valididate_list: list[str] = ["invalid", "valid-domain.example.com", "invalid_domain*.com"]
-    print(f"Checking domain validation against list: {', '.join(valididate_list)}")
+    # print(f"Checking domain validation against list: {', '.join(valididate_list)}")
     for _ in valididate_list:
         is_valid = validate_domain(_)
-        print(f"{_} is {str(is_valid)}")
+        # print(f"{_} is {str(is_valid)}")
```

