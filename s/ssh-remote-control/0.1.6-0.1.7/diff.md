# Comparing `tmp/ssh_remote_control-0.1.6.tar.gz` & `tmp/ssh_remote_control-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_remote_control-0.1.6.tar", last modified: Sun Jun 25 04:10:15 2023, max compression
+gzip compressed data, was "ssh_remote_control-0.1.7.tar", last modified: Mon Jun 26 09:20:05 2023, max compression
```

## Comparing `ssh_remote_control-0.1.6.tar` & `ssh_remote_control-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.549109 ssh_remote_control-0.1.6/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     1569 2023-06-25 04:10:15.548107 ssh_remote_control-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      973 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.6/README.md
--rw-rw-rw-   0        0        0      846 2023-06-25 04:08:58.000000 ssh_remote_control-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 04:10:15.550104 ssh_remote_control-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.438638 ssh_remote_control-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.480322 ssh_remote_control-0.1.6/src/ssh_remote_control/
--rw-rw-rw-   0        0        0    10704 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/__init__.py
--rw-rw-rw-   0        0        0     6659 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/command.py
--rw-rw-rw-   0        0        0     3503 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/command_set.py
-drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.546105 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/
--rw-rw-rw-   0        0        0      161 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/const.py
--rw-rw-rw-   0        0        0     3978 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/linux.py
--rw-rw-rw-   0        0        0     3813 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/windows_cmd.py
--rw-rw-rw-   0        0        0     4078 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/windows_ps.py
--rw-rw-rw-   0        0        0      645 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/event.py
--rw-rw-rw-   0        0        0      222 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/helpers.py
--rw-rw-rw-   0        0        0     1313 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/locker.py
--rw-rw-rw-   0        0        0     3824 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/manager.py
--rw-rw-rw-   0        0        0     6757 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/sensor.py
-drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.527110 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/
--rw-rw-rw-   0        0        0     1569 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.127841 ssh_remote_control-0.1.7/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1569 2023-06-26 09:20:05.122837 ssh_remote_control-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.7/README.md
+-rw-rw-rw-   0        0        0      846 2023-06-26 09:15:45.000000 ssh_remote_control-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 09:20:05.127841 ssh_remote_control-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.020843 ssh_remote_control-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.067837 ssh_remote_control-0.1.7/src/ssh_remote_control/
+-rw-rw-rw-   0        0        0    10701 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/__init__.py
+-rw-rw-rw-   0        0        0     6641 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/command.py
+-rw-rw-rw-   0        0        0     3503 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/command_set.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.120834 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/
+-rw-rw-rw-   0        0        0      161 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/const.py
+-rw-rw-rw-   0        0        0     3969 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/linux.py
+-rw-rw-rw-   0        0        0     3813 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/windows_cmd.py
+-rw-rw-rw-   0        0        0     4078 2023-06-26 09:13:12.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/windows_ps.py
+-rw-rw-rw-   0        0        0      645 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/event.py
+-rw-rw-rw-   0        0        0      222 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/helpers.py
+-rw-rw-rw-   0        0        0     1313 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/locker.py
+-rw-rw-rw-   0        0        0     3995 2023-06-26 09:13:11.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/manager.py
+-rw-rw-rw-   0        0        0     8323 2023-06-26 09:17:08.000000 ssh_remote_control-0.1.7/src/ssh_remote_control/sensor.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:20:05.109834 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/
+-rw-rw-rw-   0        0        0     1569 2023-06-26 09:20:04.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-06-26 09:20:05.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:20:04.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-26 09:20:04.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-26 09:20:04.000000 ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/top_level.txt
```

### Comparing `ssh_remote_control-0.1.6/LICENSE` & `ssh_remote_control-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.6/PKG-INFO` & `ssh_remote_control-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_remote_control
-Version: 0.1.6
+Version: 0.1.7
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.6/README.md` & `ssh_remote_control-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.6/pyproject.toml` & `ssh_remote_control-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_remote_control"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor remote devices through SSH"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/__init__.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         if not self.state.is_connected:
             return
 
         self._ssh_client.close()
         self.state.update(IS_CONNECTED, False)
 
         for command in self.sensor_commands:
-            command.set_sensor_values(None)
+            command.update_sensors(None)
 
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
     ) -> CommandOutput:
         loop = asyncio.get_running_loop()
         timeout = command_timeout or self.command_timeout
