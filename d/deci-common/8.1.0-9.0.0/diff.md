# Comparing `tmp/deci_common-8.1.0.tar.gz` & `tmp/deci_common-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deci_common-8.1.0.tar", max compression
+gzip compressed data, was "deci_common-9.0.0.tar", max compression
```

## Comparing `deci_common-8.1.0.tar` & `deci_common-9.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11357 2023-02-21 15:06:30.961135 deci_common-8.1.0/LICENSE.md
--rw-r--r--   0        0        0       60 2023-02-21 15:06:30.961135 deci_common-8.1.0/README.md
--rw-r--r--   0        0        0        0 2023-02-21 15:06:30.961135 deci_common-8.1.0/deci_common/__init__.py
--rw-r--r--   0        0        0        0 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/abstractions/__init__.py
--rw-r--r--   0        0        0      713 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/abstractions/abstract_logger.py
--rw-r--r--   0        0        0      800 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/abstractions/base_model.py
--rw-r--r--   0        0        0       74 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/auto_logging/__init__.py
--rw-r--r--   0        0        0     3553 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/auto_logging/auto_logger.py
--rw-r--r--   0        0        0      831 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/auto_logging/auto_logging_conf.json
--rw-r--r--   0        0        0       68 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/aws_connection/__init__.py
--rw-r--r--   0        0        0     7226 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/aws_connection/aws_connector.py
--rw-r--r--   0        0        0        0 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_connection/__init__.py
--rw-r--r--   0        0        0     1832 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_connection/mongo_connector.py
--rw-r--r--   0        0        0    20166 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_connection/s3_connector.py
--rw-r--r--   0        0        0      148 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_interfaces/__init__.py
--rw-r--r--   0        0        0     8868 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_interfaces/files_data_interface.py
--rw-r--r--   0        0        0     3968 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_interfaces/generic_db_interface.py
--rw-r--r--   0        0        0     5969 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_interfaces/mongo_db_interface.py
--rw-r--r--   0        0        0        0 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/__init__.py
--rw-r--r--   0        0        0        0 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/enum/__init__.py
--rw-r--r--   0        0        0      715 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/enum/dataset_names.py
--rw-r--r--   0        0        0      521 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/enum/deep_learning_task.py
--rw-r--r--   0        0        0    17448 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/enum/hardware_enums.py
--rw-r--r--   0        0        0      192 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/enum/inference_transport.py
--rw-r--r--   0        0        0     1742 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/enum/model_frameworks.py
--rw-r--r--   0        0        0     7635 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/enum/models_enums.py
--rw-r--r--   0        0        0      386 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/enum/open_vino_checkpoint_types.py
--rw-r--r--   0        0        0     3236 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/hardware.py
--rw-r--r--   0        0        0     1721 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/inferencer_data_types.py
--rw-r--r--   0        0        0     5406 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/data_types/model_errors.py
--rw-r--r--   0        0        0        0 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/environment/__init__.py
--rw-r--r--   0        0        0      291 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/environment/environment_config.py
--rw-r--r--   0        0        0     3182 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/helpers.py
--rw-r--r--   0        0        0        0 2023-02-21 15:06:30.965134 deci_common-8.1.0/deci_common/py.typed
--rw-r--r--   0        0        0     1465 2023-02-21 15:06:39.809221 deci_common-8.1.0/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 deci_common-8.1.0/setup.py
--rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 deci_common-8.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-23 14:08:03.672475 deci_common-9.0.0/LICENSE.md
+-rw-r--r--   0        0        0       60 2023-02-23 14:08:03.672475 deci_common-9.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/abstractions/__init__.py
+-rw-r--r--   0        0        0      713 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/abstractions/abstract_logger.py
+-rw-r--r--   0        0        0      800 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/abstractions/base_model.py
+-rw-r--r--   0        0        0       74 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/auto_logging/__init__.py
+-rw-r--r--   0        0        0     3553 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/auto_logging/auto_logger.py
+-rw-r--r--   0        0        0      831 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/auto_logging/auto_logging_conf.json
+-rw-r--r--   0        0        0       68 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/aws_connection/__init__.py
+-rw-r--r--   0        0        0     7226 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/aws_connection/aws_connector.py
+-rw-r--r--   0        0        0        0 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_connection/__init__.py
+-rw-r--r--   0        0        0     1832 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_connection/mongo_connector.py
+-rw-r--r--   0        0        0    20166 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_connection/s3_connector.py
+-rw-r--r--   0        0        0      148 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_interfaces/__init__.py
+-rw-r--r--   0        0        0     8868 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_interfaces/files_data_interface.py
+-rw-r--r--   0        0        0     3968 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_interfaces/generic_db_interface.py
+-rw-r--r--   0        0        0     5969 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_interfaces/mongo_db_interface.py
+-rw-r--r--   0        0        0        0 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/enum/__init__.py
+-rw-r--r--   0        0        0      715 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/enum/dataset_names.py
+-rw-r--r--   0        0        0      521 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/enum/deep_learning_task.py
+-rw-r--r--   0        0        0    17448 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/enum/hardware_enums.py
+-rw-r--r--   0        0        0      192 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/enum/inference_transport.py
+-rw-r--r--   0        0        0     1742 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/enum/model_frameworks.py
+-rw-r--r--   0        0        0     7635 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/enum/models_enums.py
+-rw-r--r--   0        0        0      386 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/enum/open_vino_checkpoint_types.py
+-rw-r--r--   0        0        0     3065 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/hardware.py
+-rw-r--r--   0        0        0     1721 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/inferencer_data_types.py
+-rw-r--r--   0        0        0     5406 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/data_types/model_errors.py
+-rw-r--r--   0        0        0        0 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/environment/__init__.py
+-rw-r--r--   0        0        0      291 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/environment/environment_config.py
+-rw-r--r--   0        0        0     3182 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/helpers.py
+-rw-r--r--   0        0        0        0 2023-02-23 14:08:03.672475 deci_common-9.0.0/deci_common/py.typed
+-rw-r--r--   0        0        0     1465 2023-02-23 14:08:11.720513 deci_common-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 deci_common-9.0.0/setup.py
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 deci_common-9.0.0/PKG-INFO
```

### Comparing `deci_common-8.1.0/LICENSE.md` & `deci_common-9.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/abstractions/abstract_logger.py` & `deci_common-9.0.0/deci_common/abstractions/abstract_logger.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/abstractions/base_model.py` & `deci_common-9.0.0/deci_common/abstractions/base_model.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/auto_logging/auto_logger.py` & `deci_common-9.0.0/deci_common/auto_logging/auto_logger.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/auto_logging/auto_logging_conf.json` & `deci_common-9.0.0/deci_common/auto_logging/auto_logging_conf.json`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/aws_connection/aws_connector.py` & `deci_common-9.0.0/deci_common/aws_connection/aws_connector.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_connection/mongo_connector.py` & `deci_common-9.0.0/deci_common/data_connection/mongo_connector.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_connection/s3_connector.py` & `deci_common-9.0.0/deci_common/data_connection/s3_connector.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_interfaces/files_data_interface.py` & `deci_common-9.0.0/deci_common/data_interfaces/files_data_interface.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_interfaces/generic_db_interface.py` & `deci_common-9.0.0/deci_common/data_interfaces/generic_db_interface.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_interfaces/mongo_db_interface.py` & `deci_common-9.0.0/deci_common/data_interfaces/mongo_db_interface.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_types/enum/dataset_names.py` & `deci_common-9.0.0/deci_common/data_types/enum/dataset_names.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_types/enum/deep_learning_task.py` & `deci_common-9.0.0/deci_common/data_types/enum/deep_learning_task.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_types/enum/hardware_enums.py` & `deci_common-9.0.0/deci_common/data_types/enum/hardware_enums.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_types/enum/model_frameworks.py` & `deci_common-9.0.0/deci_common/data_types/enum/model_frameworks.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_types/enum/models_enums.py` & `deci_common-9.0.0/deci_common/data_types/enum/models_enums.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_types/hardware.py` & `deci_common-9.0.0/deci_common/data_types/hardware.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,55 +8,53 @@
     HardwareEnvironment,
     HardwareVendor,
     HardwareLabel,
     HardwareTaint,
     MapHardwareTypeToVendor,
     HardwareMachineModel,
     MapHardwareTypeToEnvironment,
-    HardwareImageDistribution,
-    HardwareImageRepository,
     MapHardwareTypeToImageDistribution,
     MapHardwareTypeToImageRepository,
     HardwareGroup,
     MapHardwareTypeToGroup,
     HardwareTypeLabel,
 )
 
 
 # TODO move all hardwaretype usage to use thic class insted.
 class HardwareReturnSchema(Schema):
     """
     A logic schema of hardware
     """
 
-    name: HardwareType
-    label: HardwareTypeLabel
+    name: str
+    label: str
     vendor: Optional[HardwareVendor] = None
     machine: Optional[HardwareMachineModel] = None
     group: Optional[HardwareGroup] = None
     future: bool = False
     deprecated: bool = False
 
 
 class Hardware(Schema):
     """
     A logic schema of hardware
     """
 
-    name: HardwareType
+    name: str
     type: InferenceHardware
     # equals None for backwards compatibility of benchmark jobs who does not have it.
-    machine: Optional[HardwareMachineModel] = None
+    machine: Optional[str] = None
     cost_per_hour: int = 0
     environment: Optional[HardwareEnvironment]
     vendor: HardwareVendor
-    label: HardwareLabel
-    taint: HardwareTaint
-    image_repository: Optional[HardwareImageRepository]
-    image_distribution: Optional[HardwareImageDistribution]
+    label: str
+    taint: str
+    image_repository: Optional[str]
+    image_distribution: Optional[str]
 
 
 def get_hardware_by_hardware_name(hw_name: HardwareType) -> Hardware:
     if type(hw_name) is str:
         hw_name = HardwareType(hw_name)
     inference_hardware = MapHardwareTypeToFamily[hw_name.name].value
     image_repository = getattr(MapHardwareTypeToImageRepository, hw_name.name, None)
```

