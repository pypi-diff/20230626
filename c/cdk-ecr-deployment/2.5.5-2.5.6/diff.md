# Comparing `tmp/cdk-ecr-deployment-2.5.5.tar.gz` & `tmp/cdk-ecr-deployment-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-ecr-deployment-2.5.5.tar", last modified: Sun May 29 04:46:45 2022, max compression
+gzip compressed data, was "cdk-ecr-deployment-2.5.6.tar", last modified: Sun Sep  4 12:37:11 2022, max compression
```

## Comparing `cdk-ecr-deployment-2.5.5.tar` & `cdk-ecr-deployment-2.5.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 04:46:45.382641 cdk-ecr-deployment-2.5.5/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     4905 2022-05-29 04:46:45.382641 cdk-ecr-deployment-2.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 04:46:45.382641 cdk-ecr-deployment-2.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 04:46:45.378641 cdk-ecr-deployment-2.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 04:46:45.378641 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment/
--rw-r--r--   0 runner    (1001) docker     (121)    17114 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 04:46:45.378641 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  1030819 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment/_jsii/cdk-ecr-deployment@2.5.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 04:46:32.000000 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 04:46:45.378641 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4905 2022-05-29 04:46:44.000000 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-05-29 04:46:45.000000 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 04:46:44.000000 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-29 04:46:45.000000 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-29 04:46:45.000000 cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:37:11.951699 cdk-ecr-deployment-2.5.6/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)     4905 2022-09-04 12:37:11.951699 cdk-ecr-deployment-2.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-04 12:37:11.951699 cdk-ecr-deployment-2.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:37:11.947699 cdk-ecr-deployment-2.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:37:11.947699 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment/
+-rw-r--r--   0 runner    (1001) docker     (121)    17114 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:37:11.947699 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)  1030910 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment/_jsii/cdk-ecr-deployment@2.5.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 12:37:00.000000 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:37:11.947699 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4905 2022-09-04 12:37:11.000000 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-04 12:37:11.000000 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 12:37:11.000000 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-04 12:37:11.000000 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-04 12:37:11.000000 cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment.egg-info/top_level.txt
```

### Comparing `cdk-ecr-deployment-2.5.5/LICENSE` & `cdk-ecr-deployment-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-ecr-deployment-2.5.5/PKG-INFO` & `cdk-ecr-deployment-2.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-ecr-deployment
-Version: 2.5.5
+Version: 2.5.6
 Summary: CDK construct to deploy docker image to Amazon ECR
 Home-page: https://github.com/cdklabs/cdk-ecr-deployment
 Author: wchaws
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecr-deployment
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-ecr-deployment-2.5.5/README.md` & `cdk-ecr-deployment-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `cdk-ecr-deployment-2.5.5/setup.py` & `cdk-ecr-deployment-2.5.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-ecr-deployment",
-    "version": "2.5.5",
+    "version": "2.5.6",
     "description": "CDK construct to deploy docker image to Amazon ECR",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-ecr-deployment",
     "long_description_content_type": "text/markdown",
     "author": "wchaws",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_ecr_deployment",
         "cdk_ecr_deployment._jsii"
     ],
     "package_data": {
         "cdk_ecr_deployment._jsii": [
-            "cdk-ecr-deployment@2.5.5.jsii.tgz"
+            "cdk-ecr-deployment@2.5.6.jsii.tgz"
         ],
         "cdk_ecr_deployment": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment/__init__.py` & `cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-ecr-deployment-2.5.5/src/cdk_ecr_deployment.egg-info/PKG-INFO` & `cdk-ecr-deployment-2.5.6/src/cdk_ecr_deployment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-ecr-deployment
-Version: 2.5.5
+Version: 2.5.6
 Summary: CDK construct to deploy docker image to Amazon ECR
 Home-page: https://github.com/cdklabs/cdk-ecr-deployment
 Author: wchaws
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecr-deployment
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

