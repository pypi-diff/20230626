# Comparing `tmp/mauth_client-1.5.1.tar.gz` & `tmp/mauth_client-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mauth_client-1.5.1.tar", max compression
+gzip compressed data, was "mauth_client-1.6.0.tar", max compression
```

## Comparing `mauth_client-1.5.1.tar` & `mauth_client-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1062 2023-06-15 15:49:38.533899 mauth_client-1.5.1/LICENSE.txt
--rw-r--r--   0        0        0     6084 2023-06-15 15:49:38.533899 mauth_client-1.5.1/README.md
--rw-r--r--   0        0        0      243 2023-06-15 15:49:38.533899 mauth_client-1.5.1/mauth_client/__init__.py
--rw-r--r--   0        0        0     9672 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/authenticator.py
--rw-r--r--   0        0        0      434 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/config.py
--rw-r--r--   0        0        0      479 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/consts.py
--rw-r--r--   0        0        0      633 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/exceptions.py
--rw-r--r--   0        0        0     2046 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/key_holder.py
--rw-r--r--   0        0        0       54 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/lambda_authenticator/__init__.py
--rw-r--r--   0        0        0      761 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/lambda_authenticator/lambda_authenticator.py
--rw-r--r--   0        0        0      679 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/lambda_helper.py
--rw-r--r--   0        0        0       76 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/middlewares/__init__.py
--rw-r--r--   0        0        0     4082 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/middlewares/asgi.py
--rw-r--r--   0        0        0     3864 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/middlewares/wsgi.py
--rw-r--r--   0        0        0       26 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/requests_mauth/__init__.py
--rw-r--r--   0        0        0     1304 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/requests_mauth/client.py
--rw-r--r--   0        0        0     2795 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/rsa_signer.py
--rw-r--r--   0        0        0     2324 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/rsa_verifier.py
--rw-r--r--   0        0        0     6196 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/signable.py
--rw-r--r--   0        0        0     1731 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/signed.py
--rw-r--r--   0        0        0     2849 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/signer.py
--rw-r--r--   0        0        0      820 2023-06-15 15:49:38.537899 mauth_client-1.5.1/mauth_client/utils.py
--rw-r--r--   0        0        0     1421 2023-06-15 15:49:38.537899 mauth_client-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 mauth_client-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-26 14:20:09.941851 mauth_client-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     6084 2023-06-26 14:20:09.941851 mauth_client-1.6.0/README.md
+-rw-r--r--   0        0        0      146 2023-06-26 14:20:09.941851 mauth_client-1.6.0/mauth_client/__init__.py
+-rw-r--r--   0        0        0     9672 2023-06-26 14:20:09.941851 mauth_client-1.6.0/mauth_client/authenticator.py
+-rw-r--r--   0        0        0      434 2023-06-26 14:20:09.941851 mauth_client-1.6.0/mauth_client/config.py
+-rw-r--r--   0        0        0      479 2023-06-26 14:20:09.941851 mauth_client-1.6.0/mauth_client/consts.py
+-rw-r--r--   0        0        0      633 2023-06-26 14:20:09.941851 mauth_client-1.6.0/mauth_client/exceptions.py
+-rw-r--r--   0        0        0     2046 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/key_holder.py
+-rw-r--r--   0        0        0       54 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/lambda_authenticator/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/lambda_authenticator/lambda_authenticator.py
+-rw-r--r--   0        0        0      679 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/lambda_helper.py
+-rw-r--r--   0        0        0       76 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/middlewares/__init__.py
+-rw-r--r--   0        0        0     4082 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/middlewares/asgi.py
+-rw-r--r--   0        0        0     4579 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/middlewares/wsgi.py
+-rw-r--r--   0        0        0       26 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/requests_mauth/__init__.py
+-rw-r--r--   0        0        0     1304 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/requests_mauth/client.py
+-rw-r--r--   0        0        0     2795 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/rsa_signer.py
+-rw-r--r--   0        0        0     2324 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/rsa_verifier.py
+-rw-r--r--   0        0        0     6196 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/signable.py
+-rw-r--r--   0        0        0     1731 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/signed.py
+-rw-r--r--   0        0        0     2849 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/signer.py
+-rw-r--r--   0        0        0      820 2023-06-26 14:20:09.945851 mauth_client-1.6.0/mauth_client/utils.py
+-rw-r--r--   0        0        0     1318 2023-06-26 14:20:09.945851 mauth_client-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7480 1970-01-01 00:00:00.000000 mauth_client-1.6.0/PKG-INFO
```

### Comparing `mauth_client-1.5.1/LICENSE.txt` & `mauth_client-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/README.md` & `mauth_client-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/authenticator.py` & `mauth_client-1.6.0/mauth_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/exceptions.py` & `mauth_client-1.6.0/mauth_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/key_holder.py` & `mauth_client-1.6.0/mauth_client/key_holder.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/lambda_authenticator/lambda_authenticator.py` & `mauth_client-1.6.0/mauth_client/lambda_authenticator/lambda_authenticator.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/lambda_helper.py` & `mauth_client-1.6.0/mauth_client/lambda_helper.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/middlewares/asgi.py` & `mauth_client-1.6.0/mauth_client/middlewares/asgi.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/middlewares/wsgi.py` & `mauth_client-1.6.0/mauth_client/middlewares/wsgi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 import json
 import logging
 
 from urllib.parse import quote
 
 from mauth_client.authenticator import LocalAuthenticator
 from mauth_client.config import Config
