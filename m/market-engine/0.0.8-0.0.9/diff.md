# Comparing `tmp/market-engine-0.0.8.tar.gz` & `tmp/market-engine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.0.8.tar", last modified: Thu Jun 15 00:40:55 2023, max compression
+gzip compressed data, was "market-engine-0.0.9.tar", last modified: Thu Jun 15 00:44:59 2023, max compression
```

## Comparing `market-engine-0.0.8.tar` & `market-engine-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 00:40:55.825845 market-engine-0.0.8/
--rw-rw-rw-   0        0        0      216 2023-06-15 00:40:55.825845 market-engine-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 00:40:55.821367 market-engine-0.0.8/market_engine/
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.8/market_engine/__init__.py
--rw-rw-rw-   0        0        0      932 2023-05-26 19:30:35.000000 market-engine-0.0.8/market_engine/common.py
-drwxrwxrwx   0        0        0        0 2023-06-15 00:40:55.824846 market-engine-0.0.8/market_engine/modules/
--rw-rw-rw-   0        0        0    13832 2023-06-15 00:40:37.000000 market-engine-0.0.8/market_engine/modules/MarketAPI.py
--rw-rw-rw-   0        0        0     6661 2023-06-14 23:56:00.000000 market-engine-0.0.8/market_engine/modules/MarketDB.py
--rw-rw-rw-   0        0        0    15103 2023-06-15 00:38:10.000000 market-engine-0.0.8/market_engine/modules/MarketData.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.8/market_engine/modules/__init__.py
--rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.8/market_engine/modules/categories.py
-drwxrwxrwx   0        0        0        0 2023-06-15 00:40:55.823334 market-engine-0.0.8/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-06-15 00:40:55.000000 market-engine-0.0.8/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-06-15 00:40:55.000000 market-engine-0.0.8/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 00:40:55.000000 market-engine-0.0.8/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-15 00:40:55.000000 market-engine-0.0.8/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-15 00:40:55.000000 market-engine-0.0.8/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 00:40:55.825845 market-engine-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-06-15 00:40:42.000000 market-engine-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:44:59.728463 market-engine-0.0.9/
+-rw-rw-rw-   0        0        0      216 2023-06-15 00:44:59.728463 market-engine-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 00:44:59.723464 market-engine-0.0.9/market_engine/
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.9/market_engine/__init__.py
+-rw-rw-rw-   0        0        0      932 2023-05-26 19:30:35.000000 market-engine-0.0.9/market_engine/common.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:44:59.728463 market-engine-0.0.9/market_engine/modules/
+-rw-rw-rw-   0        0        0    13903 2023-06-15 00:44:05.000000 market-engine-0.0.9/market_engine/modules/MarketAPI.py
+-rw-rw-rw-   0        0        0     6661 2023-06-14 23:56:00.000000 market-engine-0.0.9/market_engine/modules/MarketDB.py
+-rw-rw-rw-   0        0        0    15103 2023-06-15 00:38:10.000000 market-engine-0.0.9/market_engine/modules/MarketData.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.9/market_engine/modules/__init__.py
+-rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.9/market_engine/modules/categories.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:44:59.726464 market-engine-0.0.9/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 00:44:59.728463 market-engine-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-06-15 00:44:54.000000 market-engine-0.0.9/setup.py
```

### Comparing `market-engine-0.0.8/market_engine/common.py` & `market-engine-0.0.9/market_engine/common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.8/market_engine/modules/MarketAPI.py` & `market-engine-0.0.9/market_engine/modules/MarketAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,17 @@
             urls.add(link)
 
     return urls
 
 
 def get_saved_data():
     saved_data = set()
+    if not os.path.exists("output"):
+        os.makedirs("output")
+
     for file in os.listdir("output"):
         if file.endswith(".json"):
             saved_data.add(file)
 
     return saved_data
```

### Comparing `market-engine-0.0.8/market_engine/modules/MarketDB.py` & `market-engine-0.0.9/market_engine/modules/MarketDB.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.8/market_engine/modules/MarketData.py` & `market-engine-0.0.9/market_engine/modules/MarketData.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.8/market_engine/modules/categories.py` & `market-engine-0.0.9/market_engine/modules/categories.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.8/setup.py` & `market-engine-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.0.8',
+    version='0.0.9',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
```

