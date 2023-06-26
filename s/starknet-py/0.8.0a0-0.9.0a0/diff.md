# Comparing `tmp/starknet_py-0.8.0a0.tar.gz` & `tmp/starknet_py-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starknet_py-0.8.0a0.tar", max compression
+gzip compressed data, was "starknet_py-0.9.0a0.tar", max compression
```

## Comparing `starknet_py-0.8.0a0.tar` & `starknet_py-0.9.0a0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
--rw-r--r--   0        0        0     1073 2022-10-24 07:29:20.060272 starknet_py-0.8.0a0/LICENSE.txt
--rw-r--r--   0        0        0     2653 2022-10-24 07:29:20.060272 starknet_py-0.8.0a0/README.md
--rw-r--r--   0        0        0     3078 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/cairo/__init__.py
--rw-r--r--   0        0        0     2341 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/cairo/felt.py
--rw-r--r--   0        0        0      844 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/common.py
--rw-r--r--   0        0        0        0 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/compile/__init__.py
--rw-r--r--   0        0        0     4013 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/compile/compiler.py
--rw-r--r--   0        0        0      138 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/conftest.py
--rw-r--r--   0        0        0      783 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/constants.py
--rw-r--r--   0        0        0    22957 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/contract.py
--rw-r--r--   0        0        0       59 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/net/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/net/account/__init__.py
--rw-r--r--   0        0        0    28682 2022-10-24 07:29:20.064272 starknet_py-0.8.0a0/starknet_py/net/account/account_client.py
--rw-r--r--   0        0        0  1264473 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/account/compiled_account_contract.py
--rw-r--r--   0        0        0    10724 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/client.py
--rw-r--r--   0        0        0     1120 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/client_errors.py
--rw-r--r--   0        0        0     6966 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/client_models.py
--rw-r--r--   0        0        0      416 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/client_utils.py
--rw-r--r--   0        0        0    16539 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/full_node_client.py
--rw-r--r--   0        0        0    14676 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/gateway_client.py
--rw-r--r--   0        0        0     3555 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/http_client.py
--rw-r--r--   0        0        0        0 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/l1/__init__.py
--rw-r--r--   0        0        0     2904 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/l1/contracts.py
--rw-r--r--   0        0        0     7750 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/l1/messages.py
--rw-r--r--   0        0        0    11867 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/l1/starknet_l1_abi.py
--rw-r--r--   0        0        0      331 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/models/__init__.py
--rw-r--r--   0        0        0     1362 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/models/address.py
--rw-r--r--   0        0        0      879 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/models/chains.py
--rw-r--r--   0        0        0     2594 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/models/transaction.py
--rw-r--r--   0        0        0      588 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/models/typed_data.py
--rw-r--r--   0        0        0      464 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/networks.py
--rw-r--r--   0        0        0        0 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/schemas/__init__.py
--rw-r--r--   0        0        0     3082 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/schemas/common.py
--rw-r--r--   0        0        0    12850 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/schemas/gateway.py
--rw-r--r--   0        0        0    10627 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/schemas/rpc.py
--rw-r--r--   0        0        0       36 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/signer/__init__.py
--rw-r--r--   0        0        0     1233 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/signer/base_signer.py
--rw-r--r--   0        0        0     4622 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/signer/stark_curve_signer.py
--rw-r--r--   0        0        0     1619 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/net/signer/test_stark_curve_signer.py
--rw-r--r--   0        0        0     1751 2022-10-24 07:29:20.068271 starknet_py-0.8.0a0/starknet_py/proxy_check.py
--rw-r--r--   0        0        0     1042 2022-10-24 07:29:20.076272 starknet_py-0.8.0a0/starknet_py/transaction_exceptions.py
--rw-r--r--   0        0        0        0 2022-10-24 07:29:20.076272 starknet_py-0.8.0a0/starknet_py/transactions/__init__.py
--rw-r--r--   0        0        0     1851 2022-10-24 07:29:20.076272 starknet_py-0.8.0a0/starknet_py/transactions/declare.py
--rw-r--r--   0        0        0     2458 2022-10-24 07:29:20.076272 starknet_py-0.8.0a0/starknet_py/transactions/deploy.py
--rw-r--r--   0        0        0        0 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/crypto/__init__.py
--rw-r--r--   0        0        0     1311 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/crypto/facade.py
--rw-r--r--   0        0        0       87 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/data_transformer/__init__.py
--rw-r--r--   0        0        0    16310 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/data_transformer/data_transformer.py
--rw-r--r--   0        0        0      342 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/data_transformer/errors.py
--rw-r--r--   0        0        0     2311 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/data_transformer/execute_transformer.py
--rw-r--r--   0        0        0      637 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/docs.py
--rw-r--r--   0        0        0      301 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/iterable.py
--rw-r--r--   0        0        0      152 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/sync/__init__.py
--rw-r--r--   0        0        0     1355 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/sync/sync.py
--rw-r--r--   0        0        0     4994 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/typed_data.py
--rw-r--r--   0        0        0      489 2022-10-24 07:29:20.080272 starknet_py-0.8.0a0/starknet_py/utils/types.py
--rw-r--r--   0        0        0     4032 1970-01-01 00:00:00.000000 starknet_py-0.8.0a0/setup.py
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 starknet_py-0.8.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-11-14 14:35:42.435674 starknet_py-0.9.0a0/LICENSE.txt
+-rw-r--r--   0        0        0     2653 2022-11-14 14:35:42.435674 starknet_py-0.9.0a0/README.md
+-rw-r--r--   0        0        0     3206 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/cairo/__init__.py
+-rw-r--r--   0        0        0     2341 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/cairo/felt.py
+-rw-r--r--   0        0        0      844 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/common.py
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/compile/__init__.py
+-rw-r--r--   0        0        0     4013 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/compile/compiler.py
+-rw-r--r--   0        0        0      583 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/conftest.py
+-rw-r--r--   0        0        0      640 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/constants.py
+-rw-r--r--   0        0        0    21046 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/contract.py
+-rw-r--r--   0        0        0       59 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/net/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/net/account/__init__.py
+-rw-r--r--   0        0        0    27660 2022-11-14 14:35:42.439674 starknet_py-0.9.0a0/starknet_py/net/account/account_client.py
+-rw-r--r--   0        0        0  1264473 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/account/compiled_account_contract.py
+-rw-r--r--   0        0        0    10429 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/client.py
+-rw-r--r--   0        0        0     1120 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/client_errors.py
+-rw-r--r--   0        0        0     7030 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/client_models.py
+-rw-r--r--   0        0        0      965 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/client_utils.py
+-rw-r--r--   0        0        0    16863 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/full_node_client.py
+-rw-r--r--   0        0        0    14297 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/gateway_client.py
+-rw-r--r--   0        0        0     3555 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/http_client.py
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/l1/__init__.py
+-rw-r--r--   0        0        0     2904 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/l1/contracts.py
+-rw-r--r--   0        0        0     7750 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/l1/messages.py
+-rw-r--r--   0        0        0    11867 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/l1/starknet_l1_abi.py
+-rw-r--r--   0        0        0      331 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/models/__init__.py
+-rw-r--r--   0        0        0     1362 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/models/address.py
+-rw-r--r--   0        0        0      879 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/models/chains.py
+-rw-r--r--   0        0        0     2594 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/models/transaction.py
+-rw-r--r--   0        0        0      588 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/models/typed_data.py
+-rw-r--r--   0        0        0      464 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/networks.py
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/schemas/__init__.py
+-rw-r--r--   0        0        0     3082 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/schemas/common.py
+-rw-r--r--   0        0        0    12903 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/schemas/gateway.py
+-rw-r--r--   0        0        0    11084 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/schemas/rpc.py
+-rw-r--r--   0        0        0       36 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/signer/__init__.py
+-rw-r--r--   0        0        0     1233 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/signer/base_signer.py
+-rw-r--r--   0        0        0     4622 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/signer/stark_curve_signer.py
+-rw-r--r--   0        0        0     1619 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/signer/test_stark_curve_signer.py
+-rw-r--r--   0        0        0      901 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/net/test_client_utils.py
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/proxy/__init__.py
+-rw-r--r--   0        0        0     5418 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/proxy/contract_abi_resolver.py
+-rw-r--r--   0        0        0     3469 2022-11-14 14:35:42.443673 starknet_py-0.9.0a0/starknet_py/proxy/proxy_check.py
+-rw-r--r--   0        0        0     1042 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/transaction_exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/transactions/__init__.py
+-rw-r--r--   0        0        0     1851 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/transactions/declare.py
+-rw-r--r--   0        0        0     2458 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/transactions/deploy.py
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/crypto/__init__.py
+-rw-r--r--   0        0        0     1311 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/crypto/facade.py
+-rw-r--r--   0        0        0       87 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/data_transformer/__init__.py
+-rw-r--r--   0        0        0    16310 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/data_transformer/data_transformer.py
+-rw-r--r--   0        0        0      342 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/data_transformer/errors.py
+-rw-r--r--   0        0        0     2311 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/data_transformer/execute_transformer.py
+-rw-r--r--   0        0        0      637 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/docs.py
+-rw-r--r--   0        0        0      301 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/iterable.py
+-rw-r--r--   0        0        0      152 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/sync/__init__.py
+-rw-r--r--   0        0        0     1355 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/sync/sync.py
+-rw-r--r--   0        0        0     4994 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/typed_data.py
+-rw-r--r--   0        0        0      489 2022-11-14 14:35:42.451674 starknet_py-0.9.0a0/starknet_py/utils/types.py
+-rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 starknet_py-0.9.0a0/setup.py
+-rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 starknet_py-0.9.0a0/PKG-INFO
```

### Comparing `starknet_py-0.8.0a0/LICENSE.txt` & `starknet_py-0.9.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/README.md` & `starknet_py-0.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/pyproject.toml` & `starknet_py-0.9.0a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starknet-py"
-version = "0.8.0-alpha"
+version = "0.9.0-alpha"
 description = "A python SDK for StarkNet"
 authors = ["Tomasz Rejowski <tomasz.rejowski@swmansion.com>", "Jakub Ptak <jakub.ptak@swmansion.com>"]
 include = ["starknet_py", "starknet_py/utils/crypto/libcrypto_c_exports.*"]
 exclude = ["starknet_py/tests/*", "starknet_py/**/*_test.py", "starknet_py/utils/compiler/mock-contracts/**"]
 packages = [
     { include = "starknet_py" }
 ]
