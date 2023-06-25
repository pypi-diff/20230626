# Comparing `tmp/cdk-redisdb-0.0.33.tar.gz` & `tmp/cdk-redisdb-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-redisdb-0.0.33.tar", last modified: Fri Jun 23 00:18:16 2023, max compression
+gzip compressed data, was "cdk-redisdb-0.0.34.tar", last modified: Sun Jun 25 23:02:00 2023, max compression
```

## Comparing `cdk-redisdb-0.0.33.tar` & `cdk-redisdb-0.0.34.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:18:16.380401 cdk-redisdb-0.0.33/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-23 00:18:04.000000 cdk-redisdb-0.0.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 00:18:04.000000 cdk-redisdb-0.0.33/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-23 00:18:16.380401 cdk-redisdb-0.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-23 00:18:04.000000 cdk-redisdb-0.0.33/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-23 00:18:04.000000 cdk-redisdb-0.0.33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 00:18:16.380401 cdk-redisdb-0.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-23 00:18:04.000000 cdk-redisdb-0.0.33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:18:16.376401 cdk-redisdb-0.0.33/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:18:16.376401 cdk-redisdb-0.0.33/src/cdk_redisdb/
--rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-06-23 00:18:04.000000 cdk-redisdb-0.0.33/src/cdk_redisdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:18:16.376401 cdk-redisdb-0.0.33/src/cdk_redisdb/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 00:18:04.000000 cdk-redisdb-0.0.33/src/cdk_redisdb/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-06-23 00:18:04.000000 cdk-redisdb-0.0.33/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.33.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:18:04.000000 cdk-redisdb-0.0.33/src/cdk_redisdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:18:16.376401 cdk-redisdb-0.0.33/src/cdk_redisdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-23 00:18:16.000000 cdk-redisdb-0.0.33/src/cdk_redisdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-23 00:18:16.000000 cdk-redisdb-0.0.33/src/cdk_redisdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:18:16.000000 cdk-redisdb-0.0.33/src/cdk_redisdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 00:18:16.000000 cdk-redisdb-0.0.33/src/cdk_redisdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 00:18:16.000000 cdk-redisdb-0.0.33/src/cdk_redisdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:02:00.091653 cdk-redisdb-0.0.34/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-25 23:01:44.000000 cdk-redisdb-0.0.34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 23:01:44.000000 cdk-redisdb-0.0.34/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-25 23:02:00.091653 cdk-redisdb-0.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-25 23:01:44.000000 cdk-redisdb-0.0.34/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-25 23:01:44.000000 cdk-redisdb-0.0.34/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 23:02:00.091653 cdk-redisdb-0.0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-25 23:01:44.000000 cdk-redisdb-0.0.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:02:00.087653 cdk-redisdb-0.0.34/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:02:00.091653 cdk-redisdb-0.0.34/src/cdk_redisdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-06-25 23:01:44.000000 cdk-redisdb-0.0.34/src/cdk_redisdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:02:00.091653 cdk-redisdb-0.0.34/src/cdk_redisdb/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-25 23:01:44.000000 cdk-redisdb-0.0.34/src/cdk_redisdb/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26108 2023-06-25 23:01:44.000000 cdk-redisdb-0.0.34/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.34.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:01:44.000000 cdk-redisdb-0.0.34/src/cdk_redisdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:02:00.091653 cdk-redisdb-0.0.34/src/cdk_redisdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-25 23:02:00.000000 cdk-redisdb-0.0.34/src/cdk_redisdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-25 23:02:00.000000 cdk-redisdb-0.0.34/src/cdk_redisdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:02:00.000000 cdk-redisdb-0.0.34/src/cdk_redisdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 23:02:00.000000 cdk-redisdb-0.0.34/src/cdk_redisdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 23:02:00.000000 cdk-redisdb-0.0.34/src/cdk_redisdb.egg-info/top_level.txt
```

### Comparing `cdk-redisdb-0.0.33/LICENSE` & `cdk-redisdb-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.33/PKG-INFO` & `cdk-redisdb-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.33
+Version: 0.0.34
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-redisdb-0.0.33/README.md` & `cdk-redisdb-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.33/setup.py` & `cdk-redisdb-0.0.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-redisdb",
-    "version": "0.0.33",
+    "version": "0.0.34",
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "license": "Apache-2.0",
     "url": "https://github.com/forkfork/cdk-redisdb.git",
     "long_description_content_type": "text/markdown",
     "author": "Timothy Downs<timothydowns@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_redisdb",
         "cdk_redisdb._jsii"
     ],
     "package_data": {
         "cdk_redisdb._jsii": [
-            "cdk-redisdb@0.0.33.jsii.tgz"
+            "cdk-redisdb@0.0.34.jsii.tgz"
         ],
         "cdk_redisdb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-redisdb-0.0.33/src/cdk_redisdb/__init__.py` & `cdk-redisdb-0.0.34/src/cdk_redisdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.33/src/cdk_redisdb.egg-info/PKG-INFO` & `cdk-redisdb-0.0.34/src/cdk_redisdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.33
+Version: 0.0.34
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

