# Comparing `tmp/marqo-0.9.5.tar.gz` & `tmp/marqo-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-0.9.5.tar", last modified: Thu May 11 01:14:14 2023, max compression
+gzip compressed data, was "marqo-0.9.6.tar", last modified: Wed May 31 09:00:39 2023, max compression
```

## Comparing `marqo-0.9.5.tar` & `marqo-0.9.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:14:14.271015 marqo-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-05-11 01:14:00.000000 marqo-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-05-11 01:14:14.267015 marqo-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21052 2023-05-11 01:14:00.000000 marqo-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 01:14:00.000000 marqo-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 01:14:14.271015 marqo-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-11 01:14:00.000000 marqo-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:14:14.263015 marqo-0.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:14:14.267015 marqo-0.9.5/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/marqo_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-11 01:14:00.000000 marqo-0.9.5/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:14:14.267015 marqo-0.9.5/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 01:14:14.000000 marqo-0.9.5/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:39.221007 marqo-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-05-31 09:00:23.000000 marqo-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-05-31 09:00:39.217007 marqo-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21052 2023-05-31 09:00:23.000000 marqo-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 09:00:23.000000 marqo-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:00:39.221007 marqo-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-31 09:00:23.000000 marqo-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:39.213007 marqo-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:39.217007 marqo-0.9.6/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/marqo_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:39.217007 marqo-0.9.6/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-0.9.5/LICENSE` & `marqo-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-0.9.5/PKG-INFO` & `marqo-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 0.9.5
+Version: 0.9.6
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 0.9.5 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 0.9.6 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
```

### Comparing `marqo-0.9.5/README.md` & `marqo-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `marqo-0.9.5/setup.py` & `marqo-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "pydantic"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="0.9.5",
+    version="0.9.6",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-0.9.5/src/marqo/_httprequests.py` & `marqo-0.9.6/src/marqo/_httprequests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,120 +1,104 @@
 import copy
 import json
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import get_args, Any, Callable, Dict, Literal, List, Optional, Tuple, Union
 import requests
 from json.decoder import JSONDecodeError
 from marqo.config import Config
 from marqo.errors import (
     MarqoWebError,
     BackendCommunicationError,
     BackendTimeoutError
 )
 
-s = requests.Session()
-
-ALLOWED_OPERATIONS = {s.delete, s.get, s.post, s.put}
-
-OPERATION_MAPPING = {'delete': s.delete, 'get': s.get,
-                     'post': s.post, 'put': s.put}
-
+HTTP_OPERATIONS = Literal["delete", "get", "post", "put"]
+ALLOWED_OPERATIONS: Tuple[HTTP_OPERATIONS, ...] = get_args(HTTP_OPERATIONS)
+session = requests.Session()
+
+OPERATION_MAPPING = {
+    'delete': session.delete,
+    'get': session.get,
+    'post': session.post,
+    'put': session.put
+}
 
 class HttpRequests:
     def __init__(self, config: Config) -> None:
         self.config = config
-        self.session = s
+        self.headers = {'x-api-key': config.api_key} if config.api_key else {}
 
-        if config.api_key:
-            self.headers = {'x-api-key': config.api_key}
-        else:
-            self.headers = dict()
+    def _operation(self, method: HTTP_OPERATIONS) -> Callable:
+        if method not in ALLOWED_OPERATIONS:
+            raise ValueError("{} not an allowed operation {}".format(method, ALLOWED_OPERATIONS))
+
+        return OPERATION_MAPPING[method]
 
     def send_request(
         self,
-        http_method: Callable,
+        http_operation: HTTP_OPERATIONS,
         path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str], str]] = None,
         content_type: Optional[str] = None,
     ) -> Any:
-        to_verify = True
-
-        if http_method not in ALLOWED_OPERATIONS:
-            raise ValueError("{} not an allowed operation {}".format(http_method, ALLOWED_OPERATIONS))
-
         req_headers = copy.deepcopy(self.headers)
 
         if content_type is not None and content_type:
             req_headers['Content-Type'] = content_type
 
+        if not isinstance(body, (bytes, str)) and body is not None:
+            body = json.dumps(body)
+
         try:
-            request_path = self.config.url + '/' + path
-            if isinstance(body, bytes):
-                response = http_method(
-                    url=request_path,
-                    timeout=self.config.timeout,
-                    headers=req_headers,
-                    data=body,
-                    verify=to_verify
-                )
-            elif isinstance(body, str):
-                response = http_method(
-                    url=request_path,
-                    timeout=self.config.timeout,
-                    headers=req_headers,
-                    data=body,
-                    verify=to_verify
-                )
-            else:
-                response = http_method(
-                    url=request_path,
-                    timeout=self.config.timeout,
-                    headers=req_headers,
-                    data=json.dumps(body) if body else None,
-                    verify=to_verify
-                )
+            response = self._operation(http_operation)(
+                url=f"{self.config.url}/{path}",
+                timeout=self.config.timeout,
+                headers=req_headers,
+                data=body,
+                verify=True
+            )
             return self.__validate(response)
-
         except requests.exceptions.Timeout as err:
             raise BackendTimeoutError(str(err)) from err
         except requests.exceptions.ConnectionError as err:
             raise BackendCommunicationError(str(err)) from err
 
+
     def get(
         self, path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str], str]] = None,
     ) -> Any:
         content_type = None
         if body is not None:
             content_type = 'application/json'
-        return self.send_request(s.get, path=path, body=body, content_type=content_type)
+        return self.send_request('get', path=path, body=body, content_type=content_type)
 
     def post(
         self,
         path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str], str]] = None,
         content_type: Optional[str] = 'application/json',
     ) -> Any:
-        return self.send_request(s.post, path, body, content_type)
+        return self.send_request('post', path, body, content_type)
 
     def put(
         self,
         path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str], str]] = None,
         content_type: Optional[str] = None,
     ) -> Any:
         if body is not None:
             content_type = 'application/json'
-        return self.send_request(s.put, path, body, content_type)
+        return self.send_request('put', path, body, content_type)
 
     def delete(
         self,
         path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str]]] = None,
     ) -> Any:
-        return self.send_request(s.delete, path, body)
+        return self.send_request('delete', path, body)
 
     @staticmethod
     def __to_json(
         request: requests.Response
     ) -> Any:
         if request.content == b'':
             return request
```

### Comparing `marqo-0.9.5/src/marqo/client.py` & `marqo-0.9.6/src/marqo/client.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.5/src/marqo/config.py` & `marqo-0.9.6/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.5/src/marqo/defaults.py` & `marqo-0.9.6/src/marqo/defaults.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.5/src/marqo/errors.py` & `marqo-0.9.6/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.5/src/marqo/index.py` & `marqo-0.9.6/src/marqo/index.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.5/src/marqo/utils.py` & `marqo-0.9.6/src/marqo/utils.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.5/src/marqo.egg-info/PKG-INFO` & `marqo-0.9.6/src/marqo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 0.9.5
+Version: 0.9.6
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 0.9.5 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 0.9.6 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
```

