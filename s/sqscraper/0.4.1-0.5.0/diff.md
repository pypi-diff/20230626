# Comparing `tmp/sqscraper-0.4.1.tar.gz` & `tmp/sqscraper-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqscraper-0.4.1.tar", last modified: Thu Jun 22 23:15:28 2023, max compression
+gzip compressed data, was "sqscraper-0.5.0.tar", last modified: Mon Jun 26 20:10:38 2023, max compression
```

## Comparing `sqscraper-0.4.1.tar` & `sqscraper-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 23:15:28.391802 sqscraper-0.4.1/
--rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     2312 2023-06-22 23:15:28.389803 sqscraper-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.4.1/README.md
--rw-rw-rw-   0        0        0     1989 2023-06-22 23:14:09.000000 sqscraper-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 23:15:28.391802 sqscraper-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 23:15:28.222716 sqscraper-0.4.1/sqscraper/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.4.1/sqscraper/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.4.1/sqscraper/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:15:28.343213 sqscraper-0.4.1/sqscraper/cnbc/
--rw-rw-rw-   0        0        0       84 2023-06-21 17:43:19.000000 sqscraper-0.4.1/sqscraper/cnbc/__init__.py
--rw-rw-rw-   0        0        0      931 2023-06-20 22:50:22.000000 sqscraper-0.4.1/sqscraper/cnbc/_apps.py
--rw-rw-rw-   0        0        0    12837 2023-06-22 23:13:54.000000 sqscraper-0.4.1/sqscraper/cnbc/_serializer.py
--rw-rw-rw-   0        0        0    13041 2023-06-22 23:13:54.000000 sqscraper-0.4.1/sqscraper/cnbc/quote_page.py
--rw-rw-rw-   0        0        0    15339 2023-06-22 23:13:54.000000 sqscraper-0.4.1/sqscraper/cnbc/summary.py
--rw-rw-rw-   0        0        0      592 2023-06-22 05:52:27.000000 sqscraper-0.4.1/sqscraper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:15:28.233355 sqscraper-0.4.1/sqscraper.egg-info/
--rw-rw-rw-   0        0        0     2312 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      483 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 20:10:38.641201 sqscraper-0.5.0/
+-rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2312 2023-06-26 20:10:38.640201 sqscraper-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.5.0/README.md
+-rw-rw-rw-   0        0        0     1989 2023-06-26 20:09:25.000000 sqscraper-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:10:38.641201 sqscraper-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 20:10:38.422496 sqscraper-0.5.0/sqscraper/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.5.0/sqscraper/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.5.0/sqscraper/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:10:38.591949 sqscraper-0.5.0/sqscraper/cnbc/
+-rw-rw-rw-   0        0        0      117 2023-06-26 20:09:10.000000 sqscraper-0.5.0/sqscraper/cnbc/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-06-20 22:50:22.000000 sqscraper-0.5.0/sqscraper/cnbc/_apps.py
+-rw-rw-rw-   0        0        0    12837 2023-06-22 23:17:14.000000 sqscraper-0.5.0/sqscraper/cnbc/_serializer.py
+-rw-rw-rw-   0        0        0    17770 2023-06-26 20:09:10.000000 sqscraper-0.5.0/sqscraper/cnbc/charts.py
+-rw-rw-rw-   0        0        0    13041 2023-06-22 23:17:14.000000 sqscraper-0.5.0/sqscraper/cnbc/quote_page.py
+-rw-rw-rw-   0        0        0    15205 2023-06-26 20:09:10.000000 sqscraper-0.5.0/sqscraper/cnbc/summary.py
+-rw-rw-rw-   0        0        0      739 2023-06-26 20:09:10.000000 sqscraper-0.5.0/sqscraper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:10:38.469369 sqscraper-0.5.0/sqscraper.egg-info/
+-rw-rw-rw-   0        0        0     2312 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      483 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 20:10:38.000000 sqscraper-0.5.0/sqscraper.egg-info/top_level.txt
```

### Comparing `sqscraper-0.4.1/LICENSE` & `sqscraper-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqscraper-0.4.1/PKG-INFO` & `sqscraper-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.4.1
+Version: 0.5.0
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqscraper-0.4.1/pyproject.toml` & `sqscraper-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqscraper"
-version = "0.4.1"
+version = "0.5.0"
 description = "API wrapper and web scraper for select stock quote websites."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Financial and Insurance Industry",
```

### Comparing `sqscraper-0.4.1/sqscraper/cnbc/_apps.py` & `sqscraper-0.5.0/sqscraper/cnbc/_apps.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.4.1/sqscraper/cnbc/_serializer.py` & `sqscraper-0.5.0/sqscraper/cnbc/_serializer.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.4.1/sqscraper/cnbc/quote_page.py` & `sqscraper-0.5.0/sqscraper/cnbc/quote_page.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.4.1/sqscraper/cnbc/summary.py` & `sqscraper-0.5.0/sqscraper/cnbc/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 
 class _PricingMomentum(PageSection):
     """
     :param symbol:
     :param soup:
     """
