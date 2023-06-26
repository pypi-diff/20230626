# Comparing `tmp/pytedee_async-0.0.6.tar.gz` & `tmp/pytedee_async-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedee_async-0.0.6.tar", last modified: Mon Jun 26 09:55:44 2023, max compression
+gzip compressed data, was "pytedee_async-0.0.7.tar", last modified: Mon Jun 26 10:00:16 2023, max compression
```

## Comparing `pytedee_async-0.0.6.tar` & `pytedee_async-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:44.754165 pytedee_async-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 09:55:44.754165 pytedee_async-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:44.750164 pytedee_async-0.0.6/pytedee_async/
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/Lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/TedeeClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/TedeeClientException.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/pytedee_async/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:44.754165 pytedee_async-0.0.6/pytedee_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 09:55:44.000000 pytedee_async-0.0.6/pytedee_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:55:44.754165 pytedee_async-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 09:55:26.000000 pytedee_async-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/pytedee_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/Lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/TedeeClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/TedeeClientException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/pytedee_async/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/pytedee_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 10:00:16.000000 pytedee_async-0.0.7/pytedee_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:00:16.387288 pytedee_async-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 09:59:58.000000 pytedee_async-0.0.7/setup.py
```

### Comparing `pytedee_async-0.0.6/LICENSE` & `pytedee_async-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.6/PKG-INFO` & `pytedee_async-0.0.7/pytedee_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytedee_async
-Version: 0.0.6
+Name: pytedee-async
+Version: 0.0.7
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.0.6/README.md` & `pytedee_async-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.6/pytedee_async/Lock.py` & `pytedee_async-0.0.7/pytedee_async/Lock.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,20 @@
     
     @property
     def id(self):
         return self._id
     
     @property
     def type(self):
-        return self._type
+        if self._type == 2:
+            return "Tedee Pro"
+        elif self._type == 4:
+            return "Tedee Go"
+        else:
+            return "Unknown Model"
     
     @property
     def is_state_locked(self):
         return self._state == 6
     
     @property
     def is_state_unlocked(self):
```

### Comparing `pytedee_async-0.0.6/pytedee_async/TedeeClient.py` & `pytedee_async-0.0.7/pytedee_async/TedeeClient.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.0.6/pytedee_async.egg-info/PKG-INFO` & `pytedee_async-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytedee-async
-Version: 0.0.6
+Name: pytedee_async
+Version: 0.0.7
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.0.6/setup.py` & `pytedee_async-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytedee_async", 
-    version="0.0.6",
+    version="0.0.7",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     description="A Tedee Lock Client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pytedee_async",
     packages=setuptools.find_packages(),
```

