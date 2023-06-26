# Comparing `tmp/titan-iris-0.8.1.tar.gz` & `tmp/titan-iris-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.8.1.tar", last modified: Mon Jun 26 10:00:23 2023, max compression
+gzip compressed data, was "titan-iris-0.8.2.tar", last modified: Mon Jun 26 10:06:09 2023, max compression
```

## Comparing `titan-iris-0.8.1.tar` & `titan-iris-0.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.195843 titan-iris-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 10:00:08.000000 titan-iris-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 10:00:08.000000 titan-iris-0.8.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 10:00:08.000000 titan-iris-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:00:23.195843 titan-iris-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 10:00:08.000000 titan-iris-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 10:00:08.000000 titan-iris-0.8.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 10:00:08.000000 titan-iris-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 10:00:08.000000 titan-iris-0.8.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 10:00:23.195843 titan-iris-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 10:00:08.000000 titan-iris-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.187843 titan-iris-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.191843 titan-iris-0.8.1/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.191843 titan-iris-0.8.1/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.195843 titan-iris-0.8.1/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-06-26 10:00:08.000000 titan-iris-0.8.1/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.195843 titan-iris-0.8.1/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 10:00:23.000000 titan-iris-0.8.1/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:00:23.195843 titan-iris-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 10:00:08.000000 titan-iris-0.8.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 10:00:08.000000 titan-iris-0.8.1/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:06:09.641380 titan-iris-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 10:05:55.000000 titan-iris-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 10:05:55.000000 titan-iris-0.8.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 10:05:55.000000 titan-iris-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:06:09.641380 titan-iris-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 10:05:55.000000 titan-iris-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 10:05:55.000000 titan-iris-0.8.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 10:05:55.000000 titan-iris-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 10:05:55.000000 titan-iris-0.8.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 10:06:09.641380 titan-iris-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 10:05:55.000000 titan-iris-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:06:09.629380 titan-iris-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:06:09.633380 titan-iris-0.8.2/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:06:09.633380 titan-iris-0.8.2/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:06:09.637380 titan-iris-0.8.2/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-06-26 10:05:55.000000 titan-iris-0.8.2/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:06:09.637380 titan-iris-0.8.2/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:06:09.000000 titan-iris-0.8.2/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 10:06:09.000000 titan-iris-0.8.2/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:06:09.000000 titan-iris-0.8.2/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 10:06:09.000000 titan-iris-0.8.2/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 10:06:09.000000 titan-iris-0.8.2/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 10:06:09.000000 titan-iris-0.8.2/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:06:09.641380 titan-iris-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 10:05:55.000000 titan-iris-0.8.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 10:05:55.000000 titan-iris-0.8.2/tests/test_sdk.py
```

### Comparing `titan-iris-0.8.1/.gitignore` & `titan-iris-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/Dockerfile` & `titan-iris-0.8.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/PKG-INFO` & `titan-iris-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.1
+Version: 0.8.2
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.1/README.md` & `titan-iris-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/setup.py` & `titan-iris-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/iris/config.yaml` & `titan-iris-0.8.2/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/iris/gradio/run.py` & `titan-iris-0.8.2/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/iris/main.py` & `titan-iris-0.8.2/src/iris/main.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/iris/sdk/auth_utils.py` & `titan-iris-0.8.2/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/iris/sdk/conf_manager.py` & `titan-iris-0.8.2/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/iris/sdk/exception.py` & `titan-iris-0.8.2/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/iris/sdk/iris_sdk.py` & `titan-iris-0.8.2/src/iris/sdk/iris_sdk.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/iris/sdk/safe_convert.py` & `titan-iris-0.8.2/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/iris/sdk/utils.py` & `titan-iris-0.8.2/src/iris/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.8.2/src/titan_iris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.1
+Version: 0.8.2
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.1/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.8.2/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/tests/test_cli.py` & `titan-iris-0.8.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.1/tests/test_sdk.py` & `titan-iris-0.8.2/tests/test_sdk.py`

 * *Files identical despite different names*

