# Comparing `tmp/tabulario-0.3.2.tar.gz` & `tmp/tabulario-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabulario-0.3.2.tar", max compression
+gzip compressed data, was "tabulario-0.4.0rc1.tar", max compression
```

## Comparing `tabulario-0.3.2.tar` & `tabulario-0.4.0rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-06-22 18:14:34.670083 tabulario-0.3.2/LICENSE
--rw-r--r--   0        0        0     6701 2023-06-22 18:14:34.670083 tabulario-0.3.2/README.md
--rw-r--r--   0        0        0     2487 2023-06-22 18:14:45.582204 tabulario-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      785 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/__init__.py
--rw-r--r--   0        0        0     4146 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/cli.py
--rw-r--r--   0        0        0      871 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/exceptions.py
--rw-r--r--   0        0        0     5024 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/oauth.py
--rw-r--r--   0        0        0     1004 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/util.py
--rw-r--r--   0        0        0      836 2023-06-22 18:14:34.670083 tabulario-0.3.2/tabular/__init__.py
--rw-r--r--   0        0        0     4955 2023-06-22 18:14:34.670083 tabulario-0.3.2/tabular/loader.py
--rw-r--r--   0        0        0     2016 2023-06-22 18:14:34.670083 tabulario-0.3.2/tabular/tabular.py
--rw-r--r--   0        0        0     7512 1970-01-01 00:00:00.000000 tabulario-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-26 14:48:22.117095 tabulario-0.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     7126 2023-06-26 14:48:22.117095 tabulario-0.4.0rc1/README.md
+-rw-r--r--   0        0        0     2493 2023-06-26 14:48:35.917175 tabulario-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      785 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/__init__.py
+-rw-r--r--   0        0        0     4229 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/cli.py
+-rw-r--r--   0        0        0      871 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/exceptions.py
+-rw-r--r--   0        0        0     5018 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/oauth.py
+-rw-r--r--   0        0        0     1004 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/util.py
+-rw-r--r--   0        0        0      836 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tabular/__init__.py
+-rw-r--r--   0        0        0     4955 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tabular/loader.py
+-rw-r--r--   0        0        0     2111 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tabular/tabular.py
+-rw-r--r--   0        0        0     7943 1970-01-01 00:00:00.000000 tabulario-0.4.0rc1/PKG-INFO
```

### Comparing `tabulario-0.3.2/LICENSE` & `tabulario-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.2/README.md` & `tabulario-0.4.0rc1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -118,15 +118,29 @@
     "name": "Fokko",
     "region": "us-west-2"
   }
 ]
 ```
 
 ```python
->> from tabular import Tabular
->>> t = Tabular("t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI")
+>>> from tabular import Tabular
+>>> t = Tabular(credential="t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI")
+>>> t.list_warehouses()
+[
+    Warehouse(id='6efbcaf4-21ae-499d-b340-3bc1a7003f52', name='sandbox', region='us-east-1'),
+    Warehouse(id='c70f668c-4746-414f-8a74-b1e4f1f0de60', name='Fokko', region='us-west-2')
+]
+```
+
+```python
+>>> from tabular import Tabular
+>>> t = Tabular(**{
+        "rest.sigv4-enabled": "true",
+        "rest.signing-region": "us-east-1",
+        "rest.signing-name": "execute-api",
+    })
 >>> t.list_warehouses()
 [
     Warehouse(id='6efbcaf4-21ae-499d-b340-3bc1a7003f52', name='sandbox', region='us-east-1'),
     Warehouse(id='c70f668c-4746-414f-8a74-b1e4f1f0de60', name='Fokko', region='us-west-2')
 ]
 ```
```

### Comparing `tabulario-0.3.2/pyproject.toml` & `tabulario-0.4.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [tool.poetry]
 name = "tabulario"
-version = "0.3.2"
+version = "0.4.0rc1"
 readme = "README.md"
 homepage = "https://tabular.io/"
 repository = "https://github.com/tabular-io/"
 description = "Utility library for Tabular.io"
 authors = ["Tabular Technologies, Inc. <fokko@tabular.io>"]
 license = "Apache License 2.0"
 
@@ -40,15 +40,15 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
 click = "^8.1.3"
-pyiceberg = "0.3.0"
+pyiceberg = "0.4.0rc1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-checkdocs = "^2.9.0"
 pre-commit = "^2.0.0"
 coverage = { version = "^6.5.0", extras = ["toml"] }
 requests-mock = "^1.10.0"
