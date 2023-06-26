# Comparing `tmp/ledger_bitcoin-0.2.1.tar.gz` & `tmp/ledger_bitcoin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledger_bitcoin-0.2.1.tar", last modified: Tue Apr 18 14:25:56 2023, max compression
+gzip compressed data, was "ledger_bitcoin-0.2.2.tar", last modified: Mon Jun 26 13:02:35 2023, max compression
```

## Comparing `ledger_bitcoin-0.2.1.tar` & `ledger_bitcoin-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,77 @@
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/
--rw-rw-r--   0 singala   (1000) singala   (1000)    11357 2023-04-18 14:24:56.000000 ledger_bitcoin-0.2.1/LICENSE
--rw-rw-r--   0 singala   (1000) singala   (1000)     5812 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/PKG-INFO
--rw-rw-r--   0 singala   (1000) singala   (1000)     5260 2023-04-18 14:24:56.000000 ledger_bitcoin-0.2.1/README.md
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.903050 ledger_bitcoin-0.2.1/ledger_bitcoin/
--rw-rw-r--   0 singala   (1000) singala   (1000)      450 2023-04-18 14:25:09.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/__init__.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4051 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/_base58.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4265 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/_script.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     6661 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/_serialize.py
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/
--rw-rw-r--   0 singala   (1000) singala   (1000)      855 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/__init__.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4874 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/bitcoinTransaction.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     2025 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/bitcoinVarint.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    16475 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchip.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4795 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipComm.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1020 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipException.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     2713 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipHelpers.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     3416 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipUtils.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     3224 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/ledgerWrapper.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    11466 2023-04-18 14:25:09.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/client.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     9267 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/client_base.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    11336 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/client_command.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    15428 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/client_legacy.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     5937 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/command_builder.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4688 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/common.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     7153 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/errors.py
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/ledger_bitcoin/exception/
--rw-rw-r--   0 singala   (1000) singala   (1000)      806 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/exception/__init__.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1251 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/exception/device_exception.py
--rw-rw-r--   0 singala   (1000) singala   (1000)      652 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/exception/errors.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    15997 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/key.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     8383 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/merkle.py
--rw-rw-r--   0 singala   (1000) singala   (1000)    47567 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/psbt.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4206 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/ripemd.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     7623 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/transport.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     9191 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/tx.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     4397 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/ledger_bitcoin/wallet.py
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.903050 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/
--rw-rw-r--   0 singala   (1000) singala   (1000)     5812 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/PKG-INFO
--rw-rw-r--   0 singala   (1000) singala   (1000)     1427 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/SOURCES.txt
--rw-rw-r--   0 singala   (1000) singala   (1000)        1 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/dependency_links.txt
--rw-rw-r--   0 singala   (1000) singala   (1000)       84 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/requires.txt
--rw-rw-r--   0 singala   (1000) singala   (1000)       15 2023-04-18 14:25:56.000000 ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/top_level.txt
--rw-rw-r--   0 singala   (1000) singala   (1000)      159 2023-04-18 14:24:56.000000 ledger_bitcoin-0.2.1/pyproject.toml
--rw-rw-r--   0 singala   (1000) singala   (1000)      812 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/setup.cfg
-drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-04-18 14:25:56.907050 ledger_bitcoin-0.2.1/tests/
--rw-rw-r--   0 singala   (1000) singala   (1000)      431 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/tests/test_client_legacy.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1289 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/tests/test_get_extended_pubkey_legacyapp.py
--rw-rw-r--   0 singala   (1000) singala   (1000)      259 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/tests/test_get_master_fingerprint_legacyapp.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1823 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/tests/test_get_wallet_address_legacyapp.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     1050 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/tests/test_ripemd160.py
--rw-rw-r--   0 singala   (1000) singala   (1000)      447 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.1/tests/test_sign_message_legacyapp.py
--rw-rw-r--   0 singala   (1000) singala   (1000)     5504 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.1/tests/test_sign_psbt_legacyapp.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.468401 ledger_bitcoin-0.2.2/
+-rw-rw-r--   0 singala   (1000) singala   (1000)    11357 2023-04-18 14:24:56.000000 ledger_bitcoin-0.2.2/LICENSE
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5812 2023-06-26 13:02:35.468401 ledger_bitcoin-0.2.2/PKG-INFO
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5260 2023-04-18 14:24:56.000000 ledger_bitcoin-0.2.2/README.md
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.464401 ledger_bitcoin-0.2.2/ledger_bitcoin/
+-rw-rw-r--   0 singala   (1000) singala   (1000)      450 2023-06-26 12:54:10.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/__init__.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4051 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/_base58.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4265 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/_script.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     6661 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/_serialize.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.464401 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/
+-rw-rw-r--   0 singala   (1000) singala   (1000)       22 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/__init__.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.464401 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/descriptors/
+-rw-rw-r--   0 singala   (1000) singala   (1000)     7222 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/descriptors/__init__.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     2233 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/descriptors/checksum.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      196 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/descriptors/errors.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1980 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/descriptors/parsing.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      588 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/descriptors/utils.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    11936 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/key.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.468401 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/miniscript/
+-rw-rw-r--   0 singala   (1000) singala   (1000)      394 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/miniscript/__init__.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      446 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/miniscript/errors.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    39241 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/miniscript/fragments.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    22271 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/miniscript/parsing.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     2920 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/miniscript/property.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    18070 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/miniscript/satisfaction.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.468401 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/utils/
+-rw-rw-r--   0 singala   (1000) singala   (1000)        0 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/utils/__init__.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1353 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/utils/bignum.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      523 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/utils/hashes.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4226 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/utils/ripemd_fallback.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    13988 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/bip380/utils/script.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.468401 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/
+-rw-rw-r--   0 singala   (1000) singala   (1000)      855 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/__init__.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4874 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/bitcoinTransaction.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     2025 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/bitcoinVarint.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    16475 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchip.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4795 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchipComm.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1020 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchipException.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     2713 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchipHelpers.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     3416 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchipUtils.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     3224 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/ledgerWrapper.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    12355 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/client.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     9267 2023-05-29 12:33:12.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/client_base.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    11336 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/client_command.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    15428 2023-05-29 12:33:12.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/client_legacy.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5937 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/command_builder.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4688 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/common.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     7153 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/errors.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.468401 ledger_bitcoin-0.2.2/ledger_bitcoin/exception/
+-rw-rw-r--   0 singala   (1000) singala   (1000)      806 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/exception/__init__.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1251 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/exception/device_exception.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      652 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/exception/errors.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    15997 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/key.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     8383 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/merkle.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)    47567 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/psbt.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)        0 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/py.typed
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4206 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/ripemd.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5021 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/segwit_addr.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     7623 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/transport.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     9191 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/tx.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     4397 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/ledger_bitcoin/wallet.py
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.464401 ledger_bitcoin-0.2.2/ledger_bitcoin.egg-info/
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5812 2023-06-26 13:02:35.000000 ledger_bitcoin-0.2.2/ledger_bitcoin.egg-info/PKG-INFO
+-rw-rw-r--   0 singala   (1000) singala   (1000)     2241 2023-06-26 13:02:35.000000 ledger_bitcoin-0.2.2/ledger_bitcoin.egg-info/SOURCES.txt
+-rw-rw-r--   0 singala   (1000) singala   (1000)        1 2023-06-26 13:02:35.000000 ledger_bitcoin-0.2.2/ledger_bitcoin.egg-info/dependency_links.txt
+-rw-rw-r--   0 singala   (1000) singala   (1000)      111 2023-06-26 13:02:35.000000 ledger_bitcoin-0.2.2/ledger_bitcoin.egg-info/requires.txt
+-rw-rw-r--   0 singala   (1000) singala   (1000)       15 2023-06-26 13:02:35.000000 ledger_bitcoin-0.2.2/ledger_bitcoin.egg-info/top_level.txt
+-rw-rw-r--   0 singala   (1000) singala   (1000)      200 2023-06-22 07:46:59.000000 ledger_bitcoin-0.2.2/pyproject.toml
+-rw-rw-r--   0 singala   (1000) singala   (1000)      880 2023-06-26 13:02:35.468401 ledger_bitcoin-0.2.2/setup.cfg
+drwxrwxr-x   0 singala   (1000) singala   (1000)        0 2023-06-26 13:02:35.468401 ledger_bitcoin-0.2.2/tests/
+-rw-rw-r--   0 singala   (1000) singala   (1000)      431 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/tests/test_client_legacy.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1289 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/tests/test_get_extended_pubkey_legacyapp.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      259 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/tests/test_get_master_fingerprint_legacyapp.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1823 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/tests/test_get_wallet_address_legacyapp.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     1050 2023-03-31 15:12:00.000000 ledger_bitcoin-0.2.2/tests/test_ripemd160.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)      447 2023-01-28 15:06:46.000000 ledger_bitcoin-0.2.2/tests/test_sign_message_legacyapp.py
+-rw-rw-r--   0 singala   (1000) singala   (1000)     5504 2023-05-29 12:33:12.000000 ledger_bitcoin-0.2.2/tests/test_sign_psbt_legacyapp.py
```

### Comparing `ledger_bitcoin-0.2.1/LICENSE` & `ledger_bitcoin-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/PKG-INFO` & `ledger_bitcoin-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger_bitcoin
-Version: 0.2.1
+Version: 0.2.2
 Summary: Client for Ledger Nano Bitcoin application
 Home-page: https://github.com/LedgerHQ/app-bitcoin-new
 Author: Ledger
 Author-email: hello@ledger.fr
 Project-URL: Bug Tracker, https://github.com/LedgerHQ/app-bitcoin-new/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ledger_bitcoin-0.2.1/README.md` & `ledger_bitcoin-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/_base58.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/_base58.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/_script.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/_script.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/_serialize.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/_serialize.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/__init__.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/__init__.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/bitcoinTransaction.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/bitcoinTransaction.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/bitcoinVarint.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/bitcoinVarint.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchip.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchip.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipComm.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchipComm.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipException.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchipException.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipHelpers.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchipHelpers.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/btchipUtils.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/btchipUtils.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/btchip/ledgerWrapper.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/btchip/ledgerWrapper.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/client.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from packaging.version import parse as parse_version
 from typing import Tuple, List, Mapping, Optional, Union
 import base64
 from io import BytesIO, BufferedReader
