# Comparing `tmp/FlightRadarAPI-1.3.6.tar.gz` & `tmp/FlightRadarAPI-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlightRadarAPI-1.3.6.tar", last modified: Sun Jun 25 22:17:35 2023, max compression
+gzip compressed data, was "FlightRadarAPI-1.3.7.tar", last modified: Mon Jun 26 02:40:20 2023, max compression
```

## Comparing `FlightRadarAPI-1.3.6.tar` & `FlightRadarAPI-1.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 22:17:34.885899 FlightRadarAPI-1.3.6/
-drwxrwxrwx   0        0        0        0 2023-06-25 22:17:34.678128 FlightRadarAPI-1.3.6/FlightRadar24/
--rw-rw-rw-   0        0        0      577 2023-06-25 22:03:02.000000 FlightRadarAPI-1.3.6/FlightRadar24/__init__.py
--rw-rw-rw-   0        0        0     9991 2023-06-25 21:44:59.000000 FlightRadarAPI-1.3.6/FlightRadar24/api.py
--rw-rw-rw-   0        0        0     2109 2023-06-25 08:27:20.000000 FlightRadarAPI-1.3.6/FlightRadar24/core.py
-drwxrwxrwx   0        0        0        0 2023-06-25 22:17:34.721061 FlightRadarAPI-1.3.6/FlightRadar24/entities/
--rw-rw-rw-   0        0        0      113 2023-06-25 22:03:21.000000 FlightRadarAPI-1.3.6/FlightRadar24/entities/__init__.py
--rw-rw-rw-   0        0        0     3143 2023-06-25 22:05:15.000000 FlightRadarAPI-1.3.6/FlightRadar24/entities/airport.py
--rw-rw-rw-   0        0        0      849 2023-06-25 08:53:18.000000 FlightRadarAPI-1.3.6/FlightRadar24/entities/entity.py
--rw-rw-rw-   0        0        0    10171 2023-06-25 22:02:11.000000 FlightRadarAPI-1.3.6/FlightRadar24/entities/flight.py
--rw-rw-rw-   0        0        0      271 2023-06-25 08:59:59.000000 FlightRadarAPI-1.3.6/FlightRadar24/errors.py
--rw-rw-rw-   0        0        0     3091 2023-06-25 08:27:20.000000 FlightRadarAPI-1.3.6/FlightRadar24/request.py
-drwxrwxrwx   0        0        0        0 2023-06-25 22:17:34.883985 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/
--rw-rw-rw-   0        0        0     3181 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-25 22:17:33.000000 FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1110 2023-01-13 23:16:02.000000 FlightRadarAPI-1.3.6/LICENSE
--rw-rw-rw-   0        0        0     3181 2023-06-25 22:17:34.884893 FlightRadarAPI-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-06-25 08:27:20.000000 FlightRadarAPI-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 22:17:34.885899 FlightRadarAPI-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-05-28 19:59:55.000000 FlightRadarAPI-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 02:40:20.307123 FlightRadarAPI-1.3.7/
+drwxrwxrwx   0        0        0        0 2023-06-26 02:40:20.189104 FlightRadarAPI-1.3.7/FlightRadar24/
+-rw-rw-rw-   0        0        0      564 2023-06-26 01:45:52.000000 FlightRadarAPI-1.3.7/FlightRadar24/__init__.py
+-rw-rw-rw-   0        0        0    10978 2023-06-26 02:39:17.000000 FlightRadarAPI-1.3.7/FlightRadar24/api.py
+-rw-rw-rw-   0        0        0     2254 2023-06-26 01:30:55.000000 FlightRadarAPI-1.3.7/FlightRadar24/core.py
+drwxrwxrwx   0        0        0        0 2023-06-26 02:40:20.279268 FlightRadarAPI-1.3.7/FlightRadar24/entities/
+-rw-rw-rw-   0        0        0      113 2023-06-25 22:03:21.000000 FlightRadarAPI-1.3.7/FlightRadar24/entities/__init__.py
+-rw-rw-rw-   0        0        0     3143 2023-06-25 22:05:15.000000 FlightRadarAPI-1.3.7/FlightRadar24/entities/airport.py
+-rw-rw-rw-   0        0        0      849 2023-06-25 08:53:18.000000 FlightRadarAPI-1.3.7/FlightRadar24/entities/entity.py
+-rw-rw-rw-   0        0        0    10171 2023-06-25 23:54:15.000000 FlightRadarAPI-1.3.7/FlightRadar24/entities/flight.py
+-rw-rw-rw-   0        0        0      271 2023-06-25 08:59:59.000000 FlightRadarAPI-1.3.7/FlightRadar24/errors.py
+-rw-rw-rw-   0        0        0     3356 2023-06-26 01:43:43.000000 FlightRadarAPI-1.3.7/FlightRadar24/request.py
+drwxrwxrwx   0        0        0        0 2023-06-26 02:40:20.305065 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/
+-rw-rw-rw-   0        0        0     3179 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1110 2023-01-13 23:16:02.000000 FlightRadarAPI-1.3.7/LICENSE
+-rw-rw-rw-   0        0        0     3179 2023-06-26 02:40:20.306081 FlightRadarAPI-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2508 2023-06-26 01:51:29.000000 FlightRadarAPI-1.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 02:40:20.308066 FlightRadarAPI-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-05-28 19:59:55.000000 FlightRadarAPI-1.3.7/setup.py
```

### Comparing `FlightRadarAPI-1.3.6/FlightRadar24/__init__.py` & `FlightRadarAPI-1.3.7/FlightRadar24/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 See more information at:
 https://www.flightradar24.com/premium/
 https://www.flightradar24.com/terms-and-conditions
 """
 
 __author__ = "Jean Loui Bernard Silva de Jesus"
-__version__ = "1.3.6"
+__version__ = "1.3.7"
 
 from .api import FlightRadar24API, FlightTrackerConfig
-from FlightRadar24.entities import Airport, Flight
+from .entities import Airport, Flight
```

### Comparing `FlightRadarAPI-1.3.6/FlightRadar24/api.py` & `FlightRadarAPI-1.3.7/FlightRadar24/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def get_airline_logo(self, iata: str, icao: str) -> Optional[Tuple[bytes, str]]:
         """
         Download the logo of an airline from FlightRadar24 and return it as bytes.
         """
         first_logo_url = Core.airline_logo_url.format(iata, icao)
 
         # Try to get the image by the first URL option.
-        response = APIRequest(first_logo_url, headers = Core.image_headers)
+        response = APIRequest(first_logo_url, headers = Core.image_headers, exclude_status_codes=[403,])
         status_code = response.get_status_code()
 
         if not str(status_code).startswith("4"):
             return response.get_content(), first_logo_url.split(".")[-1]
 
         # Get the image by the second airline logo URL.
         second_logo_url = Core.alternative_airline_logo_url.format(icao)
@@ -76,35 +76,56 @@
         status_code = response.get_status_code()
 
         if not str(status_code).startswith("4"):
             return response.get_content(), second_logo_url.split(".")[-1]
 
     def get_airport(self, code: str) -> Airport:
         """
