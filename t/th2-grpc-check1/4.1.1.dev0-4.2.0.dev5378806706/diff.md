# Comparing `tmp/th2_grpc_check1-4.1.1.dev0.tar.gz` & `tmp/th2_grpc_check1-4.2.0.dev5378806706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_check1-4.1.1.dev0.tar", last modified: Sun Apr  2 20:21:30 2023, max compression
+gzip compressed data, was "dist/th2_grpc_check1-4.2.0.dev5378806706.tar", last modified: Mon Jun 26 13:38:17 2023, max compression
```

## Comparing `th2_grpc_check1-4.1.1.dev0.tar` & `th2_grpc_check1-4.2.0.dev5378806706.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (122)     4209 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3099 2023-04-02 20:20:42.000000 th2_grpc_check1-4.1.1.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-02 20:20:42.000000 th2_grpc_check1-4.1.1.dev0/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4576 2023-04-02 20:20:42.000000 th2_grpc_check1-4.1.1.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-04-02 20:20:42.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/check1.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5803 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/check1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    16750 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/check1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7709 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/check1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-04-02 20:21:12.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/check1_service.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4209 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-02 20:21:30.000000 th2_grpc_check1-4.1.1.dev0/th2_grpc_check1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-26 13:37:08.000000 th2_grpc_check1-4.2.0.dev5378806706/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-26 13:37:08.000000 th2_grpc_check1-4.2.0.dev5378806706/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4587 2023-06-26 13:37:08.000000 th2_grpc_check1-4.2.0.dev5378806706/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-06-26 13:37:08.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6110 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17519 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7709 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-26 13:37:50.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:16.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-26 13:38:17.000000 th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/top_level.txt
```

### Comparing `th2_grpc_check1-4.1.1.dev0/PKG-INFO` & `th2_grpc_check1-4.2.0.dev5378806706/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,85 @@
 Metadata-Version: 2.1
 Name: th2_grpc_check1
-Version: 4.1.1.dev0
+Version: 4.2.0.dev5378806706
 Summary: th2_grpc_check1
 Home-page: https://github.com/th2-net/th2-grpc-check1
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC check1 library (4.1.0)
+Description: # th2 gRPC check1 library (4.2.0)
         
