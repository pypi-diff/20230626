# Comparing `tmp/skodaconnect-1.3.5.tar.gz` & `tmp/skodaconnect-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skodaconnect-1.3.5.tar", last modified: Wed Mar 22 09:02:51 2023, max compression
+gzip compressed data, was "skodaconnect-1.3.6.tar", last modified: Mon Jun 26 07:40:26 2023, max compression
```

## Comparing `skodaconnect-1.3.5.tar` & `skodaconnect-1.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2023-03-22 09:02:51.676988 skodaconnect-1.3.5/
--rw-r--r--   0 KINIL      (502) staff       (20)      127 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/.gitignore
-drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2023-03-22 09:02:51.675138 skodaconnect-1.3.5/.settings/
--rw-r--r--   0 KINIL      (502) staff       (20)       34 2023-03-21 07:30:32.000000 skodaconnect-1.3.5/.settings/.gitignore
--rw-rw-r--   0 KINIL      (502) staff       (20)    11357 2021-09-05 08:28:52.000000 skodaconnect-1.3.5/LICENSE
--rw-r--r--   0 KINIL      (502) staff       (20)     8128 2023-03-22 09:02:51.677051 skodaconnect-1.3.5/PKG-INFO
--rw-r--r--   0 KINIL      (502) staff       (20)     7846 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/README.md
-drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2023-03-22 09:02:51.675259 skodaconnect-1.3.5/example/
--rw-r--r--   0 KINIL      (502) staff       (20)    14972 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/example/example.py
--rw-rw-r--   0 KINIL      (502) staff       (20)       47 2022-01-12 12:55:51.000000 skodaconnect-1.3.5/requirements.txt
--rw-rw-r--   0 KINIL      (502) staff       (20)      440 2023-03-22 09:02:51.677307 skodaconnect-1.3.5/setup.cfg
--rw-rw-r--   0 KINIL      (502) staff       (20)      952 2022-01-12 12:55:51.000000 skodaconnect-1.3.5/setup.py
-drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2023-03-22 09:02:51.676285 skodaconnect-1.3.5/skodaconnect/
--rw-rw-r--   0 KINIL      (502) staff       (20)      290 2021-11-17 09:16:28.000000 skodaconnect-1.3.5/skodaconnect/__init__.py
--rw-r--r--   0 KINIL      (502) staff       (20)      226 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/skodaconnect/__version__.py
--rw-r--r--   0 KINIL      (502) staff       (20)    99944 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/skodaconnect/connection.py
--rw-r--r--   0 KINIL      (502) staff       (20)     9894 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/skodaconnect/const.py
--rw-r--r--   0 KINIL      (502) staff       (20)    50236 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/skodaconnect/dashboard.py
--rw-r--r--   0 KINIL      (502) staff       (20)     3209 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/skodaconnect/exceptions.py
--rw-r--r--   0 KINIL      (502) staff       (20)     2565 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/skodaconnect/utilities.py
--rw-r--r--   0 KINIL      (502) staff       (20)   164242 2023-03-22 08:58:04.000000 skodaconnect-1.3.5/skodaconnect/vehicle.py
-drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2023-03-22 09:02:51.676889 skodaconnect-1.3.5/skodaconnect.egg-info/
--rw-rw-r--   0 KINIL      (502) staff       (20)     8128 2023-03-22 09:02:51.000000 skodaconnect-1.3.5/skodaconnect.egg-info/PKG-INFO
--rw-rw-r--   0 KINIL      (502) staff       (20)      488 2023-03-22 09:02:51.000000 skodaconnect-1.3.5/skodaconnect.egg-info/SOURCES.txt
--rw-rw-r--   0 KINIL      (502) staff       (20)        1 2023-03-22 09:02:51.000000 skodaconnect-1.3.5/skodaconnect.egg-info/dependency_links.txt
--rw-rw-r--   0 KINIL      (502) staff       (20)       47 2023-03-22 09:02:51.000000 skodaconnect-1.3.5/skodaconnect.egg-info/requires.txt
--rw-rw-r--   0 KINIL      (502) staff       (20)       13 2023-03-22 09:02:51.000000 skodaconnect-1.3.5/skodaconnect.egg-info/top_level.txt
+drwxrwxr-x   0 nivo      (1000) nivo      (1000)        0 2023-06-26 07:40:26.373707 skodaconnect-1.3.6/
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)      127 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/.gitignore
+drwxrwxr-x   0 nivo      (1000) nivo      (1000)        0 2023-06-26 07:40:26.369707 skodaconnect-1.3.6/.settings/
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)       34 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/.settings/.gitignore
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)    11357 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/LICENSE
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)     8165 2023-06-26 07:40:26.373707 skodaconnect-1.3.6/PKG-INFO
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)     7846 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/README.md
+drwxrwxr-x   0 nivo      (1000) nivo      (1000)        0 2023-06-26 07:40:26.369707 skodaconnect-1.3.6/example/
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)    14972 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/example/example.py
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)       47 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/requirements.txt
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)      440 2023-06-26 07:40:26.377707 skodaconnect-1.3.6/setup.cfg
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)      952 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/setup.py
+drwxrwxr-x   0 nivo      (1000) nivo      (1000)        0 2023-06-26 07:40:26.373707 skodaconnect-1.3.6/skodaconnect/
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)      290 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/skodaconnect/__init__.py
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)      226 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/skodaconnect/__version__.py
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)    99944 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/skodaconnect/connection.py
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)     9894 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/skodaconnect/const.py
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)    50241 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/skodaconnect/dashboard.py
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)     3209 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/skodaconnect/exceptions.py
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)     2565 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/skodaconnect/utilities.py
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)   164132 2023-06-26 07:39:57.000000 skodaconnect-1.3.6/skodaconnect/vehicle.py
+drwxrwxr-x   0 nivo      (1000) nivo      (1000)        0 2023-06-26 07:40:26.373707 skodaconnect-1.3.6/skodaconnect.egg-info/
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)     8165 2023-06-26 07:40:26.000000 skodaconnect-1.3.6/skodaconnect.egg-info/PKG-INFO
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)      488 2023-06-26 07:40:26.000000 skodaconnect-1.3.6/skodaconnect.egg-info/SOURCES.txt
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)        1 2023-06-26 07:40:26.000000 skodaconnect-1.3.6/skodaconnect.egg-info/dependency_links.txt
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)       47 2023-06-26 07:40:26.000000 skodaconnect-1.3.6/skodaconnect.egg-info/requires.txt
+-rw-rw-r--   0 nivo      (1000) nivo      (1000)       13 2023-06-26 07:40:26.000000 skodaconnect-1.3.6/skodaconnect.egg-info/top_level.txt
```

### Comparing `skodaconnect-1.3.5/LICENSE` & `skodaconnect-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.5/PKG-INFO` & `skodaconnect-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: skodaconnect
-Version: 1.3.5
+Version: 1.3.6
 Summary: Communicate with Skoda Connect
 Home-page: https://github.com/lendy007/skodaconnect
 Author: lendy007
 Author-email: lendik@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Provides: skodaconnect
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Version](https://img.shields.io/github/v/release/lendy007/skodaconnect?include_prereleases)
 ![PyPi](https://img.shields.io/pypi/v/skodaconnect?label=latest%20pypi)
 ![Downloads PyPi](https://img.shields.io/pypi/dm/skodaconnect)
@@ -119,7 +121,9 @@
 conn.get<method>                                                        # The get methods calls on API endpoints and returns data. See example.
 conn.set<method>                                                        # The set methods calls on API endpoints to set config for vehicle.
 ```
 Refrain from using methods starting with _, they are intended for internal use only.
 
 ## Further help or contributions
 For questions, further help or contributions you can join the Discord server at https://discord.gg/826X9jEtCh
+
+
```

### Comparing `skodaconnect-1.3.5/README.md` & `skodaconnect-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.5/example/example.py` & `skodaconnect-1.3.6/example/example.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.5/setup.py` & `skodaconnect-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.5/skodaconnect/connection.py` & `skodaconnect-1.3.6/skodaconnect/connection.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.5/skodaconnect/const.py` & `skodaconnect-1.3.6/skodaconnect/const.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.5/skodaconnect/dashboard.py` & `skodaconnect-1.3.6/skodaconnect/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1261,15 +1261,15 @@
             icon="mdi:clock",
             device_class="timestamp"
         ),
         Sensor(
             attr="charging_time_left",
             name="Charging time left",
             icon="mdi:battery-charging-100",
-            unit="h",
+            unit="min",
             device_class="duration"
         ),
         Sensor(
             attr="charge_rate",
             name="Charging rate",
             icon="mdi:battery-heart",
             unit="km/h"
@@ -1309,15 +1309,15 @@
             unit="°C",
             device_class="temperature"
         ),
         Sensor(
             attr="climatisation_time_left",
             name="Climatisation time left",
             icon="mdi:clock",
-            unit="h",
+            unit="min",
             device_class="duration"
         ),
         Sensor(
             attr="trip_last_average_speed",
             name="Last trip average speed",
             icon="mdi:speedometer",
             unit="km/h",
@@ -1707,8 +1707,8 @@
     def __init__(self, vehicle, **config):
         self._config = config
         self.instruments = [
             instrument
             for instrument in create_instruments()
             if instrument.setup(vehicle, **config)
         ]
-        _LOGGER.debug("Supported instruments: " + ", ".join(str(inst.attr) for inst in self.instruments))
+        _LOGGER.debug("Supported instruments: " + ", ".join(str(inst.attr) for inst in self.instruments))
```

### Comparing `skodaconnect-1.3.5/skodaconnect/exceptions.py` & `skodaconnect-1.3.6/skodaconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.5/skodaconnect/utilities.py` & `skodaconnect-1.3.6/skodaconnect/utilities.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.5/skodaconnect/vehicle.py` & `skodaconnect-1.3.6/skodaconnect/vehicle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1832,26 +1832,27 @@
             if 'connectionState' in self.attrs.get('plug', {}):
                 return True
         return False
 
     @property
     def charging_time_left(self):
         """Return minutes to charging complete"""
-        if self.external_power:
+        if not self.external_power:
+            return 0
+        try:
             if self.attrs.get('charging', {}).get('remainingToCompleteInSeconds', False):
                 minutes = int(self.attrs.get('charging', {}).get('remainingToCompleteInSeconds', 0))/60
             elif self.attrs.get('charger', {}).get('status', {}).get('batteryStatusData', {}).get('remainingChargingTime', False):
                 minutes = self.attrs.get('charger', {}).get('status', {}).get('batteryStatusData', {}).get('remainingChargingTime', {}).get('content', 0)
-            try:
-                if minutes == -1: return '00:00'
-                if minutes == 65535: return '00:00'
-                return "%02d:%02d" % divmod(minutes, 60)
-            except Exception:
-                pass
-        return '00:00'
+            if not 0 <= minutes < 65535:
+                return 0
+            return minutes
+        except Exception:
+            pass
+        return 0
 
     @property
     def is_charging_time_left_supported(self):
         """Return true if charging is supported"""
         return self.is_charging_supported
 
     @property
@@ -2160,24 +2161,24 @@
         elif self.attrs.get('airConditioningSettings', False):
             if 'targetTemperatureInKelvin' in self.attrs.get('airConditioningSettings', {}):
                 return True
         return False
 
     @property
     def climatisation_time_left(self):
-        """Return time left for climatisation in hours:minutes."""
+        """Return time left for climatisation in minutes."""
         if self.attrs.get('airConditioning', {}).get('remainingTimeToReachTargetTemperatureInSeconds', False):
             try:
                 minutes = int(self.attrs.get('airConditioning', {}).get('remainingTimeToReachTargetTemperatureInSeconds', 0))/60
                 if not 0 <= minutes <= 65535:
-                    return "00:00"
-                return "%02d:%02d" % divmod(minutes, 60)
+                    return 0
+                return minutes
             except Exception:
                 pass
-        return "00:00"
+        return 0
 
     @property
     def is_climatisation_time_left_supported(self):
         #"""Return true if remainingTimeToReachTargetTemperatureInSeconds is supported."""
         """ Return true if airConditioning is supported. """
         #if self.attrs.get('airConditioning', {}).get('remainingTimeToReachTargetTemperatureInSeconds', False):
         if self.attrs.get('airConditioning', False):
@@ -2960,15 +2961,15 @@
     @property
     def trip_longterm_entry(self):
         return self.attrs.get('longtermstatistics', {})
 
     @property
     def trip_cyclic_entry(self):
         return self.attrs.get('cyclicstatistics', {})
-        
+
     @property
     def trip_last_average_speed(self):
         return self.trip_last_entry.get('averageSpeed')
 
     @property
     def is_trip_last_average_speed_supported(self):
         response = self.trip_last_entry
```

### Comparing `skodaconnect-1.3.5/skodaconnect.egg-info/PKG-INFO` & `skodaconnect-1.3.6/skodaconnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: skodaconnect
-Version: 1.3.5
+Version: 1.3.6
 Summary: Communicate with Skoda Connect
 Home-page: https://github.com/lendy007/skodaconnect
 Author: lendy007
 Author-email: lendik@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Provides: skodaconnect
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Version](https://img.shields.io/github/v/release/lendy007/skodaconnect?include_prereleases)
 ![PyPi](https://img.shields.io/pypi/v/skodaconnect?label=latest%20pypi)
 ![Downloads PyPi](https://img.shields.io/pypi/dm/skodaconnect)
@@ -119,7 +121,9 @@
 conn.get<method>                                                        # The get methods calls on API endpoints and returns data. See example.
 conn.set<method>                                                        # The set methods calls on API endpoints to set config for vehicle.
 ```
 Refrain from using methods starting with _, they are intended for internal use only.
 
 ## Further help or contributions
 For questions, further help or contributions you can join the Discord server at https://discord.gg/826X9jEtCh
+
+
```