@@ -12,16 +12,16 @@
 readme = "README.md"
 repository = "https://github.com/software-mansion/starknet.py"
 documentation = "https://starknetpy.rtfd.io/"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.10"
 asgiref = "^3.4.1"
-sphinx = { version = "^4.3.1", optional = true }
-enum-tools = { extras = ["sphinx"], version = "0.9.0", optional = true }
+sphinx = { version = ">=4.3.1,<6.0.0", optional = true }
+enum-tools = { extras = ["sphinx"], version = "0.9.0.post1", optional = true }
 crypto-cpp-py = "^1.0.4"
 marshmallow = "^3.15.0"
 marshmallow-oneofschema = "^3.0.1"
 cairo-lang = "0.10.1"
 typing-extensions = "^4.3.0"
 
 [tool.poetry.extras]
@@ -37,31 +37,33 @@
 sphinx-rtd-theme = "^1.0.0"
 pylint = "2.13.5"
 setuptools = "^65.3.0"
 pytest-mock = "^3.6.1"
 pytest-xdist = "^2.5.0"
 web3 = { extras = ["tester"], version = "6.0.0b4" }
 pyright = "^1.1.270"
-starknet-devnet = { git = "https://github.com/Shard-Labs/starknet-devnet.git", rev = "373cb165e36cad3edce7d38f9d7ccc9ea516687b" }
 pytest-cov = "^4.0.0"
+starknet-devnet = {git = "https://github.com/Shard-Labs/starknet-devnet.git", rev = "e353f2432a2eda173192482d2569ab6b99c1231d"}
 
 [tool.poe.tasks]
 test.shell = "pytest -n auto -v --cov=starknet_py starknet_py"
 test_ci.shell = "coverage run -m pytest starknet_py"
 test_unit.shell = "pytest -n auto -v starknet_py --ignore=starknet_py/tests/e2e"
 test_e2e.shell = "pytest -n auto -v starknet_py/tests/e2e --ignore=starknet_py/tests/e2e/docs"
 test_docs.shell = "pytest -n auto -v starknet_py/tests/e2e/docs"
 test_report.shell = "coverage report"
 test_html.shell = "coverage html && open ./htmlcov/index.html"
 docs_create = { shell = "make -C docs html" }
 docs_open = { shell = "open docs/_build/html/index.html" }
 lint = "pylint starknet_py"
 format = "black starknet_py"
 format_check = "black --check starknet_py"
+format_diff = "black --diff starknet_py"
 typecheck = "pyright starknet_py"
+compile_contracts = "bash starknet_py/tests/e2e/mock/compile_contracts.sh"
 requirements_check.shell = "poetry export -f requirements.txt --without-hashes --extras docs | cmp - requirements.txt"
 ci = ["lint", "format_check", "typecheck", "requirements_check", "test_ci"]
 
 [tool.coverage.run]
 source = ["starknet_py"]
```

### Comparing `starknet_py-0.8.0a0/starknet_py/cairo/felt.py` & `starknet_py-0.9.0a0/starknet_py/cairo/felt.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/common.py` & `starknet_py-0.9.0a0/starknet_py/common.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/compile/compiler.py` & `starknet_py-0.9.0a0/starknet_py/compile/compiler.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/constants.py` & `starknet_py-0.9.0a0/starknet_py/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from starkware.starknet.services.api.feeder_gateway.response_objects import (
     TransactionStatus,
 )
-from starkware.starknet.public.abi import get_storage_var_address
 
 TxStatus = TransactionStatus
 
 ACCEPTED_STATUSES = (TxStatus.ACCEPTED_ON_L1, TxStatus.ACCEPTED_ON_L2)
 
 # Address came from starkware-libs/starknet-addresses repository: https://github.com/starkware-libs/starknet-addresses
 FEE_CONTRACT_ADDRESS = (
     "0x049d36570d4e46f48e99674bd3fcc84644ddd6b96f7c741b1562b82f9e004dc7"
 )
 
 # Address came from starknet-devnet docs https://shard-labs.github.io/starknet-devnet/docs/guide/mint-token
 DEVNET_FEE_CONTRACT_ADDRESS = (
     "0x62230ea046a9a5fbc261ac77d03c8d41e5d442db2284587570ab46455fd2488"
 )
-
-OZ_PROXY_STORAGE_KEY = get_storage_var_address("Proxy_implementation_hash")
```

### Comparing `starknet_py-0.8.0a0/starknet_py/contract.py` & `starknet_py-0.9.0a0/starknet_py/contract.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,38 +8,41 @@
     Optional,
     TypeVar,
     Union,
     Dict,
     NamedTuple,
     Any,
 )
