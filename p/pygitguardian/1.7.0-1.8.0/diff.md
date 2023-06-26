# Comparing `tmp/pygitguardian-1.7.0.tar.gz` & `tmp/pygitguardian-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygitguardian-1.7.0.tar", last modified: Mon May 29 13:50:42 2023, max compression
+gzip compressed data, was "pygitguardian-1.8.0.tar", last modified: Mon Jun 26 09:35:55 2023, max compression
```

## Comparing `pygitguardian-1.7.0.tar` & `pygitguardian-1.8.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:50:42.157011 pygitguardian-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-29 13:50:42.157011 pygitguardian-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:50:42.153011 pygitguardian-1.7.0/pygitguardian/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/iac_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18791 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:50:42.153011 pygitguardian-1.7.0/pygitguardian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-29 13:50:42.157011 pygitguardian-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:50:42.157011 pygitguardian-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/tests/test_iac_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:35:55.199980 pygitguardian-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-26 09:35:55.199980 pygitguardian-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:35:55.199980 pygitguardian-1.8.0/pygitguardian/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/pygitguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/pygitguardian/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/pygitguardian/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/pygitguardian/iac_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20471 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/pygitguardian/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/pygitguardian/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:35:55.199980 pygitguardian-1.8.0/pygitguardian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-26 09:35:55.000000 pygitguardian-1.8.0/pygitguardian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-26 09:35:55.000000 pygitguardian-1.8.0/pygitguardian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:35:55.000000 pygitguardian-1.8.0/pygitguardian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 09:35:55.000000 pygitguardian-1.8.0/pygitguardian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 09:35:55.000000 pygitguardian-1.8.0/pygitguardian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:35:55.000000 pygitguardian-1.8.0/pygitguardian.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 09:35:55.199980 pygitguardian-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:35:55.199980 pygitguardian-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22044 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/tests/test_iac_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-26 09:35:50.000000 pygitguardian-1.8.0/tests/test_utils.py
```

### Comparing `pygitguardian-1.7.0/LICENSE` & `pygitguardian-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.7.0/PKG-INFO` & `pygitguardian-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygitguardian
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python Wrapper for GitGuardian's API -- Scan security policy breaks everywhere
 Home-page: https://github.com/GitGuardian/py-gitguardian
 Author: GitGuardian
 Author-email: support@gitguardian.com
 Maintainer: GitGuardian
 License: MIT
 Keywords: api-client devsecops secrets-detection security-tools library gitguardian
```

### Comparing `pygitguardian-1.7.0/README.md` & `pygitguardian-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.7.0/pygitguardian/client.py` & `pygitguardian-1.8.0/pygitguardian/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
+import logging
 import os
 import platform
 import tarfile
+import time
 import urllib.parse
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union, cast
 
 import requests
 from requests import Response, Session, codes
 
 from .config import DEFAULT_API_VERSION, DEFAULT_BASE_URI, DEFAULT_TIMEOUT
-from .iac_models import (
-    IaCScanParameters,
-    IaCScanParametersSchema,
-    IaCScanResult,
-    IaCScanResultSchema,
-)
+from .iac_models import IaCScanParameters, IaCScanParametersSchema, IaCScanResult
 from .models import (
     Detail,
     Document,
+    DocumentSchema,
     HealthCheckResponse,
     HoneytokenResponse,
+    JWTResponse,
+    JWTService,
     MultiScanResult,
     QuotaResponse,
     ScanResult,
     SecretScanPreferences,
     ServerMetadata,
 )
 
 
+logger = logging.getLogger(__name__)
+
+
 # max files size to create a tar from
 MAX_TAR_CONTENT_SIZE = 30 * 1024 * 1024
 
 
 class ContentTooLarge(Exception):
     """
     Raised if the total size of files sent by the client exceeds MAX_TAR_CONTENT_SIZE
@@ -60,15 +63,15 @@
     :rtype: Detail
     """
     if resp.headers["content-type"] == "application/json":
         data = resp.json()
     else:
         data = {"detail": resp.text}
 
-    return cast(Detail, Detail.SCHEMA.load(data))
+    return Detail.from_dict(data)
 
 
 def is_ok(resp: Response) -> bool:
     """
     is_ok returns True is the API responded with 200
     and the content type is JSON.
     """
