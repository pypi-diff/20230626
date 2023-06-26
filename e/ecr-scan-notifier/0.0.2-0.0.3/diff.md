# Comparing `tmp/ecr-scan-notifier-0.0.2.tar.gz` & `tmp/ecr-scan-notifier-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecr-scan-notifier-0.0.2.tar", last modified: Mon Jun 19 08:12:46 2023, max compression
+gzip compressed data, was "ecr-scan-notifier-0.0.3.tar", last modified: Mon Jun 26 16:05:30 2023, max compression
```

## Comparing `ecr-scan-notifier-0.0.2.tar` & `ecr-scan-notifier-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:12:46.346728 ecr-scan-notifier-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-19 08:12:29.000000 ecr-scan-notifier-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 08:12:29.000000 ecr-scan-notifier-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-19 08:12:46.346728 ecr-scan-notifier-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-19 08:12:29.000000 ecr-scan-notifier-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-19 08:12:29.000000 ecr-scan-notifier-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:12:46.346728 ecr-scan-notifier-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-19 08:12:29.000000 ecr-scan-notifier-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:12:46.346728 ecr-scan-notifier-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:12:46.346728 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-19 08:12:29.000000 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:12:46.346728 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-19 08:12:29.000000 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-06-19 08:12:29.000000 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier/_jsii/ecr-scan-notifier@0.0.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:12:29.000000 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:12:46.346728 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-19 08:12:46.000000 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 08:12:46.000000 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:12:46.000000 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 08:12:46.000000 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 08:12:46.000000 ecr-scan-notifier-0.0.2/src/ecr_scan_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.836645 ecr-scan-notifier-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-26 16:05:30.836645 ecr-scan-notifier-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:05:30.836645 ecr-scan-notifier-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.832644 ecr-scan-notifier-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.832644 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.832644 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/_jsii/ecr-scan-notifier@0.0.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.832644 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/top_level.txt
```

### Comparing `ecr-scan-notifier-0.0.2/LICENSE` & `ecr-scan-notifier-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecr-scan-notifier-0.0.2/PKG-INFO` & `ecr-scan-notifier-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecr-scan-notifier
-Version: 0.0.2
+Version: 0.0.3
 Summary: Notifies on new AWS ECR scan results
 Home-page: https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Author: Stefan Freitag<stefan.freitag@rwe.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `ecr-scan-notifier-0.0.2/README.md` & `ecr-scan-notifier-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ecr-scan-notifier-0.0.2/setup.py` & `ecr-scan-notifier-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ecr-scan-notifier",
-    "version": "0.0.2",
+    "version": "0.0.3",
     "description": "Notifies on new AWS ECR scan results",
     "license": "Apache-2.0",
     "url": "https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@rwe.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "ecr_scan_notifier",
         "ecr_scan_notifier._jsii"
     ],
     "package_data": {
         "ecr_scan_notifier._jsii": [
-            "ecr-scan-notifier@0.0.2.jsii.tgz"
+            "ecr-scan-notifier@0.0.3.jsii.tgz"
         ],
         "ecr_scan_notifier": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ecr-scan-notifier-0.0.2/src/ecr_scan_notifier/__init__.py` & `ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `ecr-scan-notifier-0.0.2/src/ecr_scan_notifier.egg-info/PKG-INFO` & `ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecr-scan-notifier
-Version: 0.0.2
+Version: 0.0.3
 Summary: Notifies on new AWS ECR scan results
 Home-page: https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Author: Stefan Freitag<stefan.freitag@rwe.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

