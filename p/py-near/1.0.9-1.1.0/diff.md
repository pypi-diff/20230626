# Comparing `tmp/py-near-1.0.9.tar.gz` & `tmp/py_near-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-near-1.0.9.tar", last modified: Thu Feb 16 18:56:28 2023, max compression
+gzip compressed data, was "py_near-1.1.0.tar", max compression
```

## Comparing `py-near-1.0.9.tar` & `py_near-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,33 @@
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.858235 py-near-1.0.9/
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1023 2022-06-08 20:31:53.000000 py-near-1.0.9/LICENSE
--rw-r--r--   0 petrvolnov   (501) staff       (20)     6013 2023-02-16 18:56:28.858077 py-near-1.0.9/PKG-INFO
--rw-r--r--   0 petrvolnov   (501) staff       (20)     3974 2023-01-24 19:13:04.000000 py-near-1.0.9/README.md
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1550 2023-02-16 18:54:32.000000 py-near-1.0.9/pyproject.toml
--rw-r--r--   0 petrvolnov   (501) staff       (20)       38 2023-02-16 18:56:28.858281 py-near-1.0.9/setup.cfg
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.849878 py-near-1.0.9/src/
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.852521 py-near-1.0.9/src/py_near/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       50 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)    13347 2023-02-16 18:28:35.000000 py-near-1.0.9/src/py_near/account.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      163 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/constants.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.853797 py-near-1.0.9/src/py_near/dapps/
--rw-r--r--   0 petrvolnov   (501) staff       (20)        0 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      231 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/core.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.854684 py-near-1.0.9/src/py_near/dapps/ft/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       29 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/ft/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     6717 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/ft/async_client.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)       92 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/ft/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      186 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/ft/models.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      856 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/fts.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.855712 py-near-1.0.9/src/py_near/dapps/keypom/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       32 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/keypom/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1422 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/keypom/async_client.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)       45 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/keypom/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     2166 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/keypom/models.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.856505 py-near-1.0.9/src/py_near/dapps/phone/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       32 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/phone/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     6849 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/phone/async_client.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)       45 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/phone/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      332 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/phone/models.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.857273 py-near-1.0.9/src/py_near/dapps/staking/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       34 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/staking/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     5203 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/staking/async_client.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)       92 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/staking/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      124 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/staking/models.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.857823 py-near-1.0.9/src/py_near/exceptions/
--rw-r--r--   0 petrvolnov   (501) staff       (20)        0 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/exceptions/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     4617 2023-01-25 01:37:42.000000 py-near-1.0.9/src/py_near/exceptions/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     7642 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/exceptions/provider.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     6418 2023-02-16 18:54:14.000000 py-near-1.0.9/src/py_near/models.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     8053 2023-01-29 18:06:54.000000 py-near-1.0.9/src/py_near/providers.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     2330 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/transactions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1528 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/utils.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.853356 py-near-1.0.9/src/py_near.egg-info/
--rw-r--r--   0 petrvolnov   (501) staff       (20)     6013 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/PKG-INFO
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1154 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/SOURCES.txt
--rw-r--r--   0 petrvolnov   (501) staff       (20)        1 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/dependency_links.txt
--rw-r--r--   0 petrvolnov   (501) staff       (20)       40 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/requires.txt
--rw-r--r--   0 petrvolnov   (501) staff       (20)        8 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1023 2022-06-08 20:31:53.650813 py_near-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3974 2023-01-24 19:13:04.795857 py_near-1.1.0/README.md
+-rw-r--r--   0        0        0     1562 2023-06-26 05:10:51.006333 py_near-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-01-24 19:13:04.796695 py_near-1.1.0/src/py_near/__init__.py
+-rw-r--r--   0        0        0    16398 2023-06-25 09:24:16.858826 py_near-1.1.0/src/py_near/account.py
+-rw-r--r--   0        0        0      164 2023-05-05 18:03:26.714114 py_near-1.1.0/src/py_near/constants.py
+-rw-r--r--   0        0        0        0 2023-01-24 19:13:04.797084 py_near-1.1.0/src/py_near/dapps/__init__.py
+-rw-r--r--   0        0        0      231 2023-01-24 19:13:04.797225 py_near-1.1.0/src/py_near/dapps/core.py
+-rw-r--r--   0        0        0       29 2023-01-24 19:13:04.797457 py_near-1.1.0/src/py_near/dapps/ft/__init__.py
+-rw-r--r--   0        0        0     6717 2023-01-24 19:13:04.797637 py_near-1.1.0/src/py_near/dapps/ft/async_client.py
+-rw-r--r--   0        0        0       92 2023-01-24 19:13:04.797752 py_near-1.1.0/src/py_near/dapps/ft/exceptions.py
+-rw-r--r--   0        0        0      186 2023-01-24 19:13:04.797873 py_near-1.1.0/src/py_near/dapps/ft/models.py
+-rw-r--r--   0        0        0      856 2023-01-24 19:13:04.797998 py_near-1.1.0/src/py_near/dapps/fts.py
+-rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798157 py_near-1.1.0/src/py_near/dapps/keypom/__init__.py
+-rw-r--r--   0        0        0     1422 2023-01-24 19:13:04.798347 py_near-1.1.0/src/py_near/dapps/keypom/async_client.py
+-rw-r--r--   0        0        0       45 2023-01-24 19:13:04.798480 py_near-1.1.0/src/py_near/dapps/keypom/exceptions.py
+-rw-r--r--   0        0        0     2166 2023-01-24 19:13:04.798618 py_near-1.1.0/src/py_near/dapps/keypom/models.py
+-rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798770 py_near-1.1.0/src/py_near/dapps/phone/__init__.py
+-rw-r--r--   0        0        0     6849 2023-01-24 19:13:04.799023 py_near-1.1.0/src/py_near/dapps/phone/async_client.py
+-rw-r--r--   0        0        0       45 2023-01-24 19:13:04.799162 py_near-1.1.0/src/py_near/dapps/phone/exceptions.py
+-rw-r--r--   0        0        0      332 2023-01-24 19:13:04.799299 py_near-1.1.0/src/py_near/dapps/phone/models.py
+-rw-r--r--   0        0        0       34 2023-01-24 19:13:04.799462 py_near-1.1.0/src/py_near/dapps/staking/__init__.py
+-rw-r--r--   0        0        0     5203 2023-01-24 19:13:04.799614 py_near-1.1.0/src/py_near/dapps/staking/async_client.py
+-rw-r--r--   0        0        0       92 2023-01-24 19:13:04.799691 py_near-1.1.0/src/py_near/dapps/staking/exceptions.py
+-rw-r--r--   0        0        0      124 2023-01-24 19:13:04.799806 py_near-1.1.0/src/py_near/dapps/staking/models.py
+-rw-r--r--   0        0        0        0 2023-01-24 19:13:04.799907 py_near-1.1.0/src/py_near/exceptions/__init__.py
+-rw-r--r--   0        0        0     4839 2023-06-23 06:51:52.490064 py_near-1.1.0/src/py_near/exceptions/exceptions.py
+-rw-r--r--   0        0        0     7642 2023-06-23 01:16:29.606235 py_near-1.1.0/src/py_near/exceptions/provider.py
+-rw-r--r--   0        0        0     9411 2023-06-25 09:24:16.865236 py_near-1.1.0/src/py_near/models.py
+-rw-r--r--   0        0        0     8328 2023-06-26 04:51:57.598319 py_near-1.1.0/src/py_near/providers.py
+-rw-r--r--   0        0        0     2566 2023-06-25 09:24:16.867476 py_near-1.1.0/src/py_near/transactions.py
+-rw-r--r--   0        0        0      126 2023-06-26 04:51:57.591322 py_near-1.1.0/src/py_near/utils.py
+-rw-r--r--   0        0        0     4650 1970-01-01 00:00:00.000000 py_near-1.1.0/PKG-INFO
```

### Comparing `py-near-1.0.9/LICENSE` & `py_near-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-near-1.0.9/PKG-INFO` & `py_near-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,24 @@
 Metadata-Version: 2.1
 Name: py-near
