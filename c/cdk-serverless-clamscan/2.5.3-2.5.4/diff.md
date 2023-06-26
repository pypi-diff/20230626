# Comparing `tmp/cdk-serverless-clamscan-2.5.3.tar.gz` & `tmp/cdk-serverless-clamscan-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-serverless-clamscan-2.5.3.tar", last modified: Sun Jun 25 00:32:12 2023, max compression
+gzip compressed data, was "cdk-serverless-clamscan-2.5.4.tar", last modified: Mon Jun 26 00:31:48 2023, max compression
```

## Comparing `cdk-serverless-clamscan-2.5.3.tar` & `cdk-serverless-clamscan-2.5.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:32:12.361206 cdk-serverless-clamscan-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-25 00:32:12.361206 cdk-serverless-clamscan-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 00:32:12.361206 cdk-serverless-clamscan-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:32:12.357206 cdk-serverless-clamscan-2.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:32:12.357206 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan/
--rw-r--r--   0 runner    (1001) docker     (123)    33603 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:32:12.361206 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:32:12.361206 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan/_jsii/bin/0
--rw-r--r--   0 runner    (1001) docker     (123)   137090 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.5.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 00:31:58.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:32:12.357206 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-25 00:32:12.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-25 00:32:12.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 00:32:12.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 00:32:12.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-25 00:32:12.000000 cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:31:48.128883 cdk-serverless-clamscan-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-26 00:31:48.128883 cdk-serverless-clamscan-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 00:31:48.128883 cdk-serverless-clamscan-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:31:48.124883 cdk-serverless-clamscan-2.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:31:48.128883 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan/
+-rw-r--r--   0 runner    (1001) docker     (123)    33603 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:31:48.128883 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:31:48.128883 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan/_jsii/bin/0
+-rw-r--r--   0 runner    (1001) docker     (123)   137088 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.5.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:31:31.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:31:48.128883 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-26 00:31:48.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 00:31:48.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:31:48.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 00:31:48.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 00:31:48.000000 cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan.egg-info/top_level.txt
```

### Comparing `cdk-serverless-clamscan-2.5.3/LICENSE` & `cdk-serverless-clamscan-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.5.3/PKG-INFO` & `cdk-serverless-clamscan-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-serverless-clamscan
-Version: 2.5.3
+Version: 2.5.4
 Summary: Serverless architecture to virus scan objects in Amazon S3.
 Home-page: https://github.com/awslabs/cdk-serverless-clamscan
 Author: Amazon Web Services<donti@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/cdk-serverless-clamscan
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-serverless-clamscan-2.5.3/README.md` & `cdk-serverless-clamscan-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.5.3/setup.py` & `cdk-serverless-clamscan-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-serverless-clamscan",
-    "version": "2.5.3",
+    "version": "2.5.4",
     "description": "Serverless architecture to virus scan objects in Amazon S3.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/cdk-serverless-clamscan",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<donti@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_serverless_clamscan",
         "cdk_serverless_clamscan._jsii"
     ],
     "package_data": {
         "cdk_serverless_clamscan._jsii": [
-            "cdk-serverless-clamscan@2.5.3.jsii.tgz"
+            "cdk-serverless-clamscan@2.5.4.jsii.tgz"
         ],
         "cdk_serverless_clamscan": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan/__init__.py` & `cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan.egg-info/PKG-INFO` & `cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-serverless-clamscan
-Version: 2.5.3
+Version: 2.5.4
 Summary: Serverless architecture to virus scan objects in Amazon S3.
 Home-page: https://github.com/awslabs/cdk-serverless-clamscan
 Author: Amazon Web Services<donti@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/cdk-serverless-clamscan
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-serverless-clamscan-2.5.3/src/cdk_serverless_clamscan.egg-info/SOURCES.txt` & `cdk-serverless-clamscan-2.5.4/src/cdk_serverless_clamscan.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 src/cdk_serverless_clamscan/py.typed
 src/cdk_serverless_clamscan.egg-info/PKG-INFO
 src/cdk_serverless_clamscan.egg-info/SOURCES.txt
 src/cdk_serverless_clamscan.egg-info/dependency_links.txt
 src/cdk_serverless_clamscan.egg-info/requires.txt
 src/cdk_serverless_clamscan.egg-info/top_level.txt
 src/cdk_serverless_clamscan/_jsii/__init__.py
-src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.5.3.jsii.tgz
+src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.5.4.jsii.tgz
 src/cdk_serverless_clamscan/_jsii/bin/0
```