@@ -189,17 +192,26 @@
         url = self._url_from_endpoint(endpoint, version)
 
         headers = (
             {**self.session.headers, **extra_headers}
             if extra_headers
             else self.session.headers
         )
+        start = time.time()
         response: Response = self.session.request(
             method=method, url=url, timeout=self.timeout, headers=headers, **kwargs
         )
+        duration = time.time() - start
+        logger.debug(
+            "method=%s endpoint=%s status_code=%s duration=%f",
+            method,
+            endpoint,
+            response.status_code,
+            duration,
+        )
 
         self.app_version = response.headers.get("X-App-Version", self.app_version)
         self.secrets_engine_version = response.headers.get(
             "X-Secrets-Engine-Version", self.secrets_engine_version
         )
 
         return response
@@ -248,19 +260,20 @@
             extra_headers=extra_headers,
             **kwargs,
         )
 
     def post(
         self,
         endpoint: str,
-        data: Optional[Dict[str, Any]] = None,
+        data: Union[Dict[str, Any], List[Dict[str, Any]], None] = None,
         version: str = DEFAULT_API_VERSION,
         extra_headers: Optional[Dict[str, str]] = None,
         **kwargs: Any,
     ) -> Response:
+        # Be aware that self.iac_directory_scan bypass this method and calls self.request directly.
         return self.request(
             "post",
             endpoint=endpoint,
             json=data,
             version=version,
             extra_headers=extra_headers,
             **kwargs,
@@ -302,28 +315,28 @@
         :return: Detail or ScanResult response and status code
         """
 
         doc_dict = {"document": document}
         if filename:
             doc_dict["filename"] = filename
 
-        request_obj = Document.SCHEMA.load(doc_dict)
-        Document.SCHEMA.validate_size(
+        request_obj = cast(Dict[str, Any], Document.SCHEMA.load(doc_dict))
+        DocumentSchema.validate_size(
             request_obj, self.secret_scan_preferences.maximum_document_size
         )
 
         resp = self.post(
             endpoint="scan",
             data=request_obj,
             extra_headers=extra_headers,
         )
 
         obj: Union[Detail, ScanResult]
         if is_ok(resp):
-            obj = ScanResult.SCHEMA.load(resp.json())
+            obj = ScanResult.from_dict(resp.json())
         else:
             obj = load_detail(resp)
 
         obj.status_code = resp.status_code
 
         return obj
 
@@ -349,20 +362,22 @@
         max_documents = self.secret_scan_preferences.maximum_documents_per_scan
         if len(documents) > max_documents:
             raise ValueError(
                 f"too many documents submitted for scan (max={max_documents})"
             )
 
         if all(isinstance(doc, dict) for doc in documents):
-            request_obj = Document.SCHEMA.load(documents, many=True)
+            request_obj = cast(
+                List[Dict[str, Any]], Document.SCHEMA.load(documents, many=True)
+            )
         else:
             raise TypeError("each document must be a dict")
 
         for document in request_obj:
-            Document.SCHEMA.validate_size(
+            DocumentSchema.validate_size(
                 document, self.secret_scan_preferences.maximum_document_size
             )
 
         params = (
             {"ignore_known_secrets": ignore_known_secrets}
             if ignore_known_secrets
             else {}
@@ -372,15 +387,15 @@
             data=request_obj,
             extra_headers=extra_headers,
             params=params,
         )
 
         obj: Union[Detail, MultiScanResult]
         if is_ok(resp):
-            obj = MultiScanResult.SCHEMA.load(dict(scan_results=resp.json()))
+            obj = MultiScanResult.from_dict({"scan_results": resp.json()})
         else:
             obj = load_detail(resp)
 
         obj.status_code = resp.status_code
 
         return obj
 
@@ -398,15 +413,15 @@
         resp = self.get(
             endpoint="quotas",
             extra_headers=extra_headers,
         )
 
         obj: Union[Detail, QuotaResponse]
         if is_ok(resp):
-            obj = QuotaResponse.SCHEMA.load(resp.json())
+            obj = QuotaResponse.from_dict(resp.json())
         else:
             obj = load_detail(resp)
 
         obj.status_code = resp.status_code
 
         return obj
 
@@ -437,15 +452,15 @@
                 },
             )
         except requests.exceptions.ReadTimeout:
             result = Detail("The request timed out.")
             result.status_code = 504
         else:
             if is_create_ok(resp):
-                result = HoneytokenResponse.SCHEMA.load(resp.json())
+                result = HoneytokenResponse.from_dict(resp.json())
             else:
                 result = load_detail(resp)
             result.status_code = resp.status_code
         return result
 
     # For IaC Scans
     def iac_directory_scan(
@@ -454,30 +469,32 @@
         filenames: List[str],
         scan_parameters: IaCScanParameters,
         extra_headers: Optional[Dict[str, str]] = None,
     ) -> Union[Detail, IaCScanResult]:
         tar = _create_tar(directory, filenames)
         result: Union[Detail, IaCScanResult]
         try:
-            resp = self.post(
+            # bypass self.post because data argument is needed in self.request and self.post use it as json
+            resp = self.request(
+                "post",
                 endpoint="iac_scan",
                 extra_headers=extra_headers,
                 files={
                     "directory": tar,
                 },
                 data={
                     "scan_parameters": IaCScanParametersSchema().dumps(scan_parameters),
                 },
             )
         except requests.exceptions.ReadTimeout:
             result = Detail("The request timed out.")
             result.status_code = 504
         else:
             if is_ok(resp):
-                result = IaCScanResultSchema().load(resp.json())
+                result = IaCScanResult.from_dict(resp.json())
             else:
                 result = load_detail(resp)
 
             result.status_code = resp.status_code
 
         return result
 
@@ -492,11 +509,35 @@
         """
         resp = self.get("metadata")
 
         if not is_ok(resp):
             result = load_detail(resp)
             result.status_code = resp.status_code
             return result
-        metadata = ServerMetadata.SCHEMA.load(resp.json())
+        metadata = ServerMetadata.from_dict(resp.json())
 
         self.secret_scan_preferences = metadata.secret_scan_preferences
         return None
+
+    def create_jwt(
+        self,
+        jwt_audience: str,
+        service: JWTService,
+        extra_headers: Optional[Dict[str, str]] = None,
+    ) -> Union[Detail, JWTResponse]:
+        """
+        Create a JWT token for other GitGuardian services.
+        :return: Detail or JWT response and status code
+        """
+
+        resp = self.post(
+            endpoint="auth/jwt",
+            data={"audience": jwt_audience, "audience_type": service.value},
+            extra_headers=extra_headers,
+        )
+        obj: Union[Detail, JWTResponse]
+        if is_ok(resp):
+            obj = JWTResponse.from_dict(resp.json())
+        else:
+            obj = load_detail(resp)
+        obj.status_code = resp.status_code
+        return obj
```

### Comparing `pygitguardian-1.7.0/pygitguardian/models.py` & `pygitguardian-1.8.0/pygitguardian/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,74 @@
 from dataclasses import dataclass, field
 from datetime import date, datetime
+from enum import Enum
 from typing import Any, ClassVar, Dict, List, Optional, cast
 from uuid import UUID
 
 import marshmallow_dataclass
 from marshmallow import (
     EXCLUDE,
     Schema,
     ValidationError,
     fields,
     post_load,
     pre_load,
     validate,
 )
+from typing_extensions import Self
 
 from .config import DOCUMENT_SIZE_THRESHOLD_BYTES, MULTI_DOCUMENT_LIMIT
 
 
+class ToDictMixin:
+    """
+    Provides a type-safe `to_dict()` method for classes using Marshmallow
+    """
+
+    SCHEMA: ClassVar[Schema]
+
+    def to_dict(self) -> Dict[str, Any]:
+        return cast(Dict[str, Any], self.SCHEMA.dump(self))
+
+
+class FromDictMixin:
+    """This class must be used as an additional base class for all classes whose schema
+    implements a `post_load` function turning the received dict into a class instance.
+
+    It makes it possible to deserialize an object using `MyClass.from_dict(dct)` instead
+    of `MyClass.SCHEMA.load(dct)`. The `from_dict()` method is shorter, but more
+    importantly, type-safe: its return type is an instance of `MyClass`, not
+    `list[Any] | Any`.
+
+    Reference: https://marshmallow.readthedocs.io/en/stable/quickstart.html#deserializing-to-objects  E501
+    """
+
+    SCHEMA: ClassVar[Schema]
+
+    @classmethod
+    def from_dict(cls, dct: Dict[str, Any]) -> Self:
+        return cast(Self, cls.SCHEMA.load(dct))
+
+
 class BaseSchema(Schema):
     class Meta:
         ordered = True
         unknown = EXCLUDE
 
 
-class Base:
-    SCHEMA: ClassVar[BaseSchema]
-
+class Base(ToDictMixin):
     def __init__(self, status_code: Optional[int] = None) -> None:
         self.status_code = status_code
 
     def to_json(self) -> str:
         """
         to_json converts model to JSON string.
         """
         return cast(str, self.SCHEMA.dumps(self))
 
-    def to_dict(self) -> Dict:
-        """
-        to_dict converts model to a dictionary representation.
-        """
-        return cast(Dict, self.SCHEMA.dump(self))
-
     @property
     def success(self) -> bool:
         return self.__bool__()
 
     def __bool__(self) -> bool:
         return self.status_code == 200
 
@@ -118,15 +142,15 @@
         return data
 
     @post_load
     def make_detail_response(self, data: Dict[str, Any], **kwargs: Any) -> "Detail":
         return Detail(**data)
 
 
-class Detail(Base):
+class Detail(Base, FromDictMixin):
     """Detail is a response object mostly returned on error or when the
     api output is a simple string.
 
     Attributes:
         detail (str): response string
     """
 
@@ -151,15 +175,15 @@
     index_end = fields.Int(allow_none=True)
 
     @post_load
     def make_match(self, data: Dict[str, Any], **kwargs: Any) -> "Match":
         return Match(**data)
 
 
-class Match(Base):
+class Match(Base, FromDictMixin):
     """
     Match describes a found issue by GitGuardian.
     With info such as match location and type.
     Example:
     { "match": "cake.gitguardian.com",
     "index_end": 96,
     "index_start": 77,
@@ -215,15 +239,15 @@
     matches = fields.List(fields.Nested(MatchSchema), required=True)
 
     @post_load
     def make_policy_break(self, data: Dict[str, Any], **kwargs: Any) -> "PolicyBreak":
         return PolicyBreak(**data)
 
 
-class PolicyBreak(Base):
+class PolicyBreak(Base, FromDictMixin):
     """
     PolicyBreak describes a GitGuardian policy break found
     in a scan.
     A PolicyBreak can contain multiple matches, for example,
     on secrets that have a client id and client secret.
     """
 
@@ -265,15 +289,15 @@
     policy_breaks = fields.List(fields.Nested(PolicyBreakSchema), required=True)
 
     @post_load
     def make_scan_result(self, data: Dict[str, Any], **kwargs: Any) -> "ScanResult":
         return ScanResult(**data)
 
 
-class ScanResult(Base):
+class ScanResult(Base, FromDictMixin):
     """ScanResult is a response object returned on a Content Scan
 
     Attributes:
         status_code (int): response status code
         policy_break_count (int): number of policy breaks
         policy_breaks (List): policy break list
         policies (List[str]): string list of policies evaluated
@@ -351,15 +375,15 @@
     @post_load
     def make_scan_result(
         self, data: Dict[str, Any], **kwargs: Any
     ) -> "MultiScanResult":
         return MultiScanResult(**data)
 
 
-class MultiScanResult(Base):
+class MultiScanResult(Base, FromDictMixin):
     """ScanResult is a response object returned on a Content Scan
 
     Attributes:
         status_code (int): response status code
         policy_break_count (int): number of policy breaks
         policy_breaks (List): policy break list
         policies (List[str]): string list of policies evaluated
@@ -421,15 +445,15 @@
     since = fields.Date()
 
     @post_load
     def make_quota(self, data: Dict[str, Any], **kwargs: Any) -> "Quota":
         return Quota(**data)
 
 
-class Quota(Base):
+class Quota(Base, FromDictMixin):
     """
     Quota describes a quota category in the GitGuardian API.
     Allows you to check your current available quota.
     Example:
     {"count": 2,
     "limit": 5000,
     "remaining": 4998,
@@ -464,15 +488,15 @@
     @post_load
     def make_quota_response(
         self, data: Dict[str, Any], **kwargs: Any
     ) -> "QuotaResponse":
         return QuotaResponse(**data)
 
 
-class QuotaResponse(Base):
+class QuotaResponse(Base, FromDictMixin):
     """
     Quota describes a quota category in the GitGuardian API.
     Allows you to check your current available quota.
     Example:
     {"content": {
         "count": 2,
         "limit": 5000,
@@ -501,25 +525,25 @@
     revoked_at = fields.AwareDateTime(allow_none=True)
     open_events_count = fields.Int(allow_none=True)
     type_ = fields.String(data_key="type")
     creator_id = fields.Int(allow_none=True)
     revoker_id = fields.Int(allow_none=True)
     creator_api_token_id = fields.String(allow_none=True)
     revoker_api_token_id = fields.String(allow_none=True)
-    token = fields.Mapping(key=fields.String(), value=fields.String())
+    token = fields.Mapping(fields.String(), fields.String())
     tags = fields.List(fields.String())
 
     @post_load
     def make_honeytoken_response(
         self, data: Dict[str, Any], **kwargs: Any
     ) -> "HoneytokenResponse":
         return HoneytokenResponse(**data)
 
 
-class HoneytokenResponse(Base):
+class HoneytokenResponse(Base, FromDictMixin):
     """
     honeytoken creation in the GitGuardian API.
     Allows users to create and get a honeytoken.
     Example:
         {
             "id": "d45a123f-b15d-4fea-abf6-ff2a8479de5b",
             "name": "honeytoken A",
@@ -629,18 +653,50 @@
 @dataclass
 class SecretScanPreferences:
     maximum_document_size: int = DOCUMENT_SIZE_THRESHOLD_BYTES
     maximum_documents_per_scan: int = MULTI_DOCUMENT_LIMIT
 
 
 @dataclass
-class ServerMetadata(Base):
+class ServerMetadata(Base, FromDictMixin):
     version: str
     preferences: Dict[str, Any]
     secret_scan_preferences: SecretScanPreferences = field(
         default_factory=SecretScanPreferences
     )
 
 
-ServerMetadata.SCHEMA = marshmallow_dataclass.class_schema(
-    ServerMetadata, base_schema=BaseSchema
-)()
+ServerMetadata.SCHEMA = cast(
+    BaseSchema,
+    marshmallow_dataclass.class_schema(ServerMetadata, base_schema=BaseSchema)(),
+)
+
+
+class JWTResponseSchema(BaseSchema):
+    token = fields.String(required=True)
+
+    @post_load
+    def make_response(self, data: Dict[str, str], **kwargs: Any) -> "JWTResponse":
+        return JWTResponse(**data)
+
+
+class JWTResponse(Base, FromDictMixin):
+    """Token to use the HasMySecretLeaked service.
+
+    Attributes:
+        token (str): the JWT token
+    """
+
+    SCHEMA = JWTResponseSchema()
+
+    def __init__(self, token: str, **kwargs: Any) -> None:
+        super().__init__()
+        self.token = token
+
+    def __repr__(self) -> str:
+        return self.token
+
+
+class JWTService(Enum):
+    """Enum for the different services GIM can generate a JWT for."""
+
+    HMSL = "hmsl"
```

### Comparing `pygitguardian-1.7.0/pygitguardian.egg-info/PKG-INFO` & `pygitguardian-1.8.0/pygitguardian.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygitguardian
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python Wrapper for GitGuardian's API -- Scan security policy breaks everywhere
 Home-page: https://github.com/GitGuardian/py-gitguardian
 Author: GitGuardian
 Author-email: support@gitguardian.com
 Maintainer: GitGuardian
 License: MIT
 Keywords: api-client devsecops secrets-detection security-tools library gitguardian
```

### Comparing `pygitguardian-1.7.0/setup.py` & `pygitguardian-1.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     author="GitGuardian",
     author_email="support@gitguardian.com",
     maintainer="GitGuardian",
     install_requires=[
         "marshmallow>=3.5, <4",
         "requests>=2, <3",
         "marshmallow-dataclass >=8.5.8, <8.6.0",
+        "typing-extensions",
     ],
     include_package_data=True,
     zip_safe=True,
     license="MIT",
     keywords="api-client devsecops secrets-detection security-tools library gitguardian",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `pygitguardian-1.7.0/tests/test_client.py` & `pygitguardian-1.8.0/tests/test_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import json
 import re
 from collections import OrderedDict
 from datetime import date
 from typing import Any, Dict, List, Optional, Type
-from unittest.mock import Mock, patch
+from unittest.mock import patch
 
 import pytest
+import responses
 from marshmallow import ValidationError
-from requests.models import Response
+from responses import matchers
 
 from pygitguardian import GGClient
 from pygitguardian.client import is_ok, load_detail
 from pygitguardian.config import (
     DEFAULT_BASE_URI,
     DOCUMENT_SIZE_THRESHOLD_BYTES,
     MULTI_DOCUMENT_LIMIT,
 )
 from pygitguardian.models import (
     Detail,
     HoneytokenResponse,
+    JWTResponse,
+    JWTService,
     MultiScanResult,
     QuotaResponse,
     ScanResult,
 )
 
 from .conftest import my_vcr
 
@@ -514,94 +517,94 @@
                 "additional-header": "value",
                 "common-header": "add-value",
             },
             id="priority-additional-headers",
         ),
     ],
 )
-@patch("requests.Session.request")
-@my_vcr.use_cassette
+@responses.activate
 def test_extra_headers(
-    request_mock: Mock,
     client: GGClient,
     session_headers: Any,
     extra_headers: Optional[Dict[str, str]],
     expected_headers: Dict[str, str],
 ):
     """
     GIVEN client's session headers
     WHEN calling any client method with additional headers
     THEN session/method headers should be merged with priority on method headers
     """
     client.session.headers = session_headers
 
-    mock_response = Mock(spec=Response)
-    mock_response.headers = {"content-type": "text"}
-    mock_response.text = "some error"
-    mock_response.status_code = 400
-    request_mock.return_value = mock_response
+    mock_response = responses.post(
+        url=client._url_from_endpoint("multiscan", "v1"),
+        content_type="text/plain",
+        body="some error",
+        status=400,
+        match=[matchers.header_matcher(extra_headers)] if extra_headers else [],
+    )
 
     client.multi_content_scan(
         [{"filename": FILENAME, "document": DOCUMENT}],
         extra_headers=extra_headers,
     )
-    assert request_mock.called
-    _, kwargs = request_mock.call_args
-    assert expected_headers == kwargs["headers"]
+    assert mock_response.call_count == 1
 
+    # Same test for content_scan
+    mock_response = responses.post(
+        url=client._url_from_endpoint("scan", "v1"),
+        content_type="text/plain",
+        body="some error",
+        status=400,
+        match=[matchers.header_matcher(extra_headers)] if extra_headers else [],
+    )
     client.content_scan("some_string", extra_headers=extra_headers)
-    assert request_mock.called
-    _, kwargs = request_mock.call_args
-    assert expected_headers == kwargs["headers"]
+    assert mock_response.call_count == 1
 
 
-@patch("requests.Session.request")
+@responses.activate
 def test_multiscan_parameters(
-    request_mock: Mock,
     client: GGClient,
 ):
     """
     GIVEN a ggclient
     WHEN calling multi_content_scan with parameters
     THEN the parameters are passed in the request
     """
-    mock_response = Mock(spec=Response)
-    mock_response.headers = {"content-type": "application/json"}
-    mock_response.status_code = 200
-    mock_response.json.return_value = [
-        {
-            "policy_break_count": 1,
-            "policies": ["pol"],
-            "policy_breaks": [
-                {
-                    "type": "break",
-                    "policy": "mypol",
-                    "matches": [
-                        {
-                            "match": "hello",
-                            "type": "hello",
-                        }
-                    ],
-                }
-            ],
-        }
-    ]
 
-    request_mock.return_value = mock_response
-
-    params = {"ignore_known_secrets": True}
+    mock_response = responses.post(
+        url=client._url_from_endpoint("multiscan", "v1"),
+        status=200,
+        match=[matchers.query_param_matcher({"ignore_known_secrets": True})],
+        json=[
+            {
+                "policy_break_count": 1,
+                "policies": ["pol"],
+                "policy_breaks": [
+                    {
+                        "type": "break",
+                        "policy": "mypol",
+                        "matches": [
+                            {
+                                "match": "hello",
+                                "type": "hello",
+                            }
+                        ],
+                    }
+                ],
+            }
+        ],
+    )
 
     client.multi_content_scan(
         [{"filename": FILENAME, "document": DOCUMENT}],
         ignore_known_secrets=True,
     )
 
-    assert request_mock.called
-    # 1 is for kwargs
-    assert request_mock.call_args[1]["params"] == params
+    assert mock_response.call_count == 1
 
 
 def test_quota_overview(client: GGClient):
     with my_vcr.use_cassette("quota.yaml"):
         quota_response = client.quota_overview()
         assert type(repr(quota_response)) == str
         assert type(str(quota_response)) == str
@@ -616,113 +619,153 @@
 
         assert type(quota_response.to_dict()) == OrderedDict
         quota_response_json = quota_response.to_json()
         assert type(quota_response_json) == str
         assert type(json.loads(quota_response_json)) == dict
 
 
-@pytest.mark.parametrize("method", ["get", "post"])
-@patch("requests.Session.request")
-def test_versions_from_headers(request_mock: Mock, client: GGClient, method):
+@pytest.mark.parametrize("method", ["GET", "POST"])
+@responses.activate
+def test_versions_from_headers(client: GGClient, method):
+    """
+    GIVEN a GGClient instance
+    WHEN an HTTP request to GitGuardian API is made
+    THEN the app_version and secrets_engine_version fields are set from the headers of
+         the HTTP response
+    """
+    url = client._url_from_endpoint("endpoint", "v1")
     app_version_value = "1.0"
     secrets_engine_version_value = "2.0"
 
-    mock_response = Mock(spec=Response)
-    mock_response.headers = {
-        "X-App-Version": app_version_value,
-        "X-Secrets-Engine-Version": secrets_engine_version_value,
-    }
-    request_mock.return_value = mock_response
+    mock_response = responses.add(
+        method=method,
+        url=url,
+        headers={
+            "X-App-Version": app_version_value,
+            "X-Secrets-Engine-Version": secrets_engine_version_value,
+        },
+    )
 
     client.request(method=method, endpoint="endpoint")
-    assert request_mock.called
-
-    assert client.app_version is app_version_value
-    assert client.secrets_engine_version is secrets_engine_version_value
+    assert mock_response.call_count == 1
 
-    mock_response = Mock(spec=Response)
-    mock_response.headers = {}
-    request_mock.return_value = mock_response
+    assert client.app_version == app_version_value
+    assert client.secrets_engine_version == secrets_engine_version_value
 
+    # WHEN making another HTTP call whose response headers does not contain the version
+    # fields
+    # THEN known version fields remain set
+    mock_response = responses.add(method=method, url=url)
     client.request(method=method, endpoint="endpoint")
-    assert request_mock.called
+    assert mock_response.call_count == 1
 
-    assert client.app_version is app_version_value
-    assert client.secrets_engine_version is secrets_engine_version_value
+    assert client.app_version == app_version_value
+    assert client.secrets_engine_version == secrets_engine_version_value
 
+    # WHEN creating another GGClient instance
+    # THEN it already has the fields set
     other_client = GGClient(api_key="")
-    assert other_client.app_version is app_version_value
-    assert other_client.secrets_engine_version is secrets_engine_version_value
+    assert other_client.app_version == app_version_value
+    assert other_client.secrets_engine_version == secrets_engine_version_value
 
 
-@patch("requests.Session.request")
+@responses.activate
 def test_create_honeytoken(
-    request_mock: Mock,
     client: GGClient,
 ):
     """
     GIVEN a ggclient
     WHEN calling create_honeytoken with parameters
-    THEN the parameters are passed in the request and the returned honeytoken use the parameters
+    THEN the parameters are passed in the request
+    AND the returned honeytoken use the parameters
     """
-    mock_response = Mock(spec=Response)
-    mock_response.headers = {"content-type": "application/json"}
-    mock_response.status_code = 201
-    mock_response.json.return_value = {
-        "id": "d45a123f-b15d-4fea-abf6-ff2a8479de5b",
-        "name": "honeytoken A",
-        "description": "honeytoken used in the repository AA",
-        "created_at": "2019-08-22T14:15:22Z",
-        "gitguardian_url": "https://dashboard.gitguardian.com/workspace/1/honeytokens/d45a123f-b15d-4fea-abf6-ff2a8479de5b",  # noqa: E501
-        "status": "active",
-        "triggered_at": "2019-08-22T14:15:22Z",
-        "revoked_at": None,
-        "open_events_count": 2,
-        "type": "AWS",
-        "creator_id": 122,
-        "revoker_id": None,
-        "creator_api_token_id": None,
-        "revoker_api_token_id": None,
-        "token": {"access_token_id": "AAAA", "secret_key": "BBB"},
-        "tags": ["publicly_exposed"],
-    }
-
-    request_mock.return_value = mock_response
+    mock_response = responses.post(
+        url=client._url_from_endpoint("honeytokens", "v1"),
+        content_type="application/json",
+        status=201,
+        json={
+            "id": "d45a123f-b15d-4fea-abf6-ff2a8479de5b",
+            "name": "honeytoken A",
+            "description": "honeytoken used in the repository AA",
+            "created_at": "2019-08-22T14:15:22Z",
+            "gitguardian_url": "https://dashboard.gitguardian.com/workspace/1/honeytokens/d45a123f-b15d-4fea-abf6-ff2a8479de5b",  # noqa: E501
+            "status": "active",
+            "triggered_at": "2019-08-22T14:15:22Z",
+            "revoked_at": None,
+            "open_events_count": 2,
+            "type": "AWS",
+            "creator_id": 122,
+            "revoker_id": None,
+            "creator_api_token_id": None,
+            "revoker_api_token_id": None,
+            "token": {"access_token_id": "AAAA", "secret_key": "BBB"},
+            "tags": ["publicly_exposed"],
+        },
+    )
 
     result = client.create_honeytoken(
         name="honeytoken A",
         description="honeytoken used in the repository AA",
         type_="AWS",
     )
 
-    assert request_mock.called
+    assert mock_response.call_count == 1
     assert isinstance(result, HoneytokenResponse)
 
 
-@patch("requests.Session.request")
+@responses.activate
 def test_create_honeytoken_error(
-    request_mock: Mock,
     client: GGClient,
 ):
     """
     GIVEN a ggclient
     WHEN calling create_honeytoken with parameters without the right access
-    THEN I get a Detail objects containing the error detail
+    THEN I get a Detail object containing the error detail
     """
-    mock_response = Mock(spec=Response)
-    mock_response.headers = {"content-type": "application/json"}
-    mock_response.status_code = 400
-    mock_response.json.return_value = {
-        "detail": "Not authorized",
-    }
-
-    request_mock.return_value = mock_response
+    mock_response = responses.post(
+        url=client._url_from_endpoint("honeytokens", "v1"),
+        content_type="application/json",
+        status=400,
+        json={
+            "detail": "Not authorized",
+        },
+    )
 
     result = client.create_honeytoken(
         name="honeytoken A",
         description="honeytoken used in the repository AA",
         type_="AWS",
     )
 
-    assert request_mock.called
+    assert mock_response.call_count == 1
     assert isinstance(result, Detail)
-    result.status_code == 400
+
+
+@responses.activate
+def test_create_jwt(
+    client: GGClient,
+):
+    """
+    GIVEN a ggclient
+    WHEN calling create_jwt
+    THEN we receive a token
+    """
+    mock_response = responses.post(
+        url=client._url_from_endpoint("auth/jwt", "v1"),
+        match=[
+            matchers.json_params_matcher(
+                {
+                    "audience": "dummy_audience",
+                    "audience_type": "hmsl",
+                }
+            )
+        ],
+        content_type="application/json",
+        status=200,
+        json={"token": "dummy_token"},
+    )
+
+    result = client.create_jwt("dummy_audience", JWTService.HMSL)
+
+    assert mock_response.call_count == 1
+    assert isinstance(result, JWTResponse)
+    assert result.token == "dummy_token"
```

### Comparing `pygitguardian-1.7.0/tests/test_iac_models.py` & `pygitguardian-1.8.0/tests/test_iac_models.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.7.0/tests/test_models.py` & `pygitguardian-1.8.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.7.0/tests/test_utils.py` & `pygitguardian-1.8.0/tests/test_utils.py`

 * *Files identical despite different names*