-Version: 1.0.9
-Summary: Pretty simple and fully asynchronous framework for working with NEAR blockchaink
-Author-email: pvolnov <petr@herewallet.app>
-License: Permission is hereby granted, free of charge, to any
-        person obtaining a copy of this software and associated
-        documentation files (the "Software"), to deal in the
-        Software without restriction, including without
-        limitation the rights to use, copy, modify, merge,
-        publish, distribute, sublicense, and/or sell copies of
-        the Software, and to permit persons to whom the Software
-        is furnished to do so, subject to the following
-        conditions:
-        
-        The above copyright notice and this permission notice
-        shall be included in all copies or substantial portions
-        of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-        ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-        TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-        PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-        SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-        CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-        OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-        IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-        DEALINGS IN THE SOFTWARE.
-        
-Project-URL: homepage, https://github.com/pvolnov/py-near
-Project-URL: documentation, https://py-near.readthedocs.io/en/latest
-Project-URL: repository, https://github.com/pvolnov/py-near
-Project-URL: changelog, https://github.com/pvolnov/py-near/blob/main/CHANGELOG.md
-Project-URL: funding, https://opencollective.com/py-near
-Project-URL: twitter, https://twitter.com/p_volnov
-Keywords: python,near,async
+Version: 1.1.0
+Summary: Pretty simple and fully asynchronous framework for working with NEAR blockchain
+Author: pvolnov
+Author-email: petr@herewallet.app
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
+Requires-Dist: ed25519 (>=1.5,<2.0)
+Requires-Dist: pyonear (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # py-near
 
 [![Financial Contributors on Open Collective](https://opencollective.com/py-near/all/badge.svg?style=flat-square)](https://opencollective.com/py-near) 
 [![PyPi Package Version](https://img.shields.io/pypi/v/py-near?style=flat-square)](https://pypi.org/project/py-near)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/py-near)](https://pypi.python.org/pypi/py-near)
 [![Documentation Status](https://img.shields.io/readthedocs/py-near?style=flat-square)](https://py-near.readthedocs.io/en/latest)
@@ -159,7 +134,8 @@
 
 ## Contributors
 
 ### Code Contributors
 
 This project exists thanks to all the people who contribute. [[Code of conduct](CODE_OF_CONDUCT.md)].
 <a href="https://github.com/pvolnov/py-near/graphs/contributors"><img src="https://opencollective.com/py-near/contributors.svg?width=890&button=false" /></a>
+
```

### Comparing `py-near-1.0.9/README.md` & `py_near-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py-near-1.0.9/pyproject.toml` & `py_near-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-near"
-version = "1.0.6"
+version = "1.1.0"
 description="Pretty simple and fully asynchronous framework for working with NEAR blockchain"
 authors = ["pvolnov <petr@herewallet.app>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 ed25519 = "^1.5"
@@ -18,20 +18,20 @@
 flake8 = "^4.0.1"
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
 base58 = "^2.1.1"
 
 [project]
 name = "py-near"
-version = "1.0.9"
+version = "1.0.10"
 description = "Pretty simple and fully asynchronous framework for working with NEAR blockchaink"
 authors = [ {name = "pvolnov", email = "petr@herewallet.app"} ]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
-dependencies=["base58", "ed25519", "aiohttp", "pyonear", "pydantic"]
+dependencies=["base58", "ed25519", "aiohttp", "py-near-primitives", "pydantic"]
 keywords = ["python", "near", "async"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 readme = "README.md"
```

### Comparing `py-near-1.0.9/src/py_near/account.py` & `py_near-1.1.0/src/py_near/account.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import asyncio
 import collections
 import json
 from typing import List, Union, Dict, Optional
 
 import base58
-from pyonear.account_id import AccountId
-from pyonear.crypto import InMemorySigner, ED25519SecretKey, Signer
-from pyonear.transaction import Action
+import ed25519
+from py_near_primitives import DelegateAction
 
 from py_near import constants
 from py_near import transactions
 from py_near import utils
 from py_near.dapps.ft.async_client import FT
 from py_near.dapps.phone.async_client import Phone
 from py_near.dapps.staking.async_client import Staking
 from py_near.exceptions.exceptions import parse_error
 from py_near.models import (
     TransactionResult,
     ViewFunctionResult,
     PublicKey,
     AccountAccessKey,
+    DelegateActionModel,
+    Action,
 )
 from py_near.providers import JsonProvider
 
 
 class ViewFunctionError(Exception):
     pass
 
@@ -34,14 +35,15 @@
     """
 
     _access_key: dict
     _lock: asyncio.Lock = None
     _lock_by_pk: Dict[str, asyncio.Lock] = {}
     _latest_block_hash: str
     _latest_block_hash_ts: float = 0
+    _latest_block_height: int = 0
     chain_id: str = "mainnet"
 
     def __init__(
         self,
         account_id: str = None,
         private_key: Union[List[Union[str, bytes]], str, bytes] = None,
         rpc_addr="https://rpc.mainnet.near.org",
@@ -57,25 +59,26 @@
         elif isinstance(private_key, bytes):
             private_keys = [private_key]
         else:
             return
 
         self._free_signers = asyncio.Queue()
         self._signers = []
+        self._signer_by_pk: Dict[str, bytes] = {}
+
         for pk in private_keys:
             if isinstance(pk, str):
                 pk = base58.b58decode(pk.replace("ed25519:", ""))
-            key = ED25519SecretKey(pk)
-            singer = InMemorySigner(
-                AccountId(account_id),
-                key.public_key(),
-                key,
-            )
-            self._free_signers.put_nowait(singer)
-            self._signers.append(singer)
+            private_key = ed25519.SigningKey(pk)
+            public_key = base58.b58encode(
+                private_key.get_verifying_key().to_bytes()
+            ).decode("utf-8")
+            self._signer_by_pk[public_key] = pk
+            self._free_signers.put_nowait(pk)
+            self._signers.append(pk)
 
     async def startup(self):
         """
         Initialize async object
         :return:
         """
         self._lock = asyncio.Lock()
@@ -88,14 +91,17 @@
         :return: last block hash
         """
         if self._latest_block_hash_ts + 50 > utils.timestamp():
             return
         self._latest_block_hash = (await self._provider.get_status())["sync_info"][
             "latest_block_hash"
         ]
+        self._latest_block_height = (await self._provider.get_status())["sync_info"][
+            "latest_block_height"
+        ]
         self._latest_block_hash_ts = utils.timestamp()
 
     async def _sign_and_submit_tx(
         self, receiver_id, actions: List[Action], nowait=False
     ) -> Union[TransactionResult, str]:
         """
         Sign transaction and send it to blockchain
@@ -103,62 +109,71 @@
         :param actions: list of actions
         :param nowait: if nowait is True, return transaction hash, else wait execution
         confirm and return TransactionResult
         :return: transaction hash or TransactionResult
         """
         if not self._signers:
             raise ValueError("You must provide a private key or seed to call methods")
-        signer = await self._free_signers.get()
+        pk = await self._free_signers.get()
 
         try:
-            access_key = await self.get_access_key(signer)
+            access_key = await self.get_access_key(pk)
             await self._update_last_block_hash()
 
             block_hash = base58.b58decode(self._latest_block_hash.encode("utf8"))
             serialized_tx = transactions.sign_and_serialize_transaction(
+                self.account_id,
+                pk,
                 receiver_id,
                 access_key.nonce + 1,
                 actions,
                 block_hash,
-                signer,
             )
             if nowait:
                 return await self._provider.send_tx(serialized_tx)
             result = await self._provider.send_tx_and_wait(serialized_tx)
 
             if "Failure" in result["status"]:
+                if isinstance(result["status"]["Failure"]["ActionError"]["kind"], str):
+                    error_type = result["status"]["Failure"]["ActionError"]["kind"]
+                    raise parse_error(error_type, {})
+
                 error_type, args = list(
                     result["status"]["Failure"]["ActionError"]["kind"].items()
                 )[0]
                 raise parse_error(error_type, args)
             return TransactionResult(**result)
         except Exception as e:
             raise e
         finally:
-            await self._free_signers.put(signer)
+            await self._free_signers.put(pk)
 
     @property
-    def signer(self) -> Optional[InMemorySigner]:
+    def signer(self) -> Optional[bytes]:
         if not self._signers:
             return None
         return self._signers[0]
 
     @property
     def provider(self) -> JsonProvider:
         return self._provider
 
-    async def get_access_key(self, signer: Signer = None) -> AccountAccessKey:
+    async def get_access_key(self, pk: bytes) -> AccountAccessKey:
         """
         Get access key for current account
         :return: AccountAccessKey
         """
-        if signer is None:
-            signer = self._signers[0]
+        if pk is None:
+            pk = self._signers[0]
+
+        private_key = ed25519.SigningKey(pk)
+        public_key = private_key.get_verifying_key()
+
         resp = await self._provider.get_access_key(
-            self.account_id, str(signer.public_key)
+            self.account_id, base58.b58encode(public_key.to_bytes()).decode("utf8")
         )
         if "error" in resp:
             raise ValueError(resp["error"])
         return AccountAccessKey(**resp)
 
     async def get_access_key_list(self, account_id: str = None) -> List[PublicKey]:
         """
@@ -290,14 +305,32 @@
         :return: transaction hash or TransactionResult
         """
         actions = [
             transactions.create_delete_access_key_action(public_key),
         ]
         return await self._sign_and_submit_tx(self.account_id, actions, nowait)
 
+    async def call_delegate_transaction(
+        self,
+        delegate_action: Union[DelegateAction, DelegateActionModel],
+        signature: Union[bytes, str],
+        nowait=False,
+    ):
+        if isinstance(signature, str):
+            signature = base58.b58decode(signature.replace("ed25519:", ""))
+        if isinstance(delegate_action, DelegateActionModel):
+            delegate_action = delegate_action.near_delegate_action
+
+        actions = [
+            transactions.create_signed_delegate(delegate_action, signature),
+        ]
+        return await self._sign_and_submit_tx(
+            delegate_action.sender_id, actions, nowait
+        )
+
     async def deploy_contract(self, contract_code: bytes, nowait=False):
         """
         Deploy smart contract to account
         :param contract_code: smart contract code
         :param nowait: if nowait is True, return transaction hash, else wait execution
         :return: transaction hash or TransactionResult
         """
@@ -335,14 +368,64 @@
             contract_id, method_name, json.dumps(args).encode("utf8")
         )
         if "error" in result:
             raise ViewFunctionError(result["error"])
         result["result"] = json.loads("".join([chr(x) for x in result["result"]]))
         return ViewFunctionResult(**result)
 
+    async def create_delegate_action(
+        self, actions: List[Action], receiver_id, public_key: Optional[str] = None
+    ):
+        """
+        Create delegate action from list of actions
+        :param actions:
+        :param receiver_id:
+        :return:
+        """
+        if public_key is None:
+            pk = self._signers[0]
+        else:
+            pk = self._signer_by_pk[public_key]
+        access_key = await self.get_access_key(pk)
+        await self._update_last_block_hash()
+
+        private_key = ed25519.SigningKey(pk)
+        public_key = private_key.get_verifying_key()
+        return DelegateActionModel(
+            sender_id=self.account_id,
+            receiver_id=receiver_id,
+            actions=actions,
+            nonce=access_key.nonce + 1,
+            max_block_height=self._latest_block_height + 1000,
+            public_key=base58.b58encode(public_key.to_bytes()).decode("utf-8"),
+        )
+
+    def sign_delegate_transaction(
+        self, delegate_action: Union[DelegateAction, DelegateActionModel]
+    ) -> str:
+        """
+        Sign delegate transaction
+        :param delegate_action: DelegateAction or DelegateActionModel
+        :return: signature (bytes)
+        """
+        if isinstance(delegate_action, DelegateActionModel):
+            delegate_action = delegate_action.near_delegate_action
+        nep461_hash = bytes(bytearray(delegate_action.get_nep461_hash()))
+
+        public_key = base58.b58encode(
+            bytes(bytearray(delegate_action.public_key))
+        ).decode("utf-8")
+
+        if public_key not in self._signer_by_pk:
+            raise ValueError(f"Public key {public_key} not found in signer list")
+
+        private_key = ed25519.SigningKey(self._signer_by_pk[public_key])
+        sign = private_key.sign(nep461_hash)
+        return base58.b58encode(sign).decode("utf-8")
+
     async def get_balance(self, account_id: str = None) -> int:
         """
         Get account balance
         :param account_id: if account_id is None, return balance of current account
         :return: balance of account in yoctoNEAR
         """
         if account_id is None:
```

### Comparing `py-near-1.0.9/src/py_near/dapps/ft/async_client.py` & `py_near-1.1.0/src/py_near/dapps/ft/async_client.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.9/src/py_near/dapps/fts.py` & `py_near-1.1.0/src/py_near/dapps/fts.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.9/src/py_near/dapps/keypom/async_client.py` & `py_near-1.1.0/src/py_near/dapps/keypom/async_client.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.9/src/py_near/dapps/keypom/models.py` & `py_near-1.1.0/src/py_near/dapps/keypom/models.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.9/src/py_near/dapps/phone/async_client.py` & `py_near-1.1.0/src/py_near/dapps/phone/async_client.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.9/src/py_near/dapps/staking/async_client.py` & `py_near-1.1.0/src/py_near/dapps/staking/async_client.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.9/src/py_near/exceptions/exceptions.py` & `py_near-1.1.0/src/py_near/exceptions/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -166,14 +166,21 @@
 class NewReceiptValidationError(ActionErrorKind):
     """
     Error occurs when a new `ActionReceipt` created by the `FunctionCall` action fails
     """
 
     pass
 
+class DelegateActionExpired(ActionErrorKind):
+    """
+    Error occurs when a new `DelegateActionExpired` created by the `FunctionCall` action fails
+    """
+
+    pass
+
 
 _ERROR_TYPE_TO_EXCEPTION = {
     "AccountAlreadyExists": AccountAlreadyExistsError,
     "AccountDoesNotExist": AccountDoesNotExistError,
     "CreateAccountNotAllowed": CreateAccountNotAllowedError,
     "ActorNoPermission": ActorNoPermissionError,
     "DeleteKeyDoesNotExist": DeleteKeyDoesNotExistError,
@@ -182,12 +189,13 @@
     "DeleteAccountHasRent": DeleteAccountHasRentError,
     "RentUnpaid": RentUnpaidError,
     "TriesToUnstake": TriesToUnstakeError,
     "TriesToStake": TriesToStakeError,
     "FunctionCallError": FunctionCallError,
     "ExecutionError": ExecutionError,
     "NewReceiptValidationError": NewReceiptValidationError,
+    "'DelegateActionExpired'": DelegateActionExpired,
 }
 
 
 def parse_error(error_type, args):
     return _ERROR_TYPE_TO_EXCEPTION[error_type](**args)
```

### Comparing `py-near-1.0.9/src/py_near/exceptions/provider.py` & `py_near-1.1.0/src/py_near/exceptions/provider.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.9/src/py_near/providers.py` & `py_near-1.1.0/src/py_near/providers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import base64
 import json
 
 import aiohttp
 from aiohttp import ClientResponseError, ClientConnectorError
+from loguru import logger
+
+from py_near.constants import TIMEOUT_WAIT_RPC
+
 from py_near.models import TransactionResult
 
 from py_near import constants
 from py_near.exceptions.exceptions import RpcNotAvailableError
 from py_near.exceptions.provider import (
     UnknownBlockError,
     InvalidAccount,
@@ -45,59 +49,62 @@
         if isinstance(rpc_addr, tuple):
             self._rpc_addresses = ["http://{}:{}".format(*rpc_addr)]
         elif isinstance(rpc_addr, list):
             self._rpc_addresses = rpc_addr
         else:
             self._rpc_addresses = [rpc_addr]
 
-    async def call_rpc_request(self, method, params, timeout=60):
+    async def call_rpc_request(self, method, params, timeout=TIMEOUT_WAIT_RPC):
         j = {"method": method, "params": params, "id": "dontcare", "jsonrpc": "2.0"}
 
         content = None
         for rpc_addr in self._rpc_addresses:
             try:
                 async with aiohttp.ClientSession() as session:
-                    r = await session.post(rpc_addr, json=j, timeout=30)
+                    r = await session.post(rpc_addr, json=j, timeout=timeout)
                     r.raise_for_status()
                     content = json.loads(await r.text())
                 if self._rpc_addresses[0] != rpc_addr:
+                    logger.info(f"Rpc update: {rpc_addr}")
                     self._rpc_addresses.remove(rpc_addr)
                     self._rpc_addresses.insert(0, rpc_addr)
                 break
-            except ClientResponseError:
-                continue
-            except ClientConnectorError:
-                continue
-            except RpcTimeoutError:
-                continue
-            except ConnectionError:
+            except (
+                RpcTimeoutError,
+                ClientResponseError,
+                ClientConnectorError,
+                ConnectionError,
+            ) as e:
+                logger.error(f"Rpc error: {e}")
                 continue
         return content
 
     @staticmethod
     def get_error_from_response(content: dict):
         if "error" in content:
             error_code = content["error"].get("cause", {}).get("name", "")
             body = content["error"]["data"]
             error = PROVIDER_CODE_TO_EXCEPTION.get(error_code, InternalError)(
                 body, error_json=content["error"]
             )
             while True:
                 if not isinstance(body, dict):
                     break
+                if not body:
+                    return error
                 key, body = list(body.items())[0]
                 if key in ERROR_CODE_TO_EXCEPTION:
                     error = ERROR_CODE_TO_EXCEPTION[key](
                         body, error_json=content["error"]
                     )
                 else:
                     break
             return error
 
-    async def json_rpc(self, method, params, timeout=60):
+    async def json_rpc(self, method, params, timeout=TIMEOUT_WAIT_RPC):
         content = await self.call_rpc_request(method, params, timeout)
         if not content:
             raise RpcNotAvailableError("RPC not available")
 
         error = self.get_error_from_response(content)
         if error:
             raise error
@@ -125,15 +132,17 @@
             "broadcast_tx_commit",
             [signed_tx],
             timeout=timeout,
         )
 
     async def get_status(self):
         async with aiohttp.ClientSession() as session:
-            r = await session.get("%s/status" % self._rpc_addresses[0], timeout=60)
+            r = await session.get(
+                "%s/status" % self._rpc_addresses[0], timeout=TIMEOUT_WAIT_RPC
+            )
             r.raise_for_status()
             return json.loads(await r.text())
 
     async def get_validators(self):
         return await self.json_rpc("validators", [None])
 
     async def query(self, query_object):
```