-import re
+
+from .bip380.descriptors import Descriptor
 
 from .command_builder import BitcoinCommandBuilder, BitcoinInsType
 from .common import Chain, read_uint, read_varint
 from .client_command import ClientCommandInterpreter
 from .client_base import Client, TransportClient, PartialSignature
 from .client_legacy import LegacyClient
 from .exception import DeviceException
 from .errors import UnknownDeviceError
 from .merkle import get_merkleized_map_commitment
 from .wallet import WalletPolicy, WalletType
 from .psbt import PSBT, normalize_psbt
+from . import segwit_addr
 from ._serialize import deser_string
 
 
 def parse_stream_to_map(f: BufferedReader) -> Mapping[bytes, bytes]:
     result = {}
     while True:
         try:
@@ -48,19 +50,14 @@
 
         if len(pubkey_augm) not in [32, 33]:
             raise UnknownDeviceError(f"Invalid pubkey length returned: {len(pubkey_augm)}")
 
         return PartialSignature(signature=signature, pubkey=pubkey_augm)
 
 
-def _contains_a_fragment(desc_tmp: str) -> bool:
-    """Returns true if the given descriptor template contains the `a:` fragment."""
-    return any('a' in match for match in re.findall(r'[asctdvjnlu]+:', desc_tmp))
-
-
 class NewClient(Client):
     # internal use for testing: if set to True, sign_psbt will not clone the psbt before converting to psbt version 2
     _no_clone_psbt: bool = False
 
     def __init__(self, comm_client: TransportClient, chain: Chain = Chain.MAIN, debug: bool = False) -> None:
         super().__init__(comm_client, chain, debug)
         self.builder = BitcoinCommandBuilder()