```

### Comparing `tabulario-0.3.2/tab/__init__.py` & `tabulario-0.4.0rc1/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.2/tab/cli.py` & `tabulario-0.4.0rc1/tab/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,15 +119,19 @@
     _out(fresh_token)
 
 
 @run.command()
 @click.pass_obj
 @click.option("-c", "--credential")
 @click.option("-t", "--token")
-def warehouses(ctx: TabularContext, credential: List[str], token: Optional[str]):
+def warehouses(ctx: TabularContext, credential: Optional[str], token: Optional[str]):
     """Fetches all the warehouses"""
     args = _read_stdin()
     if not args:
-        args = {"token": token, "credential": credential}
+        args = {}
+        if token:
+            args["token"] = token
+        if credential:
+            args["credential"] = credential
 
     all_warehouses = Tabular(environment=ctx.environment, **args).list_warehouses()
     _out(all_warehouses)
```

### Comparing `tabulario-0.3.2/tab/exceptions.py` & `tabulario-0.4.0rc1/tab/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.2/tab/oauth.py` & `tabulario-0.4.0rc1/tab/oauth.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,25 +90,25 @@
     except HTTPError as e:
         raise ValueError(f"Request failed {response.text}") from e
 
     return response_type(**{**{"scope": None, "expires_in": None}, **response.json()})
 
 
 ENVIRONMENT_URLS = {
-    "prod": "https://api.tabular.io/ws/v1",
-    "test": "https://api.test.tabular.io/ws/v1",
-    "dev": "https://api.dev.tabular.io/ws/v1",
+    "prod": "https://api.tabular.io/ws",
+    "test": "https://api.test.tabular.io/ws",
+    "dev": "https://api.dev.tabular.io/ws",
 }
 
 
 class TabularOAuth:
     base_url: str
 
     def __init__(self, environment: str):
-        self.base_url = ENVIRONMENT_URLS[environment] + "/oauth/tokens"
+        self.base_url = ENVIRONMENT_URLS[environment] + "/v1/oauth/tokens"
 
     def request_token(self, credential: str, scopes: Optional[Any] = None) -> OAuthTokenResponse:
         if SEMICOLON in credential:
             client_id, client_secret = credential.split(SEMICOLON)
         else:
             client_id, client_secret = None, credential
```

### Comparing `tabulario-0.3.2/tab/util.py` & `tabulario-0.4.0rc1/tab/util.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.2/tabular/__init__.py` & `tabulario-0.4.0rc1/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.2/tabular/loader.py` & `tabulario-0.4.0rc1/tabular/loader.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.2/PKG-INFO` & `tabulario-0.4.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tabulario
-Version: 0.3.2
+Version: 0.4.0rc1
 Summary: Utility library for Tabular.io
 Home-page: https://tabular.io/
 License: Apache-2.0
 Author: Tabular Technologies, Inc.
 Author-email: fokko@tabular.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: pyiceberg (==0.3.0)
+Requires-Dist: pyiceberg (==0.4.0rc1)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/tabular-io/
 Description-Content-Type: text/markdown
 
 # Tab
 
 This is a helper library to easily fetch and refresh access token from Tabular.
@@ -140,16 +140,30 @@
     "name": "Fokko",
     "region": "us-west-2"
   }
 ]
 ```
 
 ```python
->> from tabular import Tabular
->>> t = Tabular("t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI")
+>>> from tabular import Tabular
+>>> t = Tabular(credential="t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI")
+>>> t.list_warehouses()
+[
+    Warehouse(id='6efbcaf4-21ae-499d-b340-3bc1a7003f52', name='sandbox', region='us-east-1'),
+    Warehouse(id='c70f668c-4746-414f-8a74-b1e4f1f0de60', name='Fokko', region='us-west-2')
+]
+```
+
+```python
+>>> from tabular import Tabular
+>>> t = Tabular(**{
+        "rest.sigv4-enabled": "true",
+        "rest.signing-region": "us-east-1",
+        "rest.signing-name": "execute-api",
+    })
 >>> t.list_warehouses()
 [
     Warehouse(id='6efbcaf4-21ae-499d-b340-3bc1a7003f52', name='sandbox', region='us-east-1'),
     Warehouse(id='c70f668c-4746-414f-8a74-b1e4f1f0de60', name='Fokko', region='us-west-2')
 ]
 ```
```