-    _url = "https://apps.cnbc.com/resources/asp/getBufferedChart.asp"
+    _post_url = "https://apps.cnbc.com/resources/asp/getBufferedChart.asp"
 
     def __init__(self, symbol: str, soup: bs4.BeautifulSoup):
         super().__init__(symbol, soup)
 
     @property
     def quote(self) -> pd.Series:
         """
@@ -214,29 +214,24 @@
         :param sma:
         :return:
         """
         regex = re.compile(r"^setPerformanceChartImg\('(.*)'\);$")
 
         params = {
             "symbol": f"{self.wsod_issue_symbol},spx" if spx else self.wsod_issue_symbol,
-            "timeFrame": 365,
-            "width": 600,
-            "height": 120,
+            "timeFrame": 365, "width": 600, "height": 120,
             "indicators": ",".join(f"sma:{x}" for x in sma)
         }
         data = {
-            "params": "&".join(f"{k}={v}" for k, v in params.items()),
-            "cht": "performance",
-            "callback": "setPerformanceChartImg",
-            "returnVars": "File.Name",
-            "..contenttype..": "text/javascript",
-            "..requester..": "ContentBuffer"
+            "params": "&".join(f"{k}={v}" for k, v in params.items()), "cht": "performance",
+            "callback": "setPerformanceChartImg", "returnVars": "File.Name",
+            "..contenttype..": "text/javascript", "..requester..": "ContentBuffer"
         }
 
-        with requests.post(self._url, data=data, timeout=100) as response:
+        with requests.post(self._post_url, data=data, timeout=100) as response:
             return f"https://apps.cnbc.com{regex.search(response.text).group(1)}"
 
 
 class _GrowthRates(PageSection):
     """
     """
     def __init__(self, symbol: str, soup: bs4.BeautifulSoup):
@@ -298,15 +293,15 @@
             lambda x: float(normalize_value(x)) if isinstance(x, str) else np.nan
         )
         dataframe.iloc[3, :] = pd.Series(dataframe.iloc[3, :], dtype="Int64")
 
         return dataframe
     
     @property
-    def javascript(self) -> str:
+    def _javascript(self) -> str:
         """
         """
         for element in self._soup.select(
             "div#category > div.subsection > script[type='text/javascript']"
         ):
             if re.search(r"j1=\[\];.*var growthData=j1;", element.text) is not None:
                 return element.text.strip()
@@ -322,15 +317,15 @@
             re.compile(r"^j1\[\d\]=\{\}$"),
             re.compile(r"^j1\[(\d)\]\.name=(.*?)$"),
             re.compile(r"^j1\[(\d)\]\.prefix=(.*?)$"),
             re.compile(r"^j1\[(\d)\]\.years=\[\]$"),
             re.compile(r"^j1\[(\d)\]\.years\[\d\]=\{\}$"),
             re.compile(r"^j1\[(\d)\]\.years\[(\d)\]\.(.*?)=(.*?)$")
         ]
-        for statement in self.javascript.split(";"):
+        for statement in self._javascript.split(";"):
             results = [r.search(statement) for r in regex]
             nonnull_results = [(i, x) for i, x in enumerate(results) if x is not None]
             if len(nonnull_results) != 1:
                 continue
             idx, res = nonnull_results[0]
 
             if idx == 0:
@@ -356,29 +351,26 @@
                 pd.DataFrame({int(x["FiscalYear"]): x for x in record["years"]})
             )
             if dataframes[i].empty:
                 continue
             
             dataframes[i].drop(index=["FiscalYear"], inplace=True)
             dataframes[i].index = [
-                "Growth Rate",
-                "Growth",
-                "Mean Estimate",
-                "Number of Estimates",
+                "Growth Rate", "Growth", "Mean Estimate", "Number of Estimates",
                 "Industry Growth Rate"
             ]
             dataframes[i].replace("--", np.nan, inplace=True)
             
         return dataframes
 
 
 class _KeyMeasures(PageSection):
     """
     """
-    _url = "https://apps.cnbc.com/resources/asp/getKeyMeasuresBuffer.asp"
+    _post_url = "https://apps.cnbc.com/resources/asp/getKeyMeasuresBuffer.asp"
 
     def __init__(self, symbol: str, soup: bs4.BeautifulSoup):
         super().__init__(symbol, soup)
 
         self._dataframes = self._scrape_table_data()
 
     @property
@@ -426,49 +418,45 @@
         dataframe.iloc[1:, :] = dataframe.iloc[1:, :].applymap(
             lambda x: float(normalize_value(x)) if isinstance(x, str) else np.nan
         )
 
         return dataframe
     
     @property
-    def issue_type(self) -> str:
+    def _issue_type(self) -> str:
         """
         """
         return re.search(r"var issueType = \"(.*?)\";", str(self._soup)).group(1)
     
     @property
-    def wsid(self) -> str:
+    def _wsid(self) -> str:
         """
         """
         return re.search(r"var wsid = \"(.*?)\";", str(self._soup)).group(1)
     
     @property
-    def wsod_company(self) -> str:
+    def _wsod_company(self) -> str:
         """
         """
         return re.search(r"var wsodCompany = \"(.*?)\";", str(self._soup)).group(1)
 
     def _scrape_table_data(self) -> typing.List[pd.DataFrame]:
         """
         :return:
         """
         tab_view = {
-          "title": "Show All",
-          "value": "*",
-          "issueType": self.issue_type,
-          "symbol": self.wsid,
-          "wsodCompany": self.wsod_company
+          "title": "Show All", "value": "*", "issueType": self._issue_type, "symbol": self._wsid,
+          "wsodCompany": self._wsod_company
         }
         data = {
-            "data": Serializer().seralize(tab_view),
-            "..contenttype..": "text/html",
+            "data": Serializer().seralize(tab_view), "..contenttype..": "text/html",
             "..requester..": "ContentBuffer"
         }
 
-        with requests.post(self._url, data, timeout=100) as response:
+        with requests.post(self._post_url, data, timeout=100) as response:
             json_data = response.json()
 
         columns = [x["title"] for x in json_data["columns"]]
         columns[columns.index("S&amp;P 500")] = "S&P 500"
 
         dataframes = []
         for section in json_data["sections"]:
```

### Comparing `sqscraper-0.4.1/sqscraper.egg-info/PKG-INFO` & `sqscraper-0.5.0/sqscraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.4.1
+Version: 0.5.0
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