-from typing import TypedDict
 
 from starkware.cairo.lang.compiler.identifier_manager import IdentifierManager
 from starkware.starknet.core.os.class_hash import compute_class_hash
 from starkware.starknet.public.abi import get_selector_from_name
 from starkware.starknet.public.abi_structs import identifier_manager_from_abi
 from starkware.starknet.services.api.contract_class import ContractClass
 from starkware.starknet.services.api.feeder_gateway.feeder_gateway_client import (
     CastableToHash,
 )
 
 from starknet_py.common import create_compiled_contract
 from starknet_py.compile.compiler import StarknetCompilationSource
+from starknet_py.proxy.contract_abi_resolver import (
+    ProxyConfig,
+    ContractAbiResolver,
+    prepare_proxy_config,
+)
 from starknet_py.net import AccountClient
 from starknet_py.net.client import Client
 from starknet_py.net.client_models import Hash, Tag
 from starknet_py.net.gateway_client import GatewayClient
 from starknet_py.net.models import (
     InvokeFunction,
     AddressRepresentation,
     parse_address,
     compute_address,
 )
-from starknet_py.proxy_check import ProxyCheck, ArgentProxyCheck, OpenZeppelinProxyCheck
 from starknet_py.transactions.deploy import make_deploy_tx
 from starknet_py.utils.crypto.facade import pedersen_hash, Call
 from starknet_py.utils.data_transformer import FunctionCallSerializer
 from starknet_py.utils.sync import add_sync_methods
 
 ABI = list
 ABIEntry = dict
@@ -151,15 +154,15 @@
     ) -> List[int]:
         """
         Calls a method without translating the result into python values.
 
         :param block_hash: Optional block hash
         :return: list of ints
         """
-        return await self._client.call_contract(invoke_tx=self, block_hash=block_hash)
+        return await self._client.call_contract(call=self, block_hash=block_hash)
 
     async def call(
         self,
         block_hash: Optional[str] = None,
     ) -> NamedTuple:
         """
         Calls a method.
@@ -368,78 +371,54 @@
         """
         return self._functions
 
     @property
     def address(self) -> int:
         return self.data.address
 
-    class ProxyConfig(TypedDict, total=False):
-        """
-        Proxy resolving configuration
-        """
-
-        max_steps: int
-        """
-        Max number of contracts that `Contract.from_address` will process before raising `RecursionError`.
-        """
-        proxy_checks: List[ProxyCheck]
-        """
-        List of classes implementing :class:`starknet_py.proxy_check.ProxyCheck` ABC,
-        that will be used for checking if contract at the address is a proxy contract.
-        """
-
     @staticmethod
     async def from_address(
         address: AddressRepresentation,
         client: Client,
         proxy_config: Union[bool, ProxyConfig] = False,
     ) -> "Contract":
         """
         Fetches ABI for given contract and creates a new Contract instance with it. If you know ABI statically you
         should create Contract's instances directly instead of using this function to avoid unnecessary API calls.
 
         :raises ContractNotFoundError: when contract is not found
-        :raises TypeError: when Client not supporting `get_code` methods is used
+        :raises TypeError: when given client's `get_class_by_hash` method does not return abi
+        :raises ProxyResolutionError: when given ProxyChecks were not sufficient to resolve proxy's implementation
         :param address: Contract's address
         :param client: Client
         :param proxy_config: Proxy resolving config
-            If set to ``True``, will use default proxy checks and :class:
-            `starknet_py.proxy_check.OpenZeppelinProxyCheck`
-            and :class:`starknet_py.proxy_check.ArgentProxyCheck` and default max_steps = 5.
+            If set to ``True``, will use default proxy checks
+            :class:`starknet_py.proxy.proxy_check.OpenZeppelinProxyCheck`
+            and :class:`starknet_py.proxy.proxy_check.ArgentProxyCheck`.
 
             If set to ``False``, :meth:`Contract.from_address` will not resolve proxies.
 
-            If a valid `ProxyConfig` is provided, will use values from that instead supplementing
-            with defaults when needed.
+            If a valid :class:`starknet_py.contract_abi_resolver.ProxyConfig` is provided, will use its values instead.
 
         :return: an initialized Contract instance
         """
-        default_config: Contract.ProxyConfig = {
-            "max_steps": 5,
-            "proxy_checks": [ArgentProxyCheck(), OpenZeppelinProxyCheck()],
-        }
-        if isinstance(proxy_config, bool):
-            proxy_config = default_config if proxy_config else {}
-        else:
-            proxy_config = {**default_config, **proxy_config}
+        address = parse_address(address)
+        proxy_config = Contract._create_proxy_config(proxy_config)
 
-        proxy_client = client.client if isinstance(client, AccountClient) else client
-        if not isinstance(proxy_client, GatewayClient):
+        if not Contract._is_abi_compatible_client(client):
+            # TODO: Add support for FullNodeClient once abi is available in RPC
             raise TypeError(
                 "Contract.from_address only supports GatewayClient or AccountClients using GatewayClient"
             )
 
-        contract = await ContractFromAddressFactory(
-            address=address,
-            client=proxy_client,
-            max_steps=proxy_config.get("max_steps", 1),
-            proxy_checks=proxy_config.get("proxy_checks", []),
-        ).make_contract()
+        abi = await ContractAbiResolver(
+            address=address, client=client, proxy_config=proxy_config
+        ).resolve()
 
-        return Contract(address=address, abi=contract.data.abi, client=client)
+        return Contract(address=address, abi=abi, client=client)
 
     @staticmethod
     async def deploy(
         client: Client,
         compilation_source: Optional[StarknetCompilationSource] = None,
         compiled_contract: Optional[str] = None,
         constructor_args: Optional[Union[List, Dict]] = None,
@@ -599,55 +578,18 @@
                 abi=abi_entry,
                 contract_data=contract_data,
                 client=client,
             )
 
         return repository
 
+    @staticmethod
+    def _create_proxy_config(proxy_config) -> ProxyConfig:
+        if proxy_config is False:
+            return ProxyConfig()
+        proxy_arg = ProxyConfig() if proxy_config is True else proxy_config
+        return prepare_proxy_config(proxy_arg)
 
-class ContractFromAddressFactory:
-    def __init__(
-        self,
-        address: AddressRepresentation,
-        client: GatewayClient,
-        max_steps: int,
-        proxy_checks: List[ProxyCheck],
-    ):
-        self._address = address
-        self._client = client
-        self._max_steps = max_steps
-        self._proxy_checks = proxy_checks
-        self._processed_addresses = set()
-
-    async def make_contract(self) -> Contract:
-        return await self._make_contract_recursively(step=1, address=self._address)
-
-    async def _make_contract_recursively(
-        self, step: int, address: AddressRepresentation
-    ) -> Contract:
-        if address in self._processed_addresses:
-            raise RecursionError("Proxy cycle detected while resolving proxies")
-
-        if step > self._max_steps:
-            raise RecursionError("Max number of steps exceeded while resolving proxies")
-
-        code = await self._client.get_code(contract_address=parse_address(address))
-        contract = Contract(
-            address=parse_address(address), abi=code.abi, client=self._client
-        )
-        self._processed_addresses.add(address)
-
-        is_proxy = False
-        address = 0
-        for proxy_check in self._proxy_checks:
-            if await proxy_check.is_proxy(contract):
-                is_proxy = True
-                address = await proxy_check.implementation_address(contract)
-                break
-
-        if not is_proxy:
-            return contract
-
-        return await self._make_contract_recursively(
-            address=address,
-            step=step + 1,
-        )
+    @staticmethod
+    def _is_abi_compatible_client(client) -> bool:
+        actual_client = client.client if isinstance(client, AccountClient) else client
+        return isinstance(actual_client, GatewayClient)
```

### Comparing `starknet_py-0.8.0a0/starknet_py/net/account/account_client.py` & `starknet_py-0.9.0a0/starknet_py/net/account/account_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Calls,
     TransactionStatus,
     DeployTransactionResponse,
     DeclareTransactionResponse,
     Transaction,
     DeployAccountTransactionResponse,
 )
