# Comparing `tmp/python_schema_registry_client-2.4.4.tar.gz` & `tmp/python_schema_registry_client-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_schema_registry_client-2.4.4.tar", max compression
+gzip compressed data, was "python_schema_registry_client-2.5.0.tar", max compression
```

## Comparing `python_schema_registry_client-2.4.4.tar` & `python_schema_registry_client-2.5.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1080 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/LICENSE
--rw-r--r--   0        0        0    11607 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/README.md
--rw-r--r--   0        0        0     2246 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/__init__.py
--rw-r--r--   0        0        0      215 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/__init__.py
--rw-r--r--   0        0        0       92 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/auth_utils.py
--rw-r--r--   0        0        0    55631 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/client.py
--rw-r--r--   0        0        0      535 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/errors.py
--rw-r--r--   0        0        0      801 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/paths.py
--rw-r--r--   0        0        0     4701 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/schema.py
--rw-r--r--   0        0        0     2328 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/status.py
--rw-r--r--   0        0        0     1419 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/urls.py
--rw-r--r--   0        0        0     1039 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/utils.py
--rw-r--r--   0        0        0        0 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/py.typed
--rw-r--r--   0        0        0      541 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/serializers/__init__.py
--rw-r--r--   0        0        0      351 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/serializers/errors.py
--rw-r--r--   0        0        0     3770 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/serializers/faust.py
--rw-r--r--   0        0        0    18116 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/serializers/message_serializer.py
--rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 python_schema_registry_client-2.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/LICENSE
+-rw-r--r--   0        0        0    11607 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/README.md
+-rw-r--r--   0        0        0     2246 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/client/__init__.py
+-rw-r--r--   0        0        0    55493 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/client/client.py
+-rw-r--r--   0        0        0      535 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/client/errors.py
+-rw-r--r--   0        0        0      801 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/client/paths.py
+-rw-r--r--   0        0        0     4701 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/client/schema.py
+-rw-r--r--   0        0        0     2328 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/client/status.py
+-rw-r--r--   0        0        0     1419 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/client/urls.py
+-rw-r--r--   0        0        0     1039 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/client/utils.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/py.typed
+-rw-r--r--   0        0        0      541 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/serializers/__init__.py
+-rw-r--r--   0        0        0      351 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/serializers/errors.py
+-rw-r--r--   0        0        0     3770 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/serializers/faust.py
+-rw-r--r--   0        0        0    18116 2023-06-26 15:32:17.922582 python_schema_registry_client-2.5.0/schema_registry/serializers/message_serializer.py
+-rw-r--r--   0        0        0    12651 1970-01-01 00:00:00.000000 python_schema_registry_client-2.5.0/PKG-INFO
```

### Comparing `python_schema_registry_client-2.4.4/LICENSE` & `python_schema_registry_client-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/README.md` & `python_schema_registry_client-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/pyproject.toml` & `python_schema_registry_client-2.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 [tool.poetry]
 name = "python-schema-registry-client"
-version = "2.4.4"
+version = "2.5.0"
 description = "Python Rest Client to interact against Schema Registry confluent server"
 authors = ["Marcos Schroh <schrohm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "schema_registry"}]
 
+classifiers = [
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
+    "Topic :: Software Development",
+]
+
 [tool.poetry.dependencies]
 python = "^3.7"
 fastavro = "^1.7.3"
 jsonschema = "^4.17.3"
 httpx = "^0.24.0"
 aiofiles = "^23.1.0"
 faust-streaming = {version = "^0.10.11", optional = true}
@@ -41,27 +54,14 @@
 [tool.poetry.extras]
 faust = ["faust-streaming"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-classifiers = [
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3 :: Only",
-    "Topic :: Software Development",
-]
-
 [tool.black]
 line-length = 120
 target_version = ['py37']
 
 [tool.mypy]
 allow_empty_bodies = true
 
@@ -95,13 +95,13 @@
     ".venv",
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.commitizen]
-version = "2.4.4"
+version = "2.5.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
 ]
 update_changelog_on_bump = true
```

### Comparing `python_schema_registry_client-2.4.4/schema_registry/client/client.py` & `python_schema_registry_client-2.5.0/schema_registry/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import logging
 import typing
 from abc import abstractmethod
 from collections import defaultdict
 from urllib.parse import urlparse
 
 import httpx
-from httpx import USE_CLIENT_DEFAULT
+from httpx import USE_CLIENT_DEFAULT, Auth, BasicAuth
 from httpx._client import UseClientDefault
 from httpx._types import TimeoutTypes
 
-from . import auth_utils, status, utils
+from . import status, utils
 from .errors import ClientError
 from .paths import paths
 from .schema import AvroSchema, BaseSchema, JsonSchema, SchemaFactory, SubjectVersion
 from .urls import UrlManager
 
 logger = logging.getLogger(__name__)
 
@@ -47,28 +47,28 @@
         cert_location str | None: Path to public key used for authentication.
         key_location str | None: Path to private key used for authentication.
         key_password str | None: Key password
         extra_headers str | None: Extra headers to add on every requests.
         timeout httpx.Timeout | None: The timeout configuration to use when sending requests.
         pool_limits httpx.Limits | None: The connection pool configuration to use when
             determining the maximum number of concurrently open HTTP connections.
