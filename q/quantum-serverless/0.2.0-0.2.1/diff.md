# Comparing `tmp/quantum_serverless-0.2.0.tar.gz` & `tmp/quantum_serverless-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.2.0.tar", last modified: Tue Jun 20 15:51:59 2023, max compression
+gzip compressed data, was "quantum_serverless-0.2.1.tar", last modified: Mon Jun 26 15:38:45 2023, max compression
```

## Comparing `quantum_serverless-0.2.0.tar` & `quantum_serverless-0.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.908800 quantum_serverless-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-20 15:51:59.908800 quantum_serverless-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/serializers/program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/visualizaiton/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/visualizaiton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/visualizaiton/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 15:51:59.908800 quantum_serverless-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/test_program_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.908800 quantum_serverless-0.2.0/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/serializers/test_program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless/visualizaiton/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/visualizaiton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/quantum_serverless/visualizaiton/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 15:38:44.000000 quantum_serverless-0.2.1/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:44.997630 quantum_serverless-0.2.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/test_program_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/core/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:45.001630 quantum_serverless-0.2.1/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-26 15:38:35.000000 quantum_serverless-0.2.1/tests/utils.py
```

### Comparing `quantum_serverless-0.2.0/PKG-INFO` & `quantum_serverless-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum_serverless
-Version: 0.2.0
+Version: 0.2.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.2.0/README.md` & `quantum_serverless-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/__init__.py` & `quantum_serverless-0.2.1/quantum_serverless/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     QuantumServerless
 """
 
 from importlib_metadata import version as metadata_version, PackageNotFoundError
 
 from .core import (
     Provider,
-    run_qiskit_remote,
     distribute_task,
     get,
     put,
     get_refs_by_status,
     KuberayProvider,
     GatewayProvider,
     save_result,
```

### Comparing `quantum_serverless-0.2.0/quantum_serverless/core/__init__.py` & `quantum_serverless-0.2.1/quantum_serverless/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     Provider
     GatewayProvider
     KuberayProvider
     ComputeResource
 
     save_result
     distribute_task
-    run_qiskit_remote
     get
     put
     get_refs_by_status
 
 
 Events classes
 --------------
@@ -60,14 +59,13 @@
 """
 
 from .provider import Provider, ComputeResource, KuberayProvider, GatewayProvider
 from .decorators import (
     remote,
     get,
     put,
-    run_qiskit_remote,
     get_refs_by_status,
     distribute_task,
 )
 from .events import RedisEventHandler, EventHandler, ExecutionMessage
 from .state import RedisStateHandler, StateHandler
 from .job import save_result
```

### Comparing `quantum_serverless-0.2.0/quantum_serverless/core/constants.py` & `quantum_serverless-0.2.1/quantum_serverless/core/constants.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/core/decorators.py` & `quantum_serverless-0.2.1/quantum_serverless/core/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     put
     run_qiskit_remote
     get_refs_by_status
     distribute_task
 """
 import functools
 import os
-import warnings
 from dataclasses import dataclass
 from typing import Optional, Dict, Any, Union, List, Callable, Sequence
 
 import ray
 from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
 from qiskit import QuantumCircuit
 from ray.runtime_env import RuntimeEnv
@@ -202,37 +201,14 @@
                 return func(*args, **kwargs)
 
         return wraps
 
     return decorator
 
 
-def run_qiskit_remote(
-    target: Optional[Union[Dict[str, Any], Target]] = None,
-    state: Optional[StateHandler] = None,
-):
-    """(Deprecated) Wraps local function as remote executable function.
-    New function will return reference object when called.
-
-    Args:
-        target: target object or dictionary for requirements for node resources
-        state: state handler
-
-    Returns:
-        object reference
-    """
-    warnings.warn(
-        "Decorator `run_qiskit_remote` is deprecated. "
-        "Please, consider using `distribute_task` instead.",
-        DeprecationWarning,
-        stacklevel=2,
-    )
-    return distribute_task(target, state)
-
-
 def distribute_task(
     target: Optional[Union[Dict[str, Any], Target]] = None,
     state: Optional[StateHandler] = None,
 ):
     """Wraps local function as remote executable function.
     New function will return reference object when called.
```

### Comparing `quantum_serverless-0.2.0/quantum_serverless/core/events.py` & `quantum_serverless-0.2.1/quantum_serverless/core/events.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/core/job.py` & `quantum_serverless-0.2.1/quantum_serverless/core/job.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 import json
 import logging
 import os
 import tarfile
 import time
 from typing import Dict, Any, Optional, List
 from uuid import uuid4