+from starknet_py.net.client_utils import _invoke_tx_to_call
 from starknet_py.net.gateway_client import GatewayClient
 from starknet_py.net.models import (
     InvokeFunction,
     StarknetChainId,
     chain_from_network,
 )
 from starknet_py.net.models.address import AddressRepresentation, parse_address
@@ -168,20 +169,24 @@
             tx_hash=tx_hash,
             wait_for_accept=wait_for_accept,
             check_interval=check_interval,
         )
 
     async def call_contract(
         self,
-        invoke_tx: Union[InvokeFunction, Call],
+        call: Call = None,  # pyright: ignore
         block_hash: Optional[Union[Hash, Tag]] = None,
         block_number: Optional[Union[int, Tag]] = None,
+        *,
+        invoke_tx: Call = None,  # pyright: ignore
     ) -> List[int]:
+        call = _invoke_tx_to_call(call=call, invoke_tx=invoke_tx)
+
         return await self.client.call_contract(
-            invoke_tx=invoke_tx, block_hash=block_hash, block_number=block_number
+            call=call, block_hash=block_hash, block_number=block_number
         )
 
     async def get_class_hash_at(
         self,
         contract_address: Hash,
         block_hash: Optional[Union[Hash, Tag]] = None,
         block_number: Optional[Union[int, Tag]] = None,
@@ -193,27 +198,23 @@
         )
 
     async def get_class_by_hash(self, class_hash: Hash) -> DeclaredContract:
         return await self.client.get_class_by_hash(class_hash=class_hash)
 
     async def _get_nonce(self) -> int:
         if self.supported_tx_version == 1:
