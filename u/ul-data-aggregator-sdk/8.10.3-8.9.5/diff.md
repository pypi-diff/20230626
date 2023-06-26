# Comparing `tmp/ul-data-aggregator-sdk-8.10.3.tar.gz` & `tmp/ul-data-aggregator-sdk-8.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-data-aggregator-sdk-8.10.3.tar", last modified: Mon Jun 26 21:41:27 2023, max compression
+gzip compressed data, was "ul-data-aggregator-sdk-8.9.5.tar", last modified: Thu Jun 22 13:30:39 2023, max compression
```

## Comparing `ul-data-aggregator-sdk-8.10.3.tar` & `ul-data-aggregator-sdk-8.9.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:41:27.939440 ul-data-aggregator-sdk-8.10.3/
--rw-r--r--   0 root         (0) root         (0)     1604 2023-06-26 21:41:27.939440 ul-data-aggregator-sdk-8.10.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1038 2022-01-13 09:34:59.000000 ul-data-aggregator-sdk-8.10.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:41:27.931439 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:41:27.931439 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-21 09:12:57.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/__tests__/test_integration_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:41:27.931439 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/brokers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/brokers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/brokers/data_aggregator_input_broker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:41:27.935440 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/constants/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/constants/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     3777 2023-04-10 10:59:35.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/constants/clock_timezones.py
--rw-rw-rw-   0 root         (0) root         (0)    17477 2023-06-16 07:41:25.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/constants/enums.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/constants/names.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2022-08-05 17:07:26.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/dag.yml
--rw-rw-rw-   0 root         (0) root         (0)    68217 2023-06-26 20:22:38.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/data_aggregator_api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-06-22 15:06:56.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/data_aggregator_api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/data_aggregator_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/data_aggregator_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2022-08-17 09:11:15.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    27414 2023-06-26 11:25:20.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/integration_message.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/lib.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-25 10:42:53.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/runtime_conf.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/self_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:41:27.935440 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-12 09:48:20.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-06-26 11:25:20.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/types/device.py
--rw-rw-rw-   0 root         (0) root         (0)     3401 2023-06-26 11:25:20.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/types/get_data_gateway_network_device_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:41:27.935440 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/devices_info_box_to_json.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-26 11:25:20.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/internal_api_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-26 11:25:20.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/internal_api_error_handler_old.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/query_params.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-21 13:15:25.000000 ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/round_dt.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 21:41:27.939440 ul-data-aggregator-sdk-8.10.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1464 2023-06-26 21:39:52.000000 ul-data-aggregator-sdk-8.10.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:41:27.939440 ul-data-aggregator-sdk-8.10.3/ul_data_aggregator_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2023-06-26 21:41:27.000000 ul-data-aggregator-sdk-8.10.3/ul_data_aggregator_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1544 2023-06-26 21:41:27.000000 ul-data-aggregator-sdk-8.10.3/ul_data_aggregator_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 21:41:27.000000 ul-data-aggregator-sdk-8.10.3/ul_data_aggregator_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-26 21:41:27.000000 ul-data-aggregator-sdk-8.10.3/ul_data_aggregator_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 21:41:27.000000 ul-data-aggregator-sdk-8.10.3/ul_data_aggregator_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2022-01-13 09:34:59.000000 ul-data-aggregator-sdk-8.9.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.042590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.042590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-21 09:12:57.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/test_integration_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.042590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/brokers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/brokers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/brokers/data_aggregator_input_broker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.046590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3777 2023-04-10 10:59:35.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/clock_timezones.py
+-rw-rw-rw-   0 root         (0) root         (0)    17477 2023-06-16 07:41:25.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/names.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2022-08-05 17:07:26.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/dag.yml
+-rw-rw-rw-   0 root         (0) root         (0)    50635 2023-06-22 13:20:40.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-22 13:20:40.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2022-08-17 09:11:15.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    26718 2023-06-22 13:20:40.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/integration_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-25 10:42:53.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/runtime_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/self_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.046590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-12 09:48:20.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/device.py
+-rw-rw-rw-   0 root         (0) root         (0)     3398 2023-06-08 09:55:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/get_data_gateway_network_device_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.050591 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/devices_info_box_to_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2022-10-12 09:48:20.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2022-11-08 19:19:34.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler_old.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/query_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-21 13:15:25.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/round_dt.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-22 13:26:15.000000 ul-data-aggregator-sdk-8.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/top_level.txt
```

### Comparing `ul-data-aggregator-sdk-8.10.3/PKG-INFO` & `ul-data-aggregator-sdk-8.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-aggregator-sdk
-Version: 8.10.3
+Version: 8.9.5
 Summary: Data aggregator sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-aggregator-sdk-8.10.3/README.md` & `ul-data-aggregator-sdk-8.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/__init__.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/__tests__/test_integration_message.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/test_integration_message.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/constants/clock_timezones.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/clock_timezones.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/constants/enums.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/enums.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/dag.yml` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/dag.yml`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/data_aggregator_sdk.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/errors.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/integration_message.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/integration_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime
 from enum import Enum, IntEnum, unique
