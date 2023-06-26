# Comparing `tmp/gardena_bluetooth-0.4.0.tar.gz` & `tmp/gardena_bluetooth-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardena_bluetooth-0.4.0.tar", max compression
+gzip compressed data, was "gardena_bluetooth-0.5.0.tar", max compression
```

## Comparing `gardena_bluetooth-0.4.0.tar` & `gardena_bluetooth-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0      704 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/README.rst
--rw-r--r--   0        0        0     2976 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/__init__.py
--rw-r--r--   0        0        0     2234 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/__main__.py
--rw-r--r--   0        0        0     3180 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/client.py
--rw-r--r--   0        0        0     4938 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/const.py
--rw-r--r--   0        0        0      186 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/exceptions.py
--rw-r--r--   0        0        0     5094 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/gardena_bluetooth/parse.py
--rw-r--r--   0        0        0      739 2023-06-25 18:06:28.231704 gardena_bluetooth-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 gardena_bluetooth-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      704 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/README.rst
+-rw-r--r--   0        0        0     4321 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/gardena_bluetooth/__init__.py
+-rw-r--r--   0        0        0     2234 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/gardena_bluetooth/__main__.py
+-rw-r--r--   0        0        0     3180 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/gardena_bluetooth/client.py
+-rw-r--r--   0        0        0     4938 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/gardena_bluetooth/const.py
+-rw-r--r--   0        0        0      186 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/gardena_bluetooth/exceptions.py
+-rw-r--r--   0        0        0     5094 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/gardena_bluetooth/parse.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/gardena_bluetooth/py.typed
+-rw-r--r--   0        0        0      792 2023-06-26 18:48:17.660159 gardena_bluetooth-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 gardena_bluetooth-0.5.0/PKG-INFO
```

### Comparing `gardena_bluetooth-0.4.0/LICENSE.txt` & `gardena_bluetooth-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.4.0/README.rst` & `gardena_bluetooth-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.4.0/gardena_bluetooth/__init__.py` & `gardena_bluetooth-0.5.0/gardena_bluetooth/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
 
 from bleak import BleakClient
 from bleak.uuids import register_uuids
+from typing import TypeVar, overload
 
 from .const import DeviceConfiguration, ScanService
 from .exceptions import CharacteristicNoAccess, CharacteristicNotFound
 from .parse import Characteristic, CharacteristicType, Service
 
 LOGGER = logging.getLogger(__name__)
+DEFAULT_MISSING = object()
+DEFAULT_TYPE = TypeVar("DEFAULT_TYPE")
 
 register_uuids(
     {
         service.uuid: f"Gardena {service.__name__}"
         for service in Service.registry.values()
     }
 )
@@ -26,28 +29,69 @@
         for char in service.characteristics()
     }
 )
 
 register_uuids({ScanService: "Husqvarna"})
 
 
-async def read_char_raw(client: BleakClient, uuid: str):
+@overload
+async def read_char_raw(client: BleakClient, uuid: str) -> bytes:
+    ...
+
+
+@overload
+async def read_char_raw(
+    client: BleakClient, uuid: str, default: DEFAULT_TYPE
+) -> bytes | DEFAULT_TYPE:
+    ...
+
+
+async def read_char_raw(
+    client: BleakClient, uuid: str, default: DEFAULT_TYPE = DEFAULT_MISSING
+) -> bytes | DEFAULT_TYPE:
     characteristic = client.services.get_characteristic(uuid)
     if characteristic is None:
+        if default is not DEFAULT_MISSING:
+            return default
         raise CharacteristicNotFound(f"Unable to find characteristic {uuid}")
     if "read" not in characteristic.properties:
+        if default is not DEFAULT_MISSING:
+            return default
         raise CharacteristicNoAccess(f"Characteristic {uuid} is not readable")
     return await client.read_gatt_char(characteristic)
 
 
+@overload
 async def read_char(
     client: BleakClient, char: Characteristic[CharacteristicType]
 ) -> CharacteristicType:
+    ...
+
+
+@overload
+async def read_char(
+    client: BleakClient,
+    char: Characteristic[CharacteristicType],
+    default: DEFAULT_TYPE,
+) -> CharacteristicType | DEFAULT_TYPE:
+    ...
+
+
+async def read_char(
+    client: BleakClient,
+    char: Characteristic[CharacteristicType],
+    default: DEFAULT_TYPE = DEFAULT_MISSING,
+) -> CharacteristicType | DEFAULT_TYPE:
     """Read data to from a characteristic."""
-    return char.decode(await read_char_raw(client, char.uuid))
+    try:
+        return char.decode(await read_char_raw(client, char.uuid))
+    except CharacteristicNotFound:
+        if default is not DEFAULT_MISSING:
+            return default
+        raise
 
 
 async def write_char_raw(
     client: BleakClient, uuid: str, data: bytes, response: bool = True
 ):
     """Write data to a characteristic."""
     characteristic = client.services.get_characteristic(uuid)
@@ -66,29 +110,37 @@
 ) -> None:
     """Write data to a characteristic."""
     data = char.encode(value)
     await write_char_raw(client, char.uuid, data, response)
 
 
 async def update_timestamp(client: BleakClient, now: datetime):
-    timestamp = await read_char(client, DeviceConfiguration.unix_timestamp)
+    try:
+        timestamp = await read_char(client, DeviceConfiguration.unix_timestamp)
+    except CharacteristicNoAccess:
+        LOGGER.debug("No timestamp defined for device")
+        return
     timestamp = timestamp.replace(tzinfo=now.tzinfo)
     delta = timestamp - now
     if abs(delta.total_seconds()) > 60:
         LOGGER.warning(
             "Updating time on device to match local time delta was %s", delta
         )
         await write_char(
             client,
             DeviceConfiguration.unix_timestamp,
             now.replace(tzinfo=None),
             True,
         )
+    else:
+        LOGGER.debug("No need to update timestamp local time delta was %s", delta)
 
 
 async def get_all_characteristics_uuid(client: BleakClient) -> set[str]:
     """Get all characteristics from device."""
-    return {
+    characteristics = {
         characteristic.uuid
         for service in client.services
         for characteristic in service.characteristics
     }
+    LOGGER.debug("Characteristics: %s", characteristics)
+    return characteristics
```

### Comparing `gardena_bluetooth-0.4.0/gardena_bluetooth/__main__.py` & `gardena_bluetooth-0.5.0/gardena_bluetooth/__main__.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.4.0/gardena_bluetooth/client.py` & `gardena_bluetooth-0.5.0/gardena_bluetooth/client.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.4.0/gardena_bluetooth/const.py` & `gardena_bluetooth-0.5.0/gardena_bluetooth/const.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.4.0/gardena_bluetooth/parse.py` & `gardena_bluetooth-0.5.0/gardena_bluetooth/parse.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.4.0/pyproject.toml` & `gardena_bluetooth-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 name = "gardena-bluetooth"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Joakim Plate <elupus@ecce.se>"]
 readme = "README.rst"
-packages = [{include = "gardena_bluetooth"}]
+packages = [
+    {include = "gardena_bluetooth"},
+    {include = "gardena_bluetooth/py.typed"},
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 bleak = "^0.20.2"
 bleak-retry-connector = "^3.0.2"
 asyncclick = {version = "^8.1.3.4", optional = true}
 tzlocal = "^5.0.1"
```

### Comparing `gardena_bluetooth-0.4.0/PKG-INFO` & `gardena_bluetooth-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gardena-bluetooth
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: Joakim Plate
 Author-email: elupus@ecce.se
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

