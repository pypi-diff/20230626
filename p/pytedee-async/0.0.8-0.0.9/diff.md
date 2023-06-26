# Comparing `tmp/pytedee_async-0.0.8.tar.gz` & `tmp/pytedee_async-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedee_async-0.0.8.tar", last modified: Mon Jun 26 10:33:15 2023, max compression
+gzip compressed data, was "pytedee_async-0.0.9.tar", last modified: Mon Jun 26 13:56:01 2023, max compression
```

## Comparing `pytedee_async-0.0.8.tar` & `pytedee_async-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:33:15.279839 pytedee_async-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 10:33:15.275839 pytedee_async-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:33:15.275839 pytedee_async-0.0.8/pytedee_async/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/Lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/TedeeClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/TedeeClientException.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/pytedee_async/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:33:15.275839 pytedee_async-0.0.8/pytedee_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 10:33:15.000000 pytedee_async-0.0.8/pytedee_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:33:15.279839 pytedee_async-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 10:33:00.000000 pytedee_async-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:56:01.424185 pytedee_async-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 13:55:47.000000 pytedee_async-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 13:56:01.424185 pytedee_async-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 13:55:47.000000 pytedee_async-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:56:01.424185 pytedee_async-0.0.9/pytedee_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-26 13:55:47.000000 pytedee_async-0.0.9/pytedee_async/Lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-06-26 13:55:47.000000 pytedee_async-0.0.9/pytedee_async/TedeeClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 13:55:47.000000 pytedee_async-0.0.9/pytedee_async/TedeeClientException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 13:55:47.000000 pytedee_async-0.0.9/pytedee_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 13:55:47.000000 pytedee_async-0.0.9/pytedee_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-26 13:55:47.000000 pytedee_async-0.0.9/pytedee_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:56:01.424185 pytedee_async-0.0.9/pytedee_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 13:56:01.000000 pytedee_async-0.0.9/pytedee_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 13:56:01.000000 pytedee_async-0.0.9/pytedee_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:56:01.000000 pytedee_async-0.0.9/pytedee_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 13:56:01.000000 pytedee_async-0.0.9/pytedee_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 13:56:01.000000 pytedee_async-0.0.9/pytedee_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:56:01.424185 pytedee_async-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 13:55:47.000000 pytedee_async-0.0.9/setup.py
```

### Comparing `pytedee_async-0.0.8/LICENSE` & `pytedee_async-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.8/PKG-INFO` & `pytedee_async-0.0.9/pytedee_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytedee_async
-Version: 0.0.8
+Name: pytedee-async
+Version: 0.0.9
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.0.8/README.md` & `pytedee_async-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.8/pytedee_async/Lock.py` & `pytedee_async-0.0.9/pytedee_async/Lock.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.8/pytedee_async/TedeeClient.py` & `pytedee_async-0.0.9/pytedee_async/TedeeClient.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,24 +2,19 @@
 Created on 01.11.2020
 
 @author: joerg.wolff@gmx.de
 '''
 import logging
 import aiohttp
 import asyncio
-from threading import Timer
 
 from .const import *
+from .Lock import Lock
+from .TedeeClientException import *
 
-try:
-    from .Lock import Lock
-    from .TedeeClientException import TedeeClientException
-except:
-    from Lock import Lock
-    from TedeeClientException import TedeeClientException
 
 _LOGGER = logging.getLogger(__name__)
     
 class TedeeClient(object):
     '''Classdocs'''
 
     def __init__(self, personalToken, timeout):
@@ -70,14 +65,18 @@
                         self._lock_id = id
                         '''store the found lock in _sensor_list and get the battery_level'''
 
                         self._sensor_list.append(lock)
 
                     if self._lock_id == None:
                         raise TedeeClientException("No lock found")
+                elif response.status == 401:
+                    raise TedeeAuthException()
+                else:
+                    raise TedeeClientException(f"Error during listing of devices. Status code {response.status}")
     
     # unlocking
     async def unlock(self, id):
         '''Unlock method'''
         lock = self.find_lock(id)
         url = API_URL_LOCK + str(id) + API_PATH_UNLOCK
         async with aiohttp.ClientSession(
@@ -87,14 +86,18 @@
             async with session.post(url) as response:
                 if response.status == 202:
                     lock.state = 4
                     _LOGGER.debug("unlock command successful, id: %d ", id)
                     await asyncio.sleep(UNLOCK_DELAY)
                     lock.state = 2
                     await self.get_state()
+                elif response.status == 401:
+                    raise TedeeAuthException()
+                else:
+                    raise TedeeClientException(f"Error during unlocking of lock {id}. Status code {response.status}")
             
     # locking
     async def lock(self, id):
         ''''Lock method'''
         lock = self.find_lock(id)
 
         url = API_URL_LOCK + str(id) + API_PATH_LOCK