@@ -90,16 +87,14 @@
 
         return response.decode()
 
     def register_wallet(self, wallet: WalletPolicy) -> Tuple[bytes, bytes]:
         if wallet.version not in [WalletType.WALLET_POLICY_V1, WalletType.WALLET_POLICY_V2]:
             raise ValueError("invalid wallet policy version")
 
-        self._validate_policy(wallet)
-
         client_intepreter = ClientCommandInterpreter()
         client_intepreter.add_known_preimage(wallet.serialize())
         client_intepreter.add_known_list([k.encode() for k in wallet.keys_info])
 
         # necessary for version 1 of the protocol (introduced in version 2.1.0)
         client_intepreter.add_known_preimage(wallet.descriptor_template.encode())
 
@@ -112,14 +107,21 @@
 
         if len(response) != 64:
             raise RuntimeError(f"Invalid response length: {len(response)}")
 
         wallet_id = response[0:32]
         wallet_hmac = response[32:64]
 
+        if self._should_validate_address(wallet):
+            # sanity check: for miniscripts, derive the first address independently with python-bip380
+            first_addr_device = self.get_wallet_address(wallet, wallet_hmac, 0, 0, False)
+
+            if first_addr_device != self._derive_segwit_address_for_policy(wallet, False, 0):
+                raise RuntimeError("Invalid address. Please update your Bitcoin app. If the problem persists, report a bug at https://github.com/LedgerHQ/app-bitcoin-new")
+
         return wallet_id, wallet_hmac
 
     def get_wallet_address(
         self,
         wallet: WalletPolicy,
         wallet_hmac: Optional[bytes],
         change: int,
@@ -129,16 +131,14 @@
 
         if not isinstance(wallet, WalletPolicy) or wallet.version not in [WalletType.WALLET_POLICY_V1, WalletType.WALLET_POLICY_V2]:
             raise ValueError("wallet type must be WalletPolicy, with version either WALLET_POLICY_V1 or WALLET_POLICY_V2")
 
         if change != 0 and change != 1:
             raise ValueError("Invalid change")
 
-        self._validate_policy(wallet)
-
         client_intepreter = ClientCommandInterpreter()
         client_intepreter.add_known_list([k.encode() for k in wallet.keys_info])
         client_intepreter.add_known_preimage(wallet.serialize())
 
         # necessary for version 1 of the protocol (introduced in version 2.1.0)
         client_intepreter.add_known_preimage(wallet.descriptor_template.encode())
 
@@ -148,19 +148,25 @@
             ),
             client_intepreter,
         )
 
         if sw != 0x9000:
             raise DeviceException(error_code=sw, ins=BitcoinInsType.GET_WALLET_ADDRESS)
 
