# Comparing `tmp/meo-0.1.4.tar.gz` & `tmp/meo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meo-0.1.4.tar", last modified: Sun Jun 25 19:28:03 2023, max compression
+gzip compressed data, was "meo-0.1.5.tar", last modified: Mon Jun 26 07:34:16 2023, max compression
```

## Comparing `meo-0.1.4.tar` & `meo-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 19:28:03.225998 meo-0.1.4/
--rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.4/LICENSE
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-25 19:28:03.225998 meo-0.1.4/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.4/README.md
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 19:28:03.225998 meo-0.1.4/meo/
--rw-r--r--   0 meo       (1000) meo       (1000)      114 2023-06-24 12:18:03.000000 meo-0.1.4/meo/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      302 2023-06-25 17:49:23.000000 meo-0.1.4/meo/__version__.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 19:28:03.225998 meo-0.1.4/meo/crack/
--rw-r--r--   0 meo       (1000) meo       (1000)      237 2023-06-25 19:24:28.000000 meo-0.1.4/meo/crack/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)     4787 2023-06-25 18:58:10.000000 meo-0.1.4/meo/crack/cracker.py
--rw-r--r--   0 meo       (1000) meo       (1000)      853 2023-06-25 19:02:15.000000 meo-0.1.4/meo/crack/pdf.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1076 2023-06-25 18:55:02.000000 meo-0.1.4/meo/crack/utils.py
--rw-r--r--   0 meo       (1000) meo       (1000)      937 2023-06-25 19:19:50.000000 meo-0.1.4/meo/crack/zip.py
--rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.4/meo/flask.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2428 2023-06-25 15:23:35.000000 meo-0.1.4/meo/io.py
--rw-r--r--   0 meo       (1000) meo       (1000)      823 2023-06-24 12:10:37.000000 meo-0.1.4/meo/net.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.4/meo/screen.py
--rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.4/meo/utils.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 19:28:03.225998 meo-0.1.4/meo.egg-info/
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-25 19:28:03.000000 meo-0.1.4/meo.egg-info/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      401 2023-06-25 19:28:03.000000 meo-0.1.4/meo.egg-info/SOURCES.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-25 19:28:03.000000 meo-0.1.4/meo.egg-info/dependency_links.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       27 2023-06-25 19:28:03.000000 meo-0.1.4/meo.egg-info/requires.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-25 19:28:03.000000 meo-0.1.4/meo.egg-info/top_level.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-25 19:28:03.225998 meo-0.1.4/setup.cfg
--rwxr-xr-x   0 meo       (1000) meo       (1000)     1361 2023-06-25 17:49:51.000000 meo-0.1.4/setup.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-25 19:28:03.225998 meo-0.1.4/test/
--rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-24 10:57:51.000000 meo-0.1.4/test/test.py
--rw-r--r--   0 meo       (1000) meo       (1000)      355 2023-06-25 19:27:38.000000 meo-0.1.4/test/test_crack.py
--rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-25 19:16:03.000000 meo-0.1.4/test/test_imp.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.606138 meo-0.1.5/
+-rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.5/LICENSE
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-26 07:34:16.606138 meo-0.1.5/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.5/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.602805 meo-0.1.5/meo/
+-rw-r--r--   0 meo       (1000) meo       (1000)      134 2023-06-26 06:49:06.000000 meo-0.1.5/meo/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      302 2023-06-26 07:34:02.000000 meo-0.1.5/meo/__version__.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.602805 meo-0.1.5/meo/crack/
+-rw-r--r--   0 meo       (1000) meo       (1000)      237 2023-06-26 07:10:23.000000 meo-0.1.5/meo/crack/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     4833 2023-06-26 06:40:46.000000 meo-0.1.5/meo/crack/cracker.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      749 2023-06-26 07:31:01.000000 meo-0.1.5/meo/crack/pdf.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1076 2023-06-25 19:31:21.000000 meo-0.1.5/meo/crack/utils.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      985 2023-06-26 07:29:34.000000 meo-0.1.5/meo/crack/zip.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.5/meo/flask.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2671 2023-06-26 07:24:35.000000 meo-0.1.5/meo/io.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      823 2023-06-24 12:10:37.000000 meo-0.1.5/meo/net.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.5/meo/screen.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.5/meo/utils.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      332 2023-06-26 06:59:04.000000 meo-0.1.5/meo/wapper.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.602805 meo-0.1.5/meo.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      415 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       27 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/requires.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-26 07:34:16.000000 meo-0.1.5/meo.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-26 07:34:16.606138 meo-0.1.5/setup.cfg
+-rwxr-xr-x   0 meo       (1000) meo       (1000)     1361 2023-06-25 19:31:21.000000 meo-0.1.5/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-26 07:34:16.602805 meo-0.1.5/test/
+-rw-r--r--   0 meo       (1000) meo       (1000)      310 2023-06-26 07:30:54.000000 meo-0.1.5/test/test.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      355 2023-06-25 19:31:21.000000 meo-0.1.5/test/test_crack.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-25 19:31:21.000000 meo-0.1.5/test/test_imp.py
```

### Comparing `meo-0.1.4/LICENSE` & `meo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meo-0.1.4/PKG-INFO` & `meo-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.4
+Version: 0.1.5
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.4/meo/crack/cracker.py` & `meo-0.1.5/meo/crack/cracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import multiprocessing
 import gc
+import os
 from .utils import *
 from tqdm.asyncio import tqdm
 import itertools
 import asyncio
 
 class Cracker:
     
     def __init__(self, path: str) -> None:
+        assert os.path.exists(path)
         self.path = path
 
     def in_multiprocess_by_seed(self, seed=PWD_SEED_COMPLEX, min_length=None, max_length=None, n_processes=8, slice_size=500, progressbar=False):
         pool = multiprocessing.Pool(n_processes)
         it = key_generator(seed, min_length, max_length)
         manager = multiprocessing.Manager()
         info = manager.dict()
```

### Comparing `meo-0.1.4/meo/crack/utils.py` & `meo-0.1.5/meo/crack/utils.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.4/meo/flask.py` & `meo-0.1.5/meo/flask.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.4/meo/io.py` & `meo-0.1.5/meo/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,23 +50,32 @@
     '''read file auto-closed'''
     with open(path, 'rb') as _f:
         content = _f.read()
     if encoding is None:
         return content
     return content.decode(encoding=encoding)
 
-def auto_decode(_bytes: bytes):
+def decode(_bytes: bytes):
     """decide encoding and decode `_bytes`"""
     assert isinstance(_bytes, bytes)
     for encoding in ["utf8", 'gbk', 'utf16', 'utf32']:
         try:
             return _bytes.decode(encoding)
         except: pass
     raise ValueError("bytes must be {utf8, gbk, utf16, utf32}")
 
+def encode(string: str):
+    assert isinstance(string, str)
+    for enc in ["utf8", 'gbk', 'utf16', 'utf32']:
+        try:
+            return string.encode(enc)
+        except: pass
+    raise ValueError("bytes must be {utf8, gbk, utf16, utf32}")
+
+
 def cat(*path):
     file_bytes = bytes()
     for p in path:
         if os.path.isfile(p):
             file_bytes += load_file(p)
         else:
             raise ValueError(f"{p} is not a file")
```

### Comparing `meo-0.1.4/meo/net.py` & `meo-0.1.5/meo/net.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.4/meo/screen.py` & `meo-0.1.5/meo/screen.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.4/meo.egg-info/PKG-INFO` & `meo-0.1.5/meo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.4
+Version: 0.1.5
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.4/setup.py` & `meo-0.1.5/setup.py`

 * *Files identical despite different names*