-from ipaddress import IPv4Address
 from typing import Optional, List, Tuple, Dict, Any
 
-from ul_api_utils.errors import ValidateApiError
+from api_utils.errors import ValidateApiError
 from pydantic import BaseModel, UUID4, root_validator, Field  # pylint: disable=no-name-in-module
 from unipipeline.message.uni_message import UniMessage
 
 from data_aggregator_sdk.types.device import NetworkSysTypeEnum
 from data_aggregator_sdk.constants.enums import IntegrationV0MessageEvent, IntegrationV0MessageMetaBSChannelProtocol, \
     ProtocolEnum, IntegrationV0MessageErrorType
 
@@ -197,26 +196,14 @@
     )
     value: datetime = Field(
         title="Clock value",
         description="Device timestamp clock value",
     )
 
 
-class IntegrationV0MessageUptime(BaseModel):
-    channel_id: int = Field(
-        1,
-        title="Channel ID",
-        description="Device channel Id",
-    )
-    uptime_s: float = Field(
-        title="Uptime seconds",
-        description="Uptime seconds value",
-    )
-
-
 class IntegrationV0MessageRelay(BaseModel):
     relay_id: int = Field(
         -1,
         title="Relay ID",
         description="Device relay ID",
     )
     value: bool = Field(
@@ -593,19 +580,14 @@
         description="Structure which contains relay info for current device",
     )
     clock: List[IntegrationV0MessageClock] = Field(
         default_factory=list,
         title="Clock info",
         description="Structure which contains clock info for current device",
     )
-    uptime: List[IntegrationV0MessageUptime] = Field(
-        default_factory=list,
-        title="Uptime info",
-        description="Structure which contains uptime info for current device",
-    )
 
 
 class IntegrationMessageMetaIotAccountGateway(BaseModel):
     network_id: UUID4 = Field(
         title="Network ID",
         description="Network identifier",
     )
@@ -674,19 +656,14 @@
         description="Sender software / hardware version",
     )
     note: str = Field(
         ...,
         title="Note about sender",
         description="Any usefull information about sender",
     )
