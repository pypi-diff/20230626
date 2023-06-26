# Comparing `tmp/eodc-2023.6.6.tar.gz` & `tmp/eodc-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.6.6.tar", max compression
+gzip compressed data, was "eodc-2023.6.7.tar", max compression
```

## Comparing `eodc-2023.6.6.tar` & `eodc-2023.6.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-06-24 09:54:08.666077 eodc-2023.6.6/README.md
--rw-r--r--   0        0        0      213 2023-06-24 09:54:08.666077 eodc-2023.6.6/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-24 09:54:08.666077 eodc-2023.6.6/eodc/dask.py
--rw-r--r--   0        0        0    10812 2023-06-24 09:54:08.666077 eodc-2023.6.6/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-06-24 09:54:08.666077 eodc-2023.6.6/eodc/settings.py
--rw-r--r--   0        0        0     1204 2023-06-24 09:54:08.666077 eodc-2023.6.6/pyproject.toml
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 eodc-2023.6.6/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-26 08:23:40.814599 eodc-2023.6.7/README.md
+-rw-r--r--   0        0        0      213 2023-06-26 08:23:40.814599 eodc-2023.6.7/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-26 08:23:40.814599 eodc-2023.6.7/eodc/dask.py
+-rw-r--r--   0        0        0    11579 2023-06-26 08:23:40.814599 eodc-2023.6.7/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-06-26 08:23:40.814599 eodc-2023.6.7/eodc/settings.py
+-rw-r--r--   0        0        0     1204 2023-06-26 08:23:40.814599 eodc-2023.6.7/pyproject.toml
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 eodc-2023.6.7/PKG-INFO
```

### Comparing `eodc-2023.6.6/README.md` & `eodc-2023.6.7/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.6/eodc/dask.py` & `eodc-2023.6.7/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.6/eodc/faas.py` & `eodc-2023.6.7/eodc/faas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import json
 import logging
 import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from time import sleep
+from typing import Optional
 
 import argo_workflows
 from argo_workflows.api import workflow_service_api
 from argo_workflows.model.io_argoproj_workflow_v1alpha1_arguments import (
     IoArgoprojWorkflowV1alpha1Arguments,
 )
 from argo_workflows.model.io_argoproj_workflow_v1alpha1_parameter import (
@@ -147,31 +149,32 @@
             )
 
     def stop_workflow(self, name):
         body = IoArgoprojWorkflowV1alpha1WorkflowStopRequest()
         self.api_instance_workflows.stop_workflow(settings.NAMESPACE, name, body=body)
         logger.info(f"Successfully stopped workflow {name}.")
 
-    def get_logs(self, workflow_name):
+    def get_logs(self, workflow_name) -> list[str]:
         # The .workflow_logs client method seems semi-broken:
         # https://github.com/argoproj/argo-workflows/issues/7781
         # Therefore this workaround is necessary!
-        return (
+        raw_logs = (
             self.api_instance_workflows.workflow_logs(
                 settings.NAMESPACE,
                 workflow_name,
                 log_options_container="main",
                 #  log_options_follow=True,
                 _check_return_type=False,
                 _preload_content=False,
             )
             .read()
             .decode("utf-8")
             .splitlines()
         )
+        return [json.loads(log)["result"]["content"] for log in raw_logs]
 
     @abstractmethod
     def get_output_stac_items(self):
         raise NotImplementedError()
 
 
 class Force(FaasProcessorBase):
@@ -250,26 +253,42 @@
         stac_items = [
             Item.from_file(link.get_absolute_href())
             for link in openeo_output_collection.get_item_links()
         ]
 
         return stac_items
 
-    def stop_openeo_job(self, openeo_job_id):
-        associated_workflows = self.api_instance_workflows.list_workflows(
+    def _get_workflows_for_job_id(
+        self, openeo_job_id, filter_workflow_status_phase: Optional[tuple[str]] = None
+    ):
+        # filter_workflow_status_phase wants to be an iterable
+        # of strings like ("Running", "Pending")
+
+        workflows_with_label = self.api_instance_workflows.list_workflows(
             namespace=settings.NAMESPACE,
             list_options_label_selector=f"openeo_job_id={openeo_job_id}",
         ).items
-        associated_unfinished_workflows = [
-            workflow
-            for workflow in associated_workflows
-            if workflow.status.phase in ("Running", "Pending")
-        ]
+
+        if filter_workflow_status_phase is not None:
+            workflows_with_label_filtered = [
+                workflow
+                for workflow in workflows_with_label
+                if workflow.status.phase in filter_workflow_status_phase
+            ]
+        else:
+            workflows_with_label_filtered = workflows_with_label
+        return workflows_with_label_filtered
+
+    def stop_openeo_job(self, openeo_job_id):
+        associated_unfinished_workflows = self._get_workflows_for_job_id(
+            openeo_job_id=openeo_job_id,
+            filter_workflow_status_phase=("Running", "Pending"),
+        )
         logger.info(
-            f"Stopping OpenEO job {openeo_job_id} with"
+            f"Stopping OpenEO job {openeo_job_id} with "
             f"{len(associated_unfinished_workflows)} unfinished sub-workflows."
         )
 
         # Need to stop all sub-jobs too!
         for workflow in associated_unfinished_workflows:
             if workflow.status.phase in ("Running", "Pending"):
                 workflow_name = workflow.metadata.name
```

### Comparing `eodc-2023.6.6/pyproject.toml` & `eodc-2023.6.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.6.6"
+version = "2023.6.7"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2023.6.6/PKG-INFO` & `eodc-2023.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.6.6
+Version: 2023.6.7
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