-            return await self.get_contract_nonce(self.address)
+            return await self.get_contract_nonce(self.address, block_hash="latest")
 
         [nonce] = await self.call_contract(
-            InvokeFunction(
-                contract_address=self.address,
-                entry_point_selector=get_selector_from_name("get_nonce"),
+            Call(
+                to_addr=self.address,
+                selector=get_selector_from_name("get_nonce"),
                 calldata=[],
-                signature=[],
-                max_fee=0,
-                version=self.supported_tx_version,
-                nonce=None,
             ),
-            block_hash="latest",
+            block_hash="pending",
         )
         return nonce
 
     def _get_default_token_address(self) -> str:
         if self.net not in [TESTNET, MAINNET]:
             raise ValueError(
                 "Token_address must be specified when using a custom net address"
@@ -236,15 +237,15 @@
 
         low, high = await self.call_contract(
             Call(
                 to_addr=parse_address(token_address),
                 selector=get_selector_from_name("balanceOf"),
                 calldata=[self.address],
             ),
-            block_hash="latest",
+            block_hash="pending",
         )
 
         return (high << 128) + low
 
     async def prepare_invoke_function(
         self,
         calls: Calls,
@@ -331,41 +332,14 @@
             max_fee = int(estimate_fee.overall_fee * 1.1)
 
         if max_fee is None:
             raise ValueError("Max_fee must be specified when invoking a transaction")
 
         return max_fee
 
-    async def sign_transaction(
-        self,
-        calls: Calls,
-        max_fee: Optional[int] = None,
-        auto_estimate: bool = False,
-        version: Optional[int] = None,
-    ) -> InvokeFunction:
-        """
-        Takes calls and creates signed InvokeFunction
-
-        :param calls: Single call or list of calls
-        :param max_fee: Max amount of Wei to be paid when executing transaction
-        :param auto_estimate: Use automatic fee estimation, not recommend as it may lead to high costs
-        :param version: Transaction version
-        :return: InvokeFunction created from the calls
-
-        .. deprecated:: 0.5.0
-            sign_transaction has been deprecated. Use :meth:`AccountClient.sign_invoke_transaction` instead.
-        """
-        warnings.warn(
-            "sign_transaction has been deprecated. Use AccountClient.sign_invoke_transaction instead.",
-            category=DeprecationWarning,
-        )
-        return await self.sign_invoke_transaction(
-            calls, max_fee, auto_estimate, version
-        )
-
     async def sign_invoke_transaction(
         self,
         calls: Calls,
         max_fee: Optional[int] = None,
         auto_estimate: bool = False,
         version: Optional[int] = None,
     ) -> InvokeFunction:
@@ -676,15 +650,15 @@
 
         call = Call(
             to_addr=self.address,
             selector=get_selector_from_name("is_valid_signature"),
             calldata=calldata,
         )
         try:
-            await self.call_contract(invoke_tx=call, block_hash="latest")
+            await self.call_contract(call=call, block_hash="pending")
             return True
         except ClientError as ex:
             if re.search(r"Signature\s.+,\sis\sinvalid", ex.message):
                 return False
             raise ex
```

### Comparing `starknet_py-0.8.0a0/starknet_py/net/account/compiled_account_contract.py` & `starknet_py-0.9.0a0/starknet_py/net/account/compiled_account_contract.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/client.py` & `starknet_py-0.9.0a0/starknet_py/net/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,17 +155,14 @@
                     TransactionStatus.ACCEPTED_ON_L1,
                     TransactionStatus.ACCEPTED_ON_L2,
                 ):
                     assert result.block_number is not None
                     return result.block_number, status
                 if status == TransactionStatus.PENDING:
                     if not wait_for_accept:
-                        # FIXME rpc receipt doesn't have block_number currently, fix this in future spec version
-                        if self.__class__.__name__ == "FullNodeClient":
-                            return -1, status
                         if result.block_number is not None:
                             return result.block_number, status
                 elif status == TransactionStatus.REJECTED:
                     raise TransactionRejectedError(
                         message=result.rejection_reason,
                     )
                 elif status == TransactionStatus.NOT_RECEIVED:
@@ -199,24 +196,24 @@
                              the block indicated by the literals `"pending"` or `"latest"`
         :return: Estimated amount of Wei executing specified transaction will cost
         """
 
     @abstractmethod
     async def call_contract(
         self,
-        invoke_tx: Union[InvokeFunction, Call],
+        call: Call,
         block_hash: Optional[Union[Hash, Tag]] = None,
         block_number: Optional[Union[int, Tag]] = None,
     ) -> List[int]:
         """
         Call the contract with given instance of InvokeTransaction
 
         Warning, InvokeFunction as call_contract parameter has been deprecated in favor of Call.
 
-        :param invoke_tx: Call or InvokeFunction (deprecated)
+        :param call: Call
         :param block_hash: Block's hash or literals `"pending"` or `"latest"`
         :param block_number: Block's number or literals `"pending"` or `"latest"`
         :return: List of integers representing contract's function output (structured like calldata)
 
         .. versionchanged:: 5.0.0
             Added `Call` as possible invoke_tx type.
             Deprecated InvokeFunction as possible invoke_tx type.
```

### Comparing `starknet_py-0.8.0a0/starknet_py/net/client_errors.py` & `starknet_py-0.9.0a0/starknet_py/net/client_errors.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/client_models.py` & `starknet_py-0.9.0a0/starknet_py/net/client_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 Deploy = as_our_module(D)
 Declare = as_our_module(DCL)
 
 
 Hash = Union[int, str]
 Tag = Literal["pending", "latest"]
 
+Abi = List[Dict[str, Any]]
+
 
 @dataclass
 class Call:
     to_addr: int
     selector: int
     calldata: List[int]
 
@@ -310,15 +312,15 @@
     declared_contracts: List[int]
 
 
 @dataclass
 class StateDiff:
     deployed_contracts: List[DeployedContract]
     storage_diffs: List[StorageDiff]
-    declared_contracts: List[int]
+    declared_contract_hashes: List[int]
 
 
 @dataclass
 class ContractCode:
     """
     Dataclass representing contract deployed to starknet
     """
@@ -352,13 +354,14 @@
 class DeclaredContract:
     """
     Dataclass representing contract declared to starknet
     """
 
     program: dict
     entry_points_by_type: EntryPointsByType
+    abi: Optional[Abi] = None
 
 
 @dataclass
 class TransactionStatusResponse:
     block_hash: Optional[int]
     transaction_status: TransactionStatus
```

### Comparing `starknet_py-0.8.0a0/starknet_py/net/full_node_client.py` & `starknet_py-0.9.0a0/starknet_py/net/full_node_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import List, Optional, Union, cast
+from typing import List, Optional, Union, cast, Dict
 
 import aiohttp
 from marshmallow import EXCLUDE
 
 from starknet_py.net.client import (
     Client,
 )
@@ -25,28 +25,29 @@
     DeclareTransactionResponse,
     DeployTransactionResponse,
     Call,
     DeployAccountTransactionResponse,
 )
 from starknet_py.net.http_client import RpcHttpClient
 from starknet_py.net.models.transaction import DeployAccount
+from starknet_py.net.models import TransactionType
 from starknet_py.net.networks import Network
 from starknet_py.net.schemas.rpc import (
     StarknetBlockSchema,
     BlockStateUpdateSchema,
     DeclaredContractSchema,
     TransactionReceiptSchema,
     TypesOfTransactionsSchema,
     SentTransactionSchema,
     DeclareTransactionResponseSchema,
     DeployTransactionResponseSchema,
     PendingTransactionsSchema,
     EstimatedFeeSchema,
 )
-from starknet_py.net.client_utils import convert_to_felt
+from starknet_py.net.client_utils import convert_to_felt, _invoke_tx_to_call
 from starknet_py.transaction_exceptions import TransactionNotReceivedError
 from starknet_py.utils.sync import add_sync_methods
 
 
 @add_sync_methods
 class FullNodeClient(Client):
     def __init__(
@@ -156,92 +157,67 @@
 
     async def estimate_fee(
         self,
         tx: Union[InvokeFunction, Declare, DeployAccount],
         block_hash: Optional[Union[Hash, Tag]] = None,
         block_number: Optional[Union[int, Tag]] = None,
     ) -> EstimatedFee:
-        if isinstance(tx, Declare):
-            raise ValueError(
-                "Estimating fee for Declare transactions is currently not supported in FullNodeClient"
-            )
-
         if isinstance(tx, DeployAccount):
             raise ValueError(
                 "Estimating fee for DeployAccount transactions is currently not supported in FullNodeClient"
             )
 
         block_identifier = get_block_identifier(
             block_hash=block_hash, block_number=block_number
         )
 
         res = await self._client.call(
             method_name="estimateFee",
             params={
-                # There is no transaction_hash field in "request" since it was an error
-                # in RPC v0.1.0 specification. It has been removed in the latest specification.
-                "request": {
-                    "max_fee": convert_to_felt(tx.max_fee),
-                    "version": hex(tx.version),
-                    "signature": [convert_to_felt(i) for i in tx.signature],
-                    "nonce": (
-                        convert_to_felt(tx.nonce) if tx.nonce is not None else None
-                    ),  # TODO: verify this is correct
-                    "type": "INVOKE",
-                    "contract_address": convert_to_felt(tx.contract_address),
-                    "entry_point_selector": convert_to_felt(tx.entry_point_selector),
-                    "calldata": [convert_to_felt(i) for i in tx.calldata],
-                },
+                "request": _create_broadcasted_txn(transaction=tx),
                 **block_identifier,
             },
         )
 
         return cast(EstimatedFee, EstimatedFeeSchema().load(res, unknown=EXCLUDE))
 
     async def call_contract(
         self,
-        invoke_tx: Union[InvokeFunction, Call],
+        call: Call = None,  # pyright: ignore
         block_hash: Optional[Union[Hash, Tag]] = None,
         block_number: Optional[Union[int, Tag]] = None,
+        *,
+        invoke_tx: Call = None,  # pyright: ignore
     ) -> List[int]:
-        if isinstance(invoke_tx, InvokeFunction):
-            warnings.warn(
-                "InvokeFunctions has been deprecated as a call_contract parameter, use Call instead.",
-                category=DeprecationWarning,
-            )
+        call = _invoke_tx_to_call(call=call, invoke_tx=invoke_tx)
 
         block_identifier = get_block_identifier(
             block_hash=block_hash, block_number=block_number
         )
         res = await self._client.call(
             method_name="call",
             params={
-                "request": _get_call_payload(invoke_tx),
+                "request": {
+                    "contract_address": convert_to_felt(call.to_addr),
+                    "entry_point_selector": convert_to_felt(call.selector),
+                    "calldata": [convert_to_felt(i1) for i1 in call.calldata],
+                },
                 **block_identifier,
             },
         )
         return [int(i, 16) for i in res]
 
     async def send_transaction(
         self, transaction: InvokeFunction
     ) -> SentTransactionResponse:
+        params = _create_broadcasted_txn(transaction=transaction)
+
         res = await self._client.call(
             method_name="addInvokeTransaction",
-            params={
-                "function_invocation": {
-                    "contract_address": convert_to_felt(transaction.contract_address),
-                    "entry_point_selector": convert_to_felt(
-                        transaction.entry_point_selector
-                    ),
-                    "calldata": [convert_to_felt(i) for i in transaction.calldata],
-                },
-                "signature": [convert_to_felt(i) for i in transaction.signature],
-                "max_fee": hex(transaction.max_fee),
-                "version": hex(transaction.version),
-            },
+            params={"invoke_transaction": {**params}},
         )
 
         return cast(
             SentTransactionResponse, SentTransactionSchema().load(res, unknown=EXCLUDE)
         )
 
     async def deploy(self, transaction: Deploy) -> DeployTransactionResponse:
@@ -252,23 +228,30 @@
         )
 
         contract_definition = transaction.dump()["contract_definition"]
 
         res = await self._client.call(
             method_name="addDeployTransaction",
             params={
-                "contract_address_salt": convert_to_felt(
-                    transaction.contract_address_salt
-                ),
-                "constructor_calldata": [
-                    convert_to_felt(i) for i in transaction.constructor_calldata
-                ],
-                "contract_definition": {
-                    "program": contract_definition["program"],
-                    "entry_points_by_type": contract_definition["entry_points_by_type"],
+                "deploy_transaction": {
+                    "contract_class": {
+                        "program": contract_definition["program"],
+                        "entry_points_by_type": contract_definition[
+                            "entry_points_by_type"
+                        ],
+                        "abi": contract_definition["abi"],
+                    },
+                    "version": hex(transaction.version),
+                    "type": "DEPLOY",
+                    "contract_address_salt": convert_to_felt(
+                        transaction.contract_address_salt
+                    ),
+                    "constructor_calldata": [
+                        convert_to_felt(i) for i in transaction.constructor_calldata
+                    ],
                 },
             },
         )
 
         return cast(
             DeployTransactionResponse,
             DeployTransactionResponseSchema().load(res, unknown=EXCLUDE),
@@ -276,25 +259,19 @@
 
     async def deploy_account(
         self, transaction: DeployAccount
     ) -> DeployAccountTransactionResponse:
         raise NotImplementedError()
 
     async def declare(self, transaction: Declare) -> DeclareTransactionResponse:
-        contract_class = transaction.dump()["contract_class"]
+        params = _create_broadcasted_txn(transaction=transaction)
 
         res = await self._client.call(
             method_name="addDeclareTransaction",
-            params={
-                "contract_class": {
-                    "program": contract_class["program"],
-                    "entry_points_by_type": contract_class["entry_points_by_type"],
-                },
-                "version": hex(transaction.version),
-            },
+            params={"declare_transaction": {**params}},
         )
 
         return cast(
             DeclareTransactionResponse,
             DeclareTransactionResponseSchema().load(res, unknown=EXCLUDE),
         )
 
@@ -313,17 +290,27 @@
                 "contract_address": convert_to_felt(contract_address),
                 **block_identifier,
             },
         )
         res = cast(str, res)
         return int(res, 16)
 
-    async def get_class_by_hash(self, class_hash: Hash) -> DeclaredContract:
+    async def get_class_by_hash(
+        self,
+        class_hash: Hash,
+        block_hash: Optional[Union[Hash, Tag]] = None,
+        block_number: Optional[Union[int, Tag]] = None,
+    ) -> DeclaredContract:
+        block_identifier = get_block_identifier(
+            block_hash=block_hash, block_number=block_number
+        )
+
         res = await self._client.call(
-            method_name="getClass", params={"class_hash": convert_to_felt(class_hash)}
+            method_name="getClass",
+            params={"class_hash": convert_to_felt(class_hash), **block_identifier},
         )
         return cast(
             DeclaredContract, DeclaredContractSchema().load(res, unknown=EXCLUDE)
         )
 
     # Only RPC methods
 
@@ -455,20 +442,56 @@
 
     if block_number is not None:
         return {"block_id": {"block_number": block_number}}
 
     return {"block_id": "pending"}
 
 
-def _get_call_payload(tx: Union[InvokeFunction, Call]) -> dict:
-    if isinstance(tx, InvokeFunction):
-        invoke = cast(InvokeFunction, tx)
+def _create_broadcasted_txn(transaction: Union[InvokeFunction, Declare]) -> Dict:
+    common_params = {
+        "max_fee": hex(transaction.max_fee),
+        "version": hex(transaction.version),
+        "signature": [convert_to_felt(i) for i in transaction.signature],
+        "nonce": convert_to_felt(transaction.nonce)
+        if transaction.nonce is not None
+        else transaction.nonce,
+    }
+
+    if transaction.tx_type == TransactionType.INVOKE_FUNCTION:
+        invoke_specific_params = {
+            "type": "INVOKE",
+            "calldata": [convert_to_felt(i) for i in transaction.calldata],
+        }
+        if transaction.version == 0:
+            params_depending_on_version = {
+                "contract_address": convert_to_felt(transaction.contract_address),
+                "entry_point_selector": convert_to_felt(
+                    transaction.entry_point_selector
+                ),
+            }
+        else:
+            params_depending_on_version = {
+                "sender_address": convert_to_felt(transaction.contract_address),
+            }
+
         return {
-            "contract_address": convert_to_felt(invoke.contract_address),
-            "entry_point_selector": convert_to_felt(invoke.entry_point_selector),
-            "calldata": [convert_to_felt(i) for i in invoke.calldata],
+            **common_params,
+            **params_depending_on_version,
+            **invoke_specific_params,
         }
-    return {
-        "contract_address": convert_to_felt(tx.to_addr),
-        "entry_point_selector": convert_to_felt(tx.selector),
-        "calldata": [convert_to_felt(i) for i in tx.calldata],
-    }
+
+    if transaction.tx_type == TransactionType.DECLARE:
+        contract_class = transaction.dump()["contract_class"]
+
+        declare_params = {
+            "contract_class": {
+                "program": contract_class["program"],
+                "entry_points_by_type": contract_class["entry_points_by_type"],
+                "abi": contract_class["abi"],
+            },
+            "sender_address": convert_to_felt(transaction.sender_address),
+            "type": "DECLARE",
+        }
+
+        return {**common_params, **declare_params}
+
+    raise TypeError("Transaction should be of type InvokeFunction or Declare")
```

### Comparing `starknet_py-0.8.0a0/starknet_py/net/gateway_client.py` & `starknet_py-0.9.0a0/starknet_py/net/gateway_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,19 @@
     DeclareTransactionResponseSchema,
     TransactionReceiptSchema,
     DeployAccountTransactionResponseSchema,
 )
 from starknet_py.net.http_client import GatewayHttpClient
 from starknet_py.net.networks import Network, net_address_from_net
 from starknet_py.net.client_errors import ContractNotFoundError
