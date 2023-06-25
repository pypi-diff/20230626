# Comparing `tmp/FlightRadarAPI-1.3.5.tar.gz` & `tmp/FlightRadarAPI-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlightRadarAPI-1.3.5.tar", last modified: Sun Jun 25 07:05:05 2023, max compression
+gzip compressed data, was "FlightRadarAPI-1.3.6.tar", last modified: Sun Jun 25 22:17:35 2023, max compression
```

## Comparing `FlightRadarAPI-1.3.5.tar` & `FlightRadarAPI-1.3.6.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 07:05:05.402528 FlightRadarAPI-1.3.5/
-drwxrwxrwx   0        0        0        0 2023-06-25 07:05:05.384741 FlightRadarAPI-1.3.5/FlightRadar24/
--rw-rw-rw-   0        0        0      553 2023-06-25 07:00:28.000000 FlightRadarAPI-1.3.5/FlightRadar24/__init__.py
--rw-rw-rw-   0        0        0     9611 2023-06-25 07:01:46.000000 FlightRadarAPI-1.3.5/FlightRadar24/api.py
--rw-rw-rw-   0        0        0     2109 2023-06-24 19:02:23.000000 FlightRadarAPI-1.3.5/FlightRadar24/core.py
--rw-rw-rw-   0        0        0      244 2023-06-25 06:53:16.000000 FlightRadarAPI-1.3.5/FlightRadar24/errors.py
--rw-rw-rw-   0        0        0    10004 2023-06-25 04:49:16.000000 FlightRadarAPI-1.3.5/FlightRadar24/flight.py
--rw-rw-rw-   0        0        0     3091 2023-06-25 06:53:31.000000 FlightRadarAPI-1.3.5/FlightRadar24/request.py
-drwxrwxrwx   0        0        0        0 2023-06-25 07:05:05.400498 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/
--rw-rw-rw-   0        0        0     3181 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-25 07:05:05.000000 FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.5/LICENSE
--rw-rw-rw-   0        0        0     3181 2023-06-25 07:05:05.400498 FlightRadarAPI-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-06-25 03:54:22.000000 FlightRadarAPI-1.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 07:05:05.402528 FlightRadarAPI-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-06-25 06:47:19.000000 FlightRadarAPI-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 22:17:34.885899 FlightRadarAPI-1.3.6/
+drwxrwxrwx   0        0        0        0 2023-06-25 22:17:34.678128 FlightRadarAPI-1.3.6/FlightRadar24/
+-rw-rw-rw-   0        0        0      577 2023-06-25 22:03:02.000000 FlightRadarAPI-1.3.6/FlightRadar24/__init__.py
+-rw-rw-rw-   0        0        0     9991 2023-06-25 21:44:59.000000 FlightRadarAPI-1.3.6/FlightRadar24/api.py
+-rw-rw-rw-   0        0        0     2109 2023-06-25 08:27:20.000000 FlightRadarAPI-1.3.6/FlightRadar24/core.py
+drwxrwxrwx   0        0        0        0 2023-06-25 22:17:34.721061 FlightRadarAPI-1.3.6/FlightRadar24/entities/
+-rw-rw-rw-   0        0        0      113 2023-06-25 22:03:21.000000 FlightRadarAPI-1.3.6/FlightRadar24/entities/__init__.py
+-rw-rw-rw-   0        0        0     3143 2023-06-25 22:05:15.000000 FlightRadarAPI-1.3.6/FlightRadar24/entities/airport.py
+-rw-rw-rw-   0        0        0      849 2023-06-25 08:53:18.000000 FlightRadarAPI-1.3.6/FlightRadar24/entities/entity.py
+-rw-rw-rw-   0        0        0    10171 2023-06-25 22:02:11.000000 FlightRadarAPI-1.3.6/FlightRadar24/entities/flight.py
+-rw-rw-rw-   0        0        0      271 2023-06-25 08:59:59.000000 FlightRadarAPI-1.3.6/FlightRadar24/errors.py
+-rw-rw-rw-   0        0        0     3091 2023-06-25 08:27:20.000000 FlightRadarAPI-1.3.6/FlightRadar24/request.py
+drwxrwxrwx   0        0        0        0 2023-06-25 22:17:34.883985 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/
+-rw-rw-rw-   0        0        0     3181 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1110 2023-01-13 23:16:02.000000 FlightRadarAPI-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0     3181 2023-06-25 22:17:34.884893 FlightRadarAPI-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-06-25 08:27:20.000000 FlightRadarAPI-1.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 22:17:34.885899 FlightRadarAPI-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-05-28 19:59:55.000000 FlightRadarAPI-1.3.6/setup.py
```

### Comparing `FlightRadarAPI-1.3.5/FlightRadar24/__init__.py` & `FlightRadarAPI-1.3.6/FlightRadar24/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 See more information at:
 https://www.flightradar24.com/premium/
 https://www.flightradar24.com/terms-and-conditions
 """
 
 __author__ = "Jean Loui Bernard Silva de Jesus"
-__version__ = "1.3.5"
+__version__ = "1.3.6"
 
 from .api import FlightRadar24API, FlightTrackerConfig
-from .flight import Flight
+from FlightRadar24.entities import Airport, Flight
```

### Comparing `FlightRadarAPI-1.3.5/FlightRadar24/api.py` & `FlightRadarAPI-1.3.6/FlightRadar24/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import dataclasses
 
 from .core import Core
+from .entities.airport import Airport
+from .entities.flight import Flight
 from .errors import LoginError
-from .flight import Flight
 from .request import APIRequest
 
 
 @dataclasses.dataclass
 class FlightTrackerConfig(object):
     """
     Data class with settings of the Real Time Flight Tracker.
