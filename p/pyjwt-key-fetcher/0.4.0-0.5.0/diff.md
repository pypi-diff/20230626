# Comparing `tmp/pyjwt_key_fetcher-0.4.0.tar.gz` & `tmp/pyjwt_key_fetcher-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjwt_key_fetcher-0.4.0.tar", max compression
+gzip compressed data, was "pyjwt_key_fetcher-0.5.0.tar", max compression
```

## Comparing `pyjwt_key_fetcher-0.4.0.tar` & `pyjwt_key_fetcher-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1519 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/LICENSE
--rw-r--r--   0        0        0     4878 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/README.md
--rw-r--r--   0        0        0      167 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/__init__.py
--rw-r--r--   0        0        0      714 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/errors.py
--rw-r--r--   0        0        0     5385 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/fetcher.py
--rw-r--r--   0        0        0     1672 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/http_client.py
--rw-r--r--   0        0        0     1092 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/key.py
--rw-r--r--   0        0        0     4245 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/provider.py
--rw-r--r--   0        0        0        0 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/tests/__init__.py
--rw-r--r--   0        0        0     5596 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/tests/conftest.py
--rw-r--r--   0        0        0     2077 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/tests/test_clients.py
--rw-r--r--   0        0        0     4156 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/tests/test_fetcher.py
--rw-r--r--   0        0        0     1839 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/tests/test_utils.py
--rw-r--r--   0        0        0      689 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/utils.py
--rw-r--r--   0        0        0      793 2023-02-21 13:26:33.173175 pyjwt_key_fetcher-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5844 1970-01-01 00:00:00.000000 pyjwt_key_fetcher-0.4.0/setup.py
--rw-r--r--   0        0        0     5708 1970-01-01 00:00:00.000000 pyjwt_key_fetcher-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4878 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/README.md
+-rw-r--r--   0        0        0      167 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/__init__.py
+-rw-r--r--   0        0        0      714 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/errors.py
+-rw-r--r--   0        0        0     5385 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/fetcher.py
+-rw-r--r--   0        0        0     1672 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/http_client.py
+-rw-r--r--   0        0        0     1092 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/key.py
+-rw-r--r--   0        0        0     5039 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/provider.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/tests/__init__.py
+-rw-r--r--   0        0        0     5596 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/tests/conftest.py
+-rw-r--r--   0        0        0     2077 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/tests/test_clients.py
+-rw-r--r--   0        0        0     4156 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/tests/test_fetcher.py
+-rw-r--r--   0        0        0     1839 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/tests/test_utils.py
+-rw-r--r--   0        0        0      689 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/utils.py
+-rw-r--r--   0        0        0      793 2023-06-26 12:10:20.214326 pyjwt_key_fetcher-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5708 1970-01-01 00:00:00.000000 pyjwt_key_fetcher-0.5.0/PKG-INFO
```

### Comparing `pyjwt_key_fetcher-0.4.0/LICENSE` & `pyjwt_key_fetcher-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/README.md` & `pyjwt_key_fetcher-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/errors.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/errors.py`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/fetcher.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/fetcher.py`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/http_client.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/http_client.py`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/key.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/key.py`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/provider.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,58 @@
 from typing import Any, Dict, Optional
+from uuid import uuid4
 
 import aiocache  # type: ignore
 
 from pyjwt_key_fetcher.errors import (
     JWTKeyNotFoundError,
     JWTProviderConfigError,
     JWTProviderJWKSError,
 )
 from pyjwt_key_fetcher.http_client import HTTPClient
 from pyjwt_key_fetcher.key import Key
 
 