-        return response.decode()
+        result = response.decode()
 
-    def sign_psbt(self, psbt: Union[PSBT, bytes, str], wallet: WalletPolicy, wallet_hmac: Optional[bytes]) -> List[Tuple[int, PartialSignature]]:
+        if self._should_validate_address(wallet):
+            # sanity check: for miniscripts, derive the address independently with python-bip380
 
-        self._validate_policy(wallet)
+            if result != self._derive_segwit_address_for_policy(wallet, change, address_index):
+                raise RuntimeError("Invalid address. Please update your Bitcoin app. If the problem persists, report a bug at https://github.com/LedgerHQ/app-bitcoin-new")
+
+        return result
+
+    def sign_psbt(self, psbt: Union[PSBT, bytes, str], wallet: WalletPolicy, wallet_hmac: Optional[bytes]) -> List[Tuple[int, PartialSignature]]:
 
         psbt = normalize_psbt(psbt)
 
         if psbt.version != 2:
             if self._no_clone_psbt:
                 psbt.convert_to_v2()
                 psbt_v2 = psbt
@@ -261,22 +267,26 @@
         sw, response = self._make_request(self.builder.sign_message(message_bytes, bip32_path), client_intepreter)
 
         if sw != 0x9000:
             raise DeviceException(error_code=sw, ins=BitcoinInsType.SIGN_MESSAGE)
 
         return base64.b64encode(response).decode('utf-8')
 
-    def _validate_policy(self, wallet_policy: WalletPolicy):
-        """Performs any additional checks before we use a wallet policy"""
-        if _contains_a_fragment(wallet_policy.descriptor_template):
-            _, app_version, _ = self.get_version()
-            if app_version in ["2.1.0", "2.1.1"]:
-                # Versions 2.1.0 and 2.1.1 produced incorrect scripts for policies containing
-                # the `a:` fragment.
-                raise RuntimeError("Please update your Ledger Bitcoin app.")
+    def _should_validate_address(self, wallet: WalletPolicy) -> bool:
+        # TODO: extend to taproot miniscripts once supported
+        return wallet.descriptor_template.startswith("wsh(") and not wallet.descriptor_template.startswith("wsh(sortedmulti(")
+
+    def _derive_segwit_address_for_policy(self, wallet: WalletPolicy, change: bool, address_index: int) -> bool:
+        desc = Descriptor.from_str(wallet.get_descriptor(change))
+        desc.derive(address_index)
+        spk = desc.script_pubkey
+        if spk[0:2] != b'\x00\x20' or len(spk) != 34:
+            raise RuntimeError("Invalid scriptPubKey")
+        hrp = "bc" if self.chain == Chain.MAIN else "tb"
+        return segwit_addr.encode(hrp, 0, spk[2:])
 
 
 def createClient(comm_client: Optional[TransportClient] = None, chain: Chain = Chain.MAIN, debug: bool = False) -> Union[LegacyClient, NewClient]:
     if comm_client is None:
         comm_client = TransportClient("hid")
 
     base_client = Client(comm_client, chain, debug)