@@ -105,14 +108,18 @@
             async with session.post(url) as response:
                 if response.status == 202:
                     lock.state = 5
                     _LOGGER.debug("lock command successful, id: %d ", id)
                     await asyncio.sleep(LOCK_DELAY)
                     lock.state = 6
                     await self.get_state()
+                elif response.status == 401:
+                    raise TedeeAuthException()
+                else:
+                    raise TedeeClientException(f"Error during locking of lock {id}. Status code {response.status}")
 
     # pulling  
     async def open(self, id):
         '''Open the door latch'''
         lock = self.find_lock(id)
 
         url = API_URL_LOCK + str(id) + API_PATH_PULL
@@ -125,14 +132,18 @@
                 
                 if response.status == 202:
                     lock.state = 7
                     _LOGGER.debug("open command successful, id: %d ", id)
 
                     await asyncio.sleep(lock.duration_pullspring + 1)
                     await self.get_state()
+                elif response.status == 401:
+                    raise TedeeAuthException()
+                else: 
+                    raise TedeeClientException(f"Error during unlatching of lock {id}. Status code {response.status}")
 
     def is_unlocked(self, id):
         lock = self.find_lock(id)
         return lock.state == 2
     
     def is_locked(self, id):
         lock = self.find_lock(id)
@@ -156,14 +167,16 @@
                             if id == lock.id:
                                 lock.battery_level = result["level"]
                                 _LOGGER.debug("id: %d, battery level: %d", id, lock.battery_level)
                         return True
                     except KeyError:
                         _LOGGER.error("result: %s", result)
                         return False
+                elif response.status == 401:
+                    raise TedeeAuthException()
             
     async def get_state(self):
         async with aiohttp.ClientSession(
                 headers=self._api_header, 
                 timeout=aiohttp.ClientTimeout(total=self._timeout)
             ) as session:
             async with session.get(API_URL_STATE) as response:
@@ -178,14 +191,18 @@
                                 if id == lock.id:
 
                                     lock.connected, lock.state, lock.battery_level, lock.is_charging = self.parse_lock_properties(state)
                                     _LOGGER.debug("Id: %s, State: %d, battery: %d", lock.state, lock.is_charging, lock.battery_level)
                                     break
                     except KeyError:
                         _LOGGER.error("result: %s", r.json())
+                elif response.status == 401:
+                    raise TedeeAuthException()
+                else:
+                    raise TedeeClientException(f"Error during getting state. Status code {response.status}")
 
     def parse_lock_properties(self, state: dict):
         if state["isConnected"]:
             connected = state["isConnected"]
         else:
             connected = False
 
@@ -225,8 +242,8 @@
         for lock in self._sensor_list:
             if id == lock.id:
                 return lock
         raise TedeeClientException("This Id not found")
 
     async def update(self, id):
         await self.get_state()
-        return await self.get_battery(id)
+        return await self.get_battery(id)
```

### Comparing `pytedee_async-0.0.8/pytedee_async.egg-info/PKG-INFO` & `pytedee_async-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytedee-async
-Version: 0.0.8
+Name: pytedee_async
+Version: 0.0.9
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.0.8/setup.py` & `pytedee_async-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytedee_async", 
-    version="0.0.8",
+    version="0.0.9",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     description="A Tedee Lock Client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pytedee_async",
     packages=setuptools.find_packages(),
```

