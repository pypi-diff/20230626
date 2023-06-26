# Comparing `tmp/cdklabs.cdk-appflow-0.0.7.tar.gz` & `tmp/cdklabs.cdk-appflow-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-appflow-0.0.7.tar", last modified: Sun Jun 25 00:37:58 2023, max compression
+gzip compressed data, was "cdklabs.cdk-appflow-0.0.8.tar", last modified: Mon Jun 26 00:36:15 2023, max compression
```

## Comparing `cdklabs.cdk-appflow-0.0.7.tar` & `cdklabs.cdk-appflow-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:37:58.828084 cdklabs.cdk-appflow-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-25 00:37:44.000000 cdklabs.cdk-appflow-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 00:37:44.000000 cdklabs.cdk-appflow-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-25 00:37:58.828084 cdklabs.cdk-appflow-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-06-25 00:37:44.000000 cdklabs.cdk-appflow-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-25 00:37:44.000000 cdklabs.cdk-appflow-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 00:37:58.828084 cdklabs.cdk-appflow-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-25 00:37:44.000000 cdklabs.cdk-appflow-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:37:58.824084 cdklabs.cdk-appflow-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:37:58.824084 cdklabs.cdk-appflow-0.0.7/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:37:58.824084 cdklabs.cdk-appflow-0.0.7/src/cdklabs/cdk_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)   504284 2023-06-25 00:37:44.000000 cdklabs.cdk-appflow-0.0.7/src/cdklabs/cdk_appflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:37:58.824084 cdklabs.cdk-appflow-0.0.7/src/cdklabs/cdk_appflow/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-25 00:37:44.000000 cdklabs.cdk-appflow-0.0.7/src/cdklabs/cdk_appflow/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179742 2023-06-25 00:37:44.000000 cdklabs.cdk-appflow-0.0.7/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 00:37:44.000000 cdklabs.cdk-appflow-0.0.7/src/cdklabs/cdk_appflow/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:37:58.824084 cdklabs.cdk-appflow-0.0.7/src/cdklabs.cdk_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-25 00:37:58.000000 cdklabs.cdk-appflow-0.0.7/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-25 00:37:58.000000 cdklabs.cdk-appflow-0.0.7/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 00:37:58.000000 cdklabs.cdk-appflow-0.0.7/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-25 00:37:58.000000 cdklabs.cdk-appflow-0.0.7/src/cdklabs.cdk_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 00:37:58.000000 cdklabs.cdk-appflow-0.0.7/src/cdklabs.cdk_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:36:15.645166 cdklabs.cdk-appflow-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 00:36:02.000000 cdklabs.cdk-appflow-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 00:36:02.000000 cdklabs.cdk-appflow-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-26 00:36:15.645166 cdklabs.cdk-appflow-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-06-26 00:36:02.000000 cdklabs.cdk-appflow-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 00:36:02.000000 cdklabs.cdk-appflow-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 00:36:15.645166 cdklabs.cdk-appflow-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-26 00:36:02.000000 cdklabs.cdk-appflow-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:36:15.641166 cdklabs.cdk-appflow-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:36:15.641166 cdklabs.cdk-appflow-0.0.8/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:36:15.645166 cdklabs.cdk-appflow-0.0.8/src/cdklabs/cdk_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   504284 2023-06-26 00:36:02.000000 cdklabs.cdk-appflow-0.0.8/src/cdklabs/cdk_appflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:36:15.645166 cdklabs.cdk-appflow-0.0.8/src/cdklabs/cdk_appflow/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-26 00:36:02.000000 cdklabs.cdk-appflow-0.0.8/src/cdklabs/cdk_appflow/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179741 2023-06-26 00:36:02.000000 cdklabs.cdk-appflow-0.0.8/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:36:02.000000 cdklabs.cdk-appflow-0.0.8/src/cdklabs/cdk_appflow/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:36:15.641166 cdklabs.cdk-appflow-0.0.8/src/cdklabs.cdk_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-26 00:36:15.000000 cdklabs.cdk-appflow-0.0.8/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-26 00:36:15.000000 cdklabs.cdk-appflow-0.0.8/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:36:15.000000 cdklabs.cdk-appflow-0.0.8/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 00:36:15.000000 cdklabs.cdk-appflow-0.0.8/src/cdklabs.cdk_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 00:36:15.000000 cdklabs.cdk-appflow-0.0.8/src/cdklabs.cdk_appflow.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-appflow-0.0.7/LICENSE` & `cdklabs.cdk-appflow-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.7/PKG-INFO` & `cdklabs.cdk-appflow-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-appflow
-Version: 0.0.7
+Version: 0.0.8
 Summary: @cdklabs/cdk-appflow
 Home-page: https://github.com/cdklabs/cdk-appflow.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-appflow.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.cdk-appflow-0.0.7/README.md` & `cdklabs.cdk-appflow-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.7/setup.py` & `cdklabs.cdk-appflow-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-appflow",
-    "version": "0.0.7",
+    "version": "0.0.8",
     "description": "@cdklabs/cdk-appflow",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-appflow.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdklabs.cdk_appflow",
         "cdklabs.cdk_appflow._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_appflow._jsii": [
-            "cdk-appflow@0.0.7.jsii.tgz"
+            "cdk-appflow@0.0.8.jsii.tgz"
         ],
         "cdklabs.cdk_appflow": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdklabs.cdk-appflow-0.0.7/src/cdklabs/cdk_appflow/__init__.py` & `cdklabs.cdk-appflow-0.0.8/src/cdklabs/cdk_appflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.7/src/cdklabs.cdk_appflow.egg-info/PKG-INFO` & `cdklabs.cdk-appflow-0.0.8/src/cdklabs.cdk_appflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-appflow
-Version: 0.0.7
+Version: 0.0.8
 Summary: @cdklabs/cdk-appflow
 Home-page: https://github.com/cdklabs/cdk-appflow.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-appflow.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