```

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/command.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,42 +187,42 @@
     def remove_sensor(self, key: str) -> None:
         """Remove a sensor."""
         self.sensors = [
             Sensor(key=PLACEHOLDER_KEY) if sensor.key == key else sensor
             for sensor in self.sensors
         ]
 
-    def set_sensor_values(self, output: CommandOutput | None) -> None:
-        """Set sensor values."""
+    def update_sensors(self, output: CommandOutput | None) -> None:
+        """Update sensors."""
         if output and output.code == 0:
             self.last_update = output.timestamp
             data = output.stdout
         else:
             data = None
 
         if dynamic_sensor := self.dynamic_sensor:
-            dynamic_sensor.set_value(data)
+            dynamic_sensor.update(data)
 
         else:
             if data is None:
                 data = []
 
             for i, sensor in enumerate(self.sensors):
-                sensor.set_value(data[i] if len(data) > i else None)
+                sensor.update(data[i] if len(data) > i else None)
 
     async def async_execute(
         self, manager: Manager, context: dict | None = None
     ) -> CommandOutput:
         try:
             output = await super().async_execute(manager, context)
         except (CommandFormatError, CommandExecuteError):
-            self.set_sensor_values(None)
+            self.update_sensors(None)
             raise
 
-        self.set_sensor_values(output)
+        self.update_sensors(output)
 
         return output
 
 
 class CommandFormatError(Exception):
     """Error to indicate command formatting failed."""
```

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/command_set.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/command_set.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/const.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/const.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/linux.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..command import ActionCommand, Command, SensorCommand
+from ..command import ActionCommand, SensorCommand
 from ..command_set import CommandSet
 from ..sensor import DynamicSensor, Sensor
 from .const import ActionKey, ActionName, SensorKey, SensorName
 
 linux = CommandSet(
     "Linux",
     [
@@ -89,15 +89,15 @@
                     value_type=int,
                     value_unit="MB",
                 )
             ],
             interval=30,
         ),
         SensorCommand(
-            "df -m | awk '/^\\/dev\\// {{print $4 \"|\" $6}}'",
+            "df -m | awk '/^\\/dev\\// {{print $6 \"|\" $4}}'",
             [
                 DynamicSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     value_type=int,
                     value_unit="MB",
                     separator="|",
```

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/windows_cmd.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/windows_ps.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/default_command_sets/windows_ps.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 )
             ],
             interval=30,
         ),
         SensorCommand(
             "Get-CimInstance Win32_LogicalDisk | "
             + "Select DeviceID, FreeSpace | ForEach-Object "
-            + '{{[math]::Round($_.FreeSpace/1MB)+"|"+$_.DeviceID}}',
+            + '{{$_.DeviceID+"|"+[math]::Round($_.FreeSpace/1MB)}}',
             [
                 DynamicSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     value_type=int,
                     value_unit="MB",
                     separator="|",
```

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/event.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/event.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/locker.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/locker.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/manager.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -94,34 +94,42 @@
                 await self.async_execute_command(command)
             except (CommandFormatError, CommandExecuteError):
                 if validate:
                     raise
 
         return sensors
 
-    async def async_set_switch(self, key: str, value: bool) -> None:
-        """Set a switch.
+    async def async_set_sensor_value(
+        self, key: str, value: str | int | float | bool, *, validate: bool = False
+    ) -> Sensor:
+        """Set the value of a sensor.
 
         Raises:
-            CommandFormatError
-            CommandExecuteError
+            CommandFormatError (validate)
+            CommandExecuteError (validate)
         """
-        sensor = await self.async_poll_sensor(key, validate=True)
+        sensors = await self.async_set_sensor_values([key], [value], validate=validate)
+        return sensors[0]
 
-        if sensor.value == value:
-            return
-
-        command = sensor.switch_on if value else sensor.switch_off
-        await self.async_execute_command(command, context={"id": sensor.child_id})
-        await self.async_poll_sensor(key, validate=True)
-
-    async def async_toggle_switch(self, key: str) -> None:
-        """Toggle a switch.
+    async def async_set_sensor_values(
+        self,
+        keys: Sequence[str],
+        values: Sequence[str | int | float | bool],
+        *,
+        validate: bool = False,
+    ) -> list[Sensor]:
+        """Set the value of multiple sensors.
 
         Raises:
-            CommandFormatError
-            CommandExecuteError
+            CommandFormatError (validate)
+            CommandExecuteError (validate)
         """
-        sensor = await self.async_poll_sensor(key, validate=True)
-        command = sensor.switch_off if sensor.value else sensor.switch_on
-        await self.async_execute_command(command, context={"id": sensor.child_id})
-        await self.async_poll_sensor(key, validate=True)
+        sensors = await self.async_poll_sensors(keys, validate=validate)
+
+        for i, sensor in enumerate(sensors):
+            try:
+                await sensor.async_set(self, values[i])
+            except (CommandFormatError, CommandExecuteError):
+                if validate:
+                    raise
+
+        return await self.async_poll_sensors(keys, validate=validate)
```

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control/sensor.py` & `ssh_remote_control-0.1.7/src/ssh_remote_control/sensor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
-from collections.abc import Callable
 import logging
+from collections.abc import Callable
 from typing import TYPE_CHECKING, Any
 
 from .event import Event
 from .helpers import name_to_key
 
 if TYPE_CHECKING:
     from .command import Command
+    from .manager import Manager
 
 _LOGGER = logging.getLogger(__name__)
 
 TRUE_STRINGS = ["true", "enabled", "on", "active", "1"]
 FALSE_STRINGS = ["false", "disabled", "off", "inactive", "0"]
 
 
@@ -42,21 +43,22 @@
 class DynamicData:
     """The DynamicData class"""
 
     def __init__(
         self,
         parent_name: str | None,
         parent_key: str,
+        data_id: str,
         data_value_string: str,
-        data_name: str,
-        data_id: str | None = None,
+        data_name: str | None = None,
     ) -> None:
-        self.id = data_id or data_name
-        self.key = f"{parent_key}_{name_to_key(self.id)}"
-        self.name = f"{parent_name} {data_name}" if parent_name else data_name
+        name = data_name or data_id
+        self.id = data_id
+        self.key = f"{parent_key}_{name_to_key(name)}"
+        self.name = f"{parent_name} {name}" if parent_name else name
         self.value_string = data_value_string
 
 
 class Sensor:
     """The Sensor class."""
 
     value: Any | None = None
@@ -66,117 +68,155 @@
         self,
         name: str | None = None,
         key: str | None = None,
         child_id: str | None = None,
         *,
         value_type: type | None = None,
         value_unit: str | None = None,
+        value_min: int | float | None = None,
+        value_max: int | float | None = None,
         value_renderer: Callable[[str], str] | None = None,
-        switch_on: Command | None = None,
-        switch_off: Command | None = None,
+        command_set: Command | None = None,
+        command_on: Command | None = None,
+        command_off: Command | None = None,
         payload_on: str | None = None,
         payload_off: str | None = None,
         options: dict | None = None,
     ) -> None:
         self.name = name
         self.key = key or name_to_key(name)
         self.child_id = child_id
         self.value_type = value_type or str
         self.value_unit = value_unit
+        self.value_min = value_min
+        self.value_max = value_max
         self.value_renderer = value_renderer
-        self.switch_on = switch_on
-        self.switch_off = switch_off
+        self.command_set = command_set
+        self.command_on = command_on
+        self.command_off = command_off
         self.payload_on = payload_on
         self.payload_off = payload_off
         self.options = options or {}
         self.on_update = Event()
 
     @property
-    def is_switchable(self) -> bool:
-        return self.value_type is bool and self.switch_on and self.switch_off
-
-    def set_value(self, data: str | None) -> None:
-        """Set value."""
-        value_string = data
-        value = None
-
-        if data is not None and self.value_renderer:
-            try:
-                value_string = self.value_renderer(data)
-            except Exception as exc:  # pylint: disable=broad-except
-                _LOGGER.warning("%s: Value render error: %s (%s)", self.key, exc, data)
-
-        if value_string is not None:
-            try:
-                if self.value_type is bool:
-                    value = string_to_bool(
-                        self.payload_on, self.payload_off, value_string
-                    )
-                elif self.value_type is int:
-                    value = int(float(value_string))
-                else:
-                    value = self.value_type(value_string)
-            except Exception as exc:  # pylint: disable=broad-except
-                _LOGGER.warning("%s: Value error: %s (%s)", self.key, exc, value_string)
+    def is_controllable(self) -> bool:
+        if self.value_type == bool and self.command_on and self.command_off:
+            return True
+        return self.command_set is not None
 
-        self.value = value
+    def _render(self, value_string: str | None) -> Any | None:
+        if value_string is None:
+            return None
+        if self.value_renderer:
+            value_string = self.value_renderer(value_string)
+        if self.value_type is bool:
+            return string_to_bool(self.payload_on, self.payload_off, value_string)
+        if self.value_type is int:
+            return int(float(value_string))
+        return self.value_type(value_string)
 
-        if value is not None:
-            self.last_known_value = value
+    def _validate(self, value: Any) -> bool:
+        if not isinstance(value, self.value_type):
+            return False
+        if self.value_type == str and (
+            (self.value_min and len(value) < self.value_min)
+            or (self.value_max and len(value) > self.value_max)
+        ):
+            return False
+        if self.value_type in [int, float] and (
+            (self.value_min and value < self.value_min)
+            or (self.value_max and value > self.value_max)
+        ):
+            return False
+        return True
 
+    def _update_value(self, data: str | None) -> None:
+        try:
+            value = self._render(data)
+        except Exception as exc:  # pylint: disable=broad-except
+            _LOGGER.warning("%s: Render error: %s (%s)", self.key, exc, data)
+            value = None
+
+        if self._validate(value):
+            self.value = self.last_known_value = value
+        else:
+            self.value = None
+
+    def update(self, data: str | None) -> None:
+        """Update."""
+        self._update_value(data)
         self.on_update.notify(self)
 
+    async def async_set(self, manager: Manager, value: Any) -> None:
+        """Set."""
+        if value == self.value or not self._validate(value):
+            return
+
+        if self.value_type == bool and self.command_on and self.command_off:
+            command = self.command_on if value else self.command_off
+        else:
+            command = self.command_set
+
+        await manager.async_execute_command(
+            command, context={"id": self.child_id, "value": value}
+        )
+
 
 class DynamicSensor(Sensor):
     """The DynamicSensor class."""
 
     value: list[Sensor]
 
     def __init__(
         self,
         name: str | None = None,
         key: str | None = None,
         *,
+        separator: str | None = None,
         value_type: type | None = None,
         value_unit: str | None = None,
+        value_min: int | float | None = None,
+        value_max: int | float | None = None,
         value_renderer: Callable[[str], str] | None = None,
-        switch_on: str | None = None,
-        switch_off: str | None = None,
+        command_set: Command | None = None,
+        command_on: str | None = None,
+        command_off: str | None = None,
         payload_on: str | None = None,
         payload_off: str | None = None,
-        separator: str | None = None,
         options: dict | None = None,
     ) -> None:
         super().__init__(
             name,
             key,
             value_type=value_type,
             value_unit=value_unit,
+            value_min=value_min,
+            value_max=value_max,
             value_renderer=value_renderer,
-            switch_on=switch_on,
-            switch_off=switch_off,
+            command_set=command_set,
+            command_on=command_on,
+            command_off=command_off,
             payload_on=payload_on,
             payload_off=payload_off,
             options=options,
         )
         self.separator = separator
         self.value = []
         self.on_child_added = Event()
         self.on_child_removed = Event()
 
     @property
     def children_by_key(self) -> dict[str, Sensor]:
         return {child.key: child for child in self.value}
 
-    def set_value(self, data: list[str] | None) -> None:
+    def _update_value(self, data: list[str] | None) -> None:
         if data is None:
             for child in self.value:
-                child.set_value(None)
-
-            self.on_update.notify(self)
+                child.update(None)
             return
 
         dynamic_data_list = [
             DynamicData(self.name, self.key, *data_items)
             for data_items in [line.split(self.separator, 2) for line in data]
             if len(data_items) >= 2
         ]
@@ -188,38 +228,38 @@
         for key, dynamic_data in dynamic_data_by_key.items():
             if key not in self.children_by_key:
                 self.add_child(dynamic_data)
 
         for child in self.value:
             if child.key in dynamic_data_by_key:
                 dynamic_data = dynamic_data_by_key[child.key]
-                child.set_value(dynamic_data.value_string)
+                child.update(dynamic_data.value_string)
             else:
                 self.remove_child(child)
 
-        self.on_update.notify(self)
-
     def add_child(self, dynamic_data: DynamicData) -> None:
         """Add a child."""
         child = Sensor(
             dynamic_data.name,
             dynamic_data.key,
             dynamic_data.id,
             value_type=self.value_type,
             value_unit=self.value_unit,
+            value_min=self.value_min,
+            value_max=self.value_max,
             value_renderer=self.value_renderer,
-            switch_on=self.switch_on,
-            switch_off=self.switch_off,
+            command_set=self.command_set,
+            command_on=self.command_on,
+            command_off=self.command_off,
             payload_on=self.payload_on,
             payload_off=self.payload_off,
             options=self.options,
         )
         self.value.append(child)
         self.on_child_added.notify(self, child)
 
     def remove_child(self, child: Sensor) -> None:
         """Remove a child."""
         if child.value is not None:
-            child.set_value(None)
-
+            child.update(None)
         self.value.remove(child)
         self.on_child_removed.notify(self, child)
```

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/PKG-INFO` & `ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-remote-control
-Version: 0.1.6
+Version: 0.1.7
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/SOURCES.txt` & `ssh_remote_control-0.1.7/src/ssh_remote_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

