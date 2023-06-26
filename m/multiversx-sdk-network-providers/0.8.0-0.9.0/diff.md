# Comparing `tmp/multiversx_sdk_network_providers-0.8.0.tar.gz` & `tmp/multiversx_sdk_network_providers-0.9.0.tar.gz`

## Comparing `multiversx_sdk_network_providers-0.8.0.tar` & `multiversx_sdk_network_providers-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.flake8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/py.typed
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/pyrightconfig.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/requirements-dev.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/requirements.txt
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.github/workflows/linter-flake8.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.github/workflows/linter-pyright.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/__init__.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/accounts.py
--rw-r--r--   0        0        0    10897 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/api_network_provider.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/api_network_provider_test.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/config.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/constants.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_query_requests.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_query_response.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_results.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/errors.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/interface.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_config.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_general_statistics.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_stake.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_status.py
--rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/proxy_network_provider.py
--rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/proxy_network_provider_test.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/resources.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/token_definitions.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/tokens.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_completion_strategy.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_events.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_logs.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_receipt.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_status.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transactions.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/utils.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/LICENSE
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/.flake8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/py.typed
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/pyrightconfig.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/requirements-dev.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/requirements.txt
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/.github/workflows/linter-flake8.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/.github/workflows/linter-pyright.yml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/__init__.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/accounts.py
+-rw-r--r--   0        0        0    10897 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/api_network_provider.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/api_network_provider_test.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/config.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/constants.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/contract_query_requests.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/contract_query_response.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/contract_results.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/errors.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/interface.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/network_config.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/network_general_statistics.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/network_stake.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/network_status.py
+-rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/proxy_network_provider.py
+-rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/proxy_network_provider_test.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/resources.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/token_definitions.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/tokens.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_completion_strategy.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_events.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_logs.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_receipt.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_status.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transactions.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/utils.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.9.0/PKG-INFO
```

### Comparing `multiversx_sdk_network_providers-0.8.0/.github/workflows/linter-flake8.yml` & `multiversx_sdk_network_providers-0.9.0/.github/workflows/linter-flake8.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/.github/workflows/linter-pyright.yml` & `multiversx_sdk_network_providers-0.9.0/.github/workflows/linter-pyright.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/.github/workflows/python-publish.yml` & `multiversx_sdk_network_providers-0.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/.github/workflows/test.yml` & `multiversx_sdk_network_providers-0.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/accounts.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/api_network_provider.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/api_network_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/api_network_provider_test.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/api_network_provider_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_query_requests.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/contract_query_requests.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_query_response.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/contract_query_response.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_results.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/contract_results.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/interface.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/interface.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_config.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/network_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_general_statistics.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/network_general_statistics.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_stake.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/network_stake.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_status.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/network_status.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/proxy_network_provider.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/proxy_network_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/proxy_network_provider_test.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/proxy_network_provider_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/resources.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/resources.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/token_definitions.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/token_definitions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/tokens.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/tokens.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_completion_strategy.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_completion_strategy.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_events.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,11 +38,11 @@
 
 
 class TransactionEventTopic:
     def __init__(self, topic: str):
         self.raw = base64.b64decode(topic.encode())
 
     def __str__(self):
-        return base64.b64encode(self.raw).decode()
+        return self.raw.decode()
 
     def hex(self):
         return self.raw.hex()
```

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_logs.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_logs.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_receipt.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_receipt.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_status.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transaction_status.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transactions.py` & `multiversx_sdk_network_providers-0.9.0/multiversx_sdk_network_providers/transactions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/.gitignore` & `multiversx_sdk_network_providers-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/LICENSE` & `multiversx_sdk_network_providers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/README.md` & `multiversx_sdk_network_providers-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.8.0/pyproject.toml` & `multiversx_sdk_network_providers-0.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "multiversx-sdk-network-providers"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "Network providers for MultiversX Python SDK."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `multiversx_sdk_network_providers-0.8.0/PKG-INFO` & `multiversx_sdk_network_providers-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-network-providers
-Version: 0.8.0
+Version: 0.9.0
 Summary: Network providers for MultiversX Python SDK.
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-network-providers
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