-        Return detailed information about an airport.
+        Return information about a specific airport.
 
         :param code: ICAO or IATA of the airport
         """
         response = APIRequest(Core.airport_data_url.format(code), headers = Core.json_headers)
         return Airport(details=response.get_content()["details"])
 
-    def get_airports(self, *, details: bool = False) -> List[Airport]:
+    def get_airport_details(self, code: str, flight_limit: int = 100) -> Dict:
+        """
+        Return the airport details from FlightRadar24.
+
+        :param code: ICAO or IATA of the airport
+        :param flight_limit: Limit of flights related to the airport
+        """
+        request_params = {"format": "json"}
+
+        if self.__login_data is not None:
+            request_params["token"] = self.__login_data["cookies"]["_frPl"]
+
+        # Insert the method parameters into the dictionary for the request.
+        request_params["code"] = code
+        request_params["limit"] = flight_limit
+
+        # Request details from the FlightRadar24.
+        response = APIRequest(Core.api_airport_data_url, request_params, Core.json_headers, exclude_status_codes=[400,])
+        content: Dict = response.get_content()
+
+        if response.get_status_code() == 400 and isinstance(content, dict) and content.get("errors"):
+            raise ValueError(content["errors"]["errors"]["parameters"]["limit"]["notBetween"])
+
+        return content["result"]["response"]
+
+    def get_airports(self) -> List[Airport]:
         """
         Return a list with all airports.
         """
         response = APIRequest(Core.airports_data_url, headers = Core.json_headers)
 
         airports: List[Airport] = list()
 
         for airport_data in response.get_content()["rows"]:
             airport = Airport(info = airport_data)
-
-            # Get airport details.
-            if details: airport = self.get_airport(airport.icao)
-
             airports.append(airport)
 
         return airports
 
     def get_bounds(self, zone: Dict[str, float]) -> str:
         """
         Convert coordinate dictionary to a string "y1, y2, x1, x2".