+def key_builder(f, *args, **kwargs) -> str:
+    """
+    Custom key builder for aiocache that uses the self.uuid instead of serializing
+    self to something that contains some memory address that might get reused later,
+    like for example <pyjwt_key_fetcher.provider.Provider object at 0x120e9a070>.
+
+    This is especially a possible problem in tests that might create a lot of
+    instances and some might end up at the same memory addresses as previously
+    existing ones.
+    """
+    ordered_kwargs = sorted(kwargs.items())
+    key = (
+        f.__module__
+        + f.__name__
+        + "."
+        + str(args[0].uuid)
+        + "."
+        + str(args[1:])
+        + str(ordered_kwargs)
+    )
+    return key
+
+
 class Provider:
     def __init__(
         self,
         iss: str,
         http_client: HTTPClient,
         config_path: str = "/.well-known/openid-configuration",
     ) -> None:
         self.iss = iss
         self.http_client = http_client
         self._configuration: Optional[Dict[str, Any]] = None
         self._jwk_map: Dict[str, Dict[str, Any]] = {}
         self.keys: Dict[str, Key] = {}
         self.config_path = config_path
+        self.uuid = uuid4()
 
     async def _config_uri(self) -> str:
         """
         Get the URI at which the configuration is expected to be found.
 
         Can be for example https://example.com/.well-known/openid-configuration
         :return: The configuration URI.
@@ -58,15 +83,15 @@
         conf = await self.get_configuration()
         try:
             jwks_uri = conf["jwks_uri"]
         except KeyError as e:
             raise JWTProviderConfigError("Missing 'jwks_uri' in configuration") from e
         return jwks_uri
 
-    @aiocache.cached(ttl=300)
+    @aiocache.cached(ttl=300, key_builder=key_builder)
     async def _fetch_jwk_map(self) -> Dict[str, Dict[str, Any]]:
         """
         Get all JWKs for an issuer as a dictionary with kid as key.
 
         Rate limited to once per 5 minutes (300 seconds).
 
         :return: A mapping of {kid: {<data_for_the_kid>}, ...}
```

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/tests/conftest.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/tests/test_clients.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/tests/test_fetcher.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/tests/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/tests/test_utils.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyjwt_key_fetcher/utils.py` & `pyjwt_key_fetcher-0.5.0/pyjwt_key_fetcher/utils.py`

 * *Files identical despite different names*

