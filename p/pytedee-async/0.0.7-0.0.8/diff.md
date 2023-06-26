# Comparing `tmp/pytedee_async-0.0.7.tar.gz` & `tmp/pytedee_async-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedee_async-0.0.7.tar", last modified: Mon Jun 26 10:00:16 2023, max compression
+gzip compressed data, was "pytedee_async-0.0.8.tar", last modified: Mon Jun 26 10:33:15 2023, max compression
```

## Comparing `pytedee_async-0.0.7.tar` & `pytedee_async-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/pytedee_async/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/Lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/TedeeClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/TedeeClientException.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/pytedee_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:33:15.279839 pytedee_async-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 10:33:15.275839 pytedee_async-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:33:15.275839 pytedee_async-0.0.8/pytedee_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/Lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/TedeeClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/TedeeClientException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:33:15.275839 pytedee_async-0.0.8/pytedee_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:33:15.279839 pytedee_async-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/setup.py
```

### Comparing `pytedee_async-0.0.7/LICENSE` & `pytedee_async-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.7/PKG-INFO` & `pytedee_async-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee_async
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.0.7/README.md` & `pytedee_async-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.7/pytedee_async/Lock.py` & `pytedee_async-0.0.8/pytedee_async/Lock.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.7/pytedee_async/TedeeClient.py` & `pytedee_async-0.0.8/pytedee_async/TedeeClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,21 +148,19 @@
             ) as session:
             async with session.get(url) as response:
                 if response.status == 200:
                     r = await response.json()
                     _LOGGER.debug("result: %s", r)
                     result = r["result"]
                     try:
-                        success = result["success"]
-                        if success:
-                            for lock in self._sensor_list:
-                                if id == lock.id:
-                                    lock.battery_level = result["level"]
-                                    _LOGGER.debug("id: %d, battery level: %d", id, lock.battery_level)
-                        return success
+                        for lock in self._sensor_list:
+                            if id == lock.id:
+                                lock.battery_level = result["level"]
+                                _LOGGER.debug("id: %d, battery level: %d", id, lock.battery_level)
+                        return True
                     except KeyError:
                         _LOGGER.error("result: %s", result)
                         return False
             
     async def get_state(self):
         async with aiohttp.ClientSession(
                 headers=self._api_header,
```

### Comparing `pytedee_async-0.0.7/pytedee_async.egg-info/PKG-INFO` & `pytedee_async-0.0.8/pytedee_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee-async
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.0.7/setup.py` & `pytedee_async-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytedee_async", 
-    version="0.0.7",
+    version="0.0.8",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     description="A Tedee Lock Client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pytedee_async",
     packages=setuptools.find_packages(),
```

