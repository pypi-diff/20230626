# Comparing `tmp/titan-iris-0.7.1.dev82.tar.gz` & `tmp/titan-iris-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.7.1.dev82.tar", last modified: Wed Jun 21 16:31:49 2023, max compression
+gzip compressed data, was "titan-iris-0.8.0.tar", last modified: Mon Jun 26 09:55:36 2023, max compression
```

## Comparing `titan-iris-0.7.1.dev82.tar` & `titan-iris-0.8.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.832139 titan-iris-0.7.1.dev82/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.832139 titan-iris-0.7.1.dev82/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.832139 titan-iris-0.7.1.dev82/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    27220 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.832139 titan-iris-0.7.1.dev82/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 09:55:22.000000 titan-iris-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 09:55:22.000000 titan-iris-0.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 09:55:22.000000 titan-iris-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 09:55:36.355721 titan-iris-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-26 09:55:22.000000 titan-iris-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 09:55:22.000000 titan-iris-0.8.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 09:55:22.000000 titan-iris-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 09:55:22.000000 titan-iris-0.8.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 09:55:36.355721 titan-iris-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 09:55:22.000000 titan-iris-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.351721 titan-iris-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-06-26 09:55:22.000000 titan-iris-0.8.0/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 09:55:36.000000 titan-iris-0.8.0/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:36.355721 titan-iris-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 09:55:22.000000 titan-iris-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 09:55:22.000000 titan-iris-0.8.0/tests/test_sdk.py
```

### Comparing `titan-iris-0.7.1.dev82/.gitignore` & `titan-iris-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/Dockerfile` & `titan-iris-0.8.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/PKG-INFO` & `titan-iris-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.7.1.dev82
+Version: 0.8.0
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.7.1.dev82/README.md` & `titan-iris-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/setup.py` & `titan-iris-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/src/iris/config.yaml` & `titan-iris-0.8.0/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/src/iris/gradio/run.py` & `titan-iris-0.8.0/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/src/iris/main.py` & `titan-iris-0.8.0/src/iris/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import typer
 import yaml
 from trogon import Trogon
 from typer.main import get_group
 import iris.sdk as sdk
 
-from .sdk.utils import exception_to_json_error, json_output_decorator, valid_qlora
+from .sdk.utils import exception_to_json_error, valid_qlora
 
 logger = getLogger(__name__)
 logger.setLevel(sdk.conf_mgr.LOG_LEVEL)
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                   sdk CLI Module                                                     #
 
@@ -568,16 +568,17 @@
     ),
     json_output: bool = JSON_ARG,
 ):
     """Delete objects from the TitanML store."""
     # delete the string from the enum
     object = object.value
     try:
-        sdk.delete(object, id, verbose=True, json_output=json_output)
-    except Exception:
+        sdk.delete(object, id, json_output=json_output)
+    except Exception as e:
+        print(exception_to_json_error(e))
         raise typer.Abort()
 
 
 @main.command()
 def pull(
     image: str = typer.Argument(..., help="The image to pull. Should be displayed in the TitanML Hub."),
     json_output: bool = JSON_ARG,
@@ -632,24 +633,24 @@
     url = f"{target}:{port}"
 
     try:
         if task == "sequence_classification":
             if context is None or context != "":
                 print("context is not necessary for classification tasks")
                 raise typer.Abort()
-            res = sdk.infer(url, task, runtime, text)
+            res = sdk.infer(url=url, task_name=task, runtime=runtime, text=text)
             print(res)
         elif task == "question_answering":
             if context is None or context == "":
                 print("context is required for question answering tasks")
                 raise typer.Abort()
             if len(text) != 1:
                 print("text should only contain one question")
                 raise typer.Abort()
-            res = sdk.infer(url, task, runtime, text, context)
+            res = sdk.infer(url=url, task_name=task, runtime=runtime, text=text, context=context)
             print(res)
         else:
             print(f"Unrecognised task {task}")
             raise typer.Abort()
     except Exception as e:
         json_error = exception_to_json_error(e)
         print(json_error)
@@ -701,29 +702,28 @@
         sdk.upload(name, src, description, json_output=json_output)
     except Exception as e:
         json_error = exception_to_json_error(e)
         print(json_error)
         raise typer.Abort()
 
 
-@json_output_decorator
 @main.command()
 def status(
     id: str = typer.Option(..., "--id", "-i", help="The id of the experiment to get the status of"),
     headers: List[str] = HEADERS_ARG,
     json_output: bool = JSON_ARG,
 ):
     """Get the status of an experiment."""
     headers = {x.partition(":")[0]: x.partition(":")[-1] for x in headers}
     summary = ""
     try:
         summary = sdk.get(
             "experiment",
             id,
-            "experiment.jobs[*].{name:name, status:status, message:message, results:results}",
+            "experiment.jobs[*].tasks[*].{name:name, status:status, message:message}",
             headers,
             json_output=json_output,
         )
         return summary
     except Exception:
         raise typer.Abort()
```

### Comparing `titan-iris-0.7.1.dev82/src/iris/sdk/auth_utils.py` & `titan-iris-0.8.0/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/src/iris/sdk/conf_manager.py` & `titan-iris-0.8.0/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/src/iris/sdk/exception.py` & `titan-iris-0.8.0/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/src/iris/sdk/iris_sdk.py` & `titan-iris-0.8.0/src/iris/sdk/iris_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 # for iris infer
 import numpy as np
 
 # for iris pull
 import requests
 import tritonclient.http
 from rich import print
-from rich.console import Console
-from rich.table import Table
 
 # internal imports
 from .auth_utils import auth, handle_bad_response
 from .conf_manager import conf_mgr
 from .exception import (
     ArtefactNotFoundError,
     ArtefactTypeInferError,
@@ -35,16 +33,17 @@
     UnknownFamilyError,
     UnsafeTensorsError,
     UploadOnPostError,
 )
 from .utils import (
     download_model,
     dump,
-    json_output_decorator,
+    handle_iris_get_response,
     make_targz,
+    print_status_dict_results,
     pull_image,
     telemetry_decorator,
     upload_from_file,
 )
 
 try:
     from importlib import metadata
@@ -99,15 +98,14 @@
 
 
 # --------------------------------------      iris post     -------------------------------------- #
 
 
 @auth
 @telemetry_decorator
-@json_output_decorator
 def post(
     headers: dict = None,
     json_output: bool = False,
     **flags: dict,
 ) -> None:
     """Dispatch a job to iris.
 
@@ -147,92 +145,93 @@
                 raise UploadOnPostError
 
     headers.update({"Authorization": f"Bearer {conf_mgr.access_token}"})
     response = requests.post(url=url, headers=headers, data=payload)
     if not response.ok:
         raise handle_bad_response(response, endpoint)  # already returns json object
     else:
+        dumped_response = dump(response)
         if json_output:
-            return dump(response)
+            print(dumped_response)
+            return dumped_response
         else:
-            return response
+            print_status_dict_results(json.loads(dumped_response)["response"])
+            return dumped_response
 
 
 # --------------------------------------       iris get     -------------------------------------- #
 
 
 @auth
 @telemetry_decorator
-@json_output_decorator
 def get(
     object: str = "experiment",
     id: Optional[str] = None,
     query: Optional[str] = None,
     headers: dict = None,
-    verbose: bool = True,
     json_output: bool = False,
 ):
     """Get objects from the TitanML Store.
 
     Args:
         object (str, optional): The object to get. Defaults to "experiment".
         id (Optional[str], optional): The id of the object. Defaults to None.
         query (Optional[str], optional): A JMESPath query to run against the returned json.
                                          Defaults to None, i.e. return everything.
         headers (dict): Custom headers to send with the get request
-        verbose (bool): Whether to print the response
         json_output (bool): Whether to return the response as a json object
 
     Returns:
         (str) A json response, formatted as: {"status": <http_response>, "response": <queried_json_response>}
     """
     if headers is None:
         headers = {}
 
     logger.debug(f"Getting from ... {conf_mgr.base}, auth from {conf_mgr.AUTH0_DOMAIN}")
     logger.debug(f"Applying custom headers {headers}")
-    endpoint = str(object) + "/"
+    endpoint = f"{object}/"
     if id:
         endpoint += id
     url = urljoin(conf_mgr.runner_url, endpoint)
     headers.update({"Authorization": f"Bearer {conf_mgr.access_token}"})
 
     response = requests.get(url=url, headers=headers)
-
     if not response.ok:
         raise handle_bad_response(response, url)
-    else:
-        try:
-            dumped_response = dump(response, query)
-            return dumped_response
-        except json.JSONDecodeError:
-            print("JSON decoding error occurred.")
-            print(response)
-            return None
+    try:
+        # get the response as a json object, this will make sure the response is valid json
+        dumped_response = dump(response, query)
+        if json_output:
+            print(dumped_response)
+        else:
+            # better user information display, return the response in a prettier table format
+            # this func only turns a valid json response into a table
+            handle_iris_get_response(dumped_response)
+        return dumped_response
+    except json.JSONDecodeError:
+        print("JSON decoding error occurred.")
+        print(response)
+        return None
 
 
 # --------------------------------------     iris delete    -------------------------------------- #
 
-console = Console()
-
 
 @auth
 @telemetry_decorator
 def delete(
     object: str,
     id: Optional[str],
-    verbose: bool = True,
     json_output: bool = False,
 ):
     """Get objects from the TitanML Store.
 
     Args:
         object (str, optional): The object to get. Defaults to "experiment".
         id (str): The id of the object to delete
-        verbose (bool, optional): Whether to print the response. Defaults to True.
         json_output (bool, optional): Whether to return the response as a json object. Defaults to False.
 
     Returns:
         (str) A json response, formatted as:
         {"status": <http_response>, "response": <queried_json_response>}
     """
     logger.debug(f"Getting from ... {conf_mgr.base}, auth from {conf_mgr.AUTH0_DOMAIN}")
@@ -241,22 +240,20 @@
     headers = {"Authorization": f"Bearer {conf_mgr.access_token}"}
 
     response = requests.delete(url=url, headers=headers)
     if not response.ok:
         raise handle_bad_response(response, endpoint)
     else:
         if response.status_code == 204:
+            response_message = {"status": "success", "response": "deleted"}
             if json_output:
-                result = json.dumps({"status": "success"}, indent=4)
+                result = json.dumps(response_message, indent=4)
                 print(result)
             else:
-                table = Table(show_header=True, header_style="bold magenta")
-                table.add_column("Status", style="dim", width=12)
-                table.add_row("success")
-                console.print(table)
+                print_status_dict_results(response_message)
         return None
 
 
 # --------------------------------------     iris download  -------------------------------------- #
 
 
 @auth
```

### Comparing `titan-iris-0.7.1.dev82/src/iris/sdk/safe_convert.py` & `titan-iris-0.8.0/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/src/iris/sdk/utils.py` & `titan-iris-0.8.0/src/iris/sdk/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 import functools
 import gzip
 import io
 import json
 import tarfile
 from logging import getLogger
 from pathlib import Path
-from typing import Callable, Optional
+from typing import Callable, Mapping, Optional
 
 import docker
 import jmespath
 import requests
 import wget
-from rich.console import Console
 from rich.progress import Progress
-from rich.table import Table
+from tabulate import tabulate
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
 from iris.sdk.exception import DownloadLinkNotFoundError
 
 from .conf_manager import conf_mgr
 
@@ -75,15 +74,14 @@
 
     # Copy the tar archive into the container
     container.put_archive(image_folder_path, tar_buffer)
 
 
 def show_progress(line, progress, tasks):  # sourcery skip: avoid-builtin-shadow
     """Show task progress for docker pull command (red for download, green for extract)."""
-    print(line["status"])
     if line["status"] == "Downloading":
         id = f'[red][Download {line["id"]}]'
     elif line["status"] == "Extracting":
         id = f'[green][Extract  {line["id"]}]'
     else:
         # skip other statuses
         return
@@ -264,114 +262,167 @@
     logger.error(e)
     error_dict = {"status": "failed", "error": str(e), "type": type(e).__name__}
     if hasattr(e, "status_code"):
         error_dict["status_code"] = e.status_code
     return json.dumps(error_dict, indent=4)
 
 
-console = Console()
+def flatten_dict(dict: dict) -> dict:
+    """Flatten a nested dictionary.
 
+    Args:
+        dict (dict): a nested dictionary
 
-def json_output_decorator(function):
-    """Decorator to print the output as a JSON dump if --json is true; else (rich) print the output."""
+    Returns:
+        dict: a flattened dictionary
+    """
+    flattened_dict = {}
+    for key, sub_dict in dict.items():
+        for sub_key, value in sub_dict.items():
+            flattened_key = f"{key}/{sub_key}"
+            flattened_dict[flattened_key] = value
+    return flattened_dict
+
+
+def print_status_dict_results(dict: Mapping[str, float]) -> None:
+    """Print a dictionary in a pretty format. Notice that the dictionary is flattened.
+
+    e.g. input should be:
+    {
+        "status": "success",
+        "message": "dispatched",
+        "output": 15
+    }.
 
-    def wrapper(*args, json_output: bool = False, **kwargs):
-        result = function(*args, json_output, **kwargs)
-        if json_output:  # If json_output flag is present (cf typer options in main.py)
-            if isinstance(result, str):  # Print any dump() output directly
-                print(result)
-            else:  # Print any other output as json string by converting it first
-                result_json = dump(result)
-                print(result_json)
-        else:  # If json_output flag is not present (cf typer options in main.py)
-            if isinstance(result, str):
-                result_json = result
-            else:
-                result_json = dump(result)  # Use dump() logic to access full response
+    Args:
+        dict (Mapping[str, float]): dictionary to print
+    """
+    headers = dict.keys()
+    table = [[dict[k] for k in headers]]
 
-            result_dict = json.loads(result_json)  # Unpack response string into dict
-            result = result_dict["response"]  # Extract the 'response' item of the status/response dict
-            # Once converted, print the respomse using Rich table
-            if "experiment" in result or "experiments" in result:
-                table = Table(
-                    "Name",
-                    "Status",
-                    "Results",
-                    show_header=True,
-                    header_style="bold magenta",
-                )
-                if "experiments" in result:
-                    experiments = result["experiments"]
-                    # Initialising flat list of all jobs
-                    jobs = []
-                    for experiment in experiments:
-                        if "jobs" in experiment:
-                            jobs = experiment["jobs"]
-
-                            if "tasks" in jobs[0]:
-                                tasks = jobs[0]["tasks"]
-                                # List of job names, statuses, and results
-                                names = []
-                                statuses = []
-                                results = []
-
-                                for task in tasks:
-                                    names.append(task["name"])
-                                    statuses.append(task["status"])
-                                    results.append(task["results"])
-
-                                # Adding rows to table, avoiding duplicates
-                                for i in range(len(tasks)):
-                                    if i == 0 or tasks[i]["name"] != tasks[i - 1]["name"]:
-                                        table.add_row(str(names[i]), str(statuses[i]), str(results[i]))
-
-            elif all(key in item for key in ["name", "status", "message", "results"] for item in result):
-                table = Table(
-                    "Name",
-                    "Status",
-                    "Results",
-                    show_header=True,
-                    header_style="bold magenta",
-                )
+    headers = [f"\033[1;31m{i}\033[0m" for i in headers]
 
-                for item in result:
-                    table.add_row(str(item["name"]), str(item["status"]), str(item["results"]))
+    print(tabulate(table, headers=headers, tablefmt="fancy_grid"))
 
-            elif "message" in result:  # For status messages (e.g. iris post, iris delete, error handling)
-                if "output" not in result:
-                    result["output"] = "None"
-                table = Table(
-                    "Status",
-                    "Message",
-                    "Output",
-                    show_header=True,
-                    header_style="bold magenta",
-                )
-                if "status" in result:
-                    table.add_row(
-                        str(result["status"]),
-                        str(result["message"]),
-                        str(result["output"]),
-                    )
-                else:
-                    table.add_row(
-                        "", str(result["message"]), str(result["output"])
-                    )  # this will never happen but just for testing
 
+def print_get_dict_results(dict: Mapping[str, float], experiment: bool = True, key_name: str = "UUID") -> None:
+    """Print a dictionary in a pretty format.
+
+    Args:
+        dict (Mapping[str, float]): dictionary to print
+        experiment (bool, optional): Whether the dict is a response from iris get experiment. Defaults to True.
+        key_name (str, optional): The name of the key to use as the first column. Defaults to "UUID".
+    """
+    dict = flatten_dict(dict) if experiment else dict
+    first_col = ["ID/Name"] if experiment else [key_name]
+
+    headers = first_col + list(next(iter(dict.values())).keys())
+    # Transform the data into a list of lists
+    table = []  # table headers
+    for key, values in dict.items():
+        row = [key]
+        for k in headers:
+            if k in {"ID/Name", key_name}:
+                pass
+            elif k == "Job Results":
+                if values[k] is not None:
+                    row.append("\n".join(values[k]))
+                else:
+                    row.append("None")
             else:
-                for key, value in result.items():
-                    table = Table(show_header=True, header_style="bold magenta")
-                    table.add_column(key)
-                    table.add_row(str(value))
+                row.append(values[k])
+        table.append(row)
+
+    headers = [f"\033[1;31m{i}\033[0m" for i in headers]  # make the headers red and bold
+    # Print the table
+    print(tabulate(table, headers=headers, tablefmt="fancy_grid"))
 
-            console.print(table)
 
-        return result
+def extract_experiment_results(experiment: dict, results_table: dict):
+    """Extract the results from a experiment dict. return a clean format of dict of results.
 
-    return wrapper
+    Args:
+        experiment (dict): dict of detailed experiment information.
+        results_table (dict): dict of results to be updated.
+    """
+    experiment_id = experiment["id"]  # store the numerical experiment id
+    results_table[experiment_id] = {}
+    if "jobs" in experiment:
+        jobs = experiment["jobs"]
+        if "tasks" in jobs[0]:
+            tasks = jobs[0]["tasks"]
+
+            # extract the results from the tasks
+            for task in tasks:
+                results_table[experiment_id][task["name"]] = {"Job Status": task["status"]}
+                results_table[experiment_id][task["name"]]["Job Results"] = (
+                    [f"{key}: {value}" for key, value in task["results"].items()] if task["results"] else None
+                )
+
+
+def handle_iris_get_response(response):
+    """Handle the response from the iris get endpoint. Turn the json response into a pretty table.
+
+    Args:
+        response (str): a json format response from the iris get endpoint.
+    """
+    json_response = json.loads(response)["response"]
+    # check if 'experiments' in the response, this is for the common case 'iris get'
+    if "experiments" in json_response:
+        experiments = json_response["experiments"]
+
+        results_table = {}
+        for experiment in experiments:
+            extract_experiment_results(experiment, results_table)
+        # sort the results table by experiment id, get the most recent 5 experiments
+        sorted_results_table = dict(sorted(results_table.items(), key=lambda item: item[0], reverse=True)[:5])
+        print_get_dict_results(sorted_results_table)
+    # check if 'experiment' in the response, this is for the case 'iris get -i <experiment_id>'
+    elif "experiment" in json_response:
+        experiment = json_response["experiment"]
+
+        results_table = {}
+        extract_experiment_results(experiment, results_table)
+        print_get_dict_results(results_table)
+    # check if 'artefacts' in the response, this is for the case 'iris get artefact'
+    elif "artefacts" in json_response:
+        artefacts = json_response["artefacts"]
+        results_table = {
+            artefact["uuid"]: {
+                "name": artefact["name"],
+                "type": artefact["artefact_type"],
+            }
+            for artefact in artefacts
+        }
+        print_get_dict_results(results_table, experiment=False, key_name="UUID")
+    # check if 'sessions' in the response, this is for the case 'iris get inference-session'
+    elif "sessions" in json_response:
+        sessions = json_response["sessions"]
+        results_table = {
+            session["uuid"]: {
+                "model": session["model"],
+                "status": session["status"],
+            }
+            for session in sessions
+        }
+        print_get_dict_results(results_table, experiment=False, key_name="UUID")
+    # check if 'message' in the response, this is for the case 'iris status'
+    elif len(json_response) > 0 and len(json_response[0][0]) > 0 and "message" in json_response[0][0]:
+        messages = json_response[0]
+        results_table = {
+            message["name"]: {
+                "status": message["status"],
+                "message": message["message"]["message"],
+                "progress": message["message"]["progress"],
+            }
+            for message in messages
+        }
+        print_get_dict_results(results_table, experiment=False, key_name="Task Name")
+    else:
+        print(json.dumps(json_response, indent=4))
 
 
 def telemetry_decorator(function: Callable):
     """Decorator to send telemetry data to the metrics server."""
 
     @functools.wraps(function)
     def wrapper(*args, **kwargs):
```

### Comparing `titan-iris-0.7.1.dev82/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.8.0/src/titan_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.7.1.dev82
+Version: 0.8.0
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.7.1.dev82/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.8.0/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev82/tests/test_cli.py` & `titan-iris-0.8.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 
 import pytest
 from pytest_mock import mocker
 from pathlib import Path
 import tempfile
 
 import json
-from rich.console import Console
-from rich.table import Table
-from urllib.parse import urljoin
 
 # decorators get applied at import time, so we need to set the environment variables before importing the module
 os.environ["IRIS_TELEMETRY_DISABLE"] = "True"
 os.environ["IRIS_AUTHENTICATE_DISABLE"] = "True"
 
 from iris.sdk import post as post
 from iris.sdk import get as get
@@ -27,15 +24,14 @@
 from iris.sdk import download as download
 from iris.sdk.exception import (
     BadRequestError,
     EndpointNotFoundError,
     InvalidCommandError,
     InvalidLoginError,
 )
-from iris.sdk.utils import json_output_decorator as json_output_decorator
 from iris.sdk.utils import upload_from_file as upload_from_file
 
 from typer.testing import CliRunner
 
 from iris.main import main
 import json
```

### Comparing `titan-iris-0.7.1.dev82/tests/test_sdk.py` & `titan-iris-0.8.0/tests/test_sdk.py`

 * *Files identical despite different names*