### Comparing `deci_common-8.1.0/deci_common/data_types/inferencer_data_types.py` & `deci_common-9.0.0/deci_common/data_types/inferencer_data_types.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/data_types/model_errors.py` & `deci_common-9.0.0/deci_common/data_types/model_errors.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/deci_common/helpers.py` & `deci_common-9.0.0/deci_common/helpers.py`

 * *Files identical despite different names*

### Comparing `deci_common-8.1.0/pyproject.toml` & `deci_common-9.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deci-common"
-version = "8.1.0"
+version = "9.0.0"
 description = "A package for Deci's common data types, connections and interfaces"
 authors = ["Deci AI <rnd@deci.ai>"]
 readme = "README.md"
 license = "Apache-2.0"
 include = ["deci_common/auto_logging/auto_logging_conf.json"]
 
 [tool.poetry.dependencies]
```

### Comparing `deci_common-8.1.0/setup.py` & `deci_common-9.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'pymongo==4.1.1',
  'python-json-logger==2.0.2',
  'python-magic>=0,<1',
  'stringcase>=1,<2']
 
 setup_kwargs = {
     'name': 'deci-common',
-    'version': '8.1.0',
+    'version': '9.0.0',
     'description': "A package for Deci's common data types, connections and interfaces",
     'long_description': '# deci-common\nCommon data types, connections and interfaces\n',
     'author': 'Deci AI',
     'author_email': 'rnd@deci.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deci_common-8.1.0/PKG-INFO` & `deci_common-9.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deci-common
-Version: 8.1.0
+Version: 9.0.0
 Summary: A package for Deci's common data types, connections and interfaces
 License: Apache-2.0
 Author: Deci AI
 Author-email: rnd@deci.ai
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

