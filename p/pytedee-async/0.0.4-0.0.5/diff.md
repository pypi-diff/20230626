# Comparing `tmp/pytedee_async-0.0.4.tar.gz` & `tmp/pytedee_async-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedee_async-0.0.4.tar", last modified: Sun Jun 25 18:50:01 2023, max compression
+gzip compressed data, was "pytedee_async-0.0.5.tar", last modified: Mon Jun 26 06:32:39 2023, max compression
```

## Comparing `pytedee_async-0.0.4.tar` & `pytedee_async-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:50:01.137050 pytedee_async-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-25 18:49:47.000000 pytedee_async-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-25 18:50:01.137050 pytedee_async-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-25 18:49:47.000000 pytedee_async-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:50:01.133049 pytedee_async-0.0.4/pytedee_async/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-25 18:49:47.000000 pytedee_async-0.0.4/pytedee_async/Lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-06-25 18:49:47.000000 pytedee_async-0.0.4/pytedee_async/TedeeClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-25 18:49:47.000000 pytedee_async-0.0.4/pytedee_async/TedeeClientException.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-25 18:49:47.000000 pytedee_async-0.0.4/pytedee_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-25 18:49:47.000000 pytedee_async-0.0.4/pytedee_async/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:50:01.137050 pytedee_async-0.0.4/pytedee_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-25 18:50:01.000000 pytedee_async-0.0.4/pytedee_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-25 18:50:01.000000 pytedee_async-0.0.4/pytedee_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:50:01.000000 pytedee_async-0.0.4/pytedee_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 18:50:01.000000 pytedee_async-0.0.4/pytedee_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 18:50:01.000000 pytedee_async-0.0.4/pytedee_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 18:50:01.137050 pytedee_async-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-25 18:49:47.000000 pytedee_async-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/pytedee_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/Lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/TedeeClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/TedeeClientException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/pytedee_async/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/pytedee_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 06:32:39.000000 pytedee_async-0.0.5/pytedee_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:32:39.530075 pytedee_async-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 06:32:21.000000 pytedee_async-0.0.5/setup.py
```

### Comparing `pytedee_async-0.0.4/LICENSE` & `pytedee_async-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.4/PKG-INFO` & `pytedee_async-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pytedee_async
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Tedee Lock Client package
-Home-page: https://github.com/zweckj/pytedee
+Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytedee_async-0.0.4/README.md` & `pytedee_async-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.4/pytedee_async/Lock.py` & `pytedee_async-0.0.5/pytedee_async/Lock.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.4/pytedee_async/TedeeClient.py` & `pytedee_async-0.0.5/pytedee_async/TedeeClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,19 @@
         
 
     @classmethod
     async def create(cls, personalToken, timeout=TIMEOUT):
         self = cls(personalToken, timeout)
         await self.get_devices()
         return self
+    
+    @property
+    def locks(self):
+        '''Return a list of locks'''
+        return self._sensor_list
 
     async def get_devices(self):
         '''Get the list of registered locks'''
 
         async with aiohttp.ClientSession(
                 headers=self._api_header, 
                 timeout=aiohttp.ClientTimeout(total=self._timeout)
@@ -65,18 +70,14 @@
                         '''store the found lock in _sensor_list and get the battery_level'''
 
                         self._sensor_list.append(lock)
 
                     if self._lock_id == None:
                         raise TedeeClientException("No lock found")
     
-    def get_locks(self):
-        '''Return a list of locks'''
-        return self._sensor_list
-    
     # unlocking
     async def unlock(self, id):
         '''Unlock method'''
         lock = self.find_lock(id)
         url = API_URL_LOCK + str(id) + API_PATH_UNLOCK
         async with aiohttp.ClientSession(
                 headers=self._api_header,
```

### Comparing `pytedee_async-0.0.4/pytedee_async.egg-info/PKG-INFO` & `pytedee_async-0.0.5/pytedee_async.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pytedee-async
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Tedee Lock Client package
-Home-page: https://github.com/zweckj/pytedee
+Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytedee_async-0.0.4/setup.py` & `pytedee_async-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytedee_async", 
-    version="0.0.4",
+    version="0.0.5",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     description="A Tedee Lock Client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/zweckj/pytedee",
+    url="https://github.com/zweckj/pytedee_async",
     packages=setuptools.find_packages(),
     install_requires=['aiohttp', 'asyncio'],
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
```

