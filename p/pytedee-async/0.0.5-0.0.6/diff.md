# Comparing `tmp/pytedee_async-0.0.5.tar.gz` & `tmp/pytedee_async-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedee_async-0.0.5.tar", last modified: Mon Jun 26 06:32:39 2023, max compression
+gzip compressed data, was "pytedee_async-0.0.6.tar", last modified: Mon Jun 26 09:55:44 2023, max compression
```

## Comparing `pytedee_async-0.0.5.tar` & `pytedee_async-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/pytedee_async/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/Lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/TedeeClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/TedeeClientException.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/pytedee_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:44.754165 pytedee_async-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 09:55:44.754165 pytedee_async-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:44.750164 pytedee_async-0.0.6/pytedee_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/Lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/TedeeClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/TedeeClientException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:44.754165 pytedee_async-0.0.6/pytedee_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:55:44.754165 pytedee_async-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/setup.py
```

### Comparing `pytedee_async-0.0.5/LICENSE` & `pytedee_async-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.5/PKG-INFO` & `pytedee_async-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee_async
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.0.5/README.md` & `pytedee_async-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.5/pytedee_async/Lock.py` & `pytedee_async-0.0.6/pytedee_async/Lock.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,34 +18,39 @@
 
     
 class Lock(object):
     '''
     classdocs
     '''
 
-    def __init__(self, name, id):
+    def __init__(self, name, id, type):
         '''
         Constructor
         '''
         self._name = name
         self._id = id
+        self._type = type
         self._state = 0
         self._battery_level = None
         self._is_connected = False
         self._is_charging = False
         
     @property
     def name(self):
         return self._name
     
     @property
     def id(self):
         return self._id
     
     @property
+    def type(self):
+        return self._type
+    
+    @property
     def is_state_locked(self):
         return self._state == 6
     
     @property
     def is_state_unlocked(self):
         return self._state == 2
```

### Comparing `pytedee_async-0.0.5/pytedee_async/TedeeClient.py` & `pytedee_async-0.0.6/pytedee_async/TedeeClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,16 @@
                     r = await response.json()
                     _LOGGER.debug("Locks %s", r)
                     result = r["result"]
 
                     for x in result:            
                         id = x["id"]
                         name = x["name"]
-                        lock = Lock(name, id)
+                        type = x["type"]
+                        lock = Lock(name, id, type)
 
                         lock.connected, lock.state, lock.battery_level, lock.is_charging = self.parse_lock_properties(x) 
                         lock.is_enabled_pullspring, lock.duration_pullspring = self.parse_pull_spring_settings(x)
                         
                         self._lock_id = id
                         '''store the found lock in _sensor_list and get the battery_level'''
```

### Comparing `pytedee_async-0.0.5/pytedee_async.egg-info/PKG-INFO` & `pytedee_async-0.0.6/pytedee_async.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee-async
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.0.5/setup.py` & `pytedee_async-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytedee_async", 
-    version="0.0.5",
+    version="0.0.6",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     description="A Tedee Lock Client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pytedee_async",
     packages=setuptools.find_packages(),
```