@@ -53,18 +54,37 @@
         if not all([Config.APP_UUID, Config.PRIVATE_KEY]):
             raise TypeError("MAuthWSGIMiddleware requires APP_UUID and PRIVATE_KEY")
         # Validate the mauth settings (MAUTH_BASE_URL, MAUTH_API_VERSION)
         if not all([Config.MAUTH_URL, Config.MAUTH_API_VERSION]):
             raise TypeError("MAuthWSGIMiddleware requires MAUTH_URL and MAUTH_API_VERSION")
 
     def _read_body(self, environ):
-        input = environ["wsgi.input"]
-        input.seek(0)
-        body = input.read()
-        input.seek(0)
+        try:
+            size = int(environ.get("CONTENT_LENGTH", 0))
+        except ValueError:
+            size = 0
+
+        if not size:
+            return b""
+
+        body = environ["wsgi.input"].read(size)
+
+        # hack way of "rewinding" body so that downstream can reuse
+        #
+        # seek() will not work because production Flask and gunicorn give
+        # objects without a seek() function and blow up...
+        # yet humorously Flask in our tests gives a normal BytesIO object
+        # that does have seek()
+        #
+        # NOTE:
+        # this will not play well with large bodies where this may result in
+        # blowing out memory, but tbh MAuth is not adequately designed for and
+        # thus should not be used with large bodies.
+        environ["wsgi.input"] = io.BytesIO(body)
+
         return body
 
     def _extract_headers(self, environ):
         """
         Adapted from werkzeug package: https://github.com/pallets/werkzeug
         """
         headers = {}
```

### Comparing `mauth_client-1.5.1/mauth_client/requests_mauth/client.py` & `mauth_client-1.6.0/mauth_client/requests_mauth/client.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/rsa_signer.py` & `mauth_client-1.6.0/mauth_client/rsa_signer.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/rsa_verifier.py` & `mauth_client-1.6.0/mauth_client/rsa_verifier.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/signable.py` & `mauth_client-1.6.0/mauth_client/signable.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/signed.py` & `mauth_client-1.6.0/mauth_client/signed.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/signer.py` & `mauth_client-1.6.0/mauth_client/signer.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/mauth_client/utils.py` & `mauth_client-1.6.0/mauth_client/utils.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.5.1/pyproject.toml` & `mauth_client-1.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 [tool.poetry]
 name = "mauth-client"
-version = "1.5.1"
+version = "1.6.0"
 description = "MAuth Client for Python"
 repository = "https://github.com/mdsol/mauth-client-python"
 authors = ["Medidata Solutions <support@mdsol.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 requests = "^2.23"
 cachetools = "^5.3"
 rsa = "^4.0"
-importlib-metadata = {version = ">=3.6", python = "<3.8"}
 asgiref = "^3.5.2"
 charset-normalizer = "^3.1.0"
 
 [tool.poetry.dev-dependencies]
 boto3 = "^1.24"
 flask = "^2"
 python-dateutil = "^2.8"
```

### Comparing `mauth_client-1.5.1/PKG-INFO` & `mauth_client-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: mauth-client
-Version: 1.5.1
+Version: 1.6.0
 Summary: MAuth Client for Python
 Home-page: https://github.com/mdsol/mauth-client-python
 License: MIT
 Author: Medidata Solutions
 Author-email: support@mdsol.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: asgiref (>=3.5.2,<4.0.0)
 Requires-Dist: cachetools (>=5.3,<6.0)
 Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0)
-Requires-Dist: importlib-metadata (>=3.6) ; python_version < "3.8"
 Requires-Dist: requests (>=2.23,<3.0)
 Requires-Dist: rsa (>=4.0,<5.0)
 Project-URL: Repository, https://github.com/mdsol/mauth-client-python
 Description-Content-Type: text/markdown
 
 # MAuth Client Python
 [![Build
```