-        This library contains proto messages and `Check1` service with RPC methods that are used in [th2 check1](https://github.com/th2-net/th2-check1 "th2-check1"). See [check1.proto](src/main/proto/th2_grpc_check1/check1.proto "check1.proto") file for details. <br>
-        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to the specified repositories.
+        This library contains proto messages and `Check1` service with RPC methods that are used
+        in [th2 check1](https://github.com/th2-net/th2-check1 "th2-check1").
+        See [check1.proto](src/main/proto/th2_grpc_check1/check1.proto "check1.proto") file for details. <br>
+        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to the specified
+        repositories.
         
         ## How to maintain a project
+        
         1. Perform the necessary changes.
         2. Update the package version of Java in `gradle.properties` file.
         3. Update the package version of Python in `package_info.json` file.
         4. Commit everything.
         
         ### Java
+        
         If you wish to manually create and publish a package for Java, run the following command:
+        
         ```
         gradle --no-daemon clean build publish artifactoryPublish \
                -Purl=${URL} \ 
                -Puser=${USER} \
                -Ppassword=${PASSWORD}
         ```
+        
         `URL`, `USER` and `PASSWORD` are parameters for publishing.
         
         ### Python
+        
         If you wish to manually create and publish a package for Python:
+        
         1. Generate services with `Gradle`:
             ```
                gradle --no-daemon clean generateProto
             ```
            You can find the generated files by following path: `src/gen/main/services/python`
         2. Generate code from `.proto` files and publish everything using `twine`:
             ```
             pip install -r requirements.txt
             pip install twine
             python setup.py generate
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
-            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
+           `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 4.2.0
+        
+        + Added golang specific properties
+        + Updated bom:4.4.0
+        + Updated grpc-service-generator:3.4.0
+        + Updated mypy-protobuf:3.4
+        
         ### 4.1.0
+        
         + merged `3.8.0`
         
         ### 4.0.0
+        
         + Migrated to `grpc-common` version with books/pages
         + Marked deprecated fields as `reserved`
         + Added `book_name` to `CheckRuleRequest`, `CheckSequenceRuleRequest` and `NoMessageCheckRequest`
         
         ### 3.8.0
         
-        + Update `th2-bom` to `4.2.0` 
-        + Update `grpc-service-generator` to `3.3.1` 
+        + Update `th2-bom` to `4.2.0`
+        + Update `grpc-service-generator` to `3.3.1`
         + Updated grpc to `1.48.1`
         + Updated protobuf to `3.21.7`
         + Add Python vulnerabilities scan
         
         ### 3.7.0
         
         + Update `th2-bom` to `4.1.0`
@@ -75,34 +93,40 @@
         #### Changed:
         
         + `grpc-common` version is updated to 3.9.0
         
         ### 3.5.0
         
         #### Added:
-        + `silence_check` parameter for `CheckSequenceRule`. Enables automated check for extra messages that match the pre-filter.
+        
+        + `silence_check` parameter for `CheckSequenceRule`. Enables automated check for extra messages that match the
+          pre-filter.
         
         #### Changed:
+        
         + Migrated `grpc-common` version from `3.7.0` to `3.8.0`
-          + Added `time_precision` and `decimal_precision` to `RootComparisonSettings` message
-          + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operations
+            + Added `time_precision` and `decimal_precision` to `RootComparisonSettings` message
+            + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operations
         
         ### 3.4.2
+        
         + Migrated `grpc-common` version from `3.6.0` to `3.7.0`
             + Added `check_repeating_group_order` parameter to `RootComparisonSettings` message
         
         ### 3.4.1
+        
         + Migrated `grpc-common` version from `3.4.0` to `3.6.0`
-          + Added the new parameters `description` to `RootMessageFilter` message
+            + Added the new parameters `description` to `RootMessageFilter` message
         
         ### 3.4.0
         
         + Update to `th2-grpc-common` version `3.4.0`
         
         ### 3.3.0
+        
         + Implemented NoMessageCheck rule task. Updated CheckSequence rule task
         
         ### 3.2.0
         
         + Implement stubs creation for Python
         
 Platform: UNKNOWN
```

### Comparing `th2_grpc_check1-4.1.1.dev0/README.md` & `th2_grpc_check1-4.2.0.dev5378806706/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,77 @@
-# th2 gRPC check1 library (4.1.0)
+# th2 gRPC check1 library (4.2.0)
 
-This library contains proto messages and `Check1` service with RPC methods that are used in [th2 check1](https://github.com/th2-net/th2-check1 "th2-check1"). See [check1.proto](src/main/proto/th2_grpc_check1/check1.proto "check1.proto") file for details. <br>
-Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to the specified repositories.
+This library contains proto messages and `Check1` service with RPC methods that are used
+in [th2 check1](https://github.com/th2-net/th2-check1 "th2-check1").
+See [check1.proto](src/main/proto/th2_grpc_check1/check1.proto "check1.proto") file for details. <br>
+Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to the specified
+repositories.
 
 ## How to maintain a project
+
 1. Perform the necessary changes.
 2. Update the package version of Java in `gradle.properties` file.
 3. Update the package version of Python in `package_info.json` file.
 4. Commit everything.
 
 ### Java
+
 If you wish to manually create and publish a package for Java, run the following command:
+
 ```
 gradle --no-daemon clean build publish artifactoryPublish \
        -Purl=${URL} \ 
        -Puser=${USER} \
        -Ppassword=${PASSWORD}
 ```
+
 `URL`, `USER` and `PASSWORD` are parameters for publishing.
 
 ### Python
+
 If you wish to manually create and publish a package for Python:
+
 1. Generate services with `Gradle`:
     ```
        gradle --no-daemon clean generateProto
     ```
    You can find the generated files by following path: `src/gen/main/services/python`
 2. Generate code from `.proto` files and publish everything using `twine`:
     ```
     pip install -r requirements.txt
     pip install twine
     python setup.py generate
     python setup.py sdist
     twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
     ```
-    `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
+   `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
 
 ## Release notes
 
+### 4.2.0
+
++ Added golang specific properties
++ Updated bom:4.4.0
++ Updated grpc-service-generator:3.4.0
++ Updated mypy-protobuf:3.4
+
 ### 4.1.0
+
 + merged `3.8.0`
 
 ### 4.0.0
+
 + Migrated to `grpc-common` version with books/pages
 + Marked deprecated fields as `reserved`
 + Added `book_name` to `CheckRuleRequest`, `CheckSequenceRuleRequest` and `NoMessageCheckRequest`
 
 ### 3.8.0
 
-+ Update `th2-bom` to `4.2.0` 
-+ Update `grpc-service-generator` to `3.3.1` 
++ Update `th2-bom` to `4.2.0`
++ Update `grpc-service-generator` to `3.3.1`
 + Updated grpc to `1.48.1`
 + Updated protobuf to `3.21.7`
 + Add Python vulnerabilities scan
 
 ### 3.7.0
 
 + Update `th2-bom` to `4.1.0`
@@ -67,32 +85,38 @@
 #### Changed:
 
 + `grpc-common` version is updated to 3.9.0
 
 ### 3.5.0
 
 #### Added:
-+ `silence_check` parameter for `CheckSequenceRule`. Enables automated check for extra messages that match the pre-filter.
+
++ `silence_check` parameter for `CheckSequenceRule`. Enables automated check for extra messages that match the
+  pre-filter.
 
 #### Changed:
+
 + Migrated `grpc-common` version from `3.7.0` to `3.8.0`
-  + Added `time_precision` and `decimal_precision` to `RootComparisonSettings` message
-  + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operations
+    + Added `time_precision` and `decimal_precision` to `RootComparisonSettings` message
+    + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operations
 
 ### 3.4.2
+
 + Migrated `grpc-common` version from `3.6.0` to `3.7.0`
     + Added `check_repeating_group_order` parameter to `RootComparisonSettings` message
 
 ### 3.4.1
+
 + Migrated `grpc-common` version from `3.4.0` to `3.6.0`
-  + Added the new parameters `description` to `RootMessageFilter` message
+    + Added the new parameters `description` to `RootMessageFilter` message
 
 ### 3.4.0
 
 + Update to `th2-grpc-common` version `3.4.0`
 
 ### 3.3.0
+
 + Implemented NoMessageCheck rule task. Updated CheckSequence rule task
 
 ### 3.2.0
 
 + Implement stubs creation for Python
```

### Comparing `th2_grpc_check1-4.1.1.dev0/setup.py` & `th2_grpc_check1-4.2.0.dev5378806706/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
     long_description_content_type='text/markdown',
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-check1',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
-        'th2-grpc-common>=4.2.0,<5',
-        'mypy-protobuf==3.2'
+        'th2-grpc-common==4.3.0.dev5378777004',
+        'mypy-protobuf==3.4'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
     }
```

### Comparing `th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/check1.proto` & `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/check1_pb2.pyi` & `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,101 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
+
+Copyright 2020-2021 Exactpro (Exactpro Systems Limited)
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.wrappers_pb2
+import sys
 import th2_grpc_common.common_pb2
-import typing
-import typing_extensions
+
+if sys.version_info >= (3, 8):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class CheckpointRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     DESCRIPTION_FIELD_NUMBER: builtins.int
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
-    description: typing.Text
+    description: builtins.str
     @property
     def parent_event_id(self) -> th2_grpc_common.common_pb2.EventID: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        description: typing.Text = ...,
-        parent_event_id: typing.Optional[th2_grpc_common.common_pb2.EventID] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["parent_event_id",b"parent_event_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description",b"description","parent_event_id",b"parent_event_id"]) -> None: ...
+        description: builtins.str = ...,
+        parent_event_id: th2_grpc_common.common_pb2.EventID | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["parent_event_id", b"parent_event_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "parent_event_id", b"parent_event_id"]) -> None: ...
+
 global___CheckpointRequest = CheckpointRequest
 
+@typing_extensions.final
 class CheckpointResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     CHECKPOINT_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     @property
     def checkpoint(self) -> th2_grpc_common.common_pb2.Checkpoint: ...
     @property
     def status(self) -> th2_grpc_common.common_pb2.RequestStatus: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        checkpoint: typing.Optional[th2_grpc_common.common_pb2.Checkpoint] = ...,
-        status: typing.Optional[th2_grpc_common.common_pb2.RequestStatus] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["checkpoint",b"checkpoint","status",b"status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["checkpoint",b"checkpoint","status",b"status"]) -> None: ...
+        checkpoint: th2_grpc_common.common_pb2.Checkpoint | None = ...,
+        status: th2_grpc_common.common_pb2.RequestStatus | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["checkpoint", b"checkpoint", "status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["checkpoint", b"checkpoint", "status", b"status"]) -> None: ...
+
 global___CheckpointResponse = CheckpointResponse
 
+@typing_extensions.final
 class ChainID(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     ID_FIELD_NUMBER: builtins.int
-    id: typing.Text
-    def __init__(self,
+    id: builtins.str
+    def __init__(
+        self,
         *,
-        id: typing.Text = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id",b"id"]) -> None: ...
+        id: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
+
 global___ChainID = ChainID
 
+@typing_extensions.final
 class CheckRuleRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     CONNECTIVITY_ID_FIELD_NUMBER: builtins.int
     ROOT_FILTER_FIELD_NUMBER: builtins.int
     CHECKPOINT_FIELD_NUMBER: builtins.int
     MESSAGE_TIMEOUT_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
@@ -72,70 +105,72 @@
     @property
     def connectivity_id(self) -> th2_grpc_common.common_pb2.ConnectionID: ...
     @property
     def root_filter(self) -> th2_grpc_common.common_pb2.RootMessageFilter: ...
     @property
     def checkpoint(self) -> th2_grpc_common.common_pb2.Checkpoint:
         """Registered Checkpoint. If the chain_id is also set in the request the checkpoint will be ignored"""
-        pass
     message_timeout: builtins.int
     """Timeout to wait for messages after checkpoint. The message's timestamp will be used to compute the timeout"""
-
     timeout: builtins.int
     """Timeout for rule execution. Uses the real time to limit the execution of the rule"""
-
     @property
     def parent_event_id(self) -> th2_grpc_common.common_pb2.EventID: ...
-    description: typing.Text
+    description: builtins.str
     direction: th2_grpc_common.common_pb2.Direction.ValueType
     @property
     def chain_id(self) -> global___ChainID:
         """The chain id to continue checking."""
-        pass
-    book_name: typing.Text
+    book_name: builtins.str
     """If it's not set the check will be started from the specified checkpoint otherwise checkpoint will be ignored"""
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        connectivity_id: typing.Optional[th2_grpc_common.common_pb2.ConnectionID] = ...,
-        root_filter: typing.Optional[th2_grpc_common.common_pb2.RootMessageFilter] = ...,
-        checkpoint: typing.Optional[th2_grpc_common.common_pb2.Checkpoint] = ...,
+        connectivity_id: th2_grpc_common.common_pb2.ConnectionID | None = ...,
+        root_filter: th2_grpc_common.common_pb2.RootMessageFilter | None = ...,
+        checkpoint: th2_grpc_common.common_pb2.Checkpoint | None = ...,
         message_timeout: builtins.int = ...,
         timeout: builtins.int = ...,
-        parent_event_id: typing.Optional[th2_grpc_common.common_pb2.EventID] = ...,
-        description: typing.Text = ...,
+        parent_event_id: th2_grpc_common.common_pb2.EventID | None = ...,
+        description: builtins.str = ...,
         direction: th2_grpc_common.common_pb2.Direction.ValueType = ...,
-        chain_id: typing.Optional[global___ChainID] = ...,
-        book_name: typing.Text = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","checkpoint",b"checkpoint","connectivity_id",b"connectivity_id","parent_event_id",b"parent_event_id","root_filter",b"root_filter"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["book_name",b"book_name","chain_id",b"chain_id","checkpoint",b"checkpoint","connectivity_id",b"connectivity_id","description",b"description","direction",b"direction","message_timeout",b"message_timeout","parent_event_id",b"parent_event_id","root_filter",b"root_filter","timeout",b"timeout"]) -> None: ...
+        chain_id: global___ChainID | None = ...,
+        book_name: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["chain_id", b"chain_id", "checkpoint", b"checkpoint", "connectivity_id", b"connectivity_id", "parent_event_id", b"parent_event_id", "root_filter", b"root_filter"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["book_name", b"book_name", "chain_id", b"chain_id", "checkpoint", b"checkpoint", "connectivity_id", b"connectivity_id", "description", b"description", "direction", b"direction", "message_timeout", b"message_timeout", "parent_event_id", b"parent_event_id", "root_filter", b"root_filter", "timeout", b"timeout"]) -> None: ...
+
 global___CheckRuleRequest = CheckRuleRequest
 
+@typing_extensions.final
 class CheckRuleResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     STATUS_FIELD_NUMBER: builtins.int
     CHAIN_ID_FIELD_NUMBER: builtins.int
     @property
     def status(self) -> th2_grpc_common.common_pb2.RequestStatus: ...
     @property
     def chain_id(self) -> global___ChainID:
         """You can use it to unite the next rule to the chain with currently submitted one"""
-        pass
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        status: typing.Optional[th2_grpc_common.common_pb2.RequestStatus] = ...,
-        chain_id: typing.Optional[global___ChainID] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","status",b"status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","status",b"status"]) -> None: ...
+        status: th2_grpc_common.common_pb2.RequestStatus | None = ...,
+        chain_id: global___ChainID | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["chain_id", b"chain_id", "status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["chain_id", b"chain_id", "status", b"status"]) -> None: ...
+
 global___CheckRuleResponse = CheckRuleResponse
 
+@typing_extensions.final
 class CheckSequenceRuleRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     PRE_FILTER_FIELD_NUMBER: builtins.int
     ROOT_MESSAGE_FILTERS_FIELD_NUMBER: builtins.int
     CHECKPOINT_FIELD_NUMBER: builtins.int
     MESSAGE_TIMEOUT_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
     CONNECTIVITY_ID_FIELD_NUMBER: builtins.int
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
@@ -148,175 +183,184 @@
     @property
     def pre_filter(self) -> global___PreFilter: ...
     @property
     def root_message_filters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[th2_grpc_common.common_pb2.RootMessageFilter]:
         """
         Either this field or message_filters must be set. If both are set the error response will be received from check1
         """
-        pass
     @property
     def checkpoint(self) -> th2_grpc_common.common_pb2.Checkpoint:
         """Registered Checkpoint. If the chain_id is also set in the request the checkpoint will be ignored"""
-        pass
     message_timeout: builtins.int
     """Timeout to wait for messages after checkpoint. The message's timestamp will be used to compute the timeout"""
-
     timeout: builtins.int
     """Timeout for rule execution. Uses the real time to limit the execution of the rule"""
-
     @property
     def connectivity_id(self) -> th2_grpc_common.common_pb2.ConnectionID: ...
     @property
     def parent_event_id(self) -> th2_grpc_common.common_pb2.EventID: ...
     check_order: builtins.bool
-    description: typing.Text
+    description: builtins.str
     direction: th2_grpc_common.common_pb2.Direction.ValueType
     @property
     def chain_id(self) -> global___ChainID:
         """The chain id to continue checking."""
-        pass
     @property
     def silence_check(self) -> google.protobuf.wrappers_pb2.BoolValue:
         """If it's not set the check will be started from the specified checkpoint otherwise checkpoint will be ignored"""
-        pass
-    book_name: typing.Text
-    def __init__(self,
+    book_name: builtins.str
+    def __init__(
+        self,
         *,
-        pre_filter: typing.Optional[global___PreFilter] = ...,
-        root_message_filters: typing.Optional[typing.Iterable[th2_grpc_common.common_pb2.RootMessageFilter]] = ...,
-        checkpoint: typing.Optional[th2_grpc_common.common_pb2.Checkpoint] = ...,
+        pre_filter: global___PreFilter | None = ...,
+        root_message_filters: collections.abc.Iterable[th2_grpc_common.common_pb2.RootMessageFilter] | None = ...,
+        checkpoint: th2_grpc_common.common_pb2.Checkpoint | None = ...,
         message_timeout: builtins.int = ...,
         timeout: builtins.int = ...,
-        connectivity_id: typing.Optional[th2_grpc_common.common_pb2.ConnectionID] = ...,
-        parent_event_id: typing.Optional[th2_grpc_common.common_pb2.EventID] = ...,
+        connectivity_id: th2_grpc_common.common_pb2.ConnectionID | None = ...,
+        parent_event_id: th2_grpc_common.common_pb2.EventID | None = ...,
         check_order: builtins.bool = ...,
-        description: typing.Text = ...,
+        description: builtins.str = ...,
         direction: th2_grpc_common.common_pb2.Direction.ValueType = ...,
-        chain_id: typing.Optional[global___ChainID] = ...,
-        silence_check: typing.Optional[google.protobuf.wrappers_pb2.BoolValue] = ...,
-        book_name: typing.Text = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","checkpoint",b"checkpoint","connectivity_id",b"connectivity_id","parent_event_id",b"parent_event_id","pre_filter",b"pre_filter","silence_check",b"silence_check"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["book_name",b"book_name","chain_id",b"chain_id","check_order",b"check_order","checkpoint",b"checkpoint","connectivity_id",b"connectivity_id","description",b"description","direction",b"direction","message_timeout",b"message_timeout","parent_event_id",b"parent_event_id","pre_filter",b"pre_filter","root_message_filters",b"root_message_filters","silence_check",b"silence_check","timeout",b"timeout"]) -> None: ...
+        chain_id: global___ChainID | None = ...,
+        silence_check: google.protobuf.wrappers_pb2.BoolValue | None = ...,
+        book_name: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["chain_id", b"chain_id", "checkpoint", b"checkpoint", "connectivity_id", b"connectivity_id", "parent_event_id", b"parent_event_id", "pre_filter", b"pre_filter", "silence_check", b"silence_check"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["book_name", b"book_name", "chain_id", b"chain_id", "check_order", b"check_order", "checkpoint", b"checkpoint", "connectivity_id", b"connectivity_id", "description", b"description", "direction", b"direction", "message_timeout", b"message_timeout", "parent_event_id", b"parent_event_id", "pre_filter", b"pre_filter", "root_message_filters", b"root_message_filters", "silence_check", b"silence_check", "timeout", b"timeout"]) -> None: ...
+
 global___CheckSequenceRuleRequest = CheckSequenceRuleRequest
 
+@typing_extensions.final
 class CheckSequenceRuleResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     STATUS_FIELD_NUMBER: builtins.int
     CHAIN_ID_FIELD_NUMBER: builtins.int
     @property
     def status(self) -> th2_grpc_common.common_pb2.RequestStatus: ...
     @property
     def chain_id(self) -> global___ChainID:
         """You can use it to unite the next rule to the chain with currently submitted one"""
-        pass
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        status: typing.Optional[th2_grpc_common.common_pb2.RequestStatus] = ...,
-        chain_id: typing.Optional[global___ChainID] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","status",b"status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","status",b"status"]) -> None: ...
+        status: th2_grpc_common.common_pb2.RequestStatus | None = ...,
+        chain_id: global___ChainID | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["chain_id", b"chain_id", "status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["chain_id", b"chain_id", "status", b"status"]) -> None: ...
+
 global___CheckSequenceRuleResponse = CheckSequenceRuleResponse
 
+@typing_extensions.final
 class PreFilter(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class FieldsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text
+        key: builtins.str
         @property
         def value(self) -> th2_grpc_common.common_pb2.ValueFilter: ...
-        def __init__(self,
+        def __init__(
+            self,
             *,
-            key: typing.Text = ...,
-            value: typing.Optional[th2_grpc_common.common_pb2.ValueFilter] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value",b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
+            key: builtins.str = ...,
+            value: th2_grpc_common.common_pb2.ValueFilter | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FIELDS_FIELD_NUMBER: builtins.int
     METADATA_FILTER_FIELD_NUMBER: builtins.int
     @property
-    def fields(self) -> google.protobuf.internal.containers.MessageMap[typing.Text, th2_grpc_common.common_pb2.ValueFilter]: ...
+    def fields(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, th2_grpc_common.common_pb2.ValueFilter]: ...
     @property
     def metadata_filter(self) -> th2_grpc_common.common_pb2.MetadataFilter: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        fields: typing.Optional[typing.Mapping[typing.Text, th2_grpc_common.common_pb2.ValueFilter]] = ...,
-        metadata_filter: typing.Optional[th2_grpc_common.common_pb2.MetadataFilter] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["metadata_filter",b"metadata_filter"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fields",b"fields","metadata_filter",b"metadata_filter"]) -> None: ...
+        fields: collections.abc.Mapping[builtins.str, th2_grpc_common.common_pb2.ValueFilter] | None = ...,
+        metadata_filter: th2_grpc_common.common_pb2.MetadataFilter | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["metadata_filter", b"metadata_filter"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["fields", b"fields", "metadata_filter", b"metadata_filter"]) -> None: ...
+
 global___PreFilter = PreFilter
 
+@typing_extensions.final
 class NoMessageCheckRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     PRE_FILTER_FIELD_NUMBER: builtins.int
     MESSAGE_TIMEOUT_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
     CHECKPOINT_FIELD_NUMBER: builtins.int
     CHAIN_ID_FIELD_NUMBER: builtins.int
     CONNECTIVITY_ID_FIELD_NUMBER: builtins.int
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     DIRECTION_FIELD_NUMBER: builtins.int
     BOOK_NAME_FIELD_NUMBER: builtins.int
     @property
     def pre_filter(self) -> global___PreFilter: ...
     message_timeout: builtins.int
     """Timeout to wait for messages after checkpoint. The message's timestamp will be used to compute the timeout"""
-
     timeout: builtins.int
     """Timeout for rule execution. Uses the real time to limit the execution of the rule"""
-
     @property
     def checkpoint(self) -> th2_grpc_common.common_pb2.Checkpoint:
         """Registered Checkpoint. If the chain_id is also set in the request the checkpoint will be ignored"""
-        pass
     @property
     def chain_id(self) -> global___ChainID:
         """You can use it to unite the next rule to the chain with currently submitted one"""
-        pass
     @property
     def connectivity_id(self) -> th2_grpc_common.common_pb2.ConnectionID: ...
     @property
     def parent_event_id(self) -> th2_grpc_common.common_pb2.EventID: ...
-    description: typing.Text
+    description: builtins.str
     direction: th2_grpc_common.common_pb2.Direction.ValueType
-    book_name: typing.Text
-    def __init__(self,
+    book_name: builtins.str
+    def __init__(
+        self,
         *,
-        pre_filter: typing.Optional[global___PreFilter] = ...,
+        pre_filter: global___PreFilter | None = ...,
         message_timeout: builtins.int = ...,
         timeout: builtins.int = ...,
-        checkpoint: typing.Optional[th2_grpc_common.common_pb2.Checkpoint] = ...,
-        chain_id: typing.Optional[global___ChainID] = ...,
-        connectivity_id: typing.Optional[th2_grpc_common.common_pb2.ConnectionID] = ...,
-        parent_event_id: typing.Optional[th2_grpc_common.common_pb2.EventID] = ...,
-        description: typing.Text = ...,
+        checkpoint: th2_grpc_common.common_pb2.Checkpoint | None = ...,
+        chain_id: global___ChainID | None = ...,
+        connectivity_id: th2_grpc_common.common_pb2.ConnectionID | None = ...,
+        parent_event_id: th2_grpc_common.common_pb2.EventID | None = ...,
+        description: builtins.str = ...,
         direction: th2_grpc_common.common_pb2.Direction.ValueType = ...,
-        book_name: typing.Text = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","checkpoint",b"checkpoint","connectivity_id",b"connectivity_id","parent_event_id",b"parent_event_id","pre_filter",b"pre_filter"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["book_name",b"book_name","chain_id",b"chain_id","checkpoint",b"checkpoint","connectivity_id",b"connectivity_id","description",b"description","direction",b"direction","message_timeout",b"message_timeout","parent_event_id",b"parent_event_id","pre_filter",b"pre_filter","timeout",b"timeout"]) -> None: ...
+        book_name: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["chain_id", b"chain_id", "checkpoint", b"checkpoint", "connectivity_id", b"connectivity_id", "parent_event_id", b"parent_event_id", "pre_filter", b"pre_filter"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["book_name", b"book_name", "chain_id", b"chain_id", "checkpoint", b"checkpoint", "connectivity_id", b"connectivity_id", "description", b"description", "direction", b"direction", "message_timeout", b"message_timeout", "parent_event_id", b"parent_event_id", "pre_filter", b"pre_filter", "timeout", b"timeout"]) -> None: ...
+
 global___NoMessageCheckRequest = NoMessageCheckRequest
 
+@typing_extensions.final
 class NoMessageCheckResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     STATUS_FIELD_NUMBER: builtins.int
     CHAIN_ID_FIELD_NUMBER: builtins.int
     @property
     def status(self) -> th2_grpc_common.common_pb2.RequestStatus: ...
     @property
     def chain_id(self) -> global___ChainID:
         """You can use it to unite the next rule to the chain with currently submitted one"""
-        pass
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        status: typing.Optional[th2_grpc_common.common_pb2.RequestStatus] = ...,
-        chain_id: typing.Optional[global___ChainID] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","status",b"status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","status",b"status"]) -> None: ...
+        status: th2_grpc_common.common_pb2.RequestStatus | None = ...,
+        chain_id: global___ChainID | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["chain_id", b"chain_id", "status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["chain_id", b"chain_id", "status", b"status"]) -> None: ...
+
 global___NoMessageCheckResponse = NoMessageCheckResponse
```

### Comparing `th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/check1_pb2_grpc.py` & `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_check1-4.1.1.dev0/th2_grpc_check1/check1_service.py` & `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1/check1_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_check1-4.1.1.dev0/th2_grpc_check1.egg-info/PKG-INFO` & `th2_grpc_check1-4.2.0.dev5378806706/th2_grpc_check1.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,85 @@
 Metadata-Version: 2.1
 Name: th2-grpc-check1
-Version: 4.1.1.dev0
+Version: 4.2.0.dev5378806706
 Summary: th2_grpc_check1
 Home-page: https://github.com/th2-net/th2-grpc-check1
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC check1 library (4.1.0)
+Description: # th2 gRPC check1 library (4.2.0)
         
-        This library contains proto messages and `Check1` service with RPC methods that are used in [th2 check1](https://github.com/th2-net/th2-check1 "th2-check1"). See [check1.proto](src/main/proto/th2_grpc_check1/check1.proto "check1.proto") file for details. <br>
-        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to the specified repositories.
+        This library contains proto messages and `Check1` service with RPC methods that are used
+        in [th2 check1](https://github.com/th2-net/th2-check1 "th2-check1").
+        See [check1.proto](src/main/proto/th2_grpc_check1/check1.proto "check1.proto") file for details. <br>
+        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to the specified
+        repositories.
         
         ## How to maintain a project
+        
         1. Perform the necessary changes.
         2. Update the package version of Java in `gradle.properties` file.
         3. Update the package version of Python in `package_info.json` file.
         4. Commit everything.
         
         ### Java
+        
         If you wish to manually create and publish a package for Java, run the following command:
+        
         ```
         gradle --no-daemon clean build publish artifactoryPublish \
                -Purl=${URL} \ 
                -Puser=${USER} \
                -Ppassword=${PASSWORD}
         ```
+        
         `URL`, `USER` and `PASSWORD` are parameters for publishing.
         
         ### Python
+        
         If you wish to manually create and publish a package for Python:
+        
         1. Generate services with `Gradle`:
             ```
                gradle --no-daemon clean generateProto
             ```
            You can find the generated files by following path: `src/gen/main/services/python`
         2. Generate code from `.proto` files and publish everything using `twine`:
             ```
             pip install -r requirements.txt
             pip install twine
             python setup.py generate
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
-            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
+           `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 4.2.0
+        
+        + Added golang specific properties
+        + Updated bom:4.4.0
+        + Updated grpc-service-generator:3.4.0
+        + Updated mypy-protobuf:3.4
+        
         ### 4.1.0
+        
         + merged `3.8.0`
         
         ### 4.0.0
+        
         + Migrated to `grpc-common` version with books/pages
         + Marked deprecated fields as `reserved`
         + Added `book_name` to `CheckRuleRequest`, `CheckSequenceRuleRequest` and `NoMessageCheckRequest`
         
         ### 3.8.0
         
-        + Update `th2-bom` to `4.2.0` 
-        + Update `grpc-service-generator` to `3.3.1` 
+        + Update `th2-bom` to `4.2.0`
+        + Update `grpc-service-generator` to `3.3.1`
         + Updated grpc to `1.48.1`
         + Updated protobuf to `3.21.7`
         + Add Python vulnerabilities scan
         
         ### 3.7.0
         
         + Update `th2-bom` to `4.1.0`
@@ -75,34 +93,40 @@
         #### Changed:
         
         + `grpc-common` version is updated to 3.9.0
         
         ### 3.5.0
         
         #### Added:
-        + `silence_check` parameter for `CheckSequenceRule`. Enables automated check for extra messages that match the pre-filter.
+        
+        + `silence_check` parameter for `CheckSequenceRule`. Enables automated check for extra messages that match the
+          pre-filter.
         
         #### Changed:
+        
         + Migrated `grpc-common` version from `3.7.0` to `3.8.0`
-          + Added `time_precision` and `decimal_precision` to `RootComparisonSettings` message
-          + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operations
+            + Added `time_precision` and `decimal_precision` to `RootComparisonSettings` message
+            + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operations
         
         ### 3.4.2
+        
         + Migrated `grpc-common` version from `3.6.0` to `3.7.0`
             + Added `check_repeating_group_order` parameter to `RootComparisonSettings` message
         
         ### 3.4.1
+        
         + Migrated `grpc-common` version from `3.4.0` to `3.6.0`
-          + Added the new parameters `description` to `RootMessageFilter` message
+            + Added the new parameters `description` to `RootMessageFilter` message
         
         ### 3.4.0
         
         + Update to `th2-grpc-common` version `3.4.0`
         
         ### 3.3.0
+        
         + Implemented NoMessageCheck rule task. Updated CheckSequence rule task
         
         ### 3.2.0
         
         + Implement stubs creation for Python
         
 Platform: UNKNOWN
```