-from starknet_py.net.client_utils import convert_to_felt, is_block_identifier
+from starknet_py.net.client_utils import (
+    convert_to_felt,
+    is_block_identifier,
+    _invoke_tx_to_call,
+)
 from starknet_py.transaction_exceptions import TransactionNotReceivedError
 from starknet_py.utils.sync import add_sync_methods
 
 
 @add_sync_methods
 class GatewayClient(Client):
     def __init__(
@@ -206,32 +210,34 @@
             params=block_identifier,
         )
 
         return EstimatedFeeSchema().load(res, unknown=EXCLUDE)  # pyright: ignore
 
     async def call_contract(
         self,
-        invoke_tx: Union[InvokeFunction, Call],
+        call: Call = None,  # pyright: ignore
         block_hash: Optional[Union[Hash, Tag]] = None,
         block_number: Optional[Union[int, Tag]] = None,
+        *,
+        invoke_tx: Call = None,  # pyright: ignore
     ) -> List[int]:
-        if isinstance(invoke_tx, InvokeFunction):
-            warnings.warn(
-                "InvokeFunctions has been deprecated as a call_contract parameter, use Call instead.",
-                category=DeprecationWarning,
-            )
+        call = _invoke_tx_to_call(call=call, invoke_tx=invoke_tx)
 
         block_identifier = get_block_identifier(
             block_hash=block_hash, block_number=block_number
         )
 
         res = await self._feeder_gateway_client.post(
             method_name="call_contract",
             params=block_identifier,
-            payload=_get_call_payload(invoke_tx),
+            payload={
+                "contract_address": hex(call.to_addr),
+                "entry_point_selector": hex(call.selector),
+                "calldata": [str(i) for i in call.calldata],
+            },
         )
 
         return [int(v, 16) for v in res["result"]]
 
     async def send_transaction(
         self,
         transaction: InvokeFunction,
@@ -404,21 +410,7 @@
             return {"blockNumber": block_hash}
         return {"blockHash": convert_to_felt(block_hash)}
 
     if block_number is not None:
         return {"blockNumber": block_number}
 
     return {"blockNumber": "pending"}
-
-
-def _get_call_payload(tx: Union[InvokeFunction, Call]) -> dict:
-    if isinstance(tx, Call):
-        return {
-            "contract_address": hex(tx.to_addr),
-            "entry_point_selector": hex(tx.selector),
-            "calldata": [str(i) for i in tx.calldata],
-        }
-    return {
-        "contract_address": hex(tx.contract_address),
-        "entry_point_selector": hex(tx.entry_point_selector),
-        "calldata": [str(i) for i in tx.calldata],
-    }
```

### Comparing `starknet_py-0.8.0a0/starknet_py/net/http_client.py` & `starknet_py-0.9.0a0/starknet_py/net/http_client.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/l1/contracts.py` & `starknet_py-0.9.0a0/starknet_py/net/l1/contracts.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/l1/messages.py` & `starknet_py-0.9.0a0/starknet_py/net/l1/messages.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/l1/starknet_l1_abi.py` & `starknet_py-0.9.0a0/starknet_py/net/l1/starknet_l1_abi.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/models/address.py` & `starknet_py-0.9.0a0/starknet_py/net/models/address.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/models/chains.py` & `starknet_py-0.9.0a0/starknet_py/net/models/chains.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/models/transaction.py` & `starknet_py-0.9.0a0/starknet_py/net/models/transaction.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/models/typed_data.py` & `starknet_py-0.9.0a0/starknet_py/net/models/typed_data.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/schemas/common.py` & `starknet_py-0.9.0a0/starknet_py/net/schemas/common.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/schemas/gateway.py` & `starknet_py-0.9.0a0/starknet_py/net/schemas/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,14 +373,15 @@
         values=fields.Raw(allow_none=True),
         data_key="program",
         required=True,
     )
     entry_points_by_type = fields.Nested(
         EntryPointsByTypeSchema(), data_key="entry_points_by_type", required=True
     )
