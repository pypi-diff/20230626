# Comparing `tmp/titan-iris-0.8.3.tar.gz` & `tmp/titan-iris-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.8.3.tar", last modified: Mon Jun 26 10:31:01 2023, max compression
+gzip compressed data, was "titan-iris-0.8.4.tar", last modified: Mon Jun 26 10:54:13 2023, max compression
```

## Comparing `titan-iris-0.8.3.tar` & `titan-iris-0.8.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:31:01.213203 titan-iris-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 10:30:47.000000 titan-iris-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 10:30:47.000000 titan-iris-0.8.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 10:30:47.000000 titan-iris-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:31:01.213203 titan-iris-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 10:30:47.000000 titan-iris-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 10:30:47.000000 titan-iris-0.8.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 10:30:47.000000 titan-iris-0.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 10:30:47.000000 titan-iris-0.8.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 10:31:01.213203 titan-iris-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 10:30:47.000000 titan-iris-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:31:01.209203 titan-iris-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:31:01.213203 titan-iris-0.8.3/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:31:01.213203 titan-iris-0.8.3/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:31:01.213203 titan-iris-0.8.3/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-06-26 10:30:47.000000 titan-iris-0.8.3/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:31:01.213203 titan-iris-0.8.3/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:31:01.000000 titan-iris-0.8.3/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 10:31:01.000000 titan-iris-0.8.3/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:31:01.000000 titan-iris-0.8.3/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 10:31:01.000000 titan-iris-0.8.3/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 10:31:01.000000 titan-iris-0.8.3/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 10:31:01.000000 titan-iris-0.8.3/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:31:01.213203 titan-iris-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 10:30:47.000000 titan-iris-0.8.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 10:30:47.000000 titan-iris-0.8.3/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.920853 titan-iris-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 10:54:01.000000 titan-iris-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 10:54:01.000000 titan-iris-0.8.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 10:54:01.000000 titan-iris-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:54:13.920853 titan-iris-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 10:54:01.000000 titan-iris-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 10:54:01.000000 titan-iris-0.8.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 10:54:01.000000 titan-iris-0.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 10:54:01.000000 titan-iris-0.8.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 10:54:13.920853 titan-iris-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 10:54:01.000000 titan-iris-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.904853 titan-iris-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.912853 titan-iris-0.8.4/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.912853 titan-iris-0.8.4/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.916853 titan-iris-0.8.4/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.916853 titan-iris-0.8.4/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.920853 titan-iris-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 10:54:01.000000 titan-iris-0.8.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 10:54:01.000000 titan-iris-0.8.4/tests/test_sdk.py
```

### Comparing `titan-iris-0.8.3/.gitignore` & `titan-iris-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/Dockerfile` & `titan-iris-0.8.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/PKG-INFO` & `titan-iris-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.3
+Version: 0.8.4
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.3/README.md` & `titan-iris-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/setup.py` & `titan-iris-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/iris/config.yaml` & `titan-iris-0.8.4/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/iris/gradio/run.py` & `titan-iris-0.8.4/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/iris/main.py` & `titan-iris-0.8.4/src/iris/main.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/iris/sdk/auth_utils.py` & `titan-iris-0.8.4/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/iris/sdk/conf_manager.py` & `titan-iris-0.8.4/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/iris/sdk/exception.py` & `titan-iris-0.8.4/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/iris/sdk/iris_sdk.py` & `titan-iris-0.8.4/src/iris/sdk/iris_sdk.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/iris/sdk/safe_convert.py` & `titan-iris-0.8.4/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/iris/sdk/utils.py` & `titan-iris-0.8.4/src/iris/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.8.4/src/titan_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.3
+Version: 0.8.4
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.3/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.8.4/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/tests/test_cli.py` & `titan-iris-0.8.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.3/tests/test_sdk.py` & `titan-iris-0.8.4/tests/test_sdk.py`

 * *Files identical despite different names*