@@ -73,29 +74,40 @@
 
         response = APIRequest(second_logo_url, headers = Core.image_headers)
         status_code = response.get_status_code()
 
         if not str(status_code).startswith("4"):
             return response.get_content(), second_logo_url.split(".")[-1]
 
-    def get_airport(self, code: str) -> Dict:
+    def get_airport(self, code: str) -> Airport:
         """
         Return detailed information about an airport.
 
         :param code: ICAO or IATA of the airport
         """
         response = APIRequest(Core.airport_data_url.format(code), headers = Core.json_headers)
-        return response.get_content()["details"]
+        return Airport(details=response.get_content()["details"])
 
-    def get_airports(self) -> List[Dict]:
+    def get_airports(self, *, details: bool = False) -> List[Airport]:
         """
         Return a list with all airports.
         """
         response = APIRequest(Core.airports_data_url, headers = Core.json_headers)
-        return response.get_content()["rows"]
+
+        airports: List[Airport] = list()
+
+        for airport_data in response.get_content()["rows"]:
+            airport = Airport(info = airport_data)
+
+            # Get airport details.
+            if details: airport = self.get_airport(airport.icao)
+
+            airports.append(airport)
+
+        return airports
 
     def get_bounds(self, zone: Dict[str, float]) -> str:
         """
         Convert coordinate dictionary to a string "y1, y2, x1, x2".
 
         :param zone: Dictionary containing the following keys: tl_y, tl_x, br_y, br_x
         """
```

### Comparing `FlightRadarAPI-1.3.5/FlightRadar24/core.py` & `FlightRadarAPI-1.3.6/FlightRadar24/core.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.5/FlightRadar24/flight.py` & `FlightRadarAPI-1.3.6/FlightRadar24/entities/flight.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # -*- coding: utf-8 -*-
 
-from typing import Any, List, Dict
+from typing import Any, Dict, List
+from .entity import Entity
 
 
-class Flight(object):
-
+class Flight(Entity):
+    """
+    Flight representation.
+    """
     __default_text = "N/A"
 
     def __init__(self, flight_id: str, info: List[Any]):
         """
         Constructor of the Flight class.
 
         :param flight_id: The flight ID specifically used by FlightRadar24
         :param info: Dictionary with received data from FlightRadar24
         """
