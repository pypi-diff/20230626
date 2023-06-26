# Comparing `tmp/titan-iris-0.8.4.tar.gz` & `tmp/titan-iris-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.8.4.tar", last modified: Mon Jun 26 10:54:13 2023, max compression
+gzip compressed data, was "titan-iris-0.8.5.tar", last modified: Mon Jun 26 11:36:14 2023, max compression
```

## Comparing `titan-iris-0.8.4.tar` & `titan-iris-0.8.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.920853 titan-iris-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 10:54:01.000000 titan-iris-0.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 10:54:01.000000 titan-iris-0.8.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 10:54:01.000000 titan-iris-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:54:13.920853 titan-iris-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 10:54:01.000000 titan-iris-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 10:54:01.000000 titan-iris-0.8.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 10:54:01.000000 titan-iris-0.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 10:54:01.000000 titan-iris-0.8.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 10:54:13.920853 titan-iris-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 10:54:01.000000 titan-iris-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.904853 titan-iris-0.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.912853 titan-iris-0.8.4/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.912853 titan-iris-0.8.4/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.916853 titan-iris-0.8.4/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-06-26 10:54:01.000000 titan-iris-0.8.4/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.916853 titan-iris-0.8.4/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 10:54:13.000000 titan-iris-0.8.4/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:54:13.920853 titan-iris-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 10:54:01.000000 titan-iris-0.8.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 10:54:01.000000 titan-iris-0.8.4/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:36:14.550314 titan-iris-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 11:35:56.000000 titan-iris-0.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 11:35:56.000000 titan-iris-0.8.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 11:35:56.000000 titan-iris-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 11:36:14.550314 titan-iris-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 11:35:56.000000 titan-iris-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 11:35:56.000000 titan-iris-0.8.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 11:35:56.000000 titan-iris-0.8.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 11:35:56.000000 titan-iris-0.8.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 11:36:14.550314 titan-iris-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 11:35:56.000000 titan-iris-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:36:14.534314 titan-iris-0.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:36:14.542314 titan-iris-0.8.5/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:36:14.542314 titan-iris-0.8.5/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:36:14.546314 titan-iris-0.8.5/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-06-26 11:35:56.000000 titan-iris-0.8.5/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:36:14.550314 titan-iris-0.8.5/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 11:36:14.000000 titan-iris-0.8.5/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 11:36:14.000000 titan-iris-0.8.5/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:36:14.000000 titan-iris-0.8.5/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 11:36:14.000000 titan-iris-0.8.5/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 11:36:14.000000 titan-iris-0.8.5/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 11:36:14.000000 titan-iris-0.8.5/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:36:14.550314 titan-iris-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 11:35:56.000000 titan-iris-0.8.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 11:35:56.000000 titan-iris-0.8.5/tests/test_sdk.py
```

### Comparing `titan-iris-0.8.4/.gitignore` & `titan-iris-0.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/Dockerfile` & `titan-iris-0.8.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/PKG-INFO` & `titan-iris-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.4
+Version: 0.8.5
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.4/README.md` & `titan-iris-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/setup.py` & `titan-iris-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/src/iris/config.yaml` & `titan-iris-0.8.5/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/src/iris/gradio/run.py` & `titan-iris-0.8.5/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/src/iris/main.py` & `titan-iris-0.8.5/src/iris/main.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/src/iris/sdk/auth_utils.py` & `titan-iris-0.8.5/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/src/iris/sdk/conf_manager.py` & `titan-iris-0.8.5/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/src/iris/sdk/exception.py` & `titan-iris-0.8.5/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/src/iris/sdk/iris_sdk.py` & `titan-iris-0.8.5/src/iris/sdk/iris_sdk.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/src/iris/sdk/safe_convert.py` & `titan-iris-0.8.5/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/src/iris/sdk/utils.py` & `titan-iris-0.8.5/src/iris/sdk/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -365,51 +365,55 @@
     Args:
         response (str): a json format response from the iris get endpoint.
     """
     json_response = json.loads(response)["response"]
     # check if 'experiments' in the response, this is for the common case 'iris get'
     if "experiments" in json_response:
         experiments = json_response["experiments"]
-
-        results_table = {}
-        for experiment in experiments:
-            extract_experiment_results(experiment, results_table)
-        # sort the results table by experiment id, get the most recent 5 experiments
-        sorted_results_table = dict(sorted(results_table.items(), key=lambda item: item[0], reverse=True)[:5])
-        print_get_dict_results(sorted_results_table)
-    # check if 'experiment' in the response, this is for the case 'iris get -i <experiment_id>'
+        if experiments:
+            results_table = {}
+            for experiment in experiments:
+                extract_experiment_results(experiment, results_table)
+            # sort the results table by experiment id, get the most recent 5 experiments
+            sorted_results_table = dict(sorted(results_table.items(), key=lambda item: item[0], reverse=True)[:5])
+            print_get_dict_results(sorted_results_table)
+        else:
+            print_status_dict_results(json_response)
     elif "experiment" in json_response:
         experiment = json_response["experiment"]
 
         results_table = {}
         extract_experiment_results(experiment, results_table)
         print_get_dict_results(results_table)
-    # check if 'artefacts' in the response, this is for the case 'iris get artefact'
     elif "artefacts" in json_response:
         artefacts = json_response["artefacts"]
-        results_table = {
-            artefact["uuid"]: {
-                "name": artefact["name"],
-                "type": artefact["artefact_type"],
+        if artefacts:
+            results_table = {
+                artefact["uuid"]: {
+                    "name": artefact["name"],
+                    "type": artefact["artefact_type"],
+                }
+                for artefact in artefacts
             }
-            for artefact in artefacts
-        }
-        print_get_dict_results(results_table, experiment=False, key_name="UUID")
-    # check if 'sessions' in the response, this is for the case 'iris get inference-session'
+            print_get_dict_results(results_table, experiment=False, key_name="UUID")
+        else:
+            print_status_dict_results(json_response)
     elif "sessions" in json_response:
         sessions = json_response["sessions"]
-        results_table = {
-            session["uuid"]: {
-                "model": session["model"],
-                "status": session["status"],
+        if sessions:
+            results_table = {
+                session["uuid"]: {
+                    "model": session["model"],
+                    "status": session["status"],
+                }
+                for session in sessions
             }
-            for session in sessions
-        }
-        print_get_dict_results(results_table, experiment=False, key_name="UUID")
-    # check if 'message' in the response, this is for the case 'iris status'
+            print_get_dict_results(results_table, experiment=False, key_name="UUID")
+        else:
+            print_status_dict_results(json_response)
     elif len(json_response) > 0 and len(json_response[0][0]) > 0 and "message" in json_response[0][0]:
         messages = json_response[0]
         results_table = {
             message["name"]: {
                 "status": message["status"],
                 "message": message["message"]["message"],
                 "progress": message["message"]["progress"],
```

### Comparing `titan-iris-0.8.4/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.8.5/src/titan_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.8.4
+Version: 0.8.5
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.8.4/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.8.5/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/tests/test_cli.py` & `titan-iris-0.8.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.8.4/tests/test_sdk.py` & `titan-iris-0.8.5/tests/test_sdk.py`

 * *Files identical despite different names*

