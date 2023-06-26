# Comparing `tmp/FlightRadarAPI-1.3.7.tar.gz` & `tmp/flightradarapi-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlightRadarAPI-1.3.7.tar", last modified: Mon Jun 26 02:40:20 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `FlightRadarAPI-1.3.7.tar` & `flightradarapi-1.3.8.tar`

### file list

```diff
@@ -1,23 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 02:40:20.307123 FlightRadarAPI-1.3.7/
-drwxrwxrwx   0        0        0        0 2023-06-26 02:40:20.189104 FlightRadarAPI-1.3.7/FlightRadar24/
--rw-rw-rw-   0        0        0      564 2023-06-26 01:45:52.000000 FlightRadarAPI-1.3.7/FlightRadar24/__init__.py
--rw-rw-rw-   0        0        0    10978 2023-06-26 02:39:17.000000 FlightRadarAPI-1.3.7/FlightRadar24/api.py
--rw-rw-rw-   0        0        0     2254 2023-06-26 01:30:55.000000 FlightRadarAPI-1.3.7/FlightRadar24/core.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:40:20.279268 FlightRadarAPI-1.3.7/FlightRadar24/entities/
--rw-rw-rw-   0        0        0      113 2023-06-25 22:03:21.000000 FlightRadarAPI-1.3.7/FlightRadar24/entities/__init__.py
--rw-rw-rw-   0        0        0     3143 2023-06-25 22:05:15.000000 FlightRadarAPI-1.3.7/FlightRadar24/entities/airport.py
--rw-rw-rw-   0        0        0      849 2023-06-25 08:53:18.000000 FlightRadarAPI-1.3.7/FlightRadar24/entities/entity.py
--rw-rw-rw-   0        0        0    10171 2023-06-25 23:54:15.000000 FlightRadarAPI-1.3.7/FlightRadar24/entities/flight.py
--rw-rw-rw-   0        0        0      271 2023-06-25 08:59:59.000000 FlightRadarAPI-1.3.7/FlightRadar24/errors.py
--rw-rw-rw-   0        0        0     3356 2023-06-26 01:43:43.000000 FlightRadarAPI-1.3.7/FlightRadar24/request.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:40:20.305065 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/
--rw-rw-rw-   0        0        0     3179 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-26 02:40:19.000000 FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1110 2023-01-13 23:16:02.000000 FlightRadarAPI-1.3.7/LICENSE
--rw-rw-rw-   0        0        0     3179 2023-06-26 02:40:20.306081 FlightRadarAPI-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     2508 2023-06-26 01:51:29.000000 FlightRadarAPI-1.3.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 02:40:20.308066 FlightRadarAPI-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-05-28 19:59:55.000000 FlightRadarAPI-1.3.7/setup.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/requirements.txt
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/__init__.py
+-rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/api.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/core.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/errors.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/request.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/entities/__init__.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/entities/airport.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/entities/entity.py
+-rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/entities/flight.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/tests/package.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/tests/test_api.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/LICENSE
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/README.md
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/PKG-INFO
```

