# Comparing `tmp/mlpype-tensorflow-0.4.4.tar.gz` & `tmp/mlpype-tensorflow-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-tensorflow-0.4.4.tar", last modified: Fri Jun 23 09:48:22 2023, max compression
+gzip compressed data, was "mlpype-tensorflow-0.4.5.tar", last modified: Mon Jun 26 20:43:18 2023, max compression
```

## Comparing `mlpype-tensorflow-0.4.4.tar` & `mlpype-tensorflow-0.4.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:22.764137 mlpype-tensorflow-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 09:48:22.764137 mlpype-tensorflow-0.4.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:22.764137 mlpype-tensorflow-0.4.4/mlpype_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 09:48:22.000000 mlpype-tensorflow-0.4.4/mlpype_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-23 09:48:22.000000 mlpype-tensorflow-0.4.4/mlpype_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:22.000000 mlpype-tensorflow-0.4.4/mlpype_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 09:48:22.000000 mlpype-tensorflow-0.4.4/mlpype_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:22.000000 mlpype-tensorflow-0.4.4/mlpype_tensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:48:22.764137 mlpype-tensorflow-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-23 09:44:01.000000 mlpype-tensorflow-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:43:18.433615 mlpype-tensorflow-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 20:43:18.433615 mlpype-tensorflow-0.4.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:43:18.433615 mlpype-tensorflow-0.4.5/mlpype_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 20:43:18.000000 mlpype-tensorflow-0.4.5/mlpype_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 20:43:18.000000 mlpype-tensorflow-0.4.5/mlpype_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:43:18.000000 mlpype-tensorflow-0.4.5/mlpype_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-26 20:43:18.000000 mlpype-tensorflow-0.4.5/mlpype_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:43:18.000000 mlpype-tensorflow-0.4.5/mlpype_tensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:43:18.433615 mlpype-tensorflow-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 20:39:45.000000 mlpype-tensorflow-0.4.5/setup.py
```

### Comparing `mlpype-tensorflow-0.4.4/setup.py` & `mlpype-tensorflow-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.4"
+    version = "0.4.5"
 
     deps = [
         f"mlpype-base=={version}",
         # on mac, it is recommended to use conda/mamba or source to install tensorflow
         "tensorflow>=2.12",
         "numpy>=1.23.0",
         "protobuf>=3.20.3",
```