-import warnings
 
 import ray.runtime_env
 import requests
 from ray.dashboard.modules.job.sdk import JobSubmissionClient
 
 from quantum_serverless.core.constants import (
     OT_PROGRAM_NAME,
@@ -55,20 +54,14 @@
 
 RuntimeEnv = ray.runtime_env.RuntimeEnv
 
 
 class BaseJobClient:
     """Base class for Job clients."""
 
-    def run_program(
-        self, program: Program, arguments: Optional[Dict[str, Any]] = None
-    ) -> "Job":
-        """Runs program."""
-        raise NotImplementedError
-
     def run(
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> "Job":
         """Runs program."""
         raise NotImplementedError
 
     def get(self, job_id) -> Optional["Job"]:
@@ -124,53 +117,18 @@
         return Job(self._job_client.get_job_info(job_id).job_id, job_client=self)
 
     def list(self, **kwargs) -> List["Job"]:
         return [
             Job(job.job_id, job_client=self) for job in self._job_client.list_jobs()
         ]
 
-    def run_program(self, program: Program, arguments: Optional[Dict[str, Any]] = None):
-        warnings.warn(
-            "`run_program` is deprecated. Please, consider using `run` instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        arguments = arguments or {}
-        arguments_string = ""
-        if program.arguments is not None:
-            arg_list = []
-            for key, value in arguments.items():
-                if isinstance(value, dict):
-                    arg_list.append(f"--{key}='{json.dumps(value)}'")
-                else:
-                    arg_list.append(f"--{key}={value}")
-            arguments_string = " ".join(arg_list)
-        entrypoint = f"python {program.entrypoint} {arguments_string}"
-
-        # set program name so OT can use it as parent span name
-        env_vars = {
-            **(program.env_vars or {}),
-            **{OT_PROGRAM_NAME: program.title},
-        }
-
-        job_id = self._job_client.submit_job(
-            entrypoint=entrypoint,
-            submission_id=f"qs_{uuid4()}",
-            runtime_env={
-                "working_dir": program.working_dir,
-                "pip": program.dependencies,
-                "env_vars": env_vars,
-            },
-        )
-        return Job(job_id=job_id, job_client=self)
-
     def run(self, program: Program, arguments: Optional[Dict[str, Any]] = None):
         arguments = arguments or {}
         arguments_string = ""
-        if program.arguments is not None:
+        if arguments is not None:
             arg_list = []
             for key, value in arguments.items():
                 if isinstance(value, dict):
                     arg_list.append(f"--{key}='{json.dumps(value)}'")
                 else:
                     arg_list.append(f"--{key}={value}")
             arguments_string = " ".join(arg_list)
@@ -205,54 +163,14 @@
             version: gateway version
             token: authorization token
         """
         self.host = host
         self.version = version
         self._token = token
 
-    def run_program(  # pylint: disable=too-many-locals
-        self, program: Program, arguments: Optional[Dict[str, Any]] = None
-    ) -> "Job":
-        warnings.warn(
-            "`run_program` is deprecated. Please, consider using `run` instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        url = f"{self.host}/api/{self.version}/programs/run/"
-        artifact_file_path = os.path.join(program.working_dir, "artifact.tar")
-
-        with tarfile.open(artifact_file_path, "w") as tar:
-            for filename in os.listdir(program.working_dir):
-                fpath = os.path.join(program.working_dir, filename)
-                tar.add(fpath, arcname=filename)
-
-        with open(artifact_file_path, "rb") as file:
-            response_data = safe_json_request(
-                request=lambda: requests.post(
-                    url=url,
-                    data={
-                        "title": program.title,
-                        "entrypoint": program.entrypoint,
-                        "arguments": json.dumps(
-                            arguments or {}, cls=QiskitObjectsEncoder
-                        ),
-                        "dependencies": json.dumps(program.dependencies or []),
-                    },
-                    files={"artifact": file},
-                    headers={"Authorization": f"Bearer {self._token}"},
-                    timeout=REQUESTS_TIMEOUT,
-                )
-            )
-            job_id = response_data.get("id")
-
-        if os.path.exists(artifact_file_path):
-            os.remove(artifact_file_path)
-
-        return Job(job_id, job_client=self)
-
     def run(  # pylint: disable=too-many-locals
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> "Job":
         url = f"{self.host}/api/{self.version}/programs/run/"
         artifact_file_path = os.path.join(program.working_dir, "artifact.tar")
 
         with tarfile.open(artifact_file_path, "w") as tar:
```

### Comparing `quantum_serverless-0.2.0/quantum_serverless/core/program.py` & `quantum_serverless-0.2.1/quantum_serverless/core/program.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     Program
 """
 import dataclasses
 import json
 import logging
 import os
 import tarfile
-import warnings
 from abc import ABC
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Dict, List, Any
 
 import requests
 
@@ -50,49 +49,36 @@
 class Program:  # pylint: disable=too-many-instance-attributes
     """Serverless Program.
 
     Args:
         title: program name
         entrypoint: is a script that will be executed as a job
             ex: job.py
-        arguments: (deprecated) arguments for entrypoint script
         env_vars: env vars
         dependencies: list of python dependencies to execute a program
         working_dir: directory where entrypoint file is located
         description: description of a program
         version: version of a program
     """
 
     title: str
     entrypoint: str
     working_dir: str = "./"
-    arguments: Optional[Dict[str, Any]] = None
     env_vars: Optional[Dict[str, str]] = None
     dependencies: Optional[List[str]] = None
     description: Optional[str] = None
     version: Optional[str] = None
     tags: Optional[List[str]] = None
 
     @classmethod
     def from_json(cls, data: Dict[str, Any]):
         """Reconstructs Program from dictionary."""
         field_names = set(f.name for f in dataclasses.fields(Program))
         return Program(**{k: v for k, v in data.items() if k in field_names})
 
-    def __post_init__(self):
-        if self.arguments is not None:
-            warnings.warn(
-                "Passing `arguments` as constructor argument to `Program` is deprecated "
-                "and will be removed in v0.2. "
-                "Please, consider passing `arguments` to `run` "
-                "method of `QuantumServerless` object.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-
 
 class ProgramStorage(ABC):
     """Base program backend to save and load programs from."""
 
     def save_program(self, program: Program) -> bool:
         """Save program in specified backend.
```

### Comparing `quantum_serverless-0.2.0/quantum_serverless/core/provider.py` & `quantum_serverless-0.2.1/quantum_serverless/core/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -248,53 +248,14 @@
             logging.warning(  # pylint: disable=logging-fstring-interpolation
                 "Job has not been found as no provider "
                 "with remote host has been configured. "
             )
             return None
         return Job(job_id=job_id, job_client=job_client)
 
-    def run_program(
-        self, program: Program, arguments: Optional[Dict[str, Any]] = None
-    ) -> Job:
-        """(Deprecated) Execute a program as a async job.
-
-        Example:
-            >>> serverless = QuantumServerless()
-            >>> program = Program(
-            >>>     "job.py",
-            >>>     arguments={"arg1": "val1"},
-            >>>     dependencies=["requests"]
-            >>> )
-            >>> job = serverless.run_program(program)
-            >>> # <Job | ...>
-
-        Args:
-            arguments: arguments to run program with
-            program: Program object
-
-        Returns:
-            Job
-        """
-        warnings.warn(
-            "`run_program` is deprecated. Please, consider using `run` instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        job_client = self.job_client()
-
-        if job_client is None:
-            logging.warning(  # pylint: disable=logging-fstring-interpolation
-                f"Job has not been submitted as no provider "
-                f"with remote host has been configured. "
-                f"Selected provider: {self}"
-            )
-            return None
-
-        return job_client.run_program(program, arguments)
-
     def run(self, program: Program, arguments: Optional[Dict[str, Any]] = None) -> Job:
         """Execute a program as a async job.
 
         Example:
             >>> serverless = QuantumServerless()
             >>> program = Program(
             >>>     "job.py",
@@ -321,27 +282,27 @@
             )
             return None
 
         return job_client.run(program, arguments)
 
 
 class KuberayProvider(Provider):
-    """Implements CRUD for Kuberay API server."""
+    """(Deprecated) Implements CRUD for Kuberay API server."""
 
     def __init__(
         self,
         name: str,
         host: Optional[str] = None,
         namespace: Optional[str] = "default",
         img: Optional[str] = RAY_IMAGE,
         token: Optional[str] = None,
         compute_resource: Optional[ComputeResource] = None,
         available_compute_resources: Optional[List[ComputeResource]] = None,
     ):
-        """Kuberay provider for serverless computation.
+        """(Deprecated) Kuberay provider for serverless computation.
 
         Example:
             >>> provider = Provider(
             >>>    name="<NAME>",
             >>>    host="<HOST>",
             >>>    namespace="<NAMESPACE>",
             >>>    token="<TOKEN>",
@@ -357,14 +318,22 @@
             namespace: namespace to deploy provider in
             image: container image to use for ray cluster
             token: authentication token for manager
             compute_resource: selected compute_resource from provider
             available_compute_resources: available clusters in provider
         """
         super().__init__(name)
+        warnings.warn(
+            "`KuberayProvider` is deprecated "
+            "and will be removed in v0.3. "
+            "Please, consider using `GatewayProvider`.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
         self.name = name
         self.host = host
         self.token = token
         self.namespace = namespace
         self.image = img
         self.compute_resource = compute_resource
         if available_compute_resources is None:
@@ -568,24 +537,14 @@
 
     def delete_compute_resource(self, resource) -> int:
         raise NotImplementedError("GatewayProvider does not support resources api yet.")
 
     def get_job_by_id(self, job_id: str) -> Optional[Job]:
         return self._job_client.get(job_id)
 
-    def run_program(
-        self, program: Program, arguments: Optional[Dict[str, Any]] = None
-    ) -> Job:
-        warnings.warn(
-            "`run_program` is deprecated. Please, consider using `run` instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self._job_client.run_program(program, arguments)
-
     def run(self, program: Program, arguments: Optional[Dict[str, Any]] = None) -> Job:
         return self._job_client.run(program, arguments)
 
     def get_jobs(self, **kwargs) -> List[Job]:
         return self._job_client.list(**kwargs)
 
     def _fetch_token(self, username: str, password: str):
```

### Comparing `quantum_serverless-0.2.0/quantum_serverless/core/state.py` & `quantum_serverless-0.2.1/quantum_serverless/core/state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/core/tracing.py` & `quantum_serverless-0.2.1/quantum_serverless/core/tracing.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/exception.py` & `quantum_serverless-0.2.1/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/library/__init__.py` & `quantum_serverless-0.2.1/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.2.1/quantum_serverless/library/transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.2.1/quantum_serverless/quantum_serverless.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 .. autosummary::
     :toctree: ../stubs/
 
     QuantumServerless
 """
 import json
 import logging
-import os
-import warnings
 from typing import Optional, Union, List, Dict, Any
 
 import requests
 from ray._private.worker import BaseContext
 
 from quantum_serverless.core.job import Job
 from quantum_serverless.core.program import Program
@@ -62,64 +60,19 @@
         elif isinstance(providers, Provider):
             providers = [providers]
         self._providers: List[Provider] = providers
         self._selected_provider: Provider = self._providers[-1]
 
         self._allocated_context: Optional[Context] = None
 
-    def __enter__(self):
-        warnings.warn(
-            "Calling `with serverless: ...` is deprecated. "
-            "Please, consider using `with serverless.context(): ...`",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self._allocated_context = self._selected_provider.context()
-        return self._allocated_context
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if self._allocated_context:
-            self._allocated_context.disconnect()
-        self._allocated_context = None
-
     @property
     def job_client(self):
         """Job client for given provider."""
         return self._selected_provider.job_client()
 
-    def run_program(
-        self, program: Program, arguments: Optional[Dict[str, Any]] = None
-    ) -> Optional[Job]:
-        """(Deprecated) Execute a program as a async job
-
-        Example:
-            >>> serverless = QuantumServerless()
-            >>> program = Program(
-            >>>     "job.py",
-            >>>     dependencies=["requests"]
-            >>> )
-            >>> job = serverless.run_program(program, {"arg1": 1})
-            >>> # <Job | ...>
-
-        Args:
-            arguments: arguments to run program with
-            program: Program object
-
-        Returns:
-            Job
-        """
-        warnings.warn(
-            "`run_program` is deprecated. Please, consider using `run` instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        if program.arguments is not None:
-            arguments = program.arguments
-        return self._selected_provider.run_program(program, arguments)
-
     def run(
         self, program: Program, arguments: Optional[Dict[str, Any]] = None
     ) -> Optional[Job]:
         """Execute a program as a async job
 
         Example:
             >>> serverless = QuantumServerless()
@@ -133,16 +86,14 @@
         Args:
             arguments: arguments to run program with
             program: Program object
 
         Returns:
             Job
         """
-        if program.arguments is not None:
-            arguments = program.arguments
         return self._selected_provider.run(program, arguments)
 
     def get_job_by_id(self, job_id: str) -> Optional[Job]:
         """Returns job by job id.
 
         Args:
             job_id: job id
@@ -275,68 +226,14 @@
         return Widget(self._selected_provider).show()
 
     def __repr__(self):
         providers = ", ".join(provider.name for provider in self.providers())
         return f"<QuantumServerless | providers [{providers}]>"
 
 
-def load_config(config: Optional[Dict[str, Any]] = None) -> List[Provider]:
-    """Loads providers from configuration."""
-    local_provider = Provider(
-        name="local",
-        compute_resource=ComputeResource(name="local"),
-        available_compute_resources=[ComputeResource(name="local")],
-    )
-    providers = [local_provider]
-
-    if config is not None:
-        for provider_config in config.get("providers", []):
-            compute_resource = None
-            if provider_config.get("compute_resource"):
-                compute_resource = ComputeResource(
-                    **provider_config.get("compute_resource")
-                )
-            # support compute_resource definition
-            if provider_config.get("cluster"):
-                warnings.warn(
-                    "Clusters has been deprecated in favor of compute resources."
-                    "Use `compute_resource` instead of `compute_resource`.",
-                    DeprecationWarning,
-                )
-                compute_resource = ComputeResource(
-                    **provider_config.get("compute_resource")
-                )
-
-            available_compute_resources = []
-            if provider_config.get("available_compute_resources"):
-                for resource_json in provider_config.get("available_compute_resources"):
-                    available_compute_resources.append(ComputeResource(**resource_json))
-            providers.append(
-                Provider(
-                    **{
-                        **provider_config,
-                        **{
-                            "compute_resource": compute_resource,
-                            "available_compute_resources": available_compute_resources,
-                        },
-                    }
-                )
-            )
-
-    if os.environ.get("QS_CLUSTER_MANAGER_ADDRESS", None):
-        auto_discovered_provider = get_auto_discovered_provider(
-            manager_address=os.environ.get("QS_CLUSTER_MANAGER_ADDRESS"),
-            token=os.environ.get("QS_CLUSTER_MANAGER_TOKEN"),
-        )
-        if auto_discovered_provider is not None:
-            providers.append(auto_discovered_provider)
-
-    return providers
-
-
 def get_auto_discovered_provider(
     manager_address: str, token: Optional[str] = None
 ) -> Optional[Provider]:
     """Makes http request to manager to get available clusters."""
     compute_resources = []
 
     headers = {"Authorization": f"Bearer {token}"} if token else None
```

### Comparing `quantum_serverless-0.2.0/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.2.1/quantum_serverless/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/serializers/program_serializers.py` & `quantum_serverless-0.2.1/quantum_serverless/serializers/program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.2.1/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.2.1/quantum_serverless/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/utils/errors.py` & `quantum_serverless-0.2.1/quantum_serverless/utils/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/utils/json.py` & `quantum_serverless-0.2.1/quantum_serverless/utils/json.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/utils/storage.py` & `quantum_serverless-0.2.1/quantum_serverless/utils/storage.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/visualizaiton/__init__.py` & `quantum_serverless-0.2.1/quantum_serverless/visualizaiton/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless/visualizaiton/widget.py` & `quantum_serverless-0.2.1/quantum_serverless/visualizaiton/widget.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/quantum_serverless.egg-info/PKG-INFO` & `quantum_serverless-0.2.1/quantum_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-serverless
-Version: 0.2.0
+Version: 0.2.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.2.0/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.2.1/quantum_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/setup.py` & `quantum_serverless-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/tests/core/test_decorator.py` & `quantum_serverless-0.2.1/tests/core/test_decorator.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/tests/core/test_program.py` & `quantum_serverless-0.2.1/tests/core/test_program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/tests/core/test_program_repository.py` & `quantum_serverless-0.2.1/tests/core/test_program_repository.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/tests/core/test_state.py` & `quantum_serverless-0.2.1/tests/core/test_state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/tests/library/test_transpiler.py` & `quantum_serverless-0.2.1/tests/library/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/tests/serializers/test_program_serializers.py` & `quantum_serverless-0.2.1/tests/serializers/test_program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/tests/serializers/test_serializers.py` & `quantum_serverless-0.2.1/tests/serializers/test_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/tests/test_quantum_serverless.py` & `quantum_serverless-0.2.1/tests/test_quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.2.0/tests/utils.py` & `quantum_serverless-0.2.1/tests/utils.py`

 * *Files identical despite different names*

