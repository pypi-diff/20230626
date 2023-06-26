# Comparing `tmp/cdktf-tf-module-stack-2.0.8.tar.gz` & `tmp/cdktf-tf-module-stack-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-tf-module-stack-2.0.8.tar", last modified: Tue Jan 31 00:26:12 2023, max compression
+gzip compressed data, was "cdktf-tf-module-stack-2.0.9.tar", last modified: Wed Feb  1 00:29:16 2023, max compression
```

## Comparing `cdktf-tf-module-stack-2.0.8.tar` & `cdktf-tf-module-stack-2.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:26:12.903476 cdktf-tf-module-stack-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-31 00:25:58.000000 cdktf-tf-module-stack-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-31 00:25:58.000000 cdktf-tf-module-stack-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-01-31 00:26:12.903476 cdktf-tf-module-stack-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-01-31 00:25:58.000000 cdktf-tf-module-stack-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-31 00:25:58.000000 cdktf-tf-module-stack-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 00:26:12.903476 cdktf-tf-module-stack-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-01-31 00:25:58.000000 cdktf-tf-module-stack-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:26:12.903476 cdktf-tf-module-stack-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:26:12.903476 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack/
--rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-01-31 00:25:58.000000 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:26:12.903476 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-31 00:25:58.000000 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36336 2023-01-31 00:25:58.000000 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack/_jsii/tf-module-stack@2.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 00:25:58.000000 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:26:12.903476 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-01-31 00:26:12.000000 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-31 00:26:12.000000 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 00:26:12.000000 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-31 00:26:12.000000 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 00:26:12.000000 cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:29:16.653287 cdktf-tf-module-stack-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-01 00:29:02.000000 cdktf-tf-module-stack-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-01 00:29:02.000000 cdktf-tf-module-stack-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-02-01 00:29:16.649287 cdktf-tf-module-stack-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-02-01 00:29:02.000000 cdktf-tf-module-stack-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-01 00:29:02.000000 cdktf-tf-module-stack-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 00:29:16.653287 cdktf-tf-module-stack-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-02-01 00:29:02.000000 cdktf-tf-module-stack-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:29:16.649287 cdktf-tf-module-stack-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:29:16.649287 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-02-01 00:29:02.000000 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:29:16.649287 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-01 00:29:02.000000 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36334 2023-02-01 00:29:02.000000 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack/_jsii/tf-module-stack@2.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 00:29:02.000000 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:29:16.649287 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-02-01 00:29:16.000000 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-01 00:29:16.000000 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 00:29:16.000000 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-01 00:29:16.000000 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-01 00:29:16.000000 cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack.egg-info/top_level.txt
```

### Comparing `cdktf-tf-module-stack-2.0.8/LICENSE` & `cdktf-tf-module-stack-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-tf-module-stack-2.0.8/PKG-INFO` & `cdktf-tf-module-stack-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-tf-module-stack
-Version: 2.0.8
+Version: 2.0.9
 Summary: A drop-in replacement for cdktf.TerraformStack that let's you define Terraform modules as construct
 Home-page: https://github.com/DanielMSchmidt/cdktf-tf-module-stack.git
 Author: Daniel Schmidt<danielmschmidt92@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DanielMSchmidt/cdktf-tf-module-stack.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdktf-tf-module-stack-2.0.8/README.md` & `cdktf-tf-module-stack-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-tf-module-stack-2.0.8/setup.py` & `cdktf-tf-module-stack-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-tf-module-stack",
-    "version": "2.0.8",
+    "version": "2.0.9",
     "description": "A drop-in replacement for cdktf.TerraformStack that let's you define Terraform modules as construct",
     "license": "Apache-2.0",
     "url": "https://github.com/DanielMSchmidt/cdktf-tf-module-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "Daniel Schmidt<danielmschmidt92@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_tf_module_stack",
         "cdktf_tf_module_stack._jsii"
     ],
     "package_data": {
         "cdktf_tf_module_stack._jsii": [
-            "tf-module-stack@2.0.8.jsii.tgz"
+            "tf-module-stack@2.0.9.jsii.tgz"
         ],
         "cdktf_tf_module_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack/__init__.py` & `cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-tf-module-stack-2.0.8/src/cdktf_tf_module_stack.egg-info/PKG-INFO` & `cdktf-tf-module-stack-2.0.9/src/cdktf_tf_module_stack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-tf-module-stack
-Version: 2.0.8
+Version: 2.0.9
 Summary: A drop-in replacement for cdktf.TerraformStack that let's you define Terraform modules as construct
 Home-page: https://github.com/DanielMSchmidt/cdktf-tf-module-stack.git
 Author: Daniel Schmidt<danielmschmidt92@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DanielMSchmidt/cdktf-tf-module-stack.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