-        auth auth_utils.Auth | None: Auth credentials.
+        auth httpx.Auth | None: Auth credentials.
     """
 
     def __init__(
         self,
         url: typing.Union[str, typing.Dict],
         ca_location: typing.Optional[str] = None,
         cert_location: typing.Optional[str] = None,
         key_location: typing.Optional[str] = None,
         key_password: typing.Optional[str] = None,
         extra_headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Optional[httpx.Timeout] = None,
         pool_limits: typing.Optional[httpx.Limits] = None,
-        auth: typing.Optional[auth_utils.Auth] = None,
+        auth: typing.Optional[Auth] = None,
     ) -> None:
         if isinstance(url, str):
             conf = {
                 utils.URL: url,
                 utils.SSL_CA_LOCATION: ca_location,
                 utils.SSL_CERTIFICATE_LOCATION: cert_location,
                 utils.SSL_KEY_LOCATION: key_location,
@@ -100,43 +100,38 @@
 
     @staticmethod
     def _schema_from_result(result: typing.Dict) -> typing.Union[JsonSchema, AvroSchema]:
         schema: str = result["schema"]
         schema_type = result.get("schemaType", utils.AVRO_SCHEMA_TYPE)
         return SchemaFactory.create_schema(schema, schema_type)
 
-    def _configure_auth(self) -> typing.Tuple[str, str]:
+    def _configure_auth(self) -> Auth:
         # Check first if the credentials are sent in Auth
         if self.auth is not None:
-            return (
-                self.auth.username,
-                self.auth.password,
-            )
+            return self.auth
 
         # This part should be deprecated with a new mayor version. Url should be only a string
         url = self.conf["url"]
         auth_provider = self.conf.pop("basic.auth.credentials.source", "URL").upper()  # type: ignore
 
         if auth_provider not in utils.VALID_AUTH_PROVIDERS:
             raise ValueError(
                 f"""
                 schema.registry.basic.auth.credentials.source
                 must be one of {utils.VALID_AUTH_PROVIDERS}
                 """
             )
 
         if auth_provider == "USER_INFO":
-            logger.warning(
-                "Deprecation warning: This will be deprecated in future versions. Use auth_utils.Auth instead"
-            )
-            auth = tuple(self.conf.pop("basic.auth.user.info", "").split(":"))  # type: ignore
+            logger.warning("Deprecation warning: This will be deprecated in future versions. Use httpx.Auth instead")
+            auth = BasicAuth(*self.conf.pop("basic.auth.user.info", "").split(":"))  # type: ignore
         else:
             # Credentials might be in the url.
             parsed_url = urlparse(url)
-            auth = (parsed_url.username or "", parsed_url.password or "")
+            auth = BasicAuth(parsed_url.username or "", parsed_url.password or "")
 
         # remove ignore after mypy fix https://github.com/python/mypy/issues/4805
         return auth  # type: ignore
 
     @staticmethod
     def _configure_client_tls(
         conf: dict,
@@ -265,15 +260,15 @@
         cert_location str | None: Path to public key used for authentication.
         key_location str | None: Path to private key used for authentication.
         key_password str | None: Key password
         extra_headers str | None: Extra headers to add on every requests.
         timeout httpx.Timeout | None: The timeout configuration to use when sending requests.
         pool_limits httpx.Limits | None: The connection pool configuration to use when
             determining the maximum number of concurrently open HTTP connections.
-        auth auth_utils.Auth | None: Auth credentials.
+        auth httpx.Auth | None: Auth credentials.
     """
 
     def request(
         self,
         url: str,
         method: str = "GET",
         body: typing.Optional[typing.Dict] = None,
@@ -799,15 +794,15 @@
         cert_location str | None: Path to public key used for authentication.
         key_location str | None: Path to private key used for authentication.
         key_password str | None: Key password
         extra_headers str | None: Extra headers to add on every requests.
         timeout httpx.Timeout | None: The timeout configuration to use when sending requests.
         pool_limits httpx.Limits | None: The connection pool configuration to use when
             determining the maximum number of concurrently open HTTP connections.
-        auth auth_utils.Auth | None: Auth credentials.
+        auth httpx.Auth | None: Auth credentials.
     """
 
     async def request(
         self,
         url: str,
         method: str = "GET",
         body: typing.Optional[typing.Dict] = None,
```

### Comparing `python_schema_registry_client-2.4.4/schema_registry/client/errors.py` & `python_schema_registry_client-2.5.0/schema_registry/client/errors.py`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/schema_registry/client/paths.py` & `python_schema_registry_client-2.5.0/schema_registry/client/paths.py`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/schema_registry/client/schema.py` & `python_schema_registry_client-2.5.0/schema_registry/client/schema.py`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/schema_registry/client/status.py` & `python_schema_registry_client-2.5.0/schema_registry/client/status.py`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/schema_registry/client/urls.py` & `python_schema_registry_client-2.5.0/schema_registry/client/urls.py`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/schema_registry/client/utils.py` & `python_schema_registry_client-2.5.0/schema_registry/client/utils.py`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/schema_registry/serializers/__init__.py` & `python_schema_registry_client-2.5.0/schema_registry/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/schema_registry/serializers/faust.py` & `python_schema_registry_client-2.5.0/schema_registry/serializers/faust.py`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/schema_registry/serializers/message_serializer.py` & `python_schema_registry_client-2.5.0/schema_registry/serializers/message_serializer.py`

 * *Files identical despite different names*

### Comparing `python_schema_registry_client-2.4.4/PKG-INFO` & `python_schema_registry_client-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: python-schema-registry-client
-Version: 2.4.4
+Version: 2.5.0
 Summary: Python Rest Client to interact against Schema Registry confluent server
 License: MIT
 Author: Marcos Schroh
 Author-email: schrohm@gmail.com
 Requires-Python: >=3.7,<4.0
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development
 Provides-Extra: faust
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: fastavro (>=1.7.3,<2.0.0)
 Requires-Dist: faust-streaming (>=0.10.11,<0.11.0) ; extra == "faust"
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Description-Content-Type: text/markdown
```

