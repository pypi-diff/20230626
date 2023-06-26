# Comparing `tmp/breeze_strategies-1.0.3.tar.gz` & `tmp/breeze_strategies-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-1.0.3.tar", last modified: Mon Jun 26 08:39:38 2023, max compression
+gzip compressed data, was "breeze_strategies-1.0.4.tar", last modified: Mon Jun 26 08:41:41 2023, max compression
```

## Comparing `breeze_strategies-1.0.3.tar` & `breeze_strategies-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 08:39:38.847836 breeze_strategies-1.0.3/
--rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1523 2023-06-26 08:39:38.844570 breeze_strategies-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      972 2023-06-26 08:38:46.000000 breeze_strategies-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 08:39:38.759050 breeze_strategies-1.0.3/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.3/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    20393 2023-06-23 09:58:39.000000 breeze_strategies-1.0.3/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:39:38.832950 breeze_strategies-1.0.3/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1523 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-26 08:39:38.000000 breeze_strategies-1.0.3/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 08:39:38.849846 breeze_strategies-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-26 08:38:55.000000 breeze_strategies-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:41:41.016701 breeze_strategies-1.0.4/
+-rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1543 2023-06-26 08:41:41.013174 breeze_strategies-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      992 2023-06-26 08:41:27.000000 breeze_strategies-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 08:41:40.973175 breeze_strategies-1.0.4/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.4/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    20393 2023-06-23 09:58:39.000000 breeze_strategies-1.0.4/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:41:41.010174 breeze_strategies-1.0.4/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1543 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-26 08:41:40.000000 breeze_strategies-1.0.4/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 08:41:41.017697 breeze_strategies-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-26 08:41:36.000000 breeze_strategies-1.0.4/setup.py
```

### Comparing `breeze_strategies-1.0.3/LICENSE` & `breeze_strategies-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-1.0.3/PKG-INFO` & `breeze_strategies-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 1.0.3
+Version: 1.0.4
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,21 +17,25 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.3
+pip install breeze_strategies==1.0.4
 
 ```
 
 ## Updating Library
+
+```python
+
 pip install --upgrade breeze_strategies
 
+```
 
 ## code usage
 
 ```python
 
 #Import the library
 from breeze_strategies import Strategies
```

### Comparing `breeze_strategies-1.0.3/README.md` & `breeze_strategies-1.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.3
+pip install breeze_strategies==1.0.4
 
 ```
 
 ## Updating Library
+
+```python
+
 pip install --upgrade breeze_strategies
 
+```
 
 ## code usage
 
 ```python
 
 #Import the library
 from breeze_strategies import Strategies
```

### Comparing `breeze_strategies-1.0.3/breeze_strategies/breeze_strategies.py` & `breeze_strategies-1.0.4/breeze_strategies/breeze_strategies.py`

 * *Files identical despite different names*

### Comparing `breeze_strategies-1.0.3/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-1.0.4/breeze_strategies.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 1.0.3
+Version: 1.0.4
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,21 +17,25 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.3
+pip install breeze_strategies==1.0.4
 
 ```
 
 ## Updating Library
+
+```python
+
 pip install --upgrade breeze_strategies
 
+```
 
 ## code usage
 
 ```python
 
 #Import the library
 from breeze_strategies import Strategies
```

### Comparing `breeze_strategies-1.0.3/setup.py` & `breeze_strategies-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="1.0.3",
+    version="1.0.4",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

