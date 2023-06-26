# Comparing `tmp/ipmap-1.1.0.tar.gz` & `tmp/ipmap-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipmap-1.1.0.tar", max compression
+gzip compressed data, was "ipmap-1.2.0.tar", max compression
```

## Comparing `ipmap-1.1.0.tar` & `ipmap-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1500 2023-06-08 23:34:29.022267 ipmap-1.1.0/LICENSE
--rw-r--r--   0        0        0     5274 2023-06-08 23:34:29.026267 ipmap-1.1.0/README.md
--rw-r--r--   0        0        0     1508 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/__init__.py
--rw-r--r--   0        0        0     4441 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/config.py
--rw-r--r--   0        0        0      735 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/data/settings.json
--rw-r--r--   0        0        0     2215 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/data/templates/map.html
--rw-r--r--   0        0        0     4699 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/ipmap.py
--rw-r--r--   0        0        0     1036 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/main.py
--rw-r--r--   0        0        0     2263 2023-06-08 23:34:29.026267 ipmap-1.1.0/ipmap/utils.py
--rw-r--r--   0        0        0      904 2023-06-08 23:34:29.026267 ipmap-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6200 1970-01-01 00:00:00.000000 ipmap-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1500 2023-06-26 00:49:05.041066 ipmap-1.2.0/LICENSE
+-rw-r--r--   0        0        0     6146 2023-06-26 00:49:05.041066 ipmap-1.2.0/README.md
+-rw-r--r--   0        0        0     1508 2023-06-26 00:49:05.041066 ipmap-1.2.0/ipmap/__init__.py
+-rw-r--r--   0        0        0     3880 2023-06-26 00:49:05.041066 ipmap-1.2.0/ipmap/config.py
+-rw-r--r--   0        0        0      506 2023-06-26 00:49:05.041066 ipmap-1.2.0/ipmap/data/settings.json
+-rw-r--r--   0        0        0     2215 2023-06-26 00:49:05.041066 ipmap-1.2.0/ipmap/data/templates/map.html
+-rw-r--r--   0        0        0     4670 2023-06-26 00:49:05.041066 ipmap-1.2.0/ipmap/ipmap.py
+-rw-r--r--   0        0        0      986 2023-06-26 00:49:05.041066 ipmap-1.2.0/ipmap/main.py
+-rw-r--r--   0        0        0     2426 2023-06-26 00:49:05.041066 ipmap-1.2.0/ipmap/utils.py
+-rw-r--r--   0        0        0      904 2023-06-26 00:49:05.041066 ipmap-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7072 1970-01-01 00:00:00.000000 ipmap-1.2.0/PKG-INFO
```

### Comparing `ipmap-1.1.0/LICENSE` & `ipmap-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipmap-1.1.0/ipmap/__init__.py` & `ipmap-1.2.0/ipmap/__init__.py`

 * *Files identical despite different names*

### Comparing `ipmap-1.1.0/ipmap/config.py` & `ipmap-1.2.0/ipmap/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,38 +12,19 @@
         self.patch = settings()["program"]["version"]["patch"]
         self.suffix = settings()["program"]["version"]["suffix"]
 
     def full_version(self) -> str:
         """
         Returns the full version string composed of the version components.
 
-        :return: The complete version string in the format "major.minor.patch.suffix".
+        :return: The complete version string in the format "major.minor.patchsuffix".
         """
         return f"{self.major}.{self.minor}.{self.patch}{self.suffix}"
 
 
-class Colours:
-    def __init__(self):
-        self.RED = self.get_colour("RED")
-        self.WHITE = self.get_colour("WHITE")
-        self.GREEN = self.get_colour("GREEN")
-        self.YELLOW = self.get_colour("YELLOW")
-        self.RESET = self.get_colour("RESET")
-
-    @staticmethod
-    def get_colour(colour_name: str) -> str:
-        """
-        Retrieves the value of the specified colour from the settings.
-
-        :param: colour_name (str): The name of the colour to retrieve.
-        :return: The value of the specified colour.
-        """
-        return settings()["colours"][colour_name]
-
-
 def settings() -> dict:
     """
     Loads the program's settings from /data/settings.json
 
     :return: Dictionary (JSON) containing program settings
     """
     # Get the absolute path of the current file
@@ -107,35 +88,32 @@
     return table
 
 
 def usage():
     return """
     Geolocate IP Address(es) (with an interactive map)
     --------------------------------------------------
-    ipmap map --ip <ip>
+    ipmap <ip> --map
 
     Open Google Earth on the given coordinates
     --------------------------------------------
-    ipmap earth --ip <ip>
+    ipmap <ip> --earth
 
     Lookup IP Address(es) (same as map but without an interactive map)
     ------------------------------------------------------------------
-    ipmap lookup --ip <ip>
-
-
-modes:
-    map - creates an interactive map and pin points the locations of the specified ip address(es) on it.
-    earth - opens google earth on the location of the given ip address.
-    lookup - looks up the specified ip address(es)' information.
+    ipmap <ip> --lookup
     """
 
 
 def create_parser():
     parser = argparse.ArgumentParser(description=f"{settings()['program']['name']}" 
                                                  f" — by {settings()['program']['developer']['name']}" 
                                                  f" ({settings()['program']['developer']['about']})",
                                      epilog=settings()['program']['about'], usage=usage())
