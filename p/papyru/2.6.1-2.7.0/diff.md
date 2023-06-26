# Comparing `tmp/papyru-2.6.1.tar.gz` & `tmp/papyru-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papyru-2.6.1.tar", last modified: Tue Apr 25 09:08:58 2023, max compression
+gzip compressed data, was "papyru-2.7.0.tar", last modified: Mon Jun 26 12:24:24 2023, max compression
```

## Comparing `papyru-2.6.1.tar` & `papyru-2.7.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-04-25 09:08:58.338872 papyru-2.6.1/
--rw-r--r--   0 jonas     (1000) jonas     (1000)    34523 2022-04-01 07:10:27.000000 papyru-2.6.1/LICENSE.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)      648 2023-04-25 09:08:58.338872 papyru-2.6.1/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)      634 2022-04-01 07:10:27.000000 papyru-2.6.1/README.rst
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-04-25 09:08:58.338872 papyru-2.6.1/bin/
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     3470 2022-04-01 07:10:27.000000 papyru-2.6.1/bin/generate_jsonschema.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-04-25 09:08:58.338872 papyru-2.6.1/papyru/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1206 2022-06-14 09:21:53.000000 papyru-2.6.1/papyru/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2046 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/auth.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2591 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/context.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5072 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/logger.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2719 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/logger_stdout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1670 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/logger_types.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      415 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/middleware.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4504 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/problem.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4656 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/profiler.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3140 2022-05-17 11:17:59.000000 papyru-2.6.1/papyru/resource.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2127 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/serializer.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1256 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/stack_context.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-04-25 09:08:58.338872 papyru-2.6.1/papyru/static/
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/static/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)       94 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/static/apps.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      149 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/static/urls.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2318 2022-05-17 11:17:59.000000 papyru-2.6.1/papyru/static/views.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5860 2022-12-07 12:42:18.000000 papyru-2.6.1/papyru/utils.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3921 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/validation.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-04-25 09:08:58.338872 papyru-2.6.1/papyru/varspool/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3371 2023-01-25 15:04:04.000000 papyru-2.6.1/papyru/varspool/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-04-25 09:08:58.338872 papyru-2.6.1/papyru/varspool/assets/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2338 2023-04-25 08:57:46.000000 papyru-2.6.1/papyru/varspool/assets/Job.json
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1336 2022-05-03 11:04:22.000000 papyru-2.6.1/papyru/varspool/assets/JobStatusHistory.json
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-04-25 09:08:58.338872 papyru-2.6.1/papyru/varspool/command/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7089 2023-01-24 08:33:24.000000 papyru-2.6.1/papyru/varspool/command/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4487 2023-01-03 06:59:43.000000 papyru-2.6.1/papyru/varspool/command/config.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      655 2022-12-07 17:08:10.000000 papyru-2.6.1/papyru/varspool/command/types.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1208 2023-04-25 06:32:28.000000 papyru-2.6.1/papyru/varspool/serializers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2433 2022-05-09 14:32:54.000000 papyru-2.6.1/papyru/varspool/types.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3492 2022-04-01 07:10:27.000000 papyru-2.6.1/papyru/xml_helper.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-04-25 09:08:58.338872 papyru-2.6.1/papyru.egg-info/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      648 2023-04-25 09:08:57.000000 papyru-2.6.1/papyru.egg-info/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)      860 2023-04-25 09:08:58.000000 papyru-2.6.1/papyru.egg-info/SOURCES.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-04-25 09:08:58.000000 papyru-2.6.1/papyru.egg-info/dependency_links.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)       64 2023-04-25 09:08:58.000000 papyru-2.6.1/papyru.egg-info/requires.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        7 2023-04-25 09:08:58.000000 papyru-2.6.1/papyru.egg-info/top_level.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)       38 2023-04-25 09:08:58.338872 papyru-2.6.1/setup.cfg
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1126 2023-04-25 08:56:18.000000 papyru-2.6.1/setup.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-26 12:24:24.659853 papyru-2.7.0/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    34523 2022-04-01 07:10:27.000000 papyru-2.7.0/LICENSE.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      648 2023-06-26 12:24:24.659853 papyru-2.7.0/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      634 2022-04-01 07:10:27.000000 papyru-2.7.0/README.rst
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-26 12:24:24.655853 papyru-2.7.0/bin/
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     3470 2022-04-01 07:10:27.000000 papyru-2.7.0/bin/generate_jsonschema.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-26 12:24:24.659853 papyru-2.7.0/papyru/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1206 2022-06-14 09:21:53.000000 papyru-2.7.0/papyru/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2046 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/auth.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2591 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/context.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5072 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/logger.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2719 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/logger_stdout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1670 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/logger_types.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      415 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/middleware.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4504 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/problem.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4656 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/profiler.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3140 2022-05-17 11:17:59.000000 papyru-2.7.0/papyru/resource.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2127 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/serializer.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1256 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/stack_context.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-26 12:24:24.659853 papyru-2.7.0/papyru/static/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/static/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       94 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/static/apps.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      149 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/static/urls.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2318 2022-05-17 11:17:59.000000 papyru-2.7.0/papyru/static/views.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6365 2023-06-26 12:24:00.000000 papyru-2.7.0/papyru/utils.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3921 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/validation.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-26 12:24:24.659853 papyru-2.7.0/papyru/varspool/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3371 2023-01-25 15:04:04.000000 papyru-2.7.0/papyru/varspool/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-26 12:24:24.659853 papyru-2.7.0/papyru/varspool/assets/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2338 2023-04-26 10:48:02.000000 papyru-2.7.0/papyru/varspool/assets/Job.json
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1336 2022-05-03 11:04:22.000000 papyru-2.7.0/papyru/varspool/assets/JobStatusHistory.json
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-26 12:24:24.659853 papyru-2.7.0/papyru/varspool/command/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7089 2023-01-24 08:33:24.000000 papyru-2.7.0/papyru/varspool/command/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4487 2023-01-03 06:59:43.000000 papyru-2.7.0/papyru/varspool/command/config.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      655 2022-12-07 17:08:10.000000 papyru-2.7.0/papyru/varspool/command/types.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1208 2023-04-25 06:32:28.000000 papyru-2.7.0/papyru/varspool/serializers.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2433 2022-05-09 14:32:54.000000 papyru-2.7.0/papyru/varspool/types.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3492 2022-04-01 07:10:27.000000 papyru-2.7.0/papyru/xml_helper.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-26 12:24:24.659853 papyru-2.7.0/papyru.egg-info/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      648 2023-06-26 12:24:24.000000 papyru-2.7.0/papyru.egg-info/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      860 2023-06-26 12:24:24.000000 papyru-2.7.0/papyru.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-06-26 12:24:24.000000 papyru-2.7.0/papyru.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       64 2023-06-26 12:24:24.000000 papyru-2.7.0/papyru.egg-info/requires.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        7 2023-06-26 12:24:24.000000 papyru-2.7.0/papyru.egg-info/top_level.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       38 2023-06-26 12:24:24.659853 papyru-2.7.0/setup.cfg
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1126 2023-06-26 12:23:51.000000 papyru-2.7.0/setup.py
```

### Comparing `papyru-2.6.1/LICENSE.txt` & `papyru-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/PKG-INFO` & `papyru-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papyru
-Version: 2.6.1
+Version: 2.7.0
 Summary: minimal REST library with OpenAPI-based validation for django
 Home-page: http://www.puzzleyou.net/
 Author: puzzleYOU GmbH
 Author-email: papyru@puzzleyou.net
 License: AGPLv3
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `papyru-2.6.1/README.rst` & `papyru-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/bin/generate_jsonschema.py` & `papyru-2.7.0/bin/generate_jsonschema.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/__init__.py` & `papyru-2.7.0/papyru/__init__.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/auth.py` & `papyru-2.7.0/papyru/auth.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/context.py` & `papyru-2.7.0/papyru/context.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/logger.py` & `papyru-2.7.0/papyru/logger.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/logger_stdout.py` & `papyru-2.7.0/papyru/logger_stdout.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/logger_types.py` & `papyru-2.7.0/papyru/logger_types.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/problem.py` & `papyru-2.7.0/papyru/problem.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/profiler.py` & `papyru-2.7.0/papyru/profiler.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/resource.py` & `papyru-2.7.0/papyru/resource.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/serializer.py` & `papyru-2.7.0/papyru/serializer.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/stack_context.py` & `papyru-2.7.0/papyru/stack_context.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/static/views.py` & `papyru-2.7.0/papyru/static/views.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/utils.py` & `papyru-2.7.0/papyru/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from functools import partial, wraps
 from os import getpid
 from time import sleep
 from typing import Dict
 from unittest.mock import patch
 from uuid import uuid4
 
+from django.db.models import QuerySet
+
 from papyru.logger import log_info
 
 _logger = logging.getLogger(__name__)
 
 PYTHON_REQUESTS_DEFAULT_TIMEOUT_SECONDS = 300
 
 
@@ -210,7 +212,22 @@
                         sleep(timeout)
                     else:
                         raise
 
             return func(*args, **kwargs)
         return wrapper
     return decorator
+
+
+def delete_in_chunks(query: QuerySet,
+                     chunk_size: int = 1024,
+                     chunks_to_delete: int = 512):
+    chunks_to_delete -= 1
+    affected_rows, _ = (
+        query.model
+        .objects
+        .filter(pk__in=list(
+            query.only('pk').values_list('pk', flat=True)[:chunk_size]))
+        .delete())
+
+    if affected_rows > 0 and chunks_to_delete > 0:
+        return delete_in_chunks(query, chunk_size, chunks_to_delete)
```