### Comparing `FlightRadarAPI-1.3.7/FlightRadar24/__init__.py` & `flightradarapi-1.3.8/FlightRadar24/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 See more information at:
 https://www.flightradar24.com/premium/
 https://www.flightradar24.com/terms-and-conditions
 """
 
 __author__ = "Jean Loui Bernard Silva de Jesus"
-__version__ = "1.3.7"
+__version__ = "1.3.8"
 
 from .api import FlightRadar24API, FlightTrackerConfig
 from .entities import Airport, Flight
```

### Comparing `FlightRadarAPI-1.3.7/FlightRadar24/api.py` & `flightradarapi-1.3.8/FlightRadar24/api.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.7/FlightRadar24/core.py` & `flightradarapi-1.3.8/FlightRadar24/core.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.7/FlightRadar24/entities/airport.py` & `flightradarapi-1.3.8/FlightRadar24/entities/airport.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.7/FlightRadar24/entities/entity.py` & `flightradarapi-1.3.8/FlightRadar24/entities/entity.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.7/FlightRadar24/entities/flight.py` & `flightradarapi-1.3.8/FlightRadar24/entities/flight.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.7/FlightRadar24/request.py` & `flightradarapi-1.3.8/FlightRadar24/request.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.7/FlightRadarAPI.egg-info/PKG-INFO` & `flightradarapi-1.3.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: FlightRadarAPI
-Version: 1.3.7
-Summary: API for FlightRadar24
-Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
-Author: Jean Loui Bernard Silva de Jesus
-License: MIT
-Keywords: flightradar24 api
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FlightRadarAPI
 Unofficial API for [FlightRadar24](https://www.flightradar24.com/) written in Python 3.
 
 If you want to use the data collected using this API commercially, you need to subscribe to the [Business plan](https://www.flightradar24.com/premium/).</br>
 See more information at: https://www.flightradar24.com/terms-and-conditions
 
 [![Python Package](https://github.com/JeanExtreme002/FlightRadarAPI/workflows/Python%20Package/badge.svg)](https://github.com/JeanExtreme002/FlightRadarAPI/actions)
```

### Comparing `FlightRadarAPI-1.3.7/LICENSE` & `flightradarapi-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.3.7/PKG-INFO` & `flightradarapi-1.3.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,103 @@
-Metadata-Version: 2.1
-Name: FlightRadarAPI
-Version: 1.3.7
-Summary: API for FlightRadar24
-Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
-Author: Jean Loui Bernard Silva de Jesus
-License: MIT
-Keywords: flightradar24 api
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# FlightRadarAPI
-Unofficial API for [FlightRadar24](https://www.flightradar24.com/) written in Python 3.
-
-If you want to use the data collected using this API commercially, you need to subscribe to the [Business plan](https://www.flightradar24.com/premium/).</br>
-See more information at: https://www.flightradar24.com/terms-and-conditions
-
-[![Python Package](https://github.com/JeanExtreme002/FlightRadarAPI/workflows/Python%20Package/badge.svg)](https://github.com/JeanExtreme002/FlightRadarAPI/actions)
-[![Pypi](https://img.shields.io/pypi/v/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
-[![License](https://img.shields.io/pypi/l/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
-[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/FlightRadarAPI/)
-[![Downloads](https://static.pepy.tech/personalized-badge/flightradarapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pypi.org/project/FlightRadarAPI/)
-
-# Installing FlightRadarAPI:
-```
-pip3 install FlightRadarAPI
-```
-
-# Basic Usage:
-Just create a `FlightRadar24API` object after importing it.
-
-```
-from FlightRadar24 import FlightRadar24API
-fr_api = FlightRadar24API()
-```
-
-**Getting airports list:**
-```
-airports = fr_api.get_airports()
-```
-
-**Getting airlines list:**
-```
-airlines = fr_api.get_airlines()
-```
-
-**Getting flights list:**
-```
-flights = fr_api.get_flights(...)
-```
-
-**Getting zones list:**
-```
-zones = fr_api.get_zones()
-```
-
-You can also get more information about a specific flight such as: aircraft images, estimated time, trail, etc.
-```
-details = fr_api.get_flight_details(flight.id)
-flight.set_flight_details(details)
-
-print("Flying to", flight.destination_airport_name)
-```
-
-# Filtering flights and airports:
-**Getting flights by airline:**
-```
-airline_icao = "AZU"
-thy_flights = fr_api.get_flights(airline = airline_icao)
-```
-
-**Getting flights by bounds:**
-```
-bounds = fr_api.get_bounds(zone)
-flights = fr_api.get_flights(bounds = bounds)
-```
-
-**Getting airport by ICAO or IATA:**
-```
-airport_icao = "VNLK"
-lukla_airport = fr_api.get_airport(airport_icao)
-```
-
-**Getting and configuring Real-time Flight Tracker parameters:**
-```
-config = fr_api.get_flight_tracker_config()
-
-new_config = FlightTrackerConfig(...)
-fr_api.set_flight_tracker_config(new_config, limit = 500, ...)
-```
+Metadata-Version: 2.1
+Name: FlightRadarAPI
+Version: 1.3.8
+Summary: API for FlightRadar24
+Project-URL: Homepage, https://github.com/JeanExtreme002/FlightRadarAPI
+Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: api,flightradar24
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Requires-Dist: brotli
+Requires-Dist: deprecated
+Requires-Dist: requests
+Provides-Extra: tests
+Requires-Dist: pytest; extra == 'tests'
+Description-Content-Type: text/markdown
+
+# FlightRadarAPI
+Unofficial API for [FlightRadar24](https://www.flightradar24.com/) written in Python 3.
+
+If you want to use the data collected using this API commercially, you need to subscribe to the [Business plan](https://www.flightradar24.com/premium/).</br>
+See more information at: https://www.flightradar24.com/terms-and-conditions
+
+[![Python Package](https://github.com/JeanExtreme002/FlightRadarAPI/workflows/Python%20Package/badge.svg)](https://github.com/JeanExtreme002/FlightRadarAPI/actions)
+[![Pypi](https://img.shields.io/pypi/v/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
+[![License](https://img.shields.io/pypi/l/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
+[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/FlightRadarAPI/)
+[![Downloads](https://static.pepy.tech/personalized-badge/flightradarapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pypi.org/project/FlightRadarAPI/)
+
+# Installing FlightRadarAPI:
+```
+pip3 install FlightRadarAPI
+```
+
+# Basic Usage:
+Just create a `FlightRadar24API` object after importing it.
+
+```
+from FlightRadar24 import FlightRadar24API
+fr_api = FlightRadar24API()
+```
+
+**Getting airports list:**
+```
+airports = fr_api.get_airports()
+```
+
+**Getting airlines list:**
+```
+airlines = fr_api.get_airlines()
+```
+
+**Getting flights list:**
+```
+flights = fr_api.get_flights(...)
+```
+
+**Getting zones list:**
+```
+zones = fr_api.get_zones()
+```
+
+You can also get more information about a specific flight such as: aircraft images, estimated time, trail, etc.
+```
+details = fr_api.get_flight_details(flight.id)
+flight.set_flight_details(details)
+
+print("Flying to", flight.destination_airport_name)
+```
+
+# Filtering flights and airports:
+**Getting flights by airline:**
+```
+airline_icao = "AZU"
+thy_flights = fr_api.get_flights(airline = airline_icao)
+```
+
+**Getting flights by bounds:**
+```
+bounds = fr_api.get_bounds(zone)
+flights = fr_api.get_flights(bounds = bounds)
+```
+
+**Getting airport by ICAO or IATA:**
+```
+airport_icao = "VNLK"
+lukla_airport = fr_api.get_airport(airport_icao)
+```
+
+**Getting and configuring Real-time Flight Tracker parameters:**
+```
+config = fr_api.get_flight_tracker_config()
+
+new_config = FlightTrackerConfig(...)
+fr_api.set_flight_tracker_config(new_config, limit = 500, ...)
+```
```

### Comparing `FlightRadarAPI-1.3.7/setup.py` & `flightradarapi-1.3.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,41 @@
-# -*- coding: utf-8 -*-
+[project]
+name = "FlightRadarAPI"
+dynamic = ["version"]
+description = "API for FlightRadar24"
+authors = [
+    { name = "Jean Loui Bernard Silva de Jesus", email = "jeanextreme002@gmail.com" },
+]
+license = "MIT"
+readme = "README.md"
+keywords = ["flightradar24", "api"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
+]
+exclude = ["tests"]
+requires-python = ">=3.7"
+dependencies = [
+  "Brotli",
+  "Deprecated",
+  "requests",
+]
 
-from FlightRadar24 import __version__
-from setuptools import setup, find_packages
+[project.optional-dependencies]
+tests = [
+  "pytest",
+]
 
-with open("README.md") as file:
-    README = file.read()
+[project.urls]
+"Homepage" = "https://github.com/JeanExtreme002/FlightRadarAPI"
 
-setup(
-    name = "FlightRadarAPI",
-    version = __version__,
-    description = "API for FlightRadar24",
-    long_description = README,
-    long_description_content_type = "text/markdown",
-    author = "Jean Loui Bernard Silva de Jesus",
-    url = "https://github.com/JeanExtreme002/FlightRadarAPI",
-    license = "MIT",
-    keywords = "flightradar24 api",
-    packages = find_packages(exclude = ("tests", "docs")),
-    install_requires = ["Brotli", "requests", "Deprecated"],
-    classifiers = [
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11"
-    ]
-)
+[tool.hatch.version]
+path = "FlightRadar24/__init__.py"
+
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
```

