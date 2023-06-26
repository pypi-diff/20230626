# Comparing `tmp/vdk-test-utils-0.2.824443273.tar.gz` & `tmp/vdk-test-utils-0.2.911997964.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-test-utils-0.2.824443273.tar", last modified: Fri Mar 31 14:26:29 2023, max compression
+gzip compressed data, was "vdk-test-utils-0.2.911997964.tar", last modified: Mon Jun 26 13:44:27 2023, max compression
```

## Comparing `vdk-test-utils-0.2.824443273.tar` & `vdk-test-utils-0.2.911997964.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:29.137238 vdk-test-utils-0.2.824443273/
--rw-r--r--   0 root         (0) root         (0)     1501 2023-03-31 14:26:29.137238 vdk-test-utils-0.2.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-03-31 14:26:17.000000 vdk-test-utils-0.2.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:26:29.137238 vdk-test-utils-0.2.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-03-31 14:26:21.000000 vdk-test-utils-0.2.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:29.137238 vdk-test-utils-0.2.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:29.137238 vdk-test-utils-0.2.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:29.137238 vdk-test-utils-0.2.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:29.137238 vdk-test-utils-0.2.824443273/src/vdk/plugin/test_utils/
--rw-rw-rw-   0 root         (0) root         (0)     4347 2023-03-31 14:26:17.000000 vdk-test-utils-0.2.824443273/src/vdk/plugin/test_utils/ingest_util_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     9465 2023-03-31 14:26:17.000000 vdk-test-utils-0.2.824443273/src/vdk/plugin/test_utils/util_funcs.py
--rw-rw-rw-   0 root         (0) root         (0)     5779 2023-03-31 14:26:17.000000 vdk-test-utils-0.2.824443273/src/vdk/plugin/test_utils/util_plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:29.137238 vdk-test-utils-0.2.824443273/src/vdk_test_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1501 2023-03-31 14:26:29.000000 vdk-test-utils-0.2.824443273/src/vdk_test_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2023-03-31 14:26:29.000000 vdk-test-utils-0.2.824443273/src/vdk_test_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:26:29.000000 vdk-test-utils-0.2.824443273/src/vdk_test_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-31 14:26:29.000000 vdk-test-utils-0.2.824443273/src/vdk_test_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:26:29.000000 vdk-test-utils-0.2.824443273/src/vdk_test_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:29.137238 vdk-test-utils-0.2.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-03-31 14:26:17.000000 vdk-test-utils-0.2.824443273/tests/test_util_funcs.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-03-31 14:26:17.000000 vdk-test-utils-0.2.824443273/tests/test_vdk_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-06-26 13:44:17.000000 vdk-test-utils-0.2.911997964/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.599171 vdk-test-utils-0.2.911997964/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     4347 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/ingest_util_plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     9551 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/util_funcs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/util_plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/tests/test_util_funcs.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/tests/test_vdk_test_utils.py
```

### Comparing `vdk-test-utils-0.2.824443273/PKG-INFO` & `vdk-test-utils-0.2.911997964/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-test-utils
-Version: 0.2.824443273
+Version: 0.2.911997964
 Summary: Provides utilities for testing Versatile Data Kit SDK plugins.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-test-utils-0.2.824443273/README.md` & `vdk-test-utils-0.2.911997964/README.md`

 * *Files identical despite different names*

### Comparing `vdk-test-utils-0.2.824443273/setup.py` & `vdk-test-utils-0.2.911997964/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.824443273"
+__version__ = "0.2.911997964"
 
 setuptools.setup(
     name="vdk-test-utils",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Provides utilities for testing Versatile Data Kit SDK plugins.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-test-utils-0.2.824443273/src/vdk/plugin/test_utils/ingest_util_plugins.py` & `vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/ingest_util_plugins.py`

 * *Files identical despite different names*

### Comparing `vdk-test-utils-0.2.824443273/src/vdk/plugin/test_utils/util_funcs.py` & `vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/util_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from vdk.internal.builtin_plugins.run.step import StepFunction
 from vdk.internal.cli_entry import CliEntry
 from vdk.internal.core.config import ConfigurationBuilder
 from vdk.internal.core.context import CoreContext
 from vdk.internal.core.statestore import StateStore
 from vdk.internal.plugin.plugin import PluginRegistry
 from vdk.plugin.test_utils.util_plugins import TestPropertiesPlugin
+from vdk.plugin.test_utils.util_plugins import TestSecretsPlugin
 
 
 def cli_assert(
     is_true: bool, result: Result, message: str = "result assert fails"
 ) -> None:
     """
     Test if some statement is true .
@@ -117,15 +118,15 @@
     """
 
     def __init__(self, *plugins):
         """
         :param plugins: the list of plugins that should be loaded during this test run.
         """
         self._plugins = plugins
-        self._default_plugins = [TestPropertiesPlugin()]
+        self._default_plugins = [TestPropertiesPlugin(), TestSecretsPlugin()]
 
     def clear_default_plugins(self):
         self._default_plugins.clear()
 
     def invoke(self, args, cli=cli_entry.cli, **extra) -> Result:
         plugin_registry = PluginRegistry()
         plugin_registry.add_hook_specs(InternalHookSpecs)
```

### Comparing `vdk-test-utils-0.2.824443273/src/vdk/plugin/test_utils/util_plugins.py` & `vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/util_plugins.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.api.plugin.plugin_input import IIngesterPlugin
 from vdk.api.plugin.plugin_input import IPropertiesServiceClient
+from vdk.api.plugin.plugin_input import ISecretsServiceClient
 from vdk.internal.builtin_plugins.connection.decoration_cursor import DecorationCursor
 from vdk.internal.builtin_plugins.connection.managed_connection_base import (
     ManagedConnectionBase,
 )
 from vdk.internal.builtin_plugins.connection.pep249.interfaces import PEP249Connection
 from vdk.internal.builtin_plugins.run.job_context import JobContext
 from vdk.internal.core.config import ConfigurationBuilder
@@ -144,14 +145,54 @@
     @hookimpl
     def initialize_job(self, context: JobContext) -> None:
         context.properties.set_properties_factory_method(
             "test-property-decorated", lambda: self
         )
 
 
+class TestSecretsServiceClient(ISecretsServiceClient):
+    """Testing secrets client that keeps in memory per job properties."""
+
+    def __init__(self):
+        self._secrets = {}
+
+    def read_secrets(self, job_name: str, team_name: str) -> Dict:
+        res = deepcopy(self._secrets.get(job_name, {}))
+        return res
+
+    def write_secrets(self, job_name: str, team_name: str, secrets: Dict) -> Dict:
+        self._secrets[job_name] = deepcopy(secrets)
+        return self._secrets[job_name]
+
+
+class TestSecretsPlugin:
+    def __init__(self):
+        self.secrets_client = TestSecretsServiceClient()
+
+    @hookimpl
+    def initialize_job(self, context: JobContext) -> None:
+        context.secrets.set_secrets_factory_method(
+            "default", lambda: self.secrets_client
+        )
+
+
+class TestSecretsDecoratedPlugin(ISecretsServiceClient):
+    def read_secrets(self, job_name: str, team_name: str) -> Dict:
+        raise NotImplementedError()
+
+    def write_secrets(self, job_name: str, team_name: str, secrets: Dict) -> Dict:
+        return {**secrets, **{"test": "True"}}
+
+    @hookimpl
+    def initialize_job(self, context: JobContext) -> None:
+        context.secrets.set_secrets_factory_method(
+            "test-secret-decorated", lambda: self
+        )
+
+
 class IngestIntoMemoryPlugin(IIngesterPlugin):
     """
     Create a new ingestion mechanism to ingest data into memory
     """
 
     @dataclass
     class Payload:
```

### Comparing `vdk-test-utils-0.2.824443273/src/vdk_test_utils.egg-info/PKG-INFO` & `vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-test-utils
-Version: 0.2.824443273
+Version: 0.2.911997964
 Summary: Provides utilities for testing Versatile Data Kit SDK plugins.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-test-utils-0.2.824443273/tests/test_util_funcs.py` & `vdk-test-utils-0.2.911997964/tests/test_util_funcs.py`

 * *Files identical despite different names*