@@ -129,15 +150,15 @@
         status_code = response.get_status_code()
 
         if not str(status_code).startswith("4"):
             return response.get_content(), flag_url.split(".")[-1]
 
     def get_flight_details(self, flight_id: str) -> Dict[Any, Any]:
         """
-        Return the flight details from Data Live Flightradar24.
+        Return the flight details from Data Live FlightRadar24.
         """
         response = APIRequest(Core.flight_data_url.format(flight_id), headers = Core.json_headers)
         return response.get_content()
 
     def get_flights(
         self,
         airline: str = None,
@@ -163,15 +184,15 @@
 
         # Insert the method parameters into the dictionary for the request.
         if airline: request_params["airline"] = airline
         if bounds: request_params["bounds"] = bounds.replace(",", "%2C")
         if registration: request_params["reg"] = registration
         if aircraft_type: request_params["type"] = aircraft_type
 
-        # Get all flights from Data Live Flightradar24.
+        # Get all flights from Data Live FlightRadar24.
         response = APIRequest(Core.real_time_flight_tracker_data_url, request_params, Core.json_headers)
         response = response.get_content()
 
         flights: List[Flight] = list()
 
         for flight_id, flight_info in response.items():
 
@@ -185,29 +206,29 @@
             # Set flight details.
             if details:
                 flight_details = self.get_flight_details(flight_id)
                 flight.set_flight_details(flight_details)
 
         return flights
 
+    def get_flight_tracker_config(self) -> FlightTrackerConfig:
+        """
+        Return a copy of the current config of the Real Time Flight Tracker, used by get_flights() method.
+        """
+        return dataclasses.replace(self.__flight_tracker_config)
+
     def get_login_data(self) -> Dict[Any, Any]:
         """
         Return the user data.
         """
         if not self.is_logged_in():
             raise LoginError("You must log in to your account.")
 
         return self.__login_data["userData"].copy()
 
-    def get_flight_tracker_config(self) -> FlightTrackerConfig:
-        """
-        Return a copy of the current config of the Real Time Flight Tracker, used by get_flights() method.
-        """
-        return dataclasses.replace(self.__flight_tracker_config)
-
     def get_zones(self) -> Dict[str, Dict]:
         """
         Return all major zones on the globe.
         """
         response = APIRequest(Core.zones_data_url, headers = Core.json_headers)
         zones = response.get_content()
```

### Comparing `FlightRadarAPI-1.3.6/FlightRadar24/core.py` & `FlightRadarAPI-1.3.7/FlightRadar24/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 from abc import ABC
 
 
 class Core(ABC):
 
     # Base URLs.
+    api_flightradar_base_url = "https://api.flightradar24.com/common/v1"
     cdn_flightradar_base_url = "https://cdn.flightradar24.com"
     flightradar_base_url = "https://www.flightradar24.com"
     data_live_base_url = "https://data-live.flightradar24.com"
     data_cloud_base_url = "https://data-cloud.flightradar24.com"
 
     # User login URL.
     user_login_url = flightradar_base_url + "/user/login"
     user_logout_url = flightradar_base_url + "/user/logout"
 
     # Flights data URLs.
     real_time_flight_tracker_data_url = data_cloud_base_url + "/zones/fcgi/feed.js"
     flight_data_url = data_live_base_url + "/clickhandler/?flight={}"
 
     # Airports data URLs.
+    api_airport_data_url = api_flightradar_base_url + "/airport.json"
     airport_data_url = flightradar_base_url + "/airports/traffic-stats/?airport={}"
     airports_data_url = flightradar_base_url + "/_json/airports.php"
 
     # Airlines data URL.
     airlines_data_url = flightradar_base_url + "/_json/airlines.php"
 
     # Zones data URL.
```

### Comparing `FlightRadarAPI-1.3.6/FlightRadar24/entities/airport.py` & `FlightRadarAPI-1.3.7/FlightRadar24/entities/airport.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.6/FlightRadar24/entities/entity.py` & `FlightRadarAPI-1.3.7/FlightRadar24/entities/entity.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.6/FlightRadar24/entities/flight.py` & `FlightRadarAPI-1.3.7/FlightRadar24/entities/flight.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.6/FlightRadar24/request.py` & `FlightRadarAPI-1.3.7/FlightRadar24/request.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from typing import Dict, Optional, Union
+from typing import Dict, List, Optional, Union
 
 import brotli
 import json
 import gzip
 
 import requests
 import requests.structures
@@ -24,24 +24,26 @@
 
     def __init__(
         self,
         url: str,
         params: Optional[Dict] = None,
         headers: Optional[Dict] = None,
         data: Optional[Dict] = None,
-        cookies: Optional[Dict] = None
+        cookies: Optional[Dict] = None,
+        exclude_status_codes: List[int] = list()
     ):
         """
         Constructor of the APIRequest class.
 
         :param url: URL for the request
         :param params: params that will be inserted on the URL for the request
         :param headers: headers for the request
         :param data: data for the request. If "data" is None, request will be a GET. Otherwise, it will be a POST
         :param cookies: cookies for the request
+        :param exclude_status_codes: raise for status code except those on the excluded list
         """
         self.url = url
 
         self.request_params = {
             "params": params,
             "headers": headers,
             "data": data,
@@ -55,29 +57,32 @@
 
         if self.get_status_code() == 520:
             raise CloudflareError(
                 message = "An unexpected error has occurred. Perhaps you are making too many calls?",
                 response = self.__response
             )
 
+        if self.get_status_code() not in exclude_status_codes:
+            self.__response.raise_for_status()
+
     def get_content(self) -> Union[Dict, bytes]:
         """
         Return the received content from the request.
         """
         content = self.__response.content
 
         content_encoding = self.__response.headers.get("Content-Encoding", "")
         content_type = self.__response.headers["Content-Type"]
 
         # Try to decode the content.
         try: content = self.__content_encodings[content_encoding](content)
         except Exception: pass
 
         # Return a dictionary if the content type is JSON.
-        if content_type == "application/json":
+        if "application/json" in content_type:
             return json.loads(content)
 
         return content
 
     def get_cookies(self) -> Dict:
         """
         Return the received cookies from the request.
```

### Comparing `FlightRadarAPI-1.3.6/FlightRadarAPI.egg-info/PKG-INFO` & `FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.6
+Version: 1.3.7
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FlightRadarAPI
-Unofficial API for [Flight Radar 24](https://www.flightradar24.com/) written in Python 3.
+Unofficial API for [FlightRadar24](https://www.flightradar24.com/) written in Python 3.
 
 If you want to use the data collected using this API commercially, you need to subscribe to the [Business plan](https://www.flightradar24.com/premium/).</br>
 See more information at: https://www.flightradar24.com/terms-and-conditions
 
 [![Python Package](https://github.com/JeanExtreme002/FlightRadarAPI/workflows/Python%20Package/badge.svg)](https://github.com/JeanExtreme002/FlightRadarAPI/actions)
 [![Pypi](https://img.shields.io/pypi/v/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
 [![License](https://img.shields.io/pypi/l/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
```

### Comparing `FlightRadarAPI-1.3.6/LICENSE` & `FlightRadarAPI-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.6/PKG-INFO` & `FlightRadarAPI-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.6
+Version: 1.3.7
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FlightRadarAPI
-Unofficial API for [Flight Radar 24](https://www.flightradar24.com/) written in Python 3.
+Unofficial API for [FlightRadar24](https://www.flightradar24.com/) written in Python 3.
 
 If you want to use the data collected using this API commercially, you need to subscribe to the [Business plan](https://www.flightradar24.com/premium/).</br>
 See more information at: https://www.flightradar24.com/terms-and-conditions
 
 [![Python Package](https://github.com/JeanExtreme002/FlightRadarAPI/workflows/Python%20Package/badge.svg)](https://github.com/JeanExtreme002/FlightRadarAPI/actions)
 [![Pypi](https://img.shields.io/pypi/v/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
 [![License](https://img.shields.io/pypi/l/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
```

### Comparing `FlightRadarAPI-1.3.6/README.md` & `FlightRadarAPI-1.3.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # FlightRadarAPI
-Unofficial API for [Flight Radar 24](https://www.flightradar24.com/) written in Python 3.
+Unofficial API for [FlightRadar24](https://www.flightradar24.com/) written in Python 3.
 
 If you want to use the data collected using this API commercially, you need to subscribe to the [Business plan](https://www.flightradar24.com/premium/).</br>
 See more information at: https://www.flightradar24.com/terms-and-conditions
 
 [![Python Package](https://github.com/JeanExtreme002/FlightRadarAPI/workflows/Python%20Package/badge.svg)](https://github.com/JeanExtreme002/FlightRadarAPI/actions)
 [![Pypi](https://img.shields.io/pypi/v/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
 [![License](https://img.shields.io/pypi/l/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
```

### Comparing `FlightRadarAPI-1.3.6/setup.py` & `FlightRadarAPI-1.3.7/setup.py`

 * *Files identical despite different names*

