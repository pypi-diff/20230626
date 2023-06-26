# Comparing `tmp/prefect-gcp-0.4.3.tar.gz` & `tmp/prefect-gcp-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-igqgbo2s/prefect-gcp-0.4.3.tar", last modified: Thu Jun 15 14:42:53 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-g0j5y6zy/prefect-gcp-0.4.4.tar", last modified: Mon Jun 26 16:15:16 2023, max compression
```

## Comparing `prefect-gcp-0.4.3.tar` & `prefect-gcp-0.4.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    31604 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)    29089 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31619 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29089 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/versioneer.py
```

### Comparing `prefect-gcp-0.4.3/LICENSE` & `prefect-gcp-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/PKG-INFO` & `prefect-gcp-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.3
+Version: 0.4.4
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.3 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.4 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.3/README.md` & `prefect-gcp-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/prefect_gcp/__init__.py` & `prefect-gcp-0.4.4/prefect_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/prefect_gcp/aiplatform.py` & `prefect-gcp-0.4.4/prefect_gcp/aiplatform.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         Scheduling,
         WorkerPoolSpec,
     )
     from google.cloud.aiplatform_v1.types.job_service import CancelCustomJobRequest
     from google.cloud.aiplatform_v1.types.job_state import JobState
     from google.cloud.aiplatform_v1.types.machine_resources import DiskSpec, MachineSpec
     from google.protobuf.duration_pb2 import Duration
+    from tenacity import retry, stop_after_attempt, wait_fixed, wait_random
 except ModuleNotFoundError:
     pass
 
 from prefect_gcp.credentials import GcpCredentials
 
 
 class VertexAICustomTrainingJobResult(InfrastructureResult):
@@ -279,16 +280,21 @@
             f"{self._log_prefix}: Job {self.job_name!r} starting to run "
             f"the command {' '.join(self.command)!r} in region "
             f"{self.region!r} using image {self.image!r}"
         )
 
         project = self.gcp_credentials.project
         resource_name = f"projects/{project}/locations/{self.region}"
+
+        retry_policy = retry(
+            stop=stop_after_attempt(3), wait=wait_fixed(1) + wait_random(0, 3)
+        )
+
         custom_job_run = await run_sync_in_worker_thread(
-            job_service_client.create_custom_job,
+            retry_policy(job_service_client.create_custom_job),
             parent=resource_name,
             custom_job=custom_job,
         )
 
         self.logger.info(
             f"{self._log_prefix}: Job {self.job_name!r} has successfully started; "
             f"the full job name is {custom_job_run.name!r}"
```

### Comparing `prefect-gcp-0.4.3/prefect_gcp/bigquery.py` & `prefect-gcp-0.4.4/prefect_gcp/bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/prefect_gcp/cloud_run.py` & `prefect-gcp-0.4.4/prefect_gcp/cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/prefect_gcp/cloud_storage.py` & `prefect-gcp-0.4.4/prefect_gcp/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/prefect_gcp/credentials.py` & `prefect-gcp-0.4.4/prefect_gcp/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/prefect_gcp/deployments/steps.py` & `prefect-gcp-0.4.4/prefect_gcp/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/prefect_gcp/secret_manager.py` & `prefect-gcp-0.4.4/prefect_gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/prefect_gcp/worker.py` & `prefect-gcp-0.4.4/prefect_gcp/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,18 +151,18 @@
 
 import anyio
 import googleapiclient
 from anyio.abc import TaskStatus  # noqa
 from google.api_core.client_options import ClientOptions
 from googleapiclient import discovery
 from googleapiclient.discovery import Resource
-from prefect.docker import get_prefect_image_name
 from prefect.exceptions import InfrastructureNotFound
 from prefect.logging.loggers import PrefectLogAdapter
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
+from prefect.utilities.dockerutils import get_prefect_image_name
 from prefect.utilities.pydantic import JsonPatch
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
 )
```

### Comparing `prefect-gcp-0.4.3/prefect_gcp.egg-info/PKG-INFO` & `prefect-gcp-0.4.4/prefect_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.3
+Version: 0.4.4
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.3 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.4 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.3/prefect_gcp.egg-info/SOURCES.txt` & `prefect-gcp-0.4.4/prefect_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/prefect_gcp.egg-info/requires.txt` & `prefect-gcp-0.4.4/prefect_gcp.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-prefect>=2.10.9
+prefect>=2.10.17
 google-api-python-client>=2.20.0
 google-cloud-storage>=2.0.0
+tenacity>=8.0.0
 
 [aiplatform]
 google-cloud-aiplatform
 
 [all_extras]
 google-cloud-aiplatform
 google-cloud-bigquery
```

### Comparing `prefect-gcp-0.4.3/setup.cfg` & `prefect-gcp-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/setup.py` & `prefect-gcp-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/tests/test_aiplatform.py` & `prefect-gcp-0.4.4/tests/test_aiplatform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest.mock import MagicMock, patch
 
 import pytest
 from google.cloud.aiplatform_v1.types.accelerator_type import AcceleratorType
 from google.cloud.aiplatform_v1.types.job_state import JobState
 from prefect.exceptions import InfrastructureNotFound
+from tenacity import RetryError
 
 from prefect_gcp.aiplatform import (
     VertexAICustomTrainingJob,
     VertexAICustomTrainingJobResult,
 )
 
 
@@ -142,14 +143,26 @@
         gcp_credentials = vertex_ai_custom_training_job.gcp_credentials
         gcp_credentials.job_service_client.get_custom_job.return_value = (
             failed_run_final
         )
         with pytest.raises(RuntimeError, match="my error msg"):
             vertex_ai_custom_training_job.run()
 
+    def test_run_start_error(
+        self, vertex_ai_custom_training_job: VertexAICustomTrainingJob
+    ):
+        gcp_credentials = vertex_ai_custom_training_job.gcp_credentials
+        gcp_credentials.job_service_client.create_custom_job.side_effect = (
+            RuntimeError()
+        )
+
+        with pytest.raises(RetryError):
+            vertex_ai_custom_training_job.run()
+        assert gcp_credentials.job_service_client.create_custom_job.call_count == 3
+
     def test_machine_spec(
         self, vertex_ai_custom_training_job: VertexAICustomTrainingJob
     ):
         vertex_ai_custom_training_job.accelerator_count = 1
         vertex_ai_custom_training_job.accelerator_type = "NVIDIA_TESLA_T4"
 
         job_spec = vertex_ai_custom_training_job._build_job_spec()
```

### Comparing `prefect-gcp-0.4.3/tests/test_bigquery.py` & `prefect-gcp-0.4.4/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/tests/test_block_standards.py` & `prefect-gcp-0.4.4/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/tests/test_cloud_run.py` & `prefect-gcp-0.4.4/tests/test_cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/tests/test_cloud_storage.py` & `prefect-gcp-0.4.4/tests/test_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/tests/test_credentials.py` & `prefect-gcp-0.4.4/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/tests/test_secret_manager.py` & `prefect-gcp-0.4.4/tests/test_secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/tests/test_worker.py` & `prefect-gcp-0.4.4/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.3/versioneer.py` & `prefect-gcp-0.4.4/versioneer.py`

 * *Files identical despite different names*