+    abi = fields.List(fields.Dict(), data_key="abi")
 
     @post_load
     def make_dataclass(self, data, **kwargs) -> DeclaredContract:
         return DeclaredContract(**data)
 
 
 class TransactionStatusSchema(Schema):
```

### Comparing `starknet_py-0.8.0a0/starknet_py/net/schemas/rpc.py` & `starknet_py-0.9.0a0/starknet_py/net/schemas/rpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     DeployTransaction,
     TransactionReceipt,
     SentTransactionResponse,
     DeclareTransactionResponse,
     DeployTransactionResponse,
     EstimatedFee,
     StateDiff,
+    L1HandlerTransaction,
 )
 from starknet_py.net.schemas.common import (
     Felt,
     BlockStatusField,
     StatusField,
     NonPrefixedHex,
 )
@@ -107,25 +108,27 @@
     hash = Felt(data_key="transaction_hash", required=True)
     signature = fields.List(Felt(), data_key="signature", load_default=[])
     max_fee = Felt(data_key="max_fee", load_default=0)
     version = Felt(data_key="version", required=True)
 
 
 class InvokeTransactionSchema(TransactionSchema):
-    contract_address = Felt(data_key="contract_address", required=True)
-    entry_point_selector = Felt(data_key="entry_point_selector", required=True)
+    contract_address = Felt(data_key="contract_address", load_default=None)
+    sender_address = Felt(data_key="sender_address", load_default=None)
+    entry_point_selector = Felt(data_key="entry_point_selector", load_default=None)
     calldata = fields.List(Felt(), data_key="calldata", required=True)
     nonce = Felt(data_key="nonce", load_default=None)
 
-    @pre_load
-    def preprocess(self, data, **kwargs):
-        return data
-
     @post_load
     def make_transaction(self, data, **kwargs) -> InvokeTransaction:
+        data["contract_address"] = data.get("contract_address") or data.get(
+            "sender_address"
+        )
+        del data["sender_address"]
+
         return InvokeTransaction(**data)
 
 
 class DeclareTransactionSchema(TransactionSchema):
     class_hash = Felt(data_key="class_hash", required=True)
     sender_address = Felt(data_key="sender_address", required=True)
     nonce = Felt(data_key="nonce", load_default=None)
@@ -143,22 +146,34 @@
     class_hash = Felt(data_key="class_hash", required=True)
 
     @post_load
     def make_dataclass(self, data, **kwargs) -> DeployTransaction:
         return DeployTransaction(**data)
 
 
+class L1HandlerTransactionSchema(TransactionSchema):
+    contract_address = Felt(data_key="contract_address", required=True)
+    calldata = fields.List(Felt(), data_key="calldata", required=True)
+    entry_point_selector = Felt(data_key="entry_point_selector", required=True)
+    nonce = Felt(data_key="nonce", required=True)
+
+    @post_load
+    def make_dataclass(self, data, **kwargs) -> L1HandlerTransaction:
+        return L1HandlerTransaction(**data)
+
+
 class TypesOfTransactionsSchema(OneOfSchema):
     type_field = "type"
     type_schemas = {
         "INVOKE": InvokeTransactionSchema,
         "DECLARE": DeclareTransactionSchema,
         "DEPLOY": DeployTransactionSchema,
         # FIXME add proper handling/serialization
         "DEPLOY_ACCOUNT": None,
+        "L1_HANDLER": L1HandlerTransactionSchema,
     }
 
 
 class StarknetBlockSchema(Schema):
     block_hash = Felt(data_key="block_hash", required=True)
     parent_block_hash = Felt(data_key="parent_hash", required=True)
     block_number = fields.Integer(data_key="block_number", required=True)
@@ -200,31 +215,23 @@
     class_hash = NonPrefixedHex(data_key="class_hash", required=True)
 
     @post_load
     def make_dataclass(self, data, **kwargs):
         return DeployedContract(**data)
 
 
-class DeclaredContractClassHashSchema(Schema):
-    class_hash = Felt(data_key="class_hash", required=True)
-
-    @post_load
-    def return_class_hash(self, data, **kwargs):
-        return data["class_hash"]
-
-
 class StateDiffSchema(Schema):
     deployed_contracts = fields.List(
         fields.Nested(DeployedContractSchema()),
         data_key="deployed_contracts",
         required=True,
     )