```

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/client_base.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/client_base.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/client_command.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/client_command.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/client_legacy.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/client_legacy.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/command_builder.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/command_builder.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/common.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/common.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/errors.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/errors.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/exception/__init__.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/exception/device_exception.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/exception/device_exception.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/exception/errors.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/exception/errors.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/key.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/key.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/merkle.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/merkle.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/psbt.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/psbt.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/ripemd.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/ripemd.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/transport.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/transport.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/tx.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/tx.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin/wallet.py` & `ledger_bitcoin-0.2.2/ledger_bitcoin/wallet.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/PKG-INFO` & `ledger_bitcoin-0.2.2/ledger_bitcoin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger-bitcoin
-Version: 0.2.1
+Version: 0.2.2
 Summary: Client for Ledger Nano Bitcoin application
 Home-page: https://github.com/LedgerHQ/app-bitcoin-new
 Author: Ledger
 Author-email: hello@ledger.fr
 Project-URL: Bug Tracker, https://github.com/LedgerHQ/app-bitcoin-new/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ledger_bitcoin-0.2.1/ledger_bitcoin.egg-info/SOURCES.txt` & `ledger_bitcoin-0.2.2/ledger_bitcoin.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,23 +12,43 @@
 ledger_bitcoin/client_legacy.py
 ledger_bitcoin/command_builder.py
 ledger_bitcoin/common.py
 ledger_bitcoin/errors.py
 ledger_bitcoin/key.py
 ledger_bitcoin/merkle.py
 ledger_bitcoin/psbt.py
+ledger_bitcoin/py.typed
 ledger_bitcoin/ripemd.py
+ledger_bitcoin/segwit_addr.py
 ledger_bitcoin/transport.py
 ledger_bitcoin/tx.py
 ledger_bitcoin/wallet.py
 ledger_bitcoin.egg-info/PKG-INFO
 ledger_bitcoin.egg-info/SOURCES.txt
 ledger_bitcoin.egg-info/dependency_links.txt
 ledger_bitcoin.egg-info/requires.txt
 ledger_bitcoin.egg-info/top_level.txt
+ledger_bitcoin/bip380/__init__.py
+ledger_bitcoin/bip380/key.py
+ledger_bitcoin/bip380/descriptors/__init__.py
+ledger_bitcoin/bip380/descriptors/checksum.py
+ledger_bitcoin/bip380/descriptors/errors.py
+ledger_bitcoin/bip380/descriptors/parsing.py
+ledger_bitcoin/bip380/descriptors/utils.py
+ledger_bitcoin/bip380/miniscript/__init__.py
+ledger_bitcoin/bip380/miniscript/errors.py
+ledger_bitcoin/bip380/miniscript/fragments.py
+ledger_bitcoin/bip380/miniscript/parsing.py
+ledger_bitcoin/bip380/miniscript/property.py
+ledger_bitcoin/bip380/miniscript/satisfaction.py
+ledger_bitcoin/bip380/utils/__init__.py
+ledger_bitcoin/bip380/utils/bignum.py
+ledger_bitcoin/bip380/utils/hashes.py
+ledger_bitcoin/bip380/utils/ripemd_fallback.py
+ledger_bitcoin/bip380/utils/script.py
 ledger_bitcoin/btchip/__init__.py
 ledger_bitcoin/btchip/bitcoinTransaction.py
 ledger_bitcoin/btchip/bitcoinVarint.py
 ledger_bitcoin/btchip/btchip.py
 ledger_bitcoin/btchip/btchipComm.py
 ledger_bitcoin/btchip/btchipException.py
 ledger_bitcoin/btchip/btchipHelpers.py
```

### Comparing `ledger_bitcoin-0.2.1/setup.cfg` & `ledger_bitcoin-0.2.2/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -14,18 +14,23 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
+	bip32~=3.0,
+	coincurve~=18.0,
 	typing-extensions>=3.7
 	ledgercomm>=1.1.0
 	packaging>=21.3
 
+[options.package_data]
+* = py.typed
+
 [options.extras_require]
 hid = hidapi>=0.9.0.post3
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.utils
```

### Comparing `ledger_bitcoin-0.2.1/tests/test_get_extended_pubkey_legacyapp.py` & `ledger_bitcoin-0.2.2/tests/test_get_extended_pubkey_legacyapp.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/tests/test_get_wallet_address_legacyapp.py` & `ledger_bitcoin-0.2.2/tests/test_get_wallet_address_legacyapp.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/tests/test_ripemd160.py` & `ledger_bitcoin-0.2.2/tests/test_ripemd160.py`

 * *Files identical despite different names*

### Comparing `ledger_bitcoin-0.2.1/tests/test_sign_psbt_legacyapp.py` & `ledger_bitcoin-0.2.2/tests/test_sign_psbt_legacyapp.py`

 * *Files identical despite different names*