-    parser.add_argument("mode", help="init mode", choices=["earth", "lookup", "map"])
-    parser.add_argument("-i", "--ip", help="ip")
+    parser.add_argument("ip", help="target ip address")
+    parser.add_argument("-e", "--earth", help="Open Google Earth on the location of a given ip", action="store_true")
+    parser.add_argument("-l", "--lookup", help="Lookup an ip (like --map, but without an interactive map)",
+                        action="store_true")
+    parser.add_argument("-m", "--map", help="Geolocate an ip (with an interactive map)", action="store_true")
     parser.add_argument("-o", "--output", help="map output name (default %(default)s)", default="ipmap")
     parser.add_argument("-v", "--version", action="version", version=Version().full_version())
     return parser
```

### Comparing `ipmap-1.1.0/ipmap/data/templates/map.html` & `ipmap-1.2.0/ipmap/data/templates/map.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 <!DOCTYPE html>
 <html>
   <head>
     <title>{}</title>
     <meta charset="utf-8" />
-    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.3/dist/leaflet.css"/>
+    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"/>
     <style>
       body {{
         padding: 0;
         margin: 0;
       }}
       html, body, #map {{
         height: 100%;
         width: 100%;
       }}
     </style>
   </head>
   <body>
     <div id="map"></div>
 
-    <script src="https://unpkg.com/leaflet@1.9.3/dist/leaflet.js"></script>
+    <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
 
     <script>
         var popup = L.popup();
         var coordinates = {};
 
         var map = L.map('map').setView([0, 0], 2);
         mapLink =
```

### Comparing `ipmap-1.1.0/ipmap/ipmap.py` & `ipmap-1.2.0/ipmap/ipmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 import webbrowser
 from rich import print as xprint
 from ipmap.utils import send_request
-from ipmap.config import Colours, create_ip_table
-
-colour = Colours()
+from ipmap.config import create_ip_table
 
 
 def get_ip_data(ip_address: str) -> list:
     """
     Gets the geolocation information of given IP Addresses.
 
     :param ip_address: IP Addresses to look up
```

### Comparing `ipmap-1.1.0/ipmap/main.py` & `ipmap-1.2.0/ipmap/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 def run():
     clear_screen()
     xprint(f"Starting {settings()['program']['name']} v{Version().full_version()} at {time.asctime()}")
     path_finder(["maps"])
     check_updates()
     try:
-        if args.mode == "earth":
-            open_google_earth(get_ip_data(args.ip))
-        elif args.mode == "lookup":
-            get_ip_data(args.ip)
-        elif args.mode == "map":
-            generated_map = create_map(get_ip_data(args.ip), format_map_name(args.output))
-            xprint(f"Opening map: {generated_map}")
-            webbrowser.open(generated_map)
+        if args:
+            if args.earth:
+                open_google_earth(get_ip_data(args.ip))
+            if args.lookup:
+                get_ip_data(args.ip)
+            if args.map:
+                generated_map = create_map(get_ip_data(args.ip), format_map_name(args.output))
+                xprint(f"Opening map: {generated_map}")
+                webbrowser.open(generated_map)
     except KeyboardInterrupt:
-        xprint(f"\nUser interruption detected ({colour.YELLOW}Ctrl+C{colour.RESET}).")
-    except Exception as error:
-        xprint(f"Error: {colour.RED}{error}{colour.RESET}")
-
+        xprint("\nUser interruption detected (Ctrl+C).")
+    except Exception as e:
+        xprint(f"Error: {e}")
```

### Comparing `ipmap-1.1.0/ipmap/utils.py` & `ipmap-1.2.0/ipmap/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import os
 import subprocess
-import urllib.request
 from rich import print as xprint
+from urllib.request import urlopen
 from rich.markdown import Markdown
 from ipmap.config import json, Version
+from urllib.error import HTTPError, URLError
 
 
 def send_request(endpoint) -> dict:
     """
     Sends a GET request to the specified endpoint and returns JSON
 
     :param endpoint: url endpoint to send request to
     :return: Dictionary response (JSON)
     """
-    with urllib.request.urlopen(endpoint) as response:
-        response_data = json.loads(response.read().decode())
-    return response_data
+    try:
+        with urlopen(endpoint) as response:
+            response_data = json.loads(response.read().decode())
+        return response_data
+    except (URLError, HTTPError) as error:
+        xprint(f"Error: {error}")
 
 
 # Check program updates
 def check_updates() -> None:
     """
     Checks for latest updates by retrieving the release tag from the releases page of the program from GitHub
     Then compares the remote version tag with the tag in the program.
@@ -57,10 +61,10 @@
 
 
 def clear_screen() -> None:
     """
     Clear the terminal screen/
     If Operating system is Windows, uses the 'cls' command. Otherwise, uses the 'clear' command
 
-    :return: None
+    :return: Uhh a cleared screen? haha
     """
     subprocess.call("cmd.exe /c cls" if os.name == "nt" else "clear")
```

### Comparing `ipmap-1.1.0/pyproject.toml` & `ipmap-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 include = [
     {path = "ipmap/data/templates/map.html"},
     {path = "ipmap/data/settings.json"}
 ]
 name = "ipmap"
-version = "1.1.0"
+version = "1.2.0"
 description = "A cross-platform easy-to-use ip geolocation & mapping tool."
 authors = ["Richard Mwewa <rly0nheart@duck.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://github.com/rly0nheart/ipmap"
 repository = "https://github.com/rly0nheart/ipmap"
 keywords = ["mapping", "geolocation", "ip-address-geolocation", "ip-address-lookup", "ip-mapping"]
```

