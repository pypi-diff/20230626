# Comparing `tmp/cdk-image-pipeline-0.3.4.tar.gz` & `tmp/cdk-image-pipeline-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-image-pipeline-0.3.4.tar", last modified: Thu Jun  8 00:48:14 2023, max compression
+gzip compressed data, was "cdk-image-pipeline-0.3.5.tar", last modified: Mon Jun 26 15:36:49 2023, max compression
```

## Comparing `cdk-image-pipeline-0.3.4.tar` & `cdk-image-pipeline-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:48:14.951472 cdk-image-pipeline-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-08 00:48:03.000000 cdk-image-pipeline-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 00:48:03.000000 cdk-image-pipeline-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-08 00:48:14.951472 cdk-image-pipeline-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-08 00:48:03.000000 cdk-image-pipeline-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 00:48:03.000000 cdk-image-pipeline-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:48:14.951472 cdk-image-pipeline-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-08 00:48:03.000000 cdk-image-pipeline-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:48:14.951472 cdk-image-pipeline-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:48:14.951472 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-06-08 00:48:03.000000 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:48:14.951472 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-08 00:48:03.000000 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-06-08 00:48:03.000000 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.3.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:48:03.000000 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:48:14.951472 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-08 00:48:14.000000 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-08 00:48:14.000000 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:48:14.000000 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 00:48:14.000000 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 00:48:14.000000 cdk-image-pipeline-0.3.4/src/cdk_image_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:36:49.644778 cdk-image-pipeline-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-26 15:36:37.000000 cdk-image-pipeline-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 15:36:37.000000 cdk-image-pipeline-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-26 15:36:49.644778 cdk-image-pipeline-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-26 15:36:37.000000 cdk-image-pipeline-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 15:36:37.000000 cdk-image-pipeline-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:36:49.644778 cdk-image-pipeline-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-26 15:36:37.000000 cdk-image-pipeline-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:36:49.640778 cdk-image-pipeline-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:36:49.640778 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-06-26 15:36:37.000000 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:36:49.644778 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-26 15:36:37.000000 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28188 2023-06-26 15:36:37.000000 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.3.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:36:37.000000 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:36:49.640778 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-26 15:36:49.000000 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-26 15:36:49.000000 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:36:49.000000 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-26 15:36:49.000000 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 15:36:49.000000 cdk-image-pipeline-0.3.5/src/cdk_image_pipeline.egg-info/top_level.txt
```

### Comparing `cdk-image-pipeline-0.3.4/LICENSE` & `cdk-image-pipeline-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.3.4/PKG-INFO` & `cdk-image-pipeline-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.3.4
+Version: 0.3.5
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-image-pipeline-0.3.4/README.md` & `cdk-image-pipeline-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.3.4/setup.py` & `cdk-image-pipeline-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-image-pipeline",
-    "version": "0.3.4",
+    "version": "0.3.5",
     "description": "Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK",
     "license": "MIT-0",
     "url": "https://github.com/aws-samples/cdk-image-pipeline.git",
     "long_description_content_type": "text/markdown",
     "author": "Cameron Magee<magcamer@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cdk_image_pipeline",
         "cdk_image_pipeline._jsii"
     ],
     "package_data": {
         "cdk_image_pipeline._jsii": [
-            "cdk-image-pipeline@0.3.4.jsii.tgz"
+            "cdk-image-pipeline@0.3.5.jsii.tgz"
         ],
         "cdk_image_pipeline": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.82.0, <3.0.0",
-        "constructs>=10.1.215, <11.0.0",
+        "constructs>=10.2.60, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cdk-image-pipeline-0.3.4/src/cdk_image_pipeline/__init__.py` & `cdk-image-pipeline-0.3.5/src/cdk_image_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.3.4/src/cdk_image_pipeline.egg-info/PKG-INFO` & `cdk-image-pipeline-0.3.5/src/cdk_image_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.3.4
+Version: 0.3.5
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

