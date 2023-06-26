# Comparing `tmp/breeze_strategies-1.0.2.tar.gz` & `tmp/breeze_strategies-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-1.0.2.tar", last modified: Fri Jun 23 09:59:08 2023, max compression
+gzip compressed data, was "breeze_strategies-1.0.3.tar", last modified: Mon Jun 26 08:39:38 2023, max compression
```

## Comparing `breeze_strategies-1.0.2.tar` & `breeze_strategies-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:59:08.385920 breeze_strategies-1.0.2/
--rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1292 2023-06-23 09:59:08.382919 breeze_strategies-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-06-23 09:59:00.000000 breeze_strategies-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 09:59:08.351607 breeze_strategies-1.0.2/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.2/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    20393 2023-06-23 09:58:39.000000 breeze_strategies-1.0.2/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:59:08.380926 breeze_strategies-1.0.2/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1292 2023-06-23 09:59:08.000000 breeze_strategies-1.0.2/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-23 09:59:08.000000 breeze_strategies-1.0.2/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:59:08.000000 breeze_strategies-1.0.2/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-23 09:59:08.000000 breeze_strategies-1.0.2/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-23 09:59:08.000000 breeze_strategies-1.0.2/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 09:59:08.389926 breeze_strategies-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-23 09:58:48.000000 breeze_strategies-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:39:38.847836 breeze_strategies-1.0.3/
+-rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1523 2023-06-26 08:39:38.844570 breeze_strategies-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      972 2023-06-26 08:38:46.000000 breeze_strategies-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 08:39:38.759050 breeze_strategies-1.0.3/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.3/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    20393 2023-06-23 09:58:39.000000 breeze_strategies-1.0.3/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:39:38.832950 breeze_strategies-1.0.3/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1523 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 08:39:38.849846 breeze_strategies-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-26 08:38:55.000000 breeze_strategies-1.0.3/setup.py
```

### Comparing `breeze_strategies-1.0.2/LICENSE` & `breeze_strategies-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-1.0.2/PKG-INFO` & `breeze_strategies-1.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 1.0.2
+Version: 1.0.3
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,31 +17,48 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.2
+pip install breeze_strategies==1.0.3
 
 ```
 
+## Updating Library
+pip install --upgrade breeze_strategies
+
 
 ## code usage
 
 ```python
 
+#Import the library
 from breeze_strategies import Strategies
 
+#Configure the strategy using API Keys and set stoploss/takeprofit level.
+obj = Strategies(app_key = "your app key",
+                 secret_key = "your secret key",
+                 api_session = "your api session",
+                 max_profit = "your max profit",
+                 max_loss = "your max loss")
+
+#Execute the strategy
+obj.straddle(strategy_type = "long",
+             stock_code = "NIFTY",
+             strike_price = "18700",
+             quantity = "50",
+             expiry_date = "2023-06-29T06:00:00.000Z")
+
 
-obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
-obj.straddle(strategy_type = "long",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+#SquareOff existing positions and exit the strategy
+obj.stop() 
 
-obj.straddle(strategy_type = "short",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
 
-obj.stop() #for disconnection and exit of current strategy
+#Generate Profit & Loss report
 obj.get_pnl()
 
 ```
```

### Comparing `breeze_strategies-1.0.2/breeze_strategies/breeze_strategies.py` & `breeze_strategies-1.0.3/breeze_strategies/breeze_strategies.py`

 * *Files identical despite different names*

### Comparing `breeze_strategies-1.0.2/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-1.0.3/breeze_strategies.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 1.0.2
+Version: 1.0.3
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,31 +17,48 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.2
+pip install breeze_strategies==1.0.3
 
 ```
 
+## Updating Library
+pip install --upgrade breeze_strategies
+
 
 ## code usage
 
 ```python
 
+#Import the library
 from breeze_strategies import Strategies
 
+#Configure the strategy using API Keys and set stoploss/takeprofit level.
+obj = Strategies(app_key = "your app key",
+                 secret_key = "your secret key",
+                 api_session = "your api session",
+                 max_profit = "your max profit",
+                 max_loss = "your max loss")
+
+#Execute the strategy
+obj.straddle(strategy_type = "long",
+             stock_code = "NIFTY",
+             strike_price = "18700",
+             quantity = "50",
+             expiry_date = "2023-06-29T06:00:00.000Z")
+
 
-obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
-obj.straddle(strategy_type = "long",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+#SquareOff existing positions and exit the strategy
+obj.stop() 
 
-obj.straddle(strategy_type = "short",stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
 
-obj.stop() #for disconnection and exit of current strategy
+#Generate Profit & Loss report
 obj.get_pnl()
 
 ```
```

### Comparing `breeze_strategies-1.0.2/setup.py` & `breeze_strategies-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="1.0.2",
+    version="1.0.3",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