### Comparing `pyjwt_key_fetcher-0.4.0/pyproject.toml` & `pyjwt_key_fetcher-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "pyjwt-key-fetcher"
-version = "0.4.0"
+version = "0.5.0"
 description = "Async library to fetch JWKs for JWT tokens"
 authors = ["IOXIO"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ioxiocom/pyjwt-key-fetcher"
 packages = [
     {include="pyjwt_key_fetcher", from="."}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-PyJWT = {version = "^2.6.0", extras = ["crypto"]}
+PyJWT = {version = "^2.7.0", extras = ["crypto"]}
 aiohttp = {version = "^3.8.4", extras = ["speedups"]}
-cachetools = "^5.3.0"
-aiocache = "^0.12.0"
+cachetools = "^5.3.1"
+aiocache = "^0.12.1"
 
 [tool.skjold]
 report_only = false
 sources = ["pyup", "gemnasium"]
 
 [tool.poetry.dev-dependencies]
 invoke = "^2.0.0"
```

### Comparing `pyjwt_key_fetcher-0.4.0/setup.py` & `pyjwt_key_fetcher-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,133 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyjwt-key-fetcher
+Version: 0.5.0
+Summary: Async library to fetch JWKs for JWT tokens
+Home-page: https://github.com/ioxiocom/pyjwt-key-fetcher
+License: BSD-3-Clause
+Author: IOXIO
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyJWT[crypto] (>=2.7.0,<3.0.0)
+Requires-Dist: aiocache (>=0.12.1,<0.13.0)
+Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
+Requires-Dist: cachetools (>=5.3.1,<6.0.0)
+Project-URL: Repository, https://github.com/ioxiocom/pyjwt-key-fetcher
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': '.'}
+# pyjwt-key-fetcher
 
-packages = \
-['pyjwt_key_fetcher', 'pyjwt_key_fetcher.tests']
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ioxiocom/pyjwt-key-fetcher/publish.yaml)](https://github.com/ioxiocom/pyjwt-key-fetcher/actions/workflows/publish.yaml)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI](https://img.shields.io/pypi/v/pyjwt-key-fetcher)](https://pypi.org/project/pyjwt-key-fetcher/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyjwt-key-fetcher)](https://pypi.org/project/pyjwt-key-fetcher/)
+[![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyJWT[crypto]>=2.6.0,<3.0.0',
- 'aiocache>=0.12.0,<0.13.0',
- 'aiohttp[speedups]>=3.8.4,<4.0.0',
- 'cachetools>=5.3.0,<6.0.0']
-
-setup_kwargs = {
-    'name': 'pyjwt-key-fetcher',
-    'version': '0.4.0',
-    'description': 'Async library to fetch JWKs for JWT tokens',
-    'long_description': '# pyjwt-key-fetcher\n\n[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ioxiocom/pyjwt-key-fetcher/publish.yaml)](https://github.com/ioxiocom/pyjwt-key-fetcher/actions/workflows/publish.yaml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI](https://img.shields.io/pypi/v/pyjwt-key-fetcher)](https://pypi.org/project/pyjwt-key-fetcher/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyjwt-key-fetcher)](https://pypi.org/project/pyjwt-key-fetcher/)\n[![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nAsync library to fetch JWKs for JWT tokens.\n\nThis library is intended to be used together with\n[PyJWT](https://pyjwt.readthedocs.io/en/stable/) to automatically verify keys signed by\nOpenID Connect providers. It retrieves the `iss` (issuer) and the `kid` (key ID) from\nthe JWT, fetches the `.well-known/openid-configuration` from the issuer to find out the\n`jwks_uri` and fetches that to find the right key.\n\nThis should give similar ability to verify keys as for example\n[https://jwt.io/](https://jwt.io/), where you can just paste in a token, and it will\nautomatically reach out and retrieve the key for you.\n\nThe `AsyncKeyFetcher` provided by this library acts as an improved async replacement for\n[PyJWKClient](https://pyjwt.readthedocs.io/en/2.6.0/usage.html#retrieve-rsa-signing-keys-from-a-jwks-endpoint).\n\n## Installation\n\nThe package is available on PyPI:\n\n```bash\npip install pyjwt-key-fetcher\n```\n\n## Usage\n\n### Example\n\n```python\nimport asyncio\n\nimport jwt\n\nfrom pyjwt_key_fetcher import AsyncKeyFetcher\n\n\nasync def main():\n    fetcher = AsyncKeyFetcher()\n    # Token and options copied from\n    # https://pyjwt.readthedocs.io/en/2.6.0/usage.html#retrieve-rsa-signing-keys-from-a-jwks-endpoint\n    token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImtpZCI6Ik5FRTFRVVJCT1RNNE16STVSa0ZETlRZeE9UVTFNRGcyT0Rnd1EwVXpNVGsxUWpZeVJrUkZRdyJ9.eyJpc3MiOiJodHRwczovL2Rldi04N2V2eDlydS5hdXRoMC5jb20vIiwic3ViIjoiYVc0Q2NhNzl4UmVMV1V6MGFFMkg2a0QwTzNjWEJWdENAY2xpZW50cyIsImF1ZCI6Imh0dHBzOi8vZXhwZW5zZXMtYXBpIiwiaWF0IjoxNTcyMDA2OTU0LCJleHAiOjE1NzIwMDY5NjQsImF6cCI6ImFXNENjYTc5eFJlTFdVejBhRTJINmtEME8zY1hCVnRDIiwiZ3R5IjoiY2xpZW50LWNyZWRlbnRpYWxzIn0.PUxE7xn52aTCohGiWoSdMBZGiYAHwE5FYie0Y1qUT68IHSTXwXVd6hn02HTah6epvHHVKA2FqcFZ4GGv5VTHEvYpeggiiZMgbxFrmTEY0csL6VNkX1eaJGcuehwQCRBKRLL3zKmA5IKGy5GeUnIbpPHLHDxr-GXvgFzsdsyWlVQvPX2xjeaQ217r2PtxDeqjlf66UYl6oY6AqNS8DH3iryCvIfCcybRZkc_hdy-6ZMoKT6Piijvk_aXdm7-QQqKJFHLuEqrVSOuBqqiNfVrG27QzAPuPOxvfXTVLXL2jek5meH6n-VWgrBdoMFH93QEszEDowDAEhQPHVs0xj7SIzA"\n    key_entry = await fetcher.get_key(token)\n    token = jwt.decode(\n        jwt=token,\n        options={"verify_exp": False},\n        audience="https://expenses-api",\n        **key_entry\n    )\n    print(token)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n### Options\n\n#### Limiting issuers\n\nYou can limit the issuers you allow fetching keys from by setting the `valid_issuers`\nwhen creating the `AsyncKeyFetcher`, like this:\n\n```python\nAsyncKeyFetcher(valid_issuers=["https://example.com"])\n```\n\n#### Adjusting caching\n\nThe `AsyncKeyFetcher` will by default cache data for up to 32 different issuers with a\nTTL of 3600 seconds (1 hour) each. This means that in case of key-revocation, the key\nwill be trusted for up to 1 hour after it was removed from the JWKs.\n\nIf a previously unseen kid for an already seen issuer is seen, it will trigger a\nre-fetch of the JWKs, provided they have not been fetched in the past 5 minutes, in\norder to rather quickly react to new keys being published.\n\nThe amount of issuers to cache data for, as well as the cache time for the data can be\nadjusted like this:\n\n```python\nAsyncKeyFetcher(cache_maxsize=10, cache_ttl=2*60*60)\n```\n\nThe minimum interval for checking for new keys can for now not be adjusted.\n\n#### Loading configuration from a custom path\n\nYou can change from which path the configuration is loaded from the issuer (`iss`). By\ndefault, the configuration is assumed to be an OpenID Connect configuration and to be\nloaded from `/.well-known/openid-configuration`. As long as the configuration contains a\n`jwks_uri` you can change the configuration to be loaded from a custom path.\n\nYou can override the config path when creating the `AsyncKeyFetcher` like this:\n\n```python\nAsyncKeyFetcher(config_path="/.well-known/dataspace/party-configuration.json")\n```\n\n#### Using your own HTTP Client\n\nThe library ships with a `DefaultHTTPClient` that uses `aiohttp` for fetching the JSON\ndata; the openid-configuration and the jwks. If you want, you can write your own custom\nclient by inheriting from the `HTTPClient`. The only requirement is that it implements\nan async function to fetch JSON from a given URL and return it as a dictionary.\n',
-    'author': 'IOXIO',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ioxiocom/pyjwt-key-fetcher',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+Async library to fetch JWKs for JWT tokens.
 
+This library is intended to be used together with
+[PyJWT](https://pyjwt.readthedocs.io/en/stable/) to automatically verify keys signed by
+OpenID Connect providers. It retrieves the `iss` (issuer) and the `kid` (key ID) from
+the JWT, fetches the `.well-known/openid-configuration` from the issuer to find out the
+`jwks_uri` and fetches that to find the right key.
+
+This should give similar ability to verify keys as for example
+[https://jwt.io/](https://jwt.io/), where you can just paste in a token, and it will
+automatically reach out and retrieve the key for you.
+
+The `AsyncKeyFetcher` provided by this library acts as an improved async replacement for
+[PyJWKClient](https://pyjwt.readthedocs.io/en/2.6.0/usage.html#retrieve-rsa-signing-keys-from-a-jwks-endpoint).
+
+## Installation
+
+The package is available on PyPI:
+
+```bash
+pip install pyjwt-key-fetcher
+```
+
+## Usage
+
+### Example
+
+```python
+import asyncio
+
+import jwt
+
+from pyjwt_key_fetcher import AsyncKeyFetcher
+
+
+async def main():
+    fetcher = AsyncKeyFetcher()
+    # Token and options copied from
+    # https://pyjwt.readthedocs.io/en/2.6.0/usage.html#retrieve-rsa-signing-keys-from-a-jwks-endpoint
+    token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImtpZCI6Ik5FRTFRVVJCT1RNNE16STVSa0ZETlRZeE9UVTFNRGcyT0Rnd1EwVXpNVGsxUWpZeVJrUkZRdyJ9.eyJpc3MiOiJodHRwczovL2Rldi04N2V2eDlydS5hdXRoMC5jb20vIiwic3ViIjoiYVc0Q2NhNzl4UmVMV1V6MGFFMkg2a0QwTzNjWEJWdENAY2xpZW50cyIsImF1ZCI6Imh0dHBzOi8vZXhwZW5zZXMtYXBpIiwiaWF0IjoxNTcyMDA2OTU0LCJleHAiOjE1NzIwMDY5NjQsImF6cCI6ImFXNENjYTc5eFJlTFdVejBhRTJINmtEME8zY1hCVnRDIiwiZ3R5IjoiY2xpZW50LWNyZWRlbnRpYWxzIn0.PUxE7xn52aTCohGiWoSdMBZGiYAHwE5FYie0Y1qUT68IHSTXwXVd6hn02HTah6epvHHVKA2FqcFZ4GGv5VTHEvYpeggiiZMgbxFrmTEY0csL6VNkX1eaJGcuehwQCRBKRLL3zKmA5IKGy5GeUnIbpPHLHDxr-GXvgFzsdsyWlVQvPX2xjeaQ217r2PtxDeqjlf66UYl6oY6AqNS8DH3iryCvIfCcybRZkc_hdy-6ZMoKT6Piijvk_aXdm7-QQqKJFHLuEqrVSOuBqqiNfVrG27QzAPuPOxvfXTVLXL2jek5meH6n-VWgrBdoMFH93QEszEDowDAEhQPHVs0xj7SIzA"
+    key_entry = await fetcher.get_key(token)
+    token = jwt.decode(
+        jwt=token,
+        options={"verify_exp": False},
+        audience="https://expenses-api",
+        **key_entry
+    )
+    print(token)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+### Options
+
+#### Limiting issuers
+
+You can limit the issuers you allow fetching keys from by setting the `valid_issuers`
+when creating the `AsyncKeyFetcher`, like this:
+
+```python
+AsyncKeyFetcher(valid_issuers=["https://example.com"])
+```
+
+#### Adjusting caching
+
+The `AsyncKeyFetcher` will by default cache data for up to 32 different issuers with a
+TTL of 3600 seconds (1 hour) each. This means that in case of key-revocation, the key
+will be trusted for up to 1 hour after it was removed from the JWKs.
+
+If a previously unseen kid for an already seen issuer is seen, it will trigger a
+re-fetch of the JWKs, provided they have not been fetched in the past 5 minutes, in
+order to rather quickly react to new keys being published.
+
+The amount of issuers to cache data for, as well as the cache time for the data can be
+adjusted like this:
+
+```python
+AsyncKeyFetcher(cache_maxsize=10, cache_ttl=2*60*60)
+```
+
+The minimum interval for checking for new keys can for now not be adjusted.
+
+#### Loading configuration from a custom path
+
+You can change from which path the configuration is loaded from the issuer (`iss`). By
+default, the configuration is assumed to be an OpenID Connect configuration and to be
+loaded from `/.well-known/openid-configuration`. As long as the configuration contains a
+`jwks_uri` you can change the configuration to be loaded from a custom path.
+
+You can override the config path when creating the `AsyncKeyFetcher` like this:
+
+```python
+AsyncKeyFetcher(config_path="/.well-known/dataspace/party-configuration.json")
+```
+
+#### Using your own HTTP Client
+
+The library ships with a `DefaultHTTPClient` that uses `aiohttp` for fetching the JSON
+data; the openid-configuration and the jwks. If you want, you can write your own custom
+client by inheriting from the `HTTPClient`. The only requirement is that it implements
+an async function to fetch JSON from a given URL and return it as a dictionary.
 
-setup(**setup_kwargs)
```

