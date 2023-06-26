# Comparing `tmp/stratus-api-integrations-0.0.8.tar.gz` & `tmp/stratus-api-integrations-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stratus-api-integrations-0.0.8.tar", last modified: Wed Dec  2 15:22:43 2020, max compression
+gzip compressed data, was "dist/stratus-api-integrations-0.0.9.tar", last modified: Wed Dec  2 15:37:41 2020, max compression
```

## Comparing `stratus-api-integrations-0.0.8.tar` & `stratus-api-integrations-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/
--rw-r--r--   0 perrystallings   (502) staff       (20)      205 2020-08-27 16:22:24.000000 stratus-api-integrations-0.0.8/MANIFEST.in
--rw-r--r--   0 perrystallings   (502) staff       (20)      475 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/PKG-INFO
--rw-r--r--   0 perrystallings   (502) staff       (20)      129 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/setup.cfg
--rw-r--r--   0 perrystallings   (502) staff       (20)     1079 2020-12-02 15:22:22.000000 stratus-api-integrations-0.0.8/setup.py
-drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/stratus_api/
-drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/
--rw-r--r--   0 perrystallings   (502) staff       (20)      185 2020-08-25 17:42:27.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/__init__.py
--rw-r--r--   0 perrystallings   (502) staff       (20)     5346 2020-12-02 15:22:02.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/base.py
--rw-r--r--   0 perrystallings   (502) staff       (20)     6599 2020-12-02 15:22:02.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/chunks.py
--rw-r--r--   0 perrystallings   (502) staff       (20)     5162 2020-10-30 16:00:01.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/distribution.py
-drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/routes/
--rw-r--r--   0 perrystallings   (502) staff       (20)        0 2020-07-21 18:42:00.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/routes/__init__.py
-drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/routes/v1/
--rw-r--r--   0 perrystallings   (502) staff       (20)        0 2020-07-23 23:14:27.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/routes/v1/__init__.py
--rw-r--r--   0 perrystallings   (502) staff       (20)     1280 2020-12-02 15:22:02.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/routes/v1/destinations.py
--rw-r--r--   0 perrystallings   (502) staff       (20)      679 2020-10-30 16:07:13.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/routes/v1/distribution.py
--rw-r--r--   0 perrystallings   (502) staff       (20)     1289 2020-12-02 15:22:02.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/routes/v1/segments.py
--rw-r--r--   0 perrystallings   (502) staff       (20)      181 2020-07-21 18:54:29.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/routes/v1/settings.py
-drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/schemas/
--rw-r--r--   0 perrystallings   (502) staff       (20)     9077 2020-08-25 20:06:41.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/schemas/v1.yaml
-drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/tasks/
--rw-r--r--   0 perrystallings   (502) staff       (20)        0 2020-07-21 19:54:45.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/tasks/__init__.py
--rw-r--r--   0 perrystallings   (502) staff       (20)      605 2020-10-30 16:00:01.000000 stratus-api-integrations-0.0.8/stratus_api/integrations/tasks/distributions.py
-drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:22:43.000000 stratus-api-integrations-0.0.8/stratus_api_integrations.egg-info/
--rw-r--r--   0 perrystallings   (502) staff       (20)      475 2020-12-02 15:22:42.000000 stratus-api-integrations-0.0.8/stratus_api_integrations.egg-info/PKG-INFO
--rw-r--r--   0 perrystallings   (502) staff       (20)      834 2020-12-02 15:22:42.000000 stratus-api-integrations-0.0.8/stratus_api_integrations.egg-info/SOURCES.txt
--rw-r--r--   0 perrystallings   (502) staff       (20)        1 2020-12-02 15:22:42.000000 stratus-api-integrations-0.0.8/stratus_api_integrations.egg-info/dependency_links.txt
--rw-r--r--   0 perrystallings   (502) staff       (20)      159 2020-12-02 15:22:42.000000 stratus-api-integrations-0.0.8/stratus_api_integrations.egg-info/requires.txt
--rw-r--r--   0 perrystallings   (502) staff       (20)       12 2020-12-02 15:22:42.000000 stratus-api-integrations-0.0.8/stratus_api_integrations.egg-info/top_level.txt
+drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/
+-rw-r--r--   0 perrystallings   (502) staff       (20)      205 2020-08-27 16:22:24.000000 stratus-api-integrations-0.0.9/MANIFEST.in
+-rw-r--r--   0 perrystallings   (502) staff       (20)      475 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/PKG-INFO
+-rw-r--r--   0 perrystallings   (502) staff       (20)      129 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/setup.cfg
+-rw-r--r--   0 perrystallings   (502) staff       (20)     1079 2020-12-02 15:33:35.000000 stratus-api-integrations-0.0.9/setup.py
+drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api/
+drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/
+-rw-r--r--   0 perrystallings   (502) staff       (20)      185 2020-08-25 17:42:27.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/__init__.py
+-rw-r--r--   0 perrystallings   (502) staff       (20)     5346 2020-12-02 15:22:02.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/base.py
+-rw-r--r--   0 perrystallings   (502) staff       (20)     1152 2020-12-02 15:22:02.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/cache.py
+-rw-r--r--   0 perrystallings   (502) staff       (20)     6587 2020-12-02 15:29:58.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/chunks.py
+-rw-r--r--   0 perrystallings   (502) staff       (20)     5162 2020-10-30 16:00:01.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/distribution.py
+drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/routes/
+-rw-r--r--   0 perrystallings   (502) staff       (20)        0 2020-07-21 18:42:00.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/routes/__init__.py
+drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/routes/v1/
+-rw-r--r--   0 perrystallings   (502) staff       (20)        0 2020-07-23 23:14:27.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/routes/v1/__init__.py
+-rw-r--r--   0 perrystallings   (502) staff       (20)     1280 2020-12-02 15:22:02.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/routes/v1/destinations.py
+-rw-r--r--   0 perrystallings   (502) staff       (20)      679 2020-10-30 16:07:13.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/routes/v1/distribution.py
+-rw-r--r--   0 perrystallings   (502) staff       (20)     1289 2020-12-02 15:22:02.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/routes/v1/segments.py
+-rw-r--r--   0 perrystallings   (502) staff       (20)      181 2020-07-21 18:54:29.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/routes/v1/settings.py
+drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/schemas/
+-rw-r--r--   0 perrystallings   (502) staff       (20)     9077 2020-08-25 20:06:41.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/schemas/v1.yaml
+drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/tasks/
+-rw-r--r--   0 perrystallings   (502) staff       (20)        0 2020-07-21 19:54:45.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/tasks/__init__.py
+-rw-r--r--   0 perrystallings   (502) staff       (20)      605 2020-10-30 16:00:01.000000 stratus-api-integrations-0.0.9/stratus_api/integrations/tasks/distributions.py
+drwxr-xr-x   0 perrystallings   (502) staff       (20)        0 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api_integrations.egg-info/
+-rw-r--r--   0 perrystallings   (502) staff       (20)      475 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api_integrations.egg-info/PKG-INFO
+-rw-r--r--   0 perrystallings   (502) staff       (20)      868 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api_integrations.egg-info/SOURCES.txt
+-rw-r--r--   0 perrystallings   (502) staff       (20)        1 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api_integrations.egg-info/dependency_links.txt
+-rw-r--r--   0 perrystallings   (502) staff       (20)      159 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api_integrations.egg-info/requires.txt
+-rw-r--r--   0 perrystallings   (502) staff       (20)       12 2020-12-02 15:37:41.000000 stratus-api-integrations-0.0.9/stratus_api_integrations.egg-info/top_level.txt
```

### Comparing `stratus-api-integrations-0.0.8/setup.py` & `stratus-api-integrations-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 # with open('requirements.txt') as f:
 #     requirements = f.readlines()
 
 setuptools.setup(
     name="stratus-api-integrations",  # Replace with your own username
-    version="0.0.8",
+    version="0.0.9",
     author="DOT",
     author_email="dot@adara.com",
     description="Simplified advertising integrations",
     long_description="",
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://bitbucket.org/adarainc/framework-auth",
```

### Comparing `stratus-api-integrations-0.0.8/stratus_api/integrations/base.py` & `stratus-api-integrations-0.0.9/stratus_api/integrations/base.py`

 * *Files identical despite different names*

### Comparing `stratus-api-integrations-0.0.8/stratus_api/integrations/chunks.py` & `stratus-api-integrations-0.0.9/stratus_api/integrations/chunks.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 
 def create_file_chunks(bucket_name, file_pattern, job_uuid, file_headers, integration_settings, delimiter='|'):
     from stratus_api.storage.gcs import download_from_storage, get_filenames_by_pattern
     import os
     import csv
     from datetime import datetime
-    from stratus_api.integrations.utils.cache import cache_data
-    from stratus_api.integrations.utils.cache import get_cached_data
+    from stratus_api.integrations.cache import cache_data
+    from stratus_api.integrations.cache import get_cached_data
 
     chunk_number = 0
     chunk_records = 0
     start = datetime.utcnow().timestamp()
     chunk_pointer = None
     chunk_writer = None
     delivered_pointer = None
```

### Comparing `stratus-api-integrations-0.0.8/stratus_api/integrations/distribution.py` & `stratus-api-integrations-0.0.9/stratus_api/integrations/distribution.py`

 * *Files identical despite different names*

### Comparing `stratus-api-integrations-0.0.8/stratus_api/integrations/routes/v1/destinations.py` & `stratus-api-integrations-0.0.9/stratus_api/integrations/routes/v1/destinations.py`

 * *Files identical despite different names*

### Comparing `stratus-api-integrations-0.0.8/stratus_api/integrations/routes/v1/distribution.py` & `stratus-api-integrations-0.0.9/stratus_api/integrations/routes/v1/distribution.py`

 * *Files identical despite different names*

### Comparing `stratus-api-integrations-0.0.8/stratus_api/integrations/routes/v1/segments.py` & `stratus-api-integrations-0.0.9/stratus_api/integrations/routes/v1/segments.py`

 * *Files identical despite different names*

### Comparing `stratus-api-integrations-0.0.8/stratus_api/integrations/schemas/v1.yaml` & `stratus-api-integrations-0.0.9/stratus_api/integrations/schemas/v1.yaml`

 * *Files identical despite different names*

### Comparing `stratus-api-integrations-0.0.8/stratus_api/integrations/tasks/distributions.py` & `stratus-api-integrations-0.0.9/stratus_api/integrations/tasks/distributions.py`

 * *Files identical despite different names*

### Comparing `stratus-api-integrations-0.0.8/stratus_api_integrations.egg-info/SOURCES.txt` & `stratus-api-integrations-0.0.9/stratus_api_integrations.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 setup.cfg
 setup.py
 stratus_api/integrations/__init__.py
 stratus_api/integrations/base.py
+stratus_api/integrations/cache.py
 stratus_api/integrations/chunks.py
 stratus_api/integrations/distribution.py
 stratus_api/integrations/routes/__init__.py
 stratus_api/integrations/routes/v1/__init__.py
 stratus_api/integrations/routes/v1/destinations.py
 stratus_api/integrations/routes/v1/distribution.py
 stratus_api/integrations/routes/v1/segments.py
```

