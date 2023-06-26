# Comparing `tmp/jobbergate_cli-3.5.0a5.tar.gz` & `tmp/jobbergate_cli-3.5.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_cli-3.5.0a5.tar", max compression
+gzip compressed data, was "jobbergate_cli-3.5.0a6.tar", max compression
```

## Comparing `jobbergate_cli-3.5.0a5.tar` & `jobbergate_cli-3.5.0a6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1082 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/LICENSE
--rw-r--r--   0        0        0     1065 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/README.rst
--rw-r--r--   0        0        0      801 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/__init__.py
--rw-r--r--   0        0        0     1112 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/application_base.py
--rw-r--r--   0        0        0    11271 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/auth.py
--rw-r--r--   0        0        0     4414 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/compat.py
--rw-r--r--   0        0        0     4355 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/config.py
--rw-r--r--   0        0        0     1139 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/constants.py
--rw-r--r--   0        0        0     3112 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/exceptions.py
--rw-r--r--   0        0        0     1134 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/jobberappslib.py
--rw-r--r--   0        0        0     1095 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/logging.py
--rw-r--r--   0        0        0     6510 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/main.py
--rw-r--r--   0        0        0     7523 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/render.py
--rw-r--r--   0        0        0     7348 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/requests.py
--rw-r--r--   0        0        0     6084 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/schemas.py
--rw-r--r--   0        0        0       66 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/__init__.py
--rw-r--r--   0        0        0       66 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/__init__.py
--rw-r--r--   0        0        0    11778 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/app.py
--rw-r--r--   0        0        0     1725 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/application_base.py
--rw-r--r--   0        0        0     1558 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/application_helpers.py
--rw-r--r--   0        0        0    13800 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/questions.py
--rw-r--r--   0        0        0    11471 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/tools.py
--rw-r--r--   0        0        0       61 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/clusters/__init__.py
--rw-r--r--   0        0        0      728 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/clusters/app.py
--rw-r--r--   0        0        0     3284 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/clusters/tools.py
--rw-r--r--   0        0        0       64 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_scripts/__init__.py
--rw-r--r--   0        0        0    11693 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_scripts/app.py
--rw-r--r--   0        0        0     6750 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_scripts/tools.py
--rw-r--r--   0        0        0       68 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_submissions/__init__.py
--rw-r--r--   0        0        0     7123 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_submissions/app.py
--rw-r--r--   0        0        0     4167 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_submissions/tools.py
--rw-r--r--   0        0        0     1370 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/text_tools.py
--rw-r--r--   0        0        0     3524 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/jobbergate_cli/time_loop.py
--rw-r--r--   0        0        0     2525 2023-06-22 17:40:41.469643 jobbergate_cli-3.5.0a5/pyproject.toml
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 jobbergate_cli-3.5.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-26 17:06:36.728536 jobbergate_cli-3.5.0a6/LICENSE
+-rw-r--r--   0        0        0     1065 2023-06-26 17:06:36.728536 jobbergate_cli-3.5.0a6/README.rst
+-rw-r--r--   0        0        0      801 2023-06-26 17:06:36.728536 jobbergate_cli-3.5.0a6/jobbergate_cli/__init__.py
+-rw-r--r--   0        0        0     1112 2023-06-26 17:06:36.728536 jobbergate_cli-3.5.0a6/jobbergate_cli/application_base.py
+-rw-r--r--   0        0        0    11271 2023-06-26 17:06:36.728536 jobbergate_cli-3.5.0a6/jobbergate_cli/auth.py
+-rw-r--r--   0        0        0     4414 2023-06-26 17:06:36.728536 jobbergate_cli-3.5.0a6/jobbergate_cli/compat.py
+-rw-r--r--   0        0        0     4355 2023-06-26 17:06:36.728536 jobbergate_cli-3.5.0a6/jobbergate_cli/config.py
+-rw-r--r--   0        0        0     1139 2023-06-26 17:06:36.728536 jobbergate_cli-3.5.0a6/jobbergate_cli/constants.py
+-rw-r--r--   0        0        0     3112 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/exceptions.py
+-rw-r--r--   0        0        0     1134 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/jobberappslib.py
+-rw-r--r--   0        0        0     1095 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/logging.py
+-rw-r--r--   0        0        0     6510 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/main.py
+-rw-r--r--   0        0        0     7523 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/render.py
+-rw-r--r--   0        0        0     7954 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/requests.py
+-rw-r--r--   0        0        0     6084 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/schemas.py
+-rw-r--r--   0        0        0       66 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/__init__.py
+-rw-r--r--   0        0        0       66 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/__init__.py
+-rw-r--r--   0        0        0    11778 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/app.py
+-rw-r--r--   0        0        0     1725 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/application_base.py
+-rw-r--r--   0        0        0     1558 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/application_helpers.py
+-rw-r--r--   0        0        0    13800 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/questions.py
+-rw-r--r--   0        0        0    11471 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/tools.py
+-rw-r--r--   0        0        0       61 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/clusters/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/clusters/app.py
+-rw-r--r--   0        0        0     3284 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/clusters/tools.py
+-rw-r--r--   0        0        0       64 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    11693 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_scripts/app.py
+-rw-r--r--   0        0        0     6750 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_scripts/tools.py
+-rw-r--r--   0        0        0       68 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     7123 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_submissions/app.py
+-rw-r--r--   0        0        0     4167 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_submissions/tools.py
+-rw-r--r--   0        0        0     1370 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/text_tools.py
+-rw-r--r--   0        0        0     3524 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/jobbergate_cli/time_loop.py
+-rw-r--r--   0        0        0     2525 2023-06-26 17:06:36.732536 jobbergate_cli-3.5.0a6/pyproject.toml
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 jobbergate_cli-3.5.0a6/PKG-INFO
```

### Comparing `jobbergate_cli-3.5.0a5/LICENSE` & `jobbergate_cli-3.5.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/README.rst` & `jobbergate_cli-3.5.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/__init__.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/application_base.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/auth.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/auth.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/compat.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/compat.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/config.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/constants.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/exceptions.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/jobberappslib.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/jobberappslib.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/logging.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/main.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/render.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/render.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/requests.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -156,14 +156,28 @@
                     {abort_message}:
                     There are [red]{fk_error.table}[/red] that reference id [bold yellow]{fk_error.pk_id}[/bold yellow].
                     """,
                 ),
                 subject=abort_subject,
                 log_message=f"Could not delete due to foreign-key constraint: {response.text}",
             )
+        elif method in ("PATCH", "PUT", "DELETE") and response.status_code == 403 and "does not own" in response.text:
+            details = response.json()["detail"]
+            raise Abort(
+                dedent(
+                    f"""
+                    {abort_message}:
+
+                    [red]You do not own this resource.[/red]
+                    Please contact the owner if you need it to be modified.
+                    """,
+                ),
+                subject=abort_subject,
+                log_message=f"Resource could not be modified by non-owner: {response.text}",
+            )
         else:
             raise Abort(
                 unwrap(
                     f"""
                     {abort_message}:
                     Received an error response.
                     """
```

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/schemas.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/app.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/application_base.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/application_helpers.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/application_helpers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/questions.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/questions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/applications/tools.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/applications/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/clusters/app.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/clusters/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/clusters/tools.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/clusters/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_scripts/app.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_scripts/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_scripts/tools.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_scripts/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_submissions/app.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_submissions/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/subapps/job_submissions/tools.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/subapps/job_submissions/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/text_tools.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/text_tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/jobbergate_cli/time_loop.py` & `jobbergate_cli-3.5.0a6/jobbergate_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.0a5/pyproject.toml` & `jobbergate_cli-3.5.0a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-cli"
-version = "3.5.0a5"
+version = "3.5.0a6"
 description = "Jobbergate CLI Client"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 packages = [ { include = "jobbergate_cli" } ]
 classifiers = [
```

### Comparing `jobbergate_cli-3.5.0a5/PKG-INFO` & `jobbergate_cli-3.5.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-cli
-Version: 3.5.0a5
+Version: 3.5.0a6
 Summary: Jobbergate CLI Client
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

