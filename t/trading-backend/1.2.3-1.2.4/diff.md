# Comparing `tmp/trading-backend-1.2.3.tar.gz` & `tmp/trading-backend-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trading-backend-1.2.3.tar", last modified: Tue May  2 21:33:02 2023, max compression
+gzip compressed data, was "trading-backend-1.2.4.tar", last modified: Mon Jun 26 19:10:42 2023, max compression
```

## Comparing `trading-backend-1.2.3.tar` & `trading-backend-1.2.4.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:33:02.956793 trading-backend-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-02 21:32:14.000000 trading-backend-1.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 21:32:14.000000 trading-backend-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 21:32:14.000000 trading-backend-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-02 21:33:02.956793 trading-backend-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-02 21:32:14.000000 trading-backend-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 21:32:14.000000 trading-backend-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 21:33:02.960793 trading-backend-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-02 21:32:14.000000 trading-backend-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:33:02.944793 trading-backend-1.2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:33:02.952793 trading-backend-1.2.3/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/exchanges/test_phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:33:02.952793 trading-backend-1.2.3/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-02 21:32:14.000000 trading-backend-1.2.3/tests/util/create_order_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:33:02.952793 trading-backend-1.2.3/trading_backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchange_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:33:02.956793 trading-backend-1.2.3/trading_backend/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 21:32:14.000000 trading-backend-1.2.3/trading_backend/exchanges/phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:33:02.956793 trading-backend-1.2.3/trading_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-02 21:33:02.000000 trading-backend-1.2.3/trading_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-02 21:33:02.000000 trading-backend-1.2.3/trading_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:33:02.000000 trading-backend-1.2.3/trading_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:33:02.000000 trading-backend-1.2.3/trading_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 21:33:02.000000 trading-backend-1.2.3/trading_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 21:33:02.000000 trading-backend-1.2.3/trading_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-26 19:10:12.000000 trading-backend-1.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-26 19:10:12.000000 trading-backend-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 19:10:12.000000 trading-backend-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-26 19:10:42.350382 trading-backend-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-26 19:10:12.000000 trading-backend-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 19:10:12.000000 trading-backend-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 19:10:42.354382 trading-backend-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-26 19:10:12.000000 trading-backend-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.346382 trading-backend-1.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_kucoin_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/exchanges/test_phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-26 19:10:12.000000 trading-backend-1.2.4/tests/util/create_order_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/trading_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchange_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/trading_backend/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/kucoinfutures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-26 19:10:12.000000 trading-backend-1.2.4/trading_backend/exchanges/phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:10:42.350382 trading-backend-1.2.4/trading_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 19:10:42.000000 trading-backend-1.2.4/trading_backend.egg-info/top_level.txt
```

### Comparing `trading-backend-1.2.3/CHANGELOG.md` & `trading-backend-1.2.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.2.4] - 2023-06-24
+### Added
+- Kucoin and Kucoin futures
+
 ## [1.2.3] - 2023-05-02
 ### Updated
 - setup.py
 
 ## [1.2.2] - 2023-05-02
 ### Remove
 - Constants