### Comparing `papyru-2.6.1/papyru/validation.py` & `papyru-2.7.0/papyru/validation.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/varspool/__init__.py` & `papyru-2.7.0/papyru/varspool/__init__.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/varspool/assets/Job.json` & `papyru-2.7.0/papyru/varspool/assets/Job.json`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/varspool/assets/JobStatusHistory.json` & `papyru-2.7.0/papyru/varspool/assets/JobStatusHistory.json`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/varspool/command/__init__.py` & `papyru-2.7.0/papyru/varspool/command/__init__.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/varspool/command/config.py` & `papyru-2.7.0/papyru/varspool/command/config.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/varspool/command/types.py` & `papyru-2.7.0/papyru/varspool/command/types.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/varspool/serializers.py` & `papyru-2.7.0/papyru/varspool/serializers.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/varspool/types.py` & `papyru-2.7.0/papyru/varspool/types.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru/xml_helper.py` & `papyru-2.7.0/papyru/xml_helper.py`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/papyru.egg-info/PKG-INFO` & `papyru-2.7.0/papyru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papyru
-Version: 2.6.1
+Version: 2.7.0
 Summary: minimal REST library with OpenAPI-based validation for django
 Home-page: http://www.puzzleyou.net/
 Author: puzzleYOU GmbH
 Author-email: papyru@puzzleyou.net
 License: AGPLv3
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `papyru-2.6.1/papyru.egg-info/SOURCES.txt` & `papyru-2.7.0/papyru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papyru-2.6.1/setup.py` & `papyru-2.7.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='papyru',
-    version='2.6.1',
+    version='2.7.0',
     description=(
         'minimal REST library with OpenAPI-based validation for django'),
     author='puzzleYOU GmbH',
     author_email='papyru@puzzleyou.net',
     url='http://www.puzzleyou.net/',
     license='AGPLv3',
     platforms=['any'],
```

