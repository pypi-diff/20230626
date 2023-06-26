# Comparing `tmp/braincube-aws-core-0.0.5.tar.gz` & `tmp/braincube-aws-core-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-0.0.5.tar", last modified: Fri Jun 23 09:50:12 2023, max compression
+gzip compressed data, was "braincube-aws-core-0.0.6.tar", last modified: Mon Jun 26 10:53:08 2023, max compression
```

## Comparing `braincube-aws-core-0.0.5.tar` & `braincube-aws-core-0.0.6.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.851637 braincube-aws-core-0.0.5/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-23 09:50:12.851879 braincube-aws-core-0.0.5/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8009 2023-06-21 20:23:04.000000 braincube-aws-core-0.0.5/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-23 09:50:12.853186 braincube-aws-core-0.0.5/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.833845 braincube-aws-core-0.0.5/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.839420 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      897 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.840020 braincube-aws-core-0.0.5/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.843306 braincube-aws-core-0.0.5/src/core/app/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/app/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-0.0.5/src/core/app/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      664 2023-06-21 16:34:05.000000 braincube-aws-core-0.0.5/src/core/app/app_event.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6598 2023-06-23 09:47:26.000000 braincube-aws-core-0.0.5/src/core/app/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4665 2023-06-22 09:23:59.000000 braincube-aws-core-0.0.5/src/core/app/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      479 2023-06-21 17:15:33.000000 braincube-aws-core-0.0.5/src/core/app/exception_handler.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.846017 braincube-aws-core-0.0.5/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.5/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.5/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.5/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    33246 2023-06-22 15:26:24.000000 braincube-aws-core-0.0.5/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.847782 braincube-aws-core-0.0.5/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.5/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.5/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.849763 braincube-aws-core-0.0.5/src/core/rules_engine/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/rules_engine/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.5/src/core/rules_engine/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.5/src/core/rules_engine/exceptions.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.5/src/core/rules_engine/rule_manager.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.851263 braincube-aws-core-0.0.5/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.5/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.5/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 10:53:08.589641 braincube-aws-core-0.0.6/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.6/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-26 10:53:08.589929 braincube-aws-core-0.0.6/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8009 2023-06-21 20:23:04.000000 braincube-aws-core-0.0.6/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.6/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-26 10:53:08.591216 braincube-aws-core-0.0.6/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.6/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 10:53:08.562296 braincube-aws-core-0.0.6/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 10:53:08.567457 braincube-aws-core-0.0.6/src/braincube_aws_core.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-26 10:53:08.000000 braincube-aws-core-0.0.6/src/braincube_aws_core.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      932 2023-06-26 10:53:08.000000 braincube-aws-core-0.0.6/src/braincube_aws_core.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-26 10:53:08.000000 braincube-aws-core-0.0.6/src/braincube_aws_core.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-26 10:53:08.000000 braincube-aws-core-0.0.6/src/braincube_aws_core.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-26 10:53:08.000000 braincube-aws-core-0.0.6/src/braincube_aws_core.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 10:53:08.567926 braincube-aws-core-0.0.6/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.6/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 10:53:08.575748 braincube-aws-core-0.0.6/src/core/app/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.6/src/core/app/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2971 2023-06-26 09:56:02.000000 braincube-aws-core-0.0.6/src/core/app/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1872 2023-06-26 06:47:29.000000 braincube-aws-core-0.0.6/src/core/app/app_event.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     5055 2023-06-26 10:17:54.000000 braincube-aws-core-0.0.6/src/core/app/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      489 2023-06-26 06:58:32.000000 braincube-aws-core-0.0.6/src/core/app/app_processor.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     5462 2023-06-26 08:24:01.000000 braincube-aws-core-0.0.6/src/core/app/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      680 2023-06-26 08:19:40.000000 braincube-aws-core-0.0.6/src/core/app/http_exception_handler.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 10:53:08.580257 braincube-aws-core-0.0.6/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.6/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.6/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.6/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.6/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33246 2023-06-22 15:26:24.000000 braincube-aws-core-0.0.6/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 10:53:08.582960 braincube-aws-core-0.0.6/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.6/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.6/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.6/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 10:53:08.586510 braincube-aws-core-0.0.6/src/core/rules_engine/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.6/src/core/rules_engine/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.6/src/core/rules_engine/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.6/src/core/rules_engine/exceptions.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.6/src/core/rules_engine/rule_manager.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 10:53:08.589043 braincube-aws-core-0.0.6/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.6/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.6/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.6/src/core/utils/data.py
```

### Comparing `braincube-aws-core-0.0.5/LICENSE` & `braincube-aws-core-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/PKG-INFO` & `braincube-aws-core-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.5
+Version: 0.0.6
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-0.0.5/README.md` & `braincube-aws-core-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/setup.cfg` & `braincube-aws-core-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core
-version = 0.0.5
+version = 0.0.6
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/PKG-INFO` & `braincube-aws-core-0.0.6/src/braincube_aws_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.5
+Version: 0.0.6
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/SOURCES.txt` & `braincube-aws-core-0.0.6/src/braincube_aws_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 src/braincube_aws_core.egg-info/requires.txt
 src/braincube_aws_core.egg-info/top_level.txt
 src/core/__init__.py
 src/core/app/__init__.py
 src/core/app/app_controller.py
 src/core/app/app_event.py
 src/core/app/app_module.py
