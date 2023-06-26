# Comparing `tmp/sorcerun-0.2.7.tar.gz` & `tmp/sorcerun-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.2.7.tar", last modified: Wed Jun 21 17:31:06 2023, max compression
+gzip compressed data, was "sorcerun-0.2.8.tar", last modified: Mon Jun 26 18:42:34 2023, max compression
```

## Comparing `sorcerun-0.2.7.tar` & `sorcerun-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:06.581747 sorcerun-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-21 17:30:55.000000 sorcerun-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 17:31:06.581747 sorcerun-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-21 17:30:55.000000 sorcerun-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:31:06.581747 sorcerun-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 17:30:55.000000 sorcerun-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:06.577747 sorcerun-0.2.7/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 17:31:06.000000 sorcerun-0.2.7/sorcerun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:06.581747 sorcerun-0.2.7/sorcerun_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-21 17:30:55.000000 sorcerun-0.2.7/sorcerun_package/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:42:34.028813 sorcerun-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-26 18:42:20.000000 sorcerun-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-26 18:42:34.028813 sorcerun-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-26 18:42:20.000000 sorcerun-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:42:34.028813 sorcerun-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-26 18:42:20.000000 sorcerun-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:42:34.024813 sorcerun-0.2.8/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 18:42:34.000000 sorcerun-0.2.8/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:42:34.028813 sorcerun-0.2.8/sorcerun_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-26 18:42:20.000000 sorcerun-0.2.8/sorcerun_package/sacred_utils.py
```

### Comparing `sorcerun-0.2.7/LICENSE` & `sorcerun-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.7/PKG-INFO` & `sorcerun-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.7
+Version: 0.2.8
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.7/README.md` & `sorcerun-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.7/setup.py` & `sorcerun-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.2.7",
+    version="0.2.8",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred==0.8.4",
         "pymongo",
         "pyyaml",
```

### Comparing `sorcerun-0.2.7/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.2.8/sorcerun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.7
+Version: 0.2.8
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.7/sorcerun_package/auth_mongodb_option.py` & `sorcerun-0.2.8/sorcerun_package/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.7/sorcerun_package/cli.py` & `sorcerun-0.2.8/sorcerun_package/cli.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.7/sorcerun_package/mongodb_utils.py` & `sorcerun-0.2.8/sorcerun_package/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.7/sorcerun_package/sacred_utils.py` & `sorcerun-0.2.8/sorcerun_package/sacred_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 from sacred import Experiment
 from sacred.observers import MongoObserver
 import importlib
 import json
 from .globals import AUTH_FILE
+import sys
+import os
 
 
 def load_adapter_function(python_file):
-    spec = importlib.util.spec_from_file_location("adapter_module", python_file)
-    adapter_module = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(adapter_module)
+    # spec = importlib.util.spec_from_file_location("adapter_module", python_file)
+    # adapter_module = importlib.util.module_from_spec(spec)
+    # spec.loader.exec_module(adapter_module)
+
+    adapter_file_dir = os.path.dirname(os.path.abspath(python_file))
+    adapter_file_name = os.path.basename(python_file).replace(".py", "")
+
+    sys.path.insert(0, adapter_file_dir)
+    adapter_module = importlib.import_module(adapter_file_name)
+    sys.path.pop(0)
     adapter_func = adapter_module.adapter
+
     return adapter_func
 
 
 def run_sacred_experiment(adapter_func, config, auth_path=AUTH_FILE):
     experiment_name = getattr(adapter_func, "experiment_name", "sorcerun_experiment")
     ex = Experiment(experiment_name)
```

