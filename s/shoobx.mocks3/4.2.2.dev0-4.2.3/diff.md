# Comparing `tmp/shoobx.mocks3-4.2.2.dev0.tar.gz` & `tmp/shoobx.mocks3-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shoobx.mocks3-4.2.2.dev0.tar", last modified: Wed Mar 22 01:31:07 2023, max compression
+gzip compressed data, was "shoobx.mocks3-4.2.3.tar", last modified: Mon Jun 26 06:03:06 2023, max compression
```

## Comparing `shoobx.mocks3-4.2.2.dev0.tar` & `shoobx.mocks3-4.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 jvance    (1000) jvance    (1000)        0 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/
--rw-rw-r--   0 jvance    (1000) jvance    (1000)       71 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/.coveragerc
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     2816 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/CHANGES.rst
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      290 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/MANIFEST.in
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     1755 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/Makefile
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     2013 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/PKG-INFO
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      943 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/README.rst
-drwxrwxr-x   0 jvance    (1000) jvance    (1000)        0 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/config/
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      153 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/config/mocks3.cfg
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      221 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/config/uwsgi.ini
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      395 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/requirements.in
--rw-rw-r--   0 jvance    (1000) jvance    (1000)       27 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/requirements.txt
-drwxrwxr-x   0 jvance    (1000) jvance    (1000)        0 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/scripts/
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     1147 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/scripts/performance.py
--rw-rw-r--   0 jvance    (1000) jvance    (1000)       38 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/setup.cfg
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     2436 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/setup.py
-drwxrwxr-x   0 jvance    (1000) jvance    (1000)        0 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/src/
-drwxrwxr-x   0 jvance    (1000) jvance    (1000)        0 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/src/shoobx/
--rw-rw-r--   0 jvance    (1000) jvance    (1000)       64 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/__init__.py
-drwxrwxr-x   0 jvance    (1000) jvance    (1000)        0 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      928 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/__init__.py
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     2340 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/config.py
--rw-rw-r--   0 jvance    (1000) jvance    (1000)    24458 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/models.py
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      664 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/responses.py
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     2141 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/run.py
-drwxrwxr-x   0 jvance    (1000) jvance    (1000)        0 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/tests/
--rw-rw-r--   0 jvance    (1000) jvance    (1000)       18 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/tests/__init__.py
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     1276 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/tests/test_config.py
--rw-rw-r--   0 jvance    (1000) jvance    (1000)    34069 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/tests/test_s3_boto3.py
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     1051 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/urls.py
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      473 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/wsgi.py
-drwxrwxr-x   0 jvance    (1000) jvance    (1000)        0 2023-03-22 01:31:07.602426 shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/
--rw-rw-r--   0 jvance    (1000) jvance    (1000)     2013 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/PKG-INFO
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      784 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/SOURCES.txt
--rw-rw-r--   0 jvance    (1000) jvance    (1000)        1 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/dependency_links.txt
--rw-rw-r--   0 jvance    (1000) jvance    (1000)       62 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/entry_points.txt
--rw-rw-r--   0 jvance    (1000) jvance    (1000)        1 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/not-zip-safe
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      137 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/requires.txt
--rw-rw-r--   0 jvance    (1000) jvance    (1000)        7 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/top_level.txt
--rw-rw-r--   0 jvance    (1000) jvance    (1000)      291 2023-03-22 01:31:07.000000 shoobx.mocks3-4.2.2.dev0/tox.ini
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/
+-rw-rw-r--   0 adi       (1000) adi       (1000)       71 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/.coveragerc
+-rw-rw-r--   0 adi       (1000) adi       (1000)     2896 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/CHANGES.rst
+-rw-rw-r--   0 adi       (1000) adi       (1000)      290 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/MANIFEST.in
+-rw-rw-r--   0 adi       (1000) adi       (1000)     1755 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/Makefile
+-rw-rw-r--   0 adi       (1000) adi       (1000)     1988 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/PKG-INFO
+-rw-rw-r--   0 adi       (1000) adi       (1000)      943 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/README.rst
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.462110 shoobx.mocks3-4.2.3/config/
+-rw-rw-r--   0 adi       (1000) adi       (1000)      153 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/config/mocks3.cfg
+-rw-rw-r--   0 adi       (1000) adi       (1000)      221 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/config/uwsgi.ini
+-rw-rw-r--   0 adi       (1000) adi       (1000)       16 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/requirements.in
+-rw-rw-r--   0 adi       (1000) adi       (1000)       27 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/requirements.txt
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.462110 shoobx.mocks3-4.2.3/scripts/
+-rw-rw-r--   0 adi       (1000) adi       (1000)     1147 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/scripts/performance.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)       38 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/setup.cfg
+-rw-rw-r--   0 adi       (1000) adi       (1000)     2431 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/setup.py
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.462110 shoobx.mocks3-4.2.3/src/
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.462110 shoobx.mocks3-4.2.3/src/shoobx/
+-rw-rw-r--   0 adi       (1000) adi       (1000)       64 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/__init__.py
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/src/shoobx/mocks3/
+-rw-rw-r--   0 adi       (1000) adi       (1000)      928 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/__init__.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)     2340 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/config.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)    24572 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/models.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)      664 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/responses.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)     2141 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/run.py
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/
+-rw-rw-r--   0 adi       (1000) adi       (1000)       18 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/__init__.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)     1276 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/test_config.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)    34069 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/test_s3_boto3.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)     1051 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/urls.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)      473 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/wsgi.py
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/
+-rw-rw-r--   0 adi       (1000) adi       (1000)     1988 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/PKG-INFO
+-rw-rw-r--   0 adi       (1000) adi       (1000)      784 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/SOURCES.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)        1 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/dependency_links.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)       61 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/entry_points.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)        1 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/not-zip-safe
+-rw-rw-r--   0 adi       (1000) adi       (1000)      137 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/requires.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)        7 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/top_level.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)      291 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/tox.ini
```

### Comparing `shoobx.mocks3-4.2.2.dev0/CHANGES.rst` & `shoobx.mocks3-4.2.3/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 =========
 CHANGELOG
 =========
 
 
