# Comparing `tmp/upathlib-0.8.1.tar.gz` & `tmp/upathlib-0.8.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upathlib-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "upathlib-0.8.2b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `upathlib-0.8.1.tar` & `upathlib-0.8.2b1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.8.1/LICENSE
--rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.8.1/README.rst
--rw-r--r--   0        0        0     1699 2023-06-19 05:49:42.294835 upathlib-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2319 2023-06-19 05:51:44.254498 upathlib-0.8.1/src/upathlib/__init__.py
--rw-r--r--   0        0        0     4694 2023-04-20 04:34:46.179551 upathlib-0.8.1/src/upathlib/_blob.py
--rw-r--r--   0        0        0    10749 2023-05-13 05:38:06.231654 upathlib-0.8.1/src/upathlib/_local.py
--rw-r--r--   0        0        0     7935 2023-04-20 04:34:46.179551 upathlib-0.8.1/src/upathlib/_tests.py
--rw-r--r--   0        0        0    34431 2023-06-19 05:53:18.492312 upathlib-0.8.1/src/upathlib/_upath.py
--rw-r--r--   0        0        0     2310 2023-06-19 05:53:18.492312 upathlib-0.8.1/src/upathlib/_util.py
--rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.8.1/src/upathlib/azure.py
--rw-r--r--   0        0        0    26174 2023-06-19 05:53:18.492312 upathlib-0.8.1/src/upathlib/gcs.py
--rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.8.1/src/upathlib/py.typed
--rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.8.1/src/upathlib/serializer.py
--rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 upathlib-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.8.2b1/LICENSE
+-rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.8.2b1/README.rst
+-rw-r--r--   0        0        0     1699 2023-06-19 05:49:42.294835 upathlib-0.8.2b1/pyproject.toml
+-rw-r--r--   0        0        0     2321 2023-06-26 06:41:12.182147 upathlib-0.8.2b1/src/upathlib/__init__.py
+-rw-r--r--   0        0        0     4694 2023-04-20 04:34:46.179551 upathlib-0.8.2b1/src/upathlib/_blob.py
+-rw-r--r--   0        0        0    10749 2023-05-13 05:38:06.231654 upathlib-0.8.2b1/src/upathlib/_local.py
+-rw-r--r--   0        0        0     7935 2023-04-20 04:34:46.179551 upathlib-0.8.2b1/src/upathlib/_tests.py
+-rw-r--r--   0        0        0    34431 2023-06-19 05:53:18.492312 upathlib-0.8.2b1/src/upathlib/_upath.py
+-rw-r--r--   0        0        0     2310 2023-06-19 05:53:18.492312 upathlib-0.8.2b1/src/upathlib/_util.py
+-rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.8.2b1/src/upathlib/azure.py
+-rw-r--r--   0        0        0    26375 2023-06-26 06:49:05.987099 upathlib-0.8.2b1/src/upathlib/gcs.py
+-rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.8.2b1/src/upathlib/py.typed
+-rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.8.2b1/src/upathlib/serializer.py
+-rw-r--r--   0        0        0     2348 1970-01-01 00:00:00.000000 upathlib-0.8.2b1/PKG-INFO
```

### Comparing `upathlib-0.8.1/LICENSE` & `upathlib-0.8.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/README.rst` & `upathlib-0.8.2b1/README.rst`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/pyproject.toml` & `upathlib-0.8.2b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/src/upathlib/__init__.py` & `upathlib-0.8.2b1/src/upathlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 One use case is the package `biglist <https://biglist.readthedocs.io/en/latest/>`__,
 where the class `Biglist <https://biglist.readthedocs.io/en/latest/#biglist.Biglist>`__ takes a Upath object to indicate its location of storage.
 It does not care whether the storage is local or in a cloud blob store---it
 simply uses the common API to operate the storage.
 """
 
-__version__ = "0.8.1"
+__version__ = "0.8.2b1"
 
 
 from pathlib import Path
 from typing import Union
 
 from ._blob import BlobUpath
 from ._local import LocalPathType, LocalUpath
```

### Comparing `upathlib-0.8.1/src/upathlib/_blob.py` & `upathlib-0.8.2b1/src/upathlib/_blob.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/src/upathlib/_local.py` & `upathlib-0.8.2b1/src/upathlib/_local.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/src/upathlib/_tests.py` & `upathlib-0.8.2b1/src/upathlib/_tests.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/src/upathlib/_upath.py` & `upathlib-0.8.2b1/src/upathlib/_upath.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/src/upathlib/_util.py` & `upathlib-0.8.2b1/src/upathlib/_util.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/src/upathlib/azure.py` & `upathlib-0.8.2b1/src/upathlib/azure.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/src/upathlib/gcs.py` & `upathlib-0.8.2b1/src/upathlib/gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import time
 from collections.abc import Iterator
 from datetime import datetime, timezone
 from io import BufferedReader, BytesIO, UnsupportedOperation
 
 import google.auth
 from google import resumable_media
-from google.api_core import exceptions
+from google.api_core import exceptions, retry
 from google.cloud import storage
 
 # 60 seconds; this is the "connection timeout" to server.
 # From my reading, it's the `timeout` parameter to `google.cloud.storage.client._connection.api_request`,
 # that is, the `timeout` parameter to `google.cloud._http.JSONConnection.api_request`.
 # `google.cloud` is repo python-cloud-core.
 from google.cloud.storage.retry import DEFAULT_RETRY
@@ -74,15 +74,20 @@
             project_id = pid
         renewed = True
 
     if (
         not credentials.token
         or (credentials.expiry - datetime.utcnow()).total_seconds() < valid_for_seconds
     ):
-        credentials.refresh(google.auth.transport.requests.Request())
+        retry.Retry(
+            predicate=retry.if_exception_type(
+                google.auth.exceptions.RefreshError,
+                google.auth.exceptions.TransportError,
+            ),
+        )(credentials.refresh)(google.auth.transport.requests.Request())
         # One check shows that this token expires in one hour.
         renewed = True
 
     if renewed:
         logger.debug("Google credentials refreshed")
 
     return project_id, credentials, renewed
```

### Comparing `upathlib-0.8.1/src/upathlib/serializer.py` & `upathlib-0.8.2b1/src/upathlib/serializer.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.1/PKG-INFO` & `upathlib-0.8.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upathlib
-Version: 0.8.1
+Version: 0.8.2b1
 Summary: The package *upathlib*
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