+        super().__init__(
+            latitude = self.__get_info(info[1]),
+            longitude = self.__get_info(info[2])
+        )
+
         self.id = flight_id
         self.icao_24bit = self.__get_info(info[0])
-        self.latitude = self.__get_info(info[1])
-        self.longitude = self.__get_info(info[2])
         self.heading = self.__get_info(info[3])
         self.altitude = self.__get_info(info[4])
         self.ground_speed = self.__get_info(info[5])
         self.squawk = self.__get_info(info[6])
         self.aircraft_code = self.__get_info(info[8])
         self.registration = self.__get_info(info[9])
         self.time = self.__get_info(info[10])
@@ -30,27 +36,27 @@
         self.number = self.__get_info(info[13])
         self.airline_iata = self.__get_info(info[13][:2])
         self.on_ground = self.__get_info(info[14])
         self.vertical_speed =self.__get_info(info[15])
         self.callsign = self.__get_info(info[16])
         self.airline_icao = self.__get_info(info[18])
 
-    def __get_details(self, data) -> Dict:
-        return dict() if data is None else data
-
-    def __get_info(self, info: Any) -> Any:
-        return info if (info or info == 0) and info != self.__default_text else self.__default_text
-
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
         template = "<({}) {} - Altitude: {} - Ground Speed: {} - Heading: {}>"
         return template.format(self.aircraft_code, self.registration, self.altitude, self.ground_speed, self.heading)
 