-    ipv4: IPv4Address = Field(
-        ...,
-        title='IPv4 sender address',
-        description="A unique numerical identifier for every sender that send through the internet",
-    )
 
 
 class IntegrationV0MessageMeta(BaseModel):
     nbfi_bs0: Optional[IntegrationV0MessageMetaNbFiBS0] = Field(
         None,
         title="NBFi BS0 meta message structure",
         description="NBFi BS0 meta message structure",
```

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/types/device.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 from uuid import UUID
 
-from ul_api_utils.api_resource.api_response_payload_alias import ApiBaseUserModelPayloadResponse
-from ul_api_utils.api_resource.api_response import JsonApiResponsePayload
+from api_utils.api_resource.api_response_payload_alias import ApiBaseUserModelPayloadResponse
+from api_utils.api_resource.api_response import JsonApiResponsePayload
 
 from data_aggregator_sdk.constants.enums import DeviceModificationTypeEnum, NetworkSysTypeEnum, NetworkTypeEnum, \
     ProtocolEnum, ResourceKind
 
 
 class ApiDataGatewayResponse(ApiBaseUserModelPayloadResponse):
     name: str
```

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/types/get_data_gateway_network_device_list.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/get_data_gateway_network_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from uuid import UUID
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 from pydantic import UUID4, BaseModel
-from ul_api_utils.api_resource.api_response_payload_alias import ApiBaseUserModelPayloadResponse, JsonApiResponsePayload
+from api_utils.api_resource.api_response_payload_alias import ApiBaseUserModelPayloadResponse, JsonApiResponsePayload
 
 from data_aggregator_sdk.constants.enums import DeviceModificationTypeEnum, NetworkSysTypeEnum, NetworkTypeEnum, ProtocolEnum
 from data_aggregator_sdk.types.device import ApiDeviceMeterPayloadResponse
 
 
 # REQUEST BODY
```

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/internal_api_error_handler.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import wraps
 from typing import Any, Callable, Dict, List, TypeVar, cast
 
-from ul_api_utils.errors import Client4XXInternalApiError, Server5XXInternalApiError, \
+from api_utils.errors import Client4XXInternalApiError, Server5XXInternalApiError, \
     ResponseJsonInternalApiError, NotFinishedRequestInternalApiError
 
 from data_aggregator_sdk.errors import DataAggregatorRequestError, DataAggregatorResponseError
 
 TKwargs = TypeVar('TKwargs', bound=Dict[str, Any])
 
 STDResp = TypeVar('STDResp', bound=Dict[str, Any] | List[Dict[str, Any]])    # TODO:  Dict[str, Any] -> JsonApiResponsePayload
```

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/internal_api_error_handler_old.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import wraps
 from typing import Any, Callable, Dict, List, TypeVar
 
-from ul_api_utils.errors import Client4XXInternalApiError, Server5XXInternalApiError, \
+from api_utils.errors import Client4XXInternalApiError, Server5XXInternalApiError, \
     ResponseJsonInternalApiError, NotFinishedRequestInternalApiError
 
 from data_aggregator_sdk.errors import DataAggregatorRequestError, DataAggregatorResponseError
 
 TKwargs = TypeVar('TKwargs', bound=Dict[str, Any])
 
 STDResp = TypeVar('STDResp', bound=Dict[str, Any] | List[Dict[str, Any]])    # TODO:  Dict[str, Any] -> JsonApiResponsePayload
```

### Comparing `ul-data-aggregator-sdk-8.10.3/data_aggregator_sdk/utils/query_params.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.3/setup.py` & `ul-data-aggregator-sdk-8.9.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-data-aggregator-sdk',
-    version='8.10.3',
+    version='8.9.5',
     description='Data aggregator sdk',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={
         '': ['*.yml'],
         'data_aggregator_sdk': ['py.typed'],
@@ -31,19 +31,12 @@
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
     platforms='any',
     install_requires=[
         'requests>=2.26.0',
         'unipipeline>=1.4.3',
-        'ul-api-utils>=7.2.8',
+        'ul-api-utils>=7.2.6',
         'wtforms==3.0.1',
         'wtforms-alchemy==0.18.0',
-        # "ul-api-utils==7.2.8",
-        # 'ul-pyncp==1.0.5',
-        # 'ul-pysmp==1.0.3',
-        # 'ul-data-gateway-sdk==0.4.5',
-        # 'ul-api-utils==7.2.7',
-        # 'ul-py-tool==1.15.20',
-        # 'ul-db-utils==2.10.7'
     ],
 )
```

### Comparing `ul-data-aggregator-sdk-8.10.3/ul_data_aggregator_sdk.egg-info/PKG-INFO` & `ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-aggregator-sdk
-Version: 8.10.3
+Version: 8.9.5
 Summary: Data aggregator sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-aggregator-sdk-8.10.3/ul_data_aggregator_sdk.egg-info/SOURCES.txt` & `ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