```

### Comparing `trading-backend-1.2.3/LICENSE` & `trading-backend-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/PKG-INFO` & `trading-backend-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.3
+Version: 1.2.4
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.3](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.4](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.3/README.md` & `trading-backend-1.2.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# trading-backend [1.2.3](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.4](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.3/setup.py` & `trading-backend-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 # from distutils.extension import Extension
 from setuptools import find_packages
 from setuptools import setup
 
-VERSION = "1.2.3"
+VERSION = "1.2.4"
 PROJECT_NAME = "trading-backend"
 
 PACKAGES = find_packages(exclude=["tests"])
 
 
 # long description from README file
 with open('README.md', encoding='utf-8') as f:
```

### Comparing `trading-backend-1.2.3/tests/exchanges/test_ascendex.py` & `trading-backend-1.2.4/tests/exchanges/test_ascendex.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import tests.util.create_order_tests as create_order_tests
 from tests import ascendex_exchange
 
 
 def test_get_name(ascendex_exchange):
-    assert exchanges.Ascendex(ascendex_exchange).get_name() == ccxt.async_support.ascendex().name.lower()
+    assert exchanges.Ascendex(ascendex_exchange).get_name() == ccxt.async_support.ascendex().id.lower()
 
 
 @pytest.mark.asyncio
 async def test_get_orders_parameters(ascendex_exchange):
     exchange = exchanges.Ascendex(ascendex_exchange)
     with mock.patch.object(exchange._exchange.connector.client, "v1PrivateGetInfo", mock.AsyncMock(return_value={})):
         await create_order_tests.create_order_mocked_test_args(
```

### Comparing `trading-backend-1.2.3/tests/exchanges/test_binance.py` & `trading-backend-1.2.4/tests/exchanges/test_binance.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import trading_backend
 from tests import binance_exchange
 
 
 def test_get_name(binance_exchange):
-    assert exchanges.Binance(binance_exchange).get_name() == ccxt.async_support.binance().name.lower()
+    assert exchanges.Binance(binance_exchange).get_name() == ccxt.async_support.binance().id.lower()
 
 
 def test_get_orders_parameters(binance_exchange):
     exchange = exchanges.Binance(binance_exchange)
     with mock.patch.object(exchange._exchange.connector.client, "uuid22",
                            mock.Mock(return_value="123456789")) as uuid22_mock:
         assert exchange.get_orders_parameters({"a": 1}) == {
```

### Comparing `trading-backend-1.2.3/tests/exchanges/test_bitget.py` & `trading-backend-1.2.4/tests/exchanges/test_bitget.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import tests.util.create_order_tests as create_order_tests
 from tests import bitget_exchange
 
 
 def test_get_name(bitget_exchange):
-    assert exchanges.Bitget(bitget_exchange).get_name() == ccxt.async_support.bitget().name.lower()
+    assert exchanges.Bitget(bitget_exchange).get_name() == ccxt.async_support.bitget().id.lower()
 
 
 @pytest.mark.asyncio
 async def test_get_orders_parameters(bitget_exchange):
     exchange = exchanges.Bitget(bitget_exchange)
     await create_order_tests.create_order_mocked_test_args(
         exchange,
```

### Comparing `trading-backend-1.2.3/tests/exchanges/test_bybit.py` & `trading-backend-1.2.4/tests/exchanges/test_bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/tests/exchanges/test_exchange.py` & `trading-backend-1.2.4/tests/exchanges/test_exchange.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/tests/exchanges/test_gateio.py` & `trading-backend-1.2.4/tests/exchanges/test_gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/tests/exchanges/test_huobi.py` & `trading-backend-1.2.4/tests/exchanges/test_huobi.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import tests.util.create_order_tests as create_order_tests
 from tests import huobi_exchange
 
 
 def test_get_name(huobi_exchange):
-    assert exchanges.Huobi(huobi_exchange).get_name() == ccxt.async_support.huobi().name.lower()
+    assert exchanges.Huobi(huobi_exchange).get_name() == ccxt.async_support.huobi().id.lower()
 
 
 @pytest.mark.asyncio
 async def test_get_orders_parameters(huobi_exchange):
     exchange = exchanges.Huobi(huobi_exchange)
     with mock.patch.object(exchange._exchange.connector.client,
                            "fetch_accounts", mock.AsyncMock(return_value=[{'id': 1}])):
```

### Comparing `trading-backend-1.2.3/tests/exchanges/test_huobipro.py` & `trading-backend-1.2.4/tests/exchanges/test_huobipro.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 import trading_backend.exchanges as exchanges
 import tests.util.create_order_tests as create_order_tests
 from tests import huobipro_exchange
 
 
 def test_get_name(huobipro_exchange):
     # huobi on ccxt
-    assert exchanges.HuobiPro(huobipro_exchange).get_name() != ccxt.async_support.huobipro().name.lower()
-    assert exchanges.HuobiPro(huobipro_exchange).get_name() == "huobipro"
+    assert exchanges.HuobiPro(huobipro_exchange).get_name() == ccxt.async_support.huobipro().id.lower()
 
 
 @pytest.mark.asyncio
 async def test_get_orders_parameters(huobipro_exchange):
     exchange = exchanges.HuobiPro(huobipro_exchange)
     with mock.patch.object(exchange._exchange.connector.client,
                            "fetch_accounts", mock.AsyncMock(return_value=[{'id': 1}])):
```

### Comparing `trading-backend-1.2.3/tests/exchanges/test_okx.py` & `trading-backend-1.2.4/tests/exchanges/test_okx.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import tests.util.create_order_tests as create_order_tests
 from tests import okx_exchange
 
 
 def test_get_name(okx_exchange):
-    assert exchanges.OKX(okx_exchange).get_name() == ccxt.async_support.okx().name.lower()
+    assert exchanges.OKX(okx_exchange).get_name() == ccxt.async_support.okx().id.lower()
 
 
 @pytest.mark.asyncio
 async def test_get_orders_parameters(okx_exchange):
     exchange = exchanges.OKX(okx_exchange)
     await create_order_tests.create_order_mocked_test_args(
         exchange,
```

### Comparing `trading-backend-1.2.3/tests/exchanges/test_phemex.py` & `trading-backend-1.2.4/tests/exchanges/test_phemex.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import tests.util.create_order_tests as create_order_tests
 from tests import phemex_exchange
 
 
 def test_get_name(phemex_exchange):
-    assert exchanges.Phemex(phemex_exchange).get_name() == ccxt.async_support.phemex().name.lower()
+    assert exchanges.Phemex(phemex_exchange).get_name() == ccxt.async_support.phemex().id.lower()
 
 
 @pytest.mark.asyncio
 async def test_get_orders_parameters(phemex_exchange):
     exchange = exchanges.Phemex(phemex_exchange)
     # stopPxEp not in ccxt "market" which is used as default value, provide it in mock
     await create_order_tests.create_order_mocked_test_args(
```

### Comparing `trading-backend-1.2.3/tests/util/__init__.py` & `trading-backend-1.2.4/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/__init__.py` & `trading-backend-1.2.4/trading_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/errors.py` & `trading-backend-1.2.4/trading_backend/errors.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchange_factory.py` & `trading-backend-1.2.4/trading_backend/exchange_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import trading_backend.exchanges as exchanges
 
 
 def create_exchange_backend(exchange) -> exchanges.Exchange:
-    return _get_exchanges().get(exchange.connector.client.name.lower(), exchanges.Exchange)(exchange)
+    # use ccxt exchange id to find exchanges (ex kucoinfutures: id: kucoinfutures, name: "Kucoin Futures")
+    return _get_exchanges().get(exchange.connector.client.id.lower(), exchanges.Exchange)(exchange)
 
 
 def is_sponsoring(exchange_name) -> bool:
     return _get_exchanges().get(exchange_name.lower(), exchanges.Exchange).is_sponsoring()
 
 
 def _get_exchanges() -> dict:
```

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/__init__.py` & `trading-backend-1.2.4/trading_backend/exchanges/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,19 +59,31 @@
 )
 
 from trading_backend.exchanges import phemex
 from trading_backend.exchanges.phemex import (
     Phemex
 )
 
+from trading_backend.exchanges import kucoin
+from trading_backend.exchanges.kucoin import (
+    Kucoin
+)
+
+from trading_backend.exchanges import kucoinfutures
+from trading_backend.exchanges.kucoinfutures import (
+    KucoinFutures
+)
+
 __all__ = [
     "Exchange",
     "Binance",
     "Bybit",
     "OKX",
     "Ascendex",
     "GateIO",
     "Huobi",
     "HuobiPro",
     "Bitget",
     "Phemex",
+    "Kucoin",
+    "KucoinFutures",
 ]
```

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/ascendex.py` & `trading-backend-1.2.4/trading_backend/exchanges/ascendex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/binance.py` & `trading-backend-1.2.4/trading_backend/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/bitget.py` & `trading-backend-1.2.4/trading_backend/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/bybit.py` & `trading-backend-1.2.4/trading_backend/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/exchange.py` & `trading-backend-1.2.4/trading_backend/exchanges/exchange.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/gateio.py` & `trading-backend-1.2.4/trading_backend/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/huobi.py` & `trading-backend-1.2.4/trading_backend/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/huobipro.py` & `trading-backend-1.2.4/trading_backend/exchanges/huobipro.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/okx.py` & `trading-backend-1.2.4/trading_backend/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend/exchanges/phemex.py` & `trading-backend-1.2.4/trading_backend/exchanges/phemex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.3/trading_backend.egg-info/PKG-INFO` & `trading-backend-1.2.4/trading_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.3
+Version: 1.2.4
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.3](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.4](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.3/trading_backend.egg-info/SOURCES.txt` & `trading-backend-1.2.4/trading_backend.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 tests/exchanges/test_binance.py
 tests/exchanges/test_bitget.py
 tests/exchanges/test_bybit.py
 tests/exchanges/test_exchange.py
 tests/exchanges/test_gateio.py
 tests/exchanges/test_huobi.py
 tests/exchanges/test_huobipro.py
+tests/exchanges/test_kucoin.py
+tests/exchanges/test_kucoin_futures.py
 tests/exchanges/test_okx.py
 tests/exchanges/test_phemex.py
 tests/util/__init__.py
 tests/util/create_order_tests.py
 trading_backend/__init__.py
 trading_backend/errors.py
 trading_backend/exchange_factory.py
@@ -32,9 +34,11 @@
 trading_backend/exchanges/binance.py
 trading_backend/exchanges/bitget.py
 trading_backend/exchanges/bybit.py
 trading_backend/exchanges/exchange.py
 trading_backend/exchanges/gateio.py
 trading_backend/exchanges/huobi.py
 trading_backend/exchanges/huobipro.py
+trading_backend/exchanges/kucoin.py
+trading_backend/exchanges/kucoinfutures.py
 trading_backend/exchanges/okx.py
 trading_backend/exchanges/phemex.py
```