+src/core/app/app_processor.py
 src/core/app/data.py
-src/core/app/exception_handler.py
+src/core/app/http_exception_handler.py
 src/core/dal/__init__.py
 src/core/dal/data.py
 src/core/dal/database_errors.py
 src/core/dal/postgres_connection.py
 src/core/dal/postgres_repository.py
 src/core/di/__init__.py
 src/core/di/data.py
```

### Comparing `braincube-aws-core-0.0.5/src/core/app/app_controller.py` & `braincube-aws-core-0.0.6/src/core/app/app_controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,38 @@
-class AppController:
-    """Module with which you can define endpoints.
+from .data import HTTPRequest
+from .app_processor import AppProcessor
+
+
+class AppController(AppProcessor):
+    """Module with which you can define AWS APIGateway endpoints.
     :param base_path: base resource url.
     """
 
     def __init__(self, base_path: str):
-        self.routes = dict()
+        self._routes = dict()
         self._base_url = base_path
 
+    @property
+    def data_type(self) -> type:
+        return HTTPRequest
+
+    @property
+    def handlers(self) -> dict[str, tuple[callable, str | None]]:
+        return self._routes
+
     def route(self, path: str, method: str, qualifier: str = None):
         """Function that represents an endpoint.
         :param path: Resource url.
         :param method: HTTP method.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         def _route(func: callable):