-4.2.2 (unreleased)
+4.2.3 (2023-06-26)
+------------------
+
+- Add checksum attributes to class Key
+
+
+4.2.2 (2023-03-21)
 ------------------
 
 - Add parameter to put_object.
 
 
 4.2.1 (2023-03-12)
 ------------------
```

### Comparing `shoobx.mocks3-4.2.2.dev0/Makefile` & `shoobx.mocks3-4.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/PKG-INFO` & `shoobx.mocks3-4.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: shoobx.mocks3
-Version: 4.2.2.dev0
+Version: 4.2.3
 Summary: Shoobx Mock S3 Implementation
 Home-page: http://shoobx.com/
 Author: Shoobx, Inc.
 Author-email: dev@shoobx.com
 License: Proprietary
 Keywords: amazon aws s3 mock moto
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,16 +19,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
-Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: dev
 
 Shoobx Mock S3 Server
 =====================
 
 .. image:: https://github.com/Shoobx/shoobx.mocks3/actions/workflows/test.yml/badge.svg
    :target: https://github.com/Shoobx/shoobx.mocks3/actions
 
@@ -45,9 +44,7 @@
 .. image:: https://api.codeclimate.com/v1/badges/74a6e72efcd89c5a702b/maintainability
    :target: https://codeclimate.com/github/Shoobx/shoobx.mocks3/maintainability
    :alt: Maintainability
 
 This package implements a mock S3 server including bucket shadowing
 support. The code is based on the `moto` package by implementing a custom
 service.
-
-
```

### Comparing `shoobx.mocks3-4.2.2.dev0/README.rst` & `shoobx.mocks3-4.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/scripts/performance.py` & `shoobx.mocks3-4.2.3/scripts/performance.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/setup.py` & `shoobx.mocks3-4.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="shoobx.mocks3",
-    version='4.2.2.dev0',
+    version='4.2.3',
     author="Shoobx, Inc.",
     author_email="dev@shoobx.com",
     description="Shoobx Mock S3 Implementation",
     long_description=read('README.rst'),
     keywords="amazon aws s3 mock moto",
     license='Proprietary',
     url="http://shoobx.com/",
```

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/__init__.py` & `shoobx.mocks3-4.2.3/src/shoobx/mocks3/__init__.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/config.py` & `shoobx.mocks3-4.2.3/src/shoobx/mocks3/config.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/models.py` & `shoobx.mocks3-4.2.3/src/shoobx/mocks3/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         bucket_name=None,
         encryption=None,
         kms_key_id=None,
         bucket_key_enabled=None,
         lock_mode=None,
         lock_legal_status="OFF",
         lock_until=None,
+        checksum_value=None,
     ):
         self.bucket = bucket
         self.name = name
         self.version = version
         self._is_versioned = is_versioned
         self.multipart = multipart
         self._path = os.path.join(bucket._path, "keys", _encode_name(name))
@@ -136,14 +137,17 @@
         self.kms_key_id = kms_key_id
         self.bucket_key_enabled = bucket_key_enabled
         self.lock_mode = lock_mode
         self.lock_legal_status = lock_legal_status
         self.lock_until = lock_until
         self._tick = 0
         self.disposed = None
+        self.checksum_value = checksum_value
+        self.checksum_algorithm = None
+
 
     def __getstate__(self):
         return self.__dict__.copy()
 
     def __setstate__(self, state):
         self.__dict__.update({k: v for k, v in state.items() if k != "value"})
```

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/responses.py` & `shoobx.mocks3-4.2.3/src/shoobx/mocks3/responses.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/run.py` & `shoobx.mocks3-4.2.3/src/shoobx/mocks3/run.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/tests/test_config.py` & `shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/tests/test_s3_boto3.py` & `shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/test_s3_boto3.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx/mocks3/urls.py` & `shoobx.mocks3-4.2.3/src/shoobx/mocks3/urls.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/PKG-INFO` & `shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: shoobx.mocks3
-Version: 4.2.2.dev0
+Version: 4.2.3
 Summary: Shoobx Mock S3 Implementation
 Home-page: http://shoobx.com/
 Author: Shoobx, Inc.
 Author-email: dev@shoobx.com
 License: Proprietary
 Keywords: amazon aws s3 mock moto
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,16 +19,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
-Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: dev
 
 Shoobx Mock S3 Server
 =====================
 
 .. image:: https://github.com/Shoobx/shoobx.mocks3/actions/workflows/test.yml/badge.svg
    :target: https://github.com/Shoobx/shoobx.mocks3/actions
 
@@ -45,9 +44,7 @@
 .. image:: https://api.codeclimate.com/v1/badges/74a6e72efcd89c5a702b/maintainability
    :target: https://codeclimate.com/github/Shoobx/shoobx.mocks3/maintainability
    :alt: Maintainability
 
 This package implements a mock S3 server including bucket shadowing
 support. The code is based on the `moto` package by implementing a custom
 service.
-
-
```

### Comparing `shoobx.mocks3-4.2.2.dev0/src/shoobx.mocks3.egg-info/SOURCES.txt` & `shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

