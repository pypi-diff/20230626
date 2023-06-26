# Comparing `tmp/cosmo_wallet_friends-0.1.0.tar.gz` & `tmp/cosmo_wallet_friends-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmo_wallet_friends-0.1.0.tar", max compression
+gzip compressed data, was "cosmo_wallet_friends-0.1.1.tar", max compression
```

## Comparing `cosmo_wallet_friends-0.1.0.tar` & `cosmo_wallet_friends-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        5 2023-06-26 19:21:15.952642 cosmo_wallet_friends-0.1.0/README.md
--rw-r--r--   0        0        0      728 2023-06-25 16:37:28.643148 cosmo_wallet_friends-0.1.0/cosmo_wallet_friends/bot/teste_bot.py
--rw-r--r--   0        0        0     1737 2023-06-26 19:07:53.112542 cosmo_wallet_friends-0.1.0/cosmo_wallet_friends/controller.py
--rw-r--r--   0        0        0      288 2023-06-26 19:20:41.616497 cosmo_wallet_friends-0.1.0/cosmo_wallet_friends/main.py
--rw-r--r--   0        0        0      515 2023-06-26 19:02:50.623423 cosmo_wallet_friends-0.1.0/cosmo_wallet_friends/models.py
--rw-r--r--   0        0        0     1386 2023-06-26 19:04:57.687831 cosmo_wallet_friends-0.1.0/cosmo_wallet_friends/wallets.py
--rw-r--r--   0        0        0      349 2023-06-26 19:18:44.483989 cosmo_wallet_friends-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 cosmo_wallet_friends-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2023-06-26 19:21:15.952642 cosmo_wallet_friends-0.1.1/README.md
+-rw-r--r--   0        0        0       91 2023-06-26 19:38:58.612722 cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-25 16:37:28.643148 cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/bot/teste_bot.py
+-rw-r--r--   0        0        0     1737 2023-06-26 19:07:53.112542 cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/controller.py
+-rw-r--r--   0        0        0      288 2023-06-26 19:20:41.616497 cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/main.py
+-rw-r--r--   0        0        0      515 2023-06-26 19:02:50.623423 cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/models.py
+-rw-r--r--   0        0        0     1386 2023-06-26 19:04:57.687831 cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/wallets.py
+-rw-r--r--   0        0        0      349 2023-06-26 19:39:04.492744 cosmo_wallet_friends-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 cosmo_wallet_friends-0.1.1/PKG-INFO
```

### Comparing `cosmo_wallet_friends-0.1.0/cosmo_wallet_friends/bot/teste_bot.py` & `cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/bot/teste_bot.py`

 * *Files identical despite different names*

### Comparing `cosmo_wallet_friends-0.1.0/cosmo_wallet_friends/controller.py` & `cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/controller.py`

 * *Files identical despite different names*

### Comparing `cosmo_wallet_friends-0.1.0/cosmo_wallet_friends/models.py` & `cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/models.py`

 * *Files identical despite different names*

### Comparing `cosmo_wallet_friends-0.1.0/cosmo_wallet_friends/wallets.py` & `cosmo_wallet_friends-0.1.1/cosmo_wallet_friends/wallets.py`

 * *Files identical despite different names*

