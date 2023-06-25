# Comparing `tmp/sentinel_analysis-0.1.2.tar.gz` & `tmp/sentinel_analysis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentinel_analysis-0.1.2.tar", max compression
+gzip compressed data, was "sentinel_analysis-0.1.3.tar", max compression
```

## Comparing `sentinel_analysis-0.1.2.tar` & `sentinel_analysis-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.2/README.md
--rw-r--r--   0        0        0      643 2023-06-25 16:03:24.260032 sentinel_analysis-0.1.2/pyproject.toml
--rw-r--r--   0        0        0  2426645 2023-06-25 11:58:26.983350 sentinel_analysis-0.1.2/sentinel_analysis/GeoIP_DBs/GeoIP.dat
--rw-r--r--   0        0        0  6025934 2023-06-25 11:58:26.991351 sentinel_analysis-0.1.2/sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat
--rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.2/sentinel_analysis/__init__.py
--rw-r--r--   0        0        0     3670 2023-06-25 11:59:13.928759 sentinel_analysis-0.1.2/sentinel_analysis/alert.py
--rw-r--r--   0        0        0     7140 2023-06-25 16:02:24.386229 sentinel_analysis-0.1.2/sentinel_analysis/main.py
--rw-r--r--   0        0        0      478 2023-06-25 11:58:27.079353 sentinel_analysis-0.1.2/sentinel_analysis/report.py
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 sentinel_analysis-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.3/README.md
+-rw-r--r--   0        0        0      669 2023-06-25 16:20:44.012087 sentinel_analysis-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.3/sentinel_analysis/__init__.py
+-rw-r--r--   0        0        0     3574 2023-06-25 16:10:47.832172 sentinel_analysis-0.1.3/sentinel_analysis/alert.py
+-rw-r--r--   0        0        0     7863 2023-06-25 18:28:36.097690 sentinel_analysis-0.1.3/sentinel_analysis/main.py
+-rw-r--r--   0        0        0      478 2023-06-25 11:58:27.079353 sentinel_analysis-0.1.3/sentinel_analysis/report.py
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 sentinel_analysis-0.1.3/PKG-INFO
```

### Comparing `sentinel_analysis-0.1.2/pyproject.toml` & `sentinel_analysis-0.1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "sentinel-analysis"
-version = "0.1.2"
+version = "0.1.3"
 description = "This tools allows for a user, by means of specified flags, to process a parquet file containing traffic dumps in search for a set of traffic patterns"
 authors = ["David Araújo <david2araujo5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sentinel_analysis"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
 matplotlib = "^3.7.1"
 pygeoip = "^0.3.2"
 dnspython = "^2.3.0"
 pandas = "^2.0.2"
 scipy = "^1.10.1"
+fastparquet = "^2023.4.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `sentinel_analysis-0.1.2/sentinel_analysis/alert.py` & `sentinel_analysis-0.1.3/sentinel_analysis/alert.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,38 +9,36 @@
     BOTNET = "botnet"
     CANDC = "c&c"
     EXFIL = "exfiltration"
     DDOS = "ddos"
 
 
 class Alert:
-    gi = pygeoip.GeoIP("./sentinel_analysis/GeoIP_DBs/GeoIP.dat")
-    gi2 = pygeoip.GeoIP("./sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat")
-
     alertID = 0
 
-    def __init__(self, addr, type):
+    def __init__(self, addr, type, gi, gi2):
         """Alert
 
         Args:
             timestamp           (datetime)      : estimated time of the beginning
             addr                (str)           : IP address
             port                (int)           : destination port
             type                (Type or str)   : type of attack detected
             proto               (str)           : transport protocol
         """
         self.id = Alert.alertID
         Alert.alertID += 1
+        self.gi, self.gi2 = gi, gi2
         self.addr = addr
         self.type = type if isinstance(type, AlertType) else AlertType(type)
 
     def resolveLocation(self):
         try:
-            cc = Alert.gi.country_code_by_addr(self.addr)
-            org = Alert.gi2.org_by_addr(self.addr)
+            cc = self.gi.country_code_by_addr(self.addr)
+            org = self.gi2.org_by_addr(self.addr)
             self.location = (cc, org)
         except Exception as e:
             self.location = "unknown"
         return self.location
 
     def resolveDNSName(self):
         try:
```

### Comparing `sentinel_analysis-0.1.2/sentinel_analysis/main.py` & `sentinel_analysis-0.1.3/sentinel_analysis/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,51 +9,49 @@
 import pygeoip
 from . import report
 from .alert import BotnetAlert, ExfiltrationAlert
 from scipy.stats import norm
 
 alerts = {}
 
+
 def printq(*args):
     if not arguments.quiet:
         print(*args)
 
 
 def dataExfiltration(percentage):
     printq(
         f"[!] IPs above the {percentage} percentile of the downloads over uploads in this session.\n"
     )
 
-    percentage = int(percentage)
+    percentage = 1 - (int(percentage) / 100)
 
     # Calculate the total downloaded and uploaded bytes per IP
     ratios = data.groupby(["src_ip"], as_index=False)[["down_bytes", "up_bytes"]].sum()
 
     # Calculate the ratio between downloaded and uploaded bytes
-    ratios["ratio"] = ratios[["down_bytes", "up_bytes"]].mean(axis=1)
-
-    # Calculate the z-score for the ratio
-    ratios["z_score"] = (ratios["ratio"] - ratios["ratio"].mean()) / ratios[
-        "ratio"
-    ].std()
+    ratios["ratio"] = ratios["down_bytes"] / ratios["up_bytes"]
 
-    # Calculate the z-score threshold based on the desired percentage
-    z_score_threshold = math.ceil((norm.ppf(percentage / 100)))
+    # Sort be ratio
+    ratios = ratios.sort_values(["ratio"], ascending=False)
 
-    # Outlier traffic. Above the average percentage defined by user
-    outliers = ratios[ratios["z_score"] > z_score_threshold]
+    # Top outliers base on percentage
+    outliers = ratios.head(int(len(ratios) * percentage))
 
-    printq(outliers.sort_values(["ratio"], ascending=False))
+    printq(outliers)
 
     for (
         _,
         row,
     ) in outliers.iterrows():
         alerts.setdefault("exfiltrations", []).append(
             ExfiltrationAlert(
+                gi=gi,
+                gi2=gi2,
                 down_byte=row.down_bytes,
                 up_byte=row.up_bytes,
                 percentage=percentage,
                 addr=row.src_ip,
             )
         )
 
@@ -101,126 +99,150 @@
 
     for (
         _,
         row,
     ) in same_subnet.iterrows():
         alerts.setdefault("botnet", []).append(
             BotnetAlert(
+                gi=gi,
+                gi2=gi2,
                 subnet=str(subnet),
                 peers=row.src_ip,
                 frequency=row.frequency,
                 addr=row.dst_ip,
             )
         )
 
 
 def countryVolume():
     printq(
         f"[!] Calculate the country of origin of the destion IPs and the connection volume for each country. Generating a PNG with the bar graph.\n"
     )
 
-    gi = pygeoip.GeoIP("./sentinel/GeoIP_DBs/GeoIP.dat")
-
     # Analyse of destination countries connection volume
     countries = data
     countries["country"] = countries["dst_ip"].apply(
         lambda ip: gi.country_code_by_addr(ip)
     )
-    volume = (
-        countries.groupby(["country"])["dst_ip"].count().sort_values(ascending=False)
+
+    # Associates each country with it's number of connection 
+    # and the total data downloads by it. For normal flows
+    # they should be directly proportional
+    volume = countries.groupby(["country"]).agg(
+        {"dst_ip": ["count"], "down_bytes": ["sum"]}
     )
+    
+    # Sorting the DataFrame by dst_ip column in descending order
+    volume = volume.sort_values(("dst_ip", "count"), ascending=False)
 
     printq(volume)
-
+    
     # Generates bar chart image
     countries = [x if x != "" else "Unknown" for x in volume.index]
-    fig, ax = plt.subplots(figsize=(15, 6))
-    ax.barh(countries, volume.values)
-    ax.set_xlabel("Country")
-    ax.set_ylabel("Number of connection")
-
-    for i, v in enumerate(volume):
-        ax.text(v, i, str(v), va="center")
+    connections = [x[0] for x in volume['dst_ip'].values]
 
-    ax.set_title("Number of connection per country")
+    fig, ax = plt.subplots(figsize=(15, 10))
+    bar_width = 0.4  # Adjust this value to change the width of each bar
 
-    filepath = "volumexcountry"
-    fig.savefig(fname=filepath)
+    # Plotting the bars for connections
+    ax.barh(countries, connections, bar_width, align="edge", label='Connections')
+    ax.set_xlabel("Number of Connections")
+    ax.set_ylabel("Country")
+    
+    # Adding labels to the bars
+    for i, conn in enumerate(connections):
+        ax.text(conn, i, str(conn), va="center")
+    ax.set_title("Number of Connections per Country")
 
+    filepath = "connectionsxcountry.png"  # Specify the desired image filename
+    fig.savefig(filepath)
+    
     return f"""
 # Connection volume by country
 
 The correlation between connection volume and country of destination can be viewed in the graphic bellow.
 
 ![Volumebycountry]({filepath}.png)
 
 """
 
+
 def trafficDistribution():
-    traffic = data    
-    traffic['hour'] = pd.to_datetime(traffic['timestamp'] / 100.0, unit='s').dt.hour
-    hourly = traffic['hour'].value_counts().sort_index()
+    traffic = data
+    traffic["hour"] = pd.to_datetime(traffic["timestamp"] / 100.0, unit="s").dt.hour
+    hourly = traffic["hour"].value_counts().sort_index()
     fig, ax = plt.subplots(figsize=(10, 6))
-    ax.bar(hourly.index,hourly.values)
+    ax.bar(hourly.index, hourly.values)
     ax.set_xlabel("Hours")
     ax.set_ylabel("Number of connections")
     ax.set_title("Connections per hour during a day")
     ax.set_xticks(range(24))
-    
+
     filepath = "connectionsxhour"
     fig.savefig(fname=filepath)
 
     printq(hourly)
 
     return f"""
 # Connection volume per hour
 
 This graph ilustrates the number of connection per hour during a day
 
 ![Connectionsperhout]({filepath}.png)
 
 """
-    
-    
+
+
 def main():
     global data
     data = pd.read_parquet(arguments.data)
 
+    global gi, gi2
+    gi = pygeoip.GeoIP(arguments.gi)
+    gi2 = pygeoip.GeoIP(arguments.gin)
+
     intro = f"""# Sentinel traffic report
 
 This report was automatically generated at **{str(datetime.datetime.utcnow())}** by the **Sentinel** service.
 """
 
     # Clean operations
     operations = dict(arguments._get_kwargs())
     del operations["data"]
+    del operations["gi"]
+    del operations["gin"]
     del operations["quiet"]
     del operations["pdf"]
 
     for key, value in list(operations.items()):
         if value:
-            value = f'"{value}"' if value and value != True else ''            
+            value = f'"{value}"' if value and value != True else ""
             func = f"{key}({value})"
             printq()
             r = eval(func)
             if r:
                 intro += r
 
     # Print results to pdf
     if dict(arguments._get_kwargs())["pdf"]:
         report.printReport(alerts, intro)
 
 
-
 def cli():
     parser = argparse.ArgumentParser(description="Traffic analysis tool.")
     parser.add_argument(
         "--data", type=str, help="Path to datafile to analyze", required=True
     )
 
+    parser.add_argument("-gi", type=str, help="Geolocation IP database", required=True)
+
+    parser.add_argument(
+        "-gin", type=str, help="Geolocation IP database with nameserver", required=True
+    )
+
     parser.add_argument(
         "-dx",
         "--dataExfiltration",
         type=int,
         help="Threshold percentage for outliers in upload/download byte amount",
     )
```

### Comparing `sentinel_analysis-0.1.2/PKG-INFO` & `sentinel_analysis-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: sentinel-analysis
-Version: 0.1.2
+Version: 0.1.3
 Summary: This tools allows for a user, by means of specified flags, to process a parquet file containing traffic dumps in search for a set of traffic patterns
 Author: David Araújo
 Author-email: david2araujo5@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dnspython (>=2.3.0,<3.0.0)
+Requires-Dist: fastparquet (>=2023.4.0,<2024.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pygeoip (>=0.3.2,<0.4.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
```