+    def __get_details(self, data) -> Dict:
+        return dict() if data is None else data
+
+    def __get_info(self, info: Any) -> Any:
+        return info if (info or info == 0) and info != self.__default_text else self.__default_text
+
     def check_info(self, **info: Any) -> bool:
         """
         Check one or more flight information.
 
         You can use the prefix "max_" or "min_" in the parameter
         to compare numeric data with ">" or "<".
 
@@ -113,28 +119,28 @@
         # Get airline data.
         airline = self.__get_details(flight_details.get("airline"))
 
         # Get airport data.
         airport = self.__get_details(flight_details.get("airport"))
 
         # Get destination data.
-        dest_aiport = self.__get_details(airport.get("destination"))
-        dest_aiport_code = self.__get_details(dest_aiport.get("code"))
-        dest_aiport_info = self.__get_details(dest_aiport.get("info"))
-        dest_aiport_position = self.__get_details(dest_aiport.get("position"))
-        dest_aiport_country = self.__get_details(dest_aiport_position.get("country"))
-        dest_aiport_timezone = self.__get_details(dest_aiport.get("timezone"))
+        dest_airport = self.__get_details(airport.get("destination"))
+        dest_airport_code = self.__get_details(dest_airport.get("code"))
+        dest_airport_info = self.__get_details(dest_airport.get("info"))
+        dest_airport_position = self.__get_details(dest_airport.get("position"))
+        dest_airport_country = self.__get_details(dest_airport_position.get("country"))
+        dest_airport_timezone = self.__get_details(dest_airport.get("timezone"))
 
         # Get origin data.
-        orig_aiport = self.__get_details(airport.get("origin"))
-        orig_aiport_code = self.__get_details(orig_aiport.get("code"))
-        orig_aiport_info = self.__get_details(orig_aiport.get("info"))
-        orig_aiport_position = self.__get_details(orig_aiport.get("position"))
-        orig_aiport_country = self.__get_details(orig_aiport_position.get("country"))
-        orig_aiport_timezone = self.__get_details(orig_aiport.get("timezone"))
+        orig_airport = self.__get_details(airport.get("origin"))
+        orig_airport_code = self.__get_details(orig_airport.get("code"))
+        orig_airport_info = self.__get_details(orig_airport.get("info"))
+        orig_airport_position = self.__get_details(orig_airport.get("position"))
+        orig_airport_country = self.__get_details(orig_airport_position.get("country"))
+        orig_airport_timezone = self.__get_details(orig_airport.get("timezone"))
 
         # Get flight history.
         history = self.__get_details(flight_details.get("flightHistory"))
 
         # Get flight status.
         status = self.__get_details(flight_details.get("status"))
 
@@ -146,58 +152,58 @@
         self.aircraft_model = self.__get_info(self.__get_details(aircraft.get("model")).get("text"))
 
         # Airline information.
         self.airline_name = self.__get_info(airline.get("name"))
         self.airline_short_name = self.__get_info(airline.get("short"))
 
         # Destination airport position.
-        self.destination_airport_altitude = self.__get_info(dest_aiport_position.get("altitude"))
-        self.destination_airport_country_code = self.__get_info(dest_aiport_country.get("code"))
-        self.destination_airport_country_name = self.__get_info(dest_aiport_country.get("name"))
-        self.destination_airport_latitude = self.__get_info(dest_aiport_position.get("latitude"))
-        self.destination_airport_longitude = self.__get_info(dest_aiport_position.get("longitude"))
+        self.destination_airport_altitude = self.__get_info(dest_airport_position.get("altitude"))
+        self.destination_airport_country_code = self.__get_info(dest_airport_country.get("code"))
+        self.destination_airport_country_name = self.__get_info(dest_airport_country.get("name"))
+        self.destination_airport_latitude = self.__get_info(dest_airport_position.get("latitude"))
+        self.destination_airport_longitude = self.__get_info(dest_airport_position.get("longitude"))
 
         # Destination airport information.
-        self.destination_airport_icao = self.__get_info(dest_aiport_code.get("icao"))
-        self.destination_airport_baggage = self.__get_info(dest_aiport_info.get("baggage"))
-        self.destination_airport_gate = self.__get_info(dest_aiport_info.get("gate"))
-        self.destination_airport_name = self.__get_info(dest_aiport.get("name"))
-        self.destination_airport_terminal = self.__get_info(dest_aiport_info.get("terminal"))
-        self.destination_airport_visible = self.__get_info(dest_aiport.get("visible"))
-        self.destination_airport_website = self.__get_info(dest_aiport.get("website"))
+        self.destination_airport_icao = self.__get_info(dest_airport_code.get("icao"))
+        self.destination_airport_baggage = self.__get_info(dest_airport_info.get("baggage"))
+        self.destination_airport_gate = self.__get_info(dest_airport_info.get("gate"))
+        self.destination_airport_name = self.__get_info(dest_airport.get("name"))
+        self.destination_airport_terminal = self.__get_info(dest_airport_info.get("terminal"))
+        self.destination_airport_visible = self.__get_info(dest_airport.get("visible"))
+        self.destination_airport_website = self.__get_info(dest_airport.get("website"))
 
         # Destination airport timezone.
-        self.destination_airport_timezone_abbr = self.__get_info(dest_aiport_timezone.get("abbr"))
-        self.destination_airport_timezone_abbr_name = self.__get_info(dest_aiport_timezone.get("abbrName"))
-        self.destination_airport_timezone_name = self.__get_info(dest_aiport_timezone.get("name"))
-        self.destination_airport_timezone_offset = self.__get_info(dest_aiport_timezone.get("offset"))
-        self.destination_airport_timezone_offsetHours = self.__get_info(dest_aiport_timezone.get("offsetHours"))
+        self.destination_airport_timezone_abbr = self.__get_info(dest_airport_timezone.get("abbr"))
+        self.destination_airport_timezone_abbr_name = self.__get_info(dest_airport_timezone.get("abbrName"))
+        self.destination_airport_timezone_name = self.__get_info(dest_airport_timezone.get("name"))
+        self.destination_airport_timezone_offset = self.__get_info(dest_airport_timezone.get("offset"))
+        self.destination_airport_timezone_offsetHours = self.__get_info(dest_airport_timezone.get("offsetHours"))
 
         # Origin airport position.
-        self.origin_airport_altitude = self.__get_info(orig_aiport_position.get("altitude"))
-        self.origin_airport_country_code = self.__get_info(orig_aiport_country.get("code"))
-        self.origin_airport_country_name = self.__get_info(orig_aiport_country.get("name"))
-        self.origin_airport_latitude = self.__get_info(orig_aiport_position.get("latitude"))
-        self.origin_airport_longitude = self.__get_info(orig_aiport_position.get("longitude"))
+        self.origin_airport_altitude = self.__get_info(orig_airport_position.get("altitude"))
+        self.origin_airport_country_code = self.__get_info(orig_airport_country.get("code"))
+        self.origin_airport_country_name = self.__get_info(orig_airport_country.get("name"))
+        self.origin_airport_latitude = self.__get_info(orig_airport_position.get("latitude"))
+        self.origin_airport_longitude = self.__get_info(orig_airport_position.get("longitude"))
 
         # Origin airport information.
-        self.origin_airport_icao = self.__get_info(orig_aiport_code.get("icao"))
-        self.origin_airport_baggage = self.__get_info(orig_aiport_info.get("baggage"))
-        self.origin_airport_gate = self.__get_info(orig_aiport_info.get("gate"))
-        self.origin_airport_name = self.__get_info(orig_aiport.get("name"))
-        self.origin_airport_terminal = self.__get_info(orig_aiport_info.get("terminal"))
-        self.origin_airport_visible = self.__get_info(orig_aiport.get("visible"))
-        self.origin_airport_website = self.__get_info(orig_aiport.get("website"))
+        self.origin_airport_icao = self.__get_info(orig_airport_code.get("icao"))
+        self.origin_airport_baggage = self.__get_info(orig_airport_info.get("baggage"))
+        self.origin_airport_gate = self.__get_info(orig_airport_info.get("gate"))
+        self.origin_airport_name = self.__get_info(orig_airport.get("name"))
+        self.origin_airport_terminal = self.__get_info(orig_airport_info.get("terminal"))
+        self.origin_airport_visible = self.__get_info(orig_airport.get("visible"))
+        self.origin_airport_website = self.__get_info(orig_airport.get("website"))
 
         # Origin airport timezone.
-        self.origin_airport_timezone_abbr = self.__get_info(orig_aiport_timezone.get("abbr"))
-        self.origin_airport_timezone_abbr_name = self.__get_info(orig_aiport_timezone.get("abbrName"))
-        self.origin_airport_timezone_name = self.__get_info(orig_aiport_timezone.get("name"))
-        self.origin_airport_timezone_offset = self.__get_info(orig_aiport_timezone.get("offset"))
-        self.origin_airport_timezone_offsetHours = self.__get_info(orig_aiport_timezone.get("offsetHours"))
+        self.origin_airport_timezone_abbr = self.__get_info(orig_airport_timezone.get("abbr"))
+        self.origin_airport_timezone_abbr_name = self.__get_info(orig_airport_timezone.get("abbrName"))
+        self.origin_airport_timezone_name = self.__get_info(orig_airport_timezone.get("name"))
+        self.origin_airport_timezone_offset = self.__get_info(orig_airport_timezone.get("offset"))
+        self.origin_airport_timezone_offsetHours = self.__get_info(orig_airport_timezone.get("offsetHours"))
 
         # Flight status.
         self.status_icon = self.__get_info(status.get("icon"))
         self.status_text = self.__get_info(status.get("text"))
 
         # Time details.
         self.time_details = self.__get_details(flight_details.get("time"))
```

### Comparing `FlightRadarAPI-1.3.5/FlightRadar24/request.py` & `FlightRadarAPI-1.3.6/FlightRadar24/request.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.5/FlightRadarAPI.egg-info/PKG-INFO` & `FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.5
+Version: 1.3.6
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.5/LICENSE` & `FlightRadarAPI-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.5/PKG-INFO` & `FlightRadarAPI-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.5
+Version: 1.3.6
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.3.5/README.md` & `FlightRadarAPI-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.5/setup.py` & `FlightRadarAPI-1.3.6/setup.py`

 * *Files identical despite different names*