-    declared_contracts = fields.List(
-        fields.Nested(DeclaredContractClassHashSchema()),
-        data_key="declared_contracts",
+    declared_contract_hashes = fields.List(
+        Felt(),
+        data_key="declared_contract_hashes",
         required=True,
     )
     storage_diffs = fields.List(
         fields.Nested(StorageDiffSchema()),
         data_key="storage_diffs",
         required=True,
     )
@@ -244,15 +251,15 @@
     def preprocess(self, data, **kwargs):
         # Remove this when support for nonces is added
         del data["state_diff"]["nonces"]
         return data
 
     @post_load
     def make_dataclass(self, data, **kwargs) -> BlockStateUpdate:
-        declared_contracts = data["state_diff"].declared_contracts
+        declared_contracts = data["state_diff"].declared_contract_hashes
         deployed_contracts = data["state_diff"].deployed_contracts
         storage_diffs = data["state_diff"].storage_diffs
         del data["state_diff"]
 
         return BlockStateUpdate(
             **data,
             declared_contracts=declared_contracts,
```

### Comparing `starknet_py-0.8.0a0/starknet_py/net/signer/base_signer.py` & `starknet_py-0.9.0a0/starknet_py/net/signer/base_signer.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/signer/stark_curve_signer.py` & `starknet_py-0.9.0a0/starknet_py/net/signer/stark_curve_signer.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/net/signer/test_stark_curve_signer.py` & `starknet_py-0.9.0a0/starknet_py/net/signer/test_stark_curve_signer.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/transaction_exceptions.py` & `starknet_py-0.9.0a0/starknet_py/transaction_exceptions.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/transactions/declare.py` & `starknet_py-0.9.0a0/starknet_py/transactions/declare.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/transactions/deploy.py` & `starknet_py-0.9.0a0/starknet_py/transactions/deploy.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/utils/crypto/facade.py` & `starknet_py-0.9.0a0/starknet_py/utils/crypto/facade.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/utils/data_transformer/data_transformer.py` & `starknet_py-0.9.0a0/starknet_py/utils/data_transformer/data_transformer.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/utils/data_transformer/execute_transformer.py` & `starknet_py-0.9.0a0/starknet_py/utils/data_transformer/execute_transformer.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/utils/docs.py` & `starknet_py-0.9.0a0/starknet_py/utils/docs.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/utils/sync/sync.py` & `starknet_py-0.9.0a0/starknet_py/utils/sync/sync.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/starknet_py/utils/typed_data.py` & `starknet_py-0.9.0a0/starknet_py/utils/typed_data.py`

 * *Files identical despite different names*

### Comparing `starknet_py-0.8.0a0/setup.py` & `starknet_py-0.9.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
  'starknet_py.compile',
  'starknet_py.net',
  'starknet_py.net.account',
  'starknet_py.net.l1',
  'starknet_py.net.models',
  'starknet_py.net.schemas',
  'starknet_py.net.signer',
+ 'starknet_py.proxy',
  'starknet_py.transactions',
  'starknet_py.utils',
  'starknet_py.utils.crypto',
  'starknet_py.utils.data_transformer',
  'starknet_py.utils.sync']
 
 package_data = \
@@ -25,19 +26,19 @@
  'cairo-lang==0.10.1',
  'crypto-cpp-py>=1.0.4,<2.0.0',
  'marshmallow-oneofschema>=3.0.1,<4.0.0',
  'marshmallow>=3.15.0,<4.0.0',
  'typing-extensions>=4.3.0,<5.0.0']
 
 extras_require = \
-{'docs': ['sphinx>=4.3.1,<5.0.0', 'enum-tools[sphinx]==0.9.0']}
+{'docs': ['sphinx>=4.3.1,<6.0.0', 'enum-tools[sphinx]==0.9.0.post1']}
 
 setup_kwargs = {
     'name': 'starknet-py',
-    'version': '0.8.0a0',
+    'version': '0.9.0a0',
     'description': 'A python SDK for StarkNet',
     'long_description': '<div align="center">\n    <img src="https://raw.githubusercontent.com/software-mansion/starknet.py/master/graphic.png" alt="starknet.py"/>\n</div>\n<h2 align="center">StarkNet SDK for Python</h2>\n\n<div align="center">\n\n[![codecov](https://codecov.io/gh/software-mansion/starknet.py/branch/master/graph/badge.svg?token=3E54E8RYSL)](https://codecov.io/gh/software-mansion/starknet.py)\n[![pypi](https://img.shields.io/pypi/v/starknet.py)](https://pypi.org/project/starknet.py/)\n[![build](https://img.shields.io/github/workflow/status/software-mansion/starknet.py/format%20-%3E%20lint%20-%3E%20test)](https://github.com/software-mansion/starknet.py/actions)\n[![docs](https://readthedocs.org/projects/starknetpy/badge/?version=latest)](https://starknetpy.readthedocs.io/en/latest/?badge=latest)\n[![license](https://img.shields.io/badge/license-MIT-black)](https://github.com/software-mansion/starknet.py/blob/master/LICENSE.txt)\n[![stars](https://img.shields.io/github/stars/software-mansion/starknet.py?color=yellow)](https://github.com/software-mansion/starknet.py/stargazers)\n[![starkware](https://img.shields.io/badge/powered_by-StarkWare-navy)](https://starkware.co)\n\n</div>\n\n## 📘 Documentation\n- [Installation](https://starknetpy.rtfd.io/en/latest/installation.html)\n- [Quickstart](https://starknetpy.rtfd.io/en/latest/quickstart.html)\n- [Guide](https://starknetpy.rtfd.io/en/latest/guide.html)\n- [API](https://starknetpy.rtfd.io/en/latest/api.html)\n\n## ⚙️ Installation\nTo install this package run\n\n```\npip install starknet.py\n```\n\nor using Poetry:\n\n```\npoetry add starknet.py\n```\n\n## ▶️ Example usage\n### Asynchronous API\nThis is the recommended way of using the SDK.\n\n```python\nfrom starknet_py.contract import Contract\nfrom starknet_py.net.client import Client\n\nkey = 1234\ncontract = await Contract.from_address("0x01336fa7c870a7403aced14dda865b75f29113230ed84e3a661f7af70fe83e7b", Client("testnet"))\ninvocation = await contract.functions["set_value"].invoke(key, 7)\nawait invocation.wait_for_acceptance()\n\n(saved,) = await contract.functions["get_value"].call(key) # 7\n```\n\n### Synchronous API\nYou can access synchronous world with `_sync` postfix.\n\n```python\nfrom starknet_py.contract import Contract\nfrom starknet_py.net.client import Client\n\nkey = 1234\ncontract = Contract.from_address_sync("0x01336fa7c870a7403aced14dda865b75f29113230ed84e3a661f7af70fe83e7b", Client("testnet"))\ninvocation = contract.functions["set_value"].invoke_sync(key, 7)\ninvocation.wait_for_acceptance_sync()\n\n(saved,) = contract.functions["get_value"].call_sync(key) # 7\n```\n\nFor more examples click [here](https://starknetpy.rtfd.io/en/latest/quickstart.html).\n',
     'author': 'Tomasz Rejowski',
     'author_email': 'tomasz.rejowski@swmansion.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/software-mansion/starknet.py',
```

### Comparing `starknet_py-0.8.0a0/PKG-INFO` & `starknet_py-0.9.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starknet-py
-Version: 0.8.0a0
+Version: 0.9.0a0
 Summary: A python SDK for StarkNet
 Home-page: https://github.com/software-mansion/starknet.py
 License: MIT
 Author: Tomasz Rejowski
 Author-email: tomasz.rejowski@swmansion.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Provides-Extra: eth-tester
 Requires-Dist: asgiref (>=3.4.1,<4.0.0)
 Requires-Dist: cairo-lang (==0.10.1)
 Requires-Dist: crypto-cpp-py (>=1.0.4,<2.0.0)
-Requires-Dist: enum-tools[sphinx] (==0.9.0); extra == "docs"
+Requires-Dist: enum-tools[sphinx] (==0.9.0.post1); extra == "docs"
 Requires-Dist: marshmallow (>=3.15.0,<4.0.0)
 Requires-Dist: marshmallow-oneofschema (>=3.0.1,<4.0.0)
-Requires-Dist: sphinx (>=4.3.1,<5.0.0); extra == "docs"
+Requires-Dist: sphinx (>=4.3.1,<6.0.0); extra == "docs"
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
 Project-URL: Documentation, https://starknetpy.rtfd.io/
 Project-URL: Repository, https://github.com/software-mansion/starknet.py
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://raw.githubusercontent.com/software-mansion/starknet.py/master/graphic.png" alt="starknet.py"/>
```

