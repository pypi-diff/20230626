# Comparing `tmp/firefly_exchange_client-0.4.0.tar.gz` & `tmp/firefly_exchange_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly_exchange_client-0.4.0.tar", last modified: Tue Jun 20 13:22:18 2023, max compression
+gzip compressed data, was "firefly_exchange_client-0.5.0.tar", last modified: Mon Jun 26 19:22:21 2023, max compression
```

## Comparing `firefly_exchange_client-0.4.0.tar` & `firefly_exchange_client-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:18.178067 firefly_exchange_client-0.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/src/firefly_exchange_client/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    37256 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/contract_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/onboarding_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/order_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/socket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:21.585265 firefly_exchange_client-0.5.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/src/firefly_exchange_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37470 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/contract_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/onboarding_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/order_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/socket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/top_level.txt
```

### Comparing `firefly_exchange_client-0.4.0/LICENSE` & `firefly_exchange_client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/PKG-INFO` & `firefly_exchange_client-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly_exchange_client
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.4.0/README.md` & `firefly_exchange_client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/pyproject.toml` & `firefly_exchange_client-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "firefly_exchange_client"
-version = "0.4.0"
+version = "0.5.0"
 description = "Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["firefly", "exchange", "decentralized", "perpetuals", "blockchain"]
 dependencies = [
   'web3 ~= 5.31.3',
   'requests ~= 2.28.1',
```

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/api_service.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/api_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 import aiohttp
 from .interfaces import *
 
 
 class APIService():
-    def __init__(self, url):
+    def __init__(self, url, UUID=""):
         self.server_url = url
         self.auth_token = None
         self.api_token = None
+        self.uuid = UUID
         self.client = aiohttp.ClientSession()
 
     async def close_session(self):
         if self.client is not None:
             return await self.client.close()
 
     async def get(self, service_url, query={}, auth_required=False):
@@ -27,43 +28,48 @@
         response = None
         if auth_required:
             response = await self.client.get(
                 url,
                 params=query,
                 headers={
                     'Authorization': 'Bearer {}'.format(self.auth_token) if self.auth_token else '',
-                    'x-api-token': self.api_token or ''
+                    'x-api-token': self.api_token or '',
+                    'x-mm-id': self.uuid or ''
+
                 }
             )
         else:
             response = await self.client.get(url, params=query)
 
         try:
             if response.status != 503:  # checking for service unavailitbility
                 return await response.json()
             else:
                 return response
         except:
             raise Exception("Error while getting {}: {}".format(url, response))
 
-    async def post(self, service_url, data, auth_required=False, contentType = ""):
+    async def post(self, service_url, data, auth_required=False, contentType=""):
         """
             Makes a POST request and returns the results
             Inputs:
                 - service_url(str): the url to make the request to.
                 - data(dict): the data to post with POST request.
                 - auth_required(bool): indicates whether authorization is required for the call or not.
         """
         url = self._create_url(service_url)
         response = None
         if auth_required:
-            headers = {'Authorization': 'Bearer {}'.format(self.auth_token)}
+            headers = {
+                'Authorization': 'Bearer {}'.format(self.auth_token),
+                'x-mm-id': self.uuid or ''
+            }
 
             if contentType is not "":
-               headers['Content-type'] = contentType
+                headers['Content-type'] = contentType
 
             response = await self.client.post(url=url, data=data, headers=headers)
         else:
             response = await self.client.post(url=url, data=data)
 
         try:
             if response.status != 503:  # checking for service unavailitbility
@@ -85,15 +91,16 @@
         url = self._create_url(service_url)
 
         response = None
         if auth_required:
             response = await self.client.delete(
                 url=url,
                 data=data,
-                headers={'Authorization': 'Bearer {}'.format(self.auth_token)})
+                headers={'Authorization': 'Bearer {}'.format(self.auth_token),
+                 'x-mm-id': self.uuid or ''})
         else:
             response = await self.client.delete(url=url, data=data)
 
         try:
             return await response.json()
         except:
             raise Exception(
```

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/client.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class FireflyClient:
     def __init__(self, are_terms_accepted, network, private_key=""):
         self.are_terms_accepted = are_terms_accepted
         self.network = network
         self.w3 = self._connect_w3(self.network["url"])
         if private_key != "":
             self.account = Account.from_key(private_key)
-        self.apis = APIService(self.network["apiGateway"])
+        self.apis = APIService(self.network["apiGateway"], default_value(self.network, "UUID", "") )
         self.dmsApi = APIService(self.network["dmsURL"])
         self.socket = Sockets(self.network["socketURL"])
         self.webSocketClient = WebsocketClient(self.network["webSocketURL"])
         self.contracts = Contracts()
         self.order_signers = {}
         self.onboarding_signer = OnboardingSigner()
         
@@ -942,8 +942,15 @@
         """
             Creates a connection to Web3 RPC given the RPC url.
         """
         try:
             return Web3(Web3.HTTPProvider(url))
         except:
             raise(Exception("Failed to connect to Host: {}".format(url)))
+           
+
+
+    async def close_connections(self):
+         # close aio http connection
+        await self.apis.close_session()
+        await self.dmsApi.close_session()
```

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/constants.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "url": "https://goerli-rollup.arbitrum.io/rpc",
     "chainId": 421613,
     "apiGateway": "https://dapi.api.arbitrum-staging.firefly.exchange",
     "dmsURL": "https://api.arbitrum-staging.firefly.exchange/dead-man-switch",
     "socketURL": "wss://dapi.api.arbitrum-staging.firefly.exchange",
     "webSocketURL": "wss://notifications.api.arbitrum-staging.firefly.exchange",
     "onboardingUrl": "https://testnet.firefly.exchange",
+    "UUID": "uuid-default"
   },
 
   "MAINNET_BOBA": {
     "url": "https://bobabeam.boba.network/",
     "chainId": 1294,
     "apiGateway": "https://dapi.firefly.exchange",
     "socketURL": "wss://dapi.firefly.exchange",
@@ -28,14 +29,15 @@
     "url": "https://arb1.arbitrum.io/rpc/",
     "chainId": 42161,
     "apiGateway": "https://dapi.api.arbitrum-prod.firefly.exchange",
     "dmsURL": "https://api.arbitrum-prod.firefly.exchange/dead-man-switch",
     "socketURL": "wss://dapi.api.arbitrum-prod.firefly.exchange",
     "webSocketURL": "wss://notifications.api.arbitrum-prod.firefly.exchange",
     "onboardingUrl": "https://trade-arb.firefly.exchange",
+    "UUID": "uuid-default"
   },
 }
 
 
 EIP712_DOMAIN_NAME = "IsolatedTrader"
```

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/contract_abis.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/contract_abis.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/contracts.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/contracts.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/enumerations.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/enumerations.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/interfaces.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/interfaces.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/onboarding_signer.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/onboarding_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/order_signer.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/order_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/signer.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/socket_manager.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/socket_manager.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/sockets.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/sockets.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/utilities.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/utilities.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client/websocket_client.py` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client/websocket_client.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/PKG-INFO` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly-exchange-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/SOURCES.txt` & `firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