-            path_ = f"{self._base_url}{path}"
-            if path_ not in self.routes:
-                self.routes[path_] = dict()
-            self.routes[path_][method] = func, qualifier
+            self._routes[f"{self._base_url}{path}::{method}"] = func, qualifier
             return func
 
         return _route
 
     def get(self, path: str = "", qualifier: str = None):
         """Function that represents an HTTP GET method endpoint.
         :param path: Resource url.
```

### Comparing `braincube-aws-core-0.0.5/src/core/app/data.py` & `braincube-aws-core-0.0.6/src/core/app/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import json
 from enum import Enum
+from json import loads
 from http import HTTPStatus
 from dataclasses import dataclass
 from typing import Generic, TypeVar, Type
 from pydantic import BaseModel, Field
 
 from ..utils.convert import try_str_to_float
 from ..utils.data import Order, OrderType, Condition, ConditionType, Pageable
@@ -11,19 +11,14 @@
 T = TypeVar("T")
 
 
 ####################################
 # Cognito
 ####################################
 
-class EventType(Enum):
-    sqs = 1
-    cognito = 2
-
-
 class CallerContext(BaseModel):
     aws_sdk_version: str = Field(alias="awsSdkVersion")
     client_id: str = Field(alias="clientId")
 
 
 class UserPoolEvent(BaseModel):
     version: str
@@ -33,90 +28,127 @@
     user_name: str = Field(alias="userName")
     caller_context: CallerContext = Field(alias="callerContext")
     request: dict
     response: dict
 
 
 ####################################
-# Rest API
+# Event
 ####################################
 
-reserved_keys = ["fields", "pageNo", "pageSize", "topSize", "order"]
+class EventType(Enum):
+    sqs = 1
+    cognito = 2
 
 
 @dataclass()
-class HTTPResponse:
-    status: HTTPStatus = HTTPStatus.OK
-    body: any = None
-    headers: dict[str, any] = None
+class EventPayload(Generic[T]):
+    event: T
+    context: dict
 
 
-@dataclass()
-class QueryParams:
-    fields: list[str] = None
-    conditions: list[Condition] = None
-    page: Pageable = Pageable()
-    order: list[Order] = None
-
+####################################
+# APIGateway
+####################################
 
 @dataclass()
 class AuthUser:
     cognito_id: str = None
     email: str = None
     email_confirmed: bool = False
 
 
 @dataclass()
+class QueryParams:
+    fields: list[str] = None
+    conditions: list[Condition] = None
+    page: Pageable = Pageable()
+    order: list[Order] = None
+
+
+@dataclass()
 class HTTPRequest(Generic[T]):
     body: T = None
     headers: dict[str, any] = None
     path_params: dict[str, any] = None
     user: AuthUser = AuthUser()
     query_params: QueryParams = QueryParams()
 
 
-def http_event_to_request(cls: Type[T], event: dict[str, any], context) -> HTTPRequest[T]:
-    data = json.loads(event["body"]) if event.get("body") else None
+@dataclass()
+class HTTPResponse:
+    status: HTTPStatus = HTTPStatus.OK
+    body: any = None
+    headers: dict[str, any] = None
+
+
+####################################
+# Helpers
+####################################
+
+
+@dataclass()
+class Handler:
+    func: callable
+    payload_type: type | None
+    dependencies: list[tuple]
+
+
+http_headers = {
+    "Access-Control-Allow-Origin": "*",
+    "Access-Control-Allow-Methods": "*",
+    "Access-Control-Allow-Credentials": True,
+    "Access-Control-Allow-Headers":
+        "Content-Type,Authorization,X-Amz-Date,X-Api-Key,X-Amz-Security-Token"
+}
+
+
+def convert_to_event_payload(cls: Type[T], event: dict[str, any], context) -> EventPayload[T]:
+    return EventPayload(cls(**event) if cls is not dict else event, context)
+
+
+def convert_to_http_request(cls: Type[T], event: dict[str, any], context) -> HTTPRequest[T]:
+    data = loads(event["body"]) if event.get("body") else None
 
     request = HTTPRequest(body=cls(**data) if cls is not dict else data,
                           headers=event.get("headers"),
                           path_params=event.get("pathParameters"))
 
     if "authorizer" in event["requestContext"]:
         claims = event["requestContext"]["authorizer"]["claims"]
         request.user = AuthUser(claims["sub"], claims["email"], claims["email_verified"] == "true")
 
     params: dict[str, any] | None = event.get("queryStringParameters")
 
     if params:
         fields = params["fields"].replace(" ", "").split(",") if params.get("fields") else list()
-        pageable = Pageable(page_param(params, alias="pageNo"),
-                            page_param(params, alias="pageSize", default=20, max_=50, min_=1),
-                            page_param(params, alias="topSize", max_=1000, min_=-1))
+        pageable = Pageable(_page_param(params, alias="pageNo"),
+                            _page_param(params, alias="pageSize", default=20, max_=50, min_=1),
+                            _page_param(params, alias="topSize", max_=1000, min_=-1))
 
         conditions = list()
         for k, v in params.items():
             key = k.strip()
-            if key in reserved_keys:
+            if key in _reserved_keys:
                 continue
             else:
                 value = v.strip()
                 value_ = value.lower()
                 if value_.startswith("range(") and value_.endswith(")"):
                     condition_type = ConditionType.range
-                    data = condition_param("range", value)
-                    if not len(data) >= 2:
+                    d = _condition_param("range", value)
+                    if not len(d) >= 2:
                         continue
                 elif value_.startswith("any(") and value_.endswith(")"):
                     condition_type = ConditionType.any
-                    data = condition_param("any", value)
+                    d = _condition_param("any", value)
                 else:
                     condition_type = ConditionType.compare
-                    data = try_str_to_float(value)
-                conditions.append(Condition(condition_type, key, data))
+                    d = try_str_to_float(value)
+                conditions.append(Condition(condition_type, key, d))
 
         order = list()
         for order_ in (params["order"].split(",") if params.get("order") else list()):
             o = order_.strip().split(" ")
             if len(o) < 1:
                 continue
             order_type = OrderType.asc
@@ -127,19 +159,22 @@
             order.append(Order(order_type, alias=o[0]))
 
         request.query_params = QueryParams(fields, conditions, pageable, order)
 
     return request
 
 
-def page_param(params: dict[str, any], alias: str, default: int = 0, max_: int = None, min_: int = 0) -> int:
+def _page_param(params: dict[str, any], alias: str, default: int = 0, max_: int = None, min_: int = 0) -> int:
     try:
         if not params.get(alias):
             return default
         value_ = int(params[alias])
         return value_ if (max_ >= value_ >= min_ if max_ else value_ >= min_) else default
     except ValueError:
         return default
 
 
-def condition_param(type_, p) -> list:
+def _condition_param(type_, p) -> list:
     return [try_str_to_float(i) for i in p[len(type_) + 1:len(p) - 1].replace(" ", "").split(",")]
+
+
+_reserved_keys = ["fields", "pageNo", "pageSize", "topSize", "order"]
```

### Comparing `braincube-aws-core-0.0.5/src/core/dal/data.py` & `braincube-aws-core-0.0.6/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/src/core/dal/postgres_connection.py` & `braincube-aws-core-0.0.6/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/src/core/dal/postgres_repository.py` & `braincube-aws-core-0.0.6/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/src/core/di/data.py` & `braincube-aws-core-0.0.6/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/src/core/di/injector.py` & `braincube-aws-core-0.0.6/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/src/core/rules_engine/data.py` & `braincube-aws-core-0.0.6/src/core/rules_engine/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/src/core/rules_engine/rule_manager.py` & `braincube-aws-core-0.0.6/src/core/rules_engine/rule_manager.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/src/core/utils/convert.py` & `braincube-aws-core-0.0.6/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.5/src/core/utils/data.py` & `braincube-aws-core-0.0.6/src/core/utils/data.py`

 * *Files identical despite different names*

