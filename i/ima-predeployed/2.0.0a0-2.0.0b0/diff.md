# Comparing `tmp/ima-predeployed-2.0.0a0.tar.gz` & `tmp/ima-predeployed-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ima-predeployed-2.0.0a0.tar", last modified: Fri Jun 23 12:40:14 2023, max compression
+gzip compressed data, was "ima-predeployed-2.0.0b0.tar", last modified: Mon Jun 12 12:03:55 2023, max compression
```

## Comparing `ima-predeployed-2.0.0a0.tar` & `ima-predeployed-2.0.0b0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:14.644279 ima-predeployed-2.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-23 12:40:14.644279 ima-predeployed-2.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-23 12:40:14.644279 ima-predeployed-2.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:14.612279 ima-predeployed-2.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:14.616279 ima-predeployed-2.0.0a0/src/ima_predeployed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:14.636279 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-06-23 12:39:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/CommunityLocker.json
--rw-r--r--   0 runner    (1001) docker     (123)   666877 2023-06-23 12:39:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/CommunityLocker.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    58650 2023-06-23 12:40:06.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC1155OnChain.json
--rw-r--r--   0 runner    (1001) docker     (123)   666876 2023-06-23 12:40:06.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC1155OnChain.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-06-23 12:40:05.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC20OnChain.json
--rw-r--r--   0 runner    (1001) docker     (123)   666874 2023-06-23 12:40:05.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC20OnChain.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    53201 2023-06-23 12:40:05.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC721OnChain.json
--rw-r--r--   0 runner    (1001) docker     (123)   666875 2023-06-23 12:40:05.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC721OnChain.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    39987 2023-06-23 12:40:04.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/EthErc20.json
--rw-r--r--   0 runner    (1001) docker     (123)   666870 2023-06-23 12:40:04.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/EthErc20.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-23 12:39:56.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/KeyStorage.json
--rw-r--r--   0 runner    (1001) docker     (123)   666872 2023-06-23 12:39:56.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/KeyStorage.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    94370 2023-06-23 12:39:57.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/MessageProxyForSchain.json
--rw-r--r--   0 runner    (1001) docker     (123)   666883 2023-06-23 12:39:57.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/MessageProxyForSchain.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-06-23 12:39:58.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManager.json
--rw-r--r--   0 runner    (1001) docker     (123)   666874 2023-06-23 12:39:58.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManager.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)   157111 2023-06-23 12:40:02.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC1155.json
--rw-r--r--   0 runner    (1001) docker     (123)   666881 2023-06-23 12:40:02.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC1155.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)   117065 2023-06-23 12:40:00.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)   666879 2023-06-23 12:40:00.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC20.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)   121494 2023-06-23 12:40:01.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC721.json
--rw-r--r--   0 runner    (1001) docker     (123)   666880 2023-06-23 12:40:01.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC721.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)   124162 2023-06-23 12:40:01.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.json
--rw-r--r--   0 runner    (1001) docker     (123)   666892 2023-06-23 12:40:01.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    48294 2023-06-23 12:40:03.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerEth.json
--rw-r--r--   0 runner    (1001) docker     (123)   666877 2023-06-23 12:40:03.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerEth.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    33186 2023-06-23 12:39:58.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerLinker.json
--rw-r--r--   0 runner    (1001) docker     (123)   666880 2023-06-23 12:39:58.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerLinker.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contract_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:14.644279 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/admin_upgradeability_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/community_locker.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/erc1155_on_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/erc20_on_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/erc721_on_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/eth_erc20.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/key_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/message_proxy_for_schain.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/proxy_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_erc1155.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_erc20.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_erc721.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_erc721_with_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_linker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/src/ima_predeployed/upgradeable_contract_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:14.620279 ima-predeployed-2.0.0a0/src/ima_predeployed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-23 12:40:14.000000 ima-predeployed-2.0.0a0/src/ima_predeployed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-23 12:40:14.000000 ima-predeployed-2.0.0a0/src/ima_predeployed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:40:14.000000 ima-predeployed-2.0.0a0/src/ima_predeployed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 12:40:14.000000 ima-predeployed-2.0.0a0/src/ima_predeployed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 12:40:14.000000 ima-predeployed-2.0.0a0/src/ima_predeployed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:14.644279 ima-predeployed-2.0.0a0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/test/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-23 12:25:59.000000 ima-predeployed-2.0.0a0/test/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 12:39:55.000000 ima-predeployed-2.0.0a0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:03:55.170870 ima-predeployed-2.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-12 12:03:55.174870 ima-predeployed-2.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-12 12:03:55.174870 ima-predeployed-2.0.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:03:55.142870 ima-predeployed-2.0.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:03:55.146870 ima-predeployed-2.0.0b0/src/ima_predeployed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:03:55.166870 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-06-12 12:03:39.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/CommunityLocker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666877 2023-06-12 12:03:39.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/CommunityLocker.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58650 2023-06-12 12:03:46.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC1155OnChain.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666876 2023-06-12 12:03:46.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC1155OnChain.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-06-12 12:03:44.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC20OnChain.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666874 2023-06-12 12:03:44.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC20OnChain.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53201 2023-06-12 12:03:45.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC721OnChain.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666875 2023-06-12 12:03:45.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC721OnChain.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39987 2023-06-12 12:03:43.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/EthErc20.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666870 2023-06-12 12:03:43.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/EthErc20.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-12 12:03:36.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/KeyStorage.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666872 2023-06-12 12:03:36.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/KeyStorage.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    94370 2023-06-12 12:03:36.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/MessageProxyForSchain.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666883 2023-06-12 12:03:36.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/MessageProxyForSchain.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-06-12 12:03:37.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManager.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666874 2023-06-12 12:03:37.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManager.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)   157111 2023-06-12 12:03:42.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666881 2023-06-12 12:03:42.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC1155.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)   117065 2023-06-12 12:03:40.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666879 2023-06-12 12:03:40.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC20.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121494 2023-06-12 12:03:40.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC721.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666880 2023-06-12 12:03:40.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC721.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)   124162 2023-06-12 12:03:41.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666892 2023-06-12 12:03:41.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48294 2023-06-12 12:03:43.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerEth.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666877 2023-06-12 12:03:43.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerEth.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33186 2023-06-12 12:03:38.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerLinker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   666880 2023-06-12 12:03:38.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerLinker.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contract_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:03:55.170870 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/admin_upgradeability_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/community_locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/erc1155_on_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/erc20_on_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/erc721_on_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/eth_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/key_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/message_proxy_for_schain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/proxy_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_erc721.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_erc721_with_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/src/ima_predeployed/upgradeable_contract_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:03:55.146870 ima-predeployed-2.0.0b0/src/ima_predeployed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-12 12:03:55.000000 ima-predeployed-2.0.0b0/src/ima_predeployed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-12 12:03:55.000000 ima-predeployed-2.0.0b0/src/ima_predeployed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:03:55.000000 ima-predeployed-2.0.0b0/src/ima_predeployed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 12:03:55.000000 ima-predeployed-2.0.0b0/src/ima_predeployed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 12:03:55.000000 ima-predeployed-2.0.0b0/src/ima_predeployed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:03:55.170870 ima-predeployed-2.0.0b0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-12 11:53:28.000000 ima-predeployed-2.0.0b0/test/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 12:03:35.000000 ima-predeployed-2.0.0b0/version.txt
```

### Comparing `ima-predeployed-2.0.0a0/LICENSE` & `ima-predeployed-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/PKG-INFO` & `ima-predeployed-2.0.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ima-predeployed
-Version: 2.0.0a0
+Version: 2.0.0b0
 Summary: A tool to generate config for predeployed IMA
 Home-page: https://github.com/skalenetwork/IMA
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ima-predeployed-2.0.0a0/setup.cfg` & `ima-predeployed-2.0.0b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/addresses.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/addresses.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/CommunityLocker.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/CommunityLocker.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/CommunityLocker.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/CommunityLocker.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC1155OnChain.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC1155OnChain.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC1155OnChain.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC1155OnChain.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC20OnChain.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC20OnChain.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC20OnChain.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC20OnChain.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC721OnChain.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC721OnChain.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/ERC721OnChain.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/ERC721OnChain.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/EthErc20.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/EthErc20.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/EthErc20.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/EthErc20.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/KeyStorage.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/KeyStorage.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/KeyStorage.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/KeyStorage.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/MessageProxyForSchain.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/MessageProxyForSchain.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/MessageProxyForSchain.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/MessageProxyForSchain.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManager.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManager.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManager.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManager.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC1155.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC1155.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC1155.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC1155.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC20.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC20.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC20.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC20.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC721.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC721.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC721.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC721.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerERC721WithMetadata.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerEth.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerEth.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerEth.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerEth.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerLinker.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerLinker.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/artifacts/TokenManagerLinker.meta.json` & `ima-predeployed-2.0.0b0/src/ima_predeployed/artifacts/TokenManagerLinker.meta.json`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contract_generator.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contract_generator.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/admin_upgradeability_proxy.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/admin_upgradeability_proxy.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/community_locker.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/community_locker.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/erc1155_on_chain.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/erc1155_on_chain.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/erc20_on_chain.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/erc20_on_chain.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/erc721_on_chain.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/erc721_on_chain.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/eth_erc20.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/eth_erc20.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/key_storage.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/key_storage.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/message_proxy_for_schain.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/message_proxy_for_schain.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_erc1155.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_erc1155.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_erc20.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_erc20.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_erc721.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_erc721.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_erc721_with_metadata.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_erc721_with_metadata.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_eth.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_eth.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/contracts/token_manager_linker.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/contracts/token_manager_linker.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/generator.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/generator.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed/upgradeable_contract_generator.py` & `ima-predeployed-2.0.0b0/src/ima_predeployed/upgradeable_contract_generator.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed.egg-info/PKG-INFO` & `ima-predeployed-2.0.0b0/src/ima_predeployed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ima-predeployed
-Version: 2.0.0a0
+Version: 2.0.0b0
 Summary: A tool to generate config for predeployed IMA
 Home-page: https://github.com/skalenetwork/IMA
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ima-predeployed-2.0.0a0/src/ima_predeployed.egg-info/SOURCES.txt` & `ima-predeployed-2.0.0b0/src/ima_predeployed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/test/test.py` & `ima-predeployed-2.0.0b0/test/test.py`

 * *Files identical despite different names*

### Comparing `ima-predeployed-2.0.0a0/test/test_generator.py` & `ima-predeployed-2.0.0b0/test/test_generator.py`

 * *Files identical despite different names*

