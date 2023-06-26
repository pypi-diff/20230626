# Comparing `tmp/titan-iris-0.8.0.tar.gz` & `tmp/titan-iris-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.8.0.tar", last modified: Mon Jun 26 09:55:36 2023, max compression
+gzip compressed data, was "titan-iris-0.8.1.tar", last modified: Mon Jun 26 10:00:23 2023, max compression
```

## Comparing `titan-iris-0.8.0.tar` & `titan-iris-0.8.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 09:55:22.000000 titan-iris-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 09:55:22.000000 titan-iris-0.8.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 09:55:22.000000 titan-iris-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 09:55:36.355721 titan-iris-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 09:55:22.000000 titan-iris-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 09:55:22.000000 titan-iris-0.8.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 09:55:22.000000 titan-iris-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 09:55:22.000000 titan-iris-0.8.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 09:55:36.355721 titan-iris-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 09:55:22.000000 titan-iris-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.351721 titan-iris-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 09:55:22.000000 titan-iris-0.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 09:55:22.000000 titan-iris-0.8.0/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.195843 titan-iris-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 10:00:08.000000 titan-iris-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 10:00:08.000000 titan-iris-0.8.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 10:00:08.000000 titan-iris-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:00:23.195843 titan-iris-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 10:00:08.000000 titan-iris-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 10:00:08.000000 titan-iris-0.8.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 10:00:08.000000 titan-iris-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 10:00:08.000000 titan-iris-0.8.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 10:00:23.195843 titan-iris-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 10:00:08.000000 titan-iris-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.187843 titan-iris-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.191843 titan-iris-0.8.1/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.191843 titan-iris-0.8.1/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.195843 titan-iris-0.8.1/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.195843 titan-iris-0.8.1/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.195843 titan-iris-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 10:00:08.000000 titan-iris-0.8.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 10:00:08.000000 titan-iris-0.8.1/tests/test_sdk.py
```

### Comparing `titan-iris-0.8.0/.gitignore` & `titan-iris-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/Dockerfile` & `titan-iris-0.8.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/PKG-INFO` & `titan-iris-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.0
+Version: 0.8.1
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.0/README.md` & `titan-iris-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/setup.py` & `titan-iris-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/iris/config.yaml` & `titan-iris-0.8.1/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/iris/gradio/run.py` & `titan-iris-0.8.1/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/iris/main.py` & `titan-iris-0.8.1/src/iris/main.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/iris/sdk/auth_utils.py` & `titan-iris-0.8.1/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/iris/sdk/conf_manager.py` & `titan-iris-0.8.1/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/iris/sdk/exception.py` & `titan-iris-0.8.1/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/iris/sdk/iris_sdk.py` & `titan-iris-0.8.1/src/iris/sdk/iris_sdk.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/iris/sdk/safe_convert.py` & `titan-iris-0.8.1/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/iris/sdk/utils.py` & `titan-iris-0.8.1/src/iris/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.8.1/src/titan_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.0
+Version: 0.8.1
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.0/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.8.1/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/tests/test_cli.py` & `titan-iris-0.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.0/tests/test_sdk.py` & `titan-iris-0.8.1/tests/test_sdk.py`

 * *Files identical despite different names*

