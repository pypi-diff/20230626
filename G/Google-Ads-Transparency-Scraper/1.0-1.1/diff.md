# Comparing `tmp/Google Ads Transparency Scraper-1.0.tar.gz` & `tmp/Google Ads Transparency Scraper-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Google Ads Transparency Scraper-1.0.tar", last modified: Mon Jun 26 05:41:34 2023, max compression
+gzip compressed data, was "Google Ads Transparency Scraper-1.1.tar", last modified: Mon Jun 26 11:24:49 2023, max compression
```

## Comparing `Google Ads Transparency Scraper-1.0.tar` & `Google Ads Transparency Scraper-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 05:41:34.638880 Google Ads Transparency Scraper-1.0/
-drwxrwxrwx   0        0        0        0 2023-06-26 05:41:34.628000 Google Ads Transparency Scraper-1.0/GoogleAdsTransparency/
--rw-rw-rw-   0        0        0       50 2023-06-26 05:30:53.000000 Google Ads Transparency Scraper-1.0/GoogleAdsTransparency/__init__.py
--rw-rw-rw-   0        0        0     8302 2023-06-26 00:31:39.000000 Google Ads Transparency Scraper-1.0/GoogleAdsTransparency/main.py
-drwxrwxrwx   0        0        0        0 2023-06-26 05:41:34.637879 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/
--rw-rw-rw-   0        0        0      849 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      849 2023-06-26 05:41:34.638880 Google Ads Transparency Scraper-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-06-26 05:37:43.000000 Google Ads Transparency Scraper-1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-06-26 05:41:34.640874 Google Ads Transparency Scraper-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-06-26 05:34:58.000000 Google Ads Transparency Scraper-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:24:49.886142 Google Ads Transparency Scraper-1.1/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:24:49.822079 Google Ads Transparency Scraper-1.1/GoogleAdsTransparency/
+-rw-rw-rw-   0        0        0       48 2023-06-26 11:13:29.000000 Google Ads Transparency Scraper-1.1/GoogleAdsTransparency/__init__.py
+-rw-rw-rw-   0        0        0     9845 2023-06-26 11:22:33.000000 Google Ads Transparency Scraper-1.1/GoogleAdsTransparency/main.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:24:49.886142 Google Ads Transparency Scraper-1.1/Google_Ads_Transparency_Scraper.egg-info/
+-rw-rw-rw-   0        0        0      849 2023-06-26 11:24:49.000000 Google Ads Transparency Scraper-1.1/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-06-26 11:24:49.000000 Google Ads Transparency Scraper-1.1/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 11:24:49.000000 Google Ads Transparency Scraper-1.1/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-26 11:24:49.000000 Google Ads Transparency Scraper-1.1/Google_Ads_Transparency_Scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-26 11:24:49.000000 Google Ads Transparency Scraper-1.1/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      849 2023-06-26 11:24:49.890153 Google Ads Transparency Scraper-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-06-26 11:23:38.000000 Google Ads Transparency Scraper-1.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-26 11:24:49.892862 Google Ads Transparency Scraper-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-06-26 11:23:04.000000 Google Ads Transparency Scraper-1.1/setup.py
```

### Comparing `Google Ads Transparency Scraper-1.0/GoogleAdsTransparency/main.py` & `Google Ads Transparency Scraper-1.1/GoogleAdsTransparency/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import requests
+from typing import Union
 from bs4 import BeautifulSoup as soap
 
 headers = {
     'authority': 'adstransparency.google.com',
     'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
     'accept-language': 'en-US,en;q=0.9',
     'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
@@ -26,104 +27,124 @@
 class GoogleAds:
     def __init__(self,  headers):
         self.reqs = requests.Session()
         self.headers = headers
         self.get_cookies()
 
     def get_cookies(self):
+        """Get Cookies from the main url https://adstransparency.google.com/ and store them in requests Session"""
         params = {
             'region': 'anywhere',
         }
         self.reqs.get('https://adstransparency.google.com/', params=params, headers=headers)#.text.replace("\/","")
         #response = str(response[response.find("tfaaReportAppInfo"):]).encode('utf8').decode('unicode_escape')
         #print(json.loads(response[response.find("["):response.find(']')+1]))
 
     def refresh_session(self):
+        """Refresh Session cookies"""
         self.reqs = requests.Session()
         self.get_cookies()
 
-    def get_all_search_suggestions(self, keyword):
+    def get_all_search_suggestions(self, keyword: str) -> list :
+        """
+            Gets All suggestions from the Google Ads Transparency for given keyword.
+            Returns list of Suggestions along with their details
+            Returns Empty list [] if no suggestion found"""
         data = {
             'f.req': '{"1":"' + keyword + '","2":10,"3":10}',
         }
         response = self.reqs.post(
             'https://adstransparency.google.com/anji/_/rpc/SearchService/SearchSuggestions',
             params={'authuser': '0'},
             data=data,
         )
         suggestions = response.json()["1"]
         if suggestions:    
             return suggestions
         return []
 
-    def get_first_search_suggestion(self, keyword):
+    def get_first_search_suggestion(self, keyword: str) -> Union[dict,None]:
+        """
+           Gets First Suggestions from the Google Ads Transparency for given keyword.
+           Returns dict of Suggestion details
+           Returns None if no suggestion found"""
+        
         if suggestions := self.get_all_search_suggestions(keyword):
             return suggestions[0]
-        return []
+        return None
 
-    def get_advistisor_by_domain(self, domain):
+    def get_advistisor_by_domain(self, domain: str)-> Union[dict,None]:
+        """
+            Makes search of domain/url and returns the Company Name and It's Advertisor Id 
+        """
         data = {
             "f.req": '{"2":40,"3":{"12":{"1":"' + domain + '"}}}'
         }
         response = self.reqs.post(
             'https://adstransparency.google.com/anji/_/rpc/SearchService/SearchCreatives',
             params={'authuser': ''},
             data=data,
         )
         response = response.json().get("1")
         if response:
             ad = response[0]
             return {"Advertisor Id": ad["1"], "Name":ad["12"]}
-        return {}
+        return None
         """if ads := response.json().get("1"):
             with open("new.json", "w") as f:
                 json.dump(ads, f)
             return [{"Advertisor Id": ad[1],"Creative Id":ad["2"]} for ad in ads]
         return []"""
 
-    def creative_search_by_advertiser_id(self, advertiser_id):
+    def creative_search_by_advertiser_id(self, advertiser_id: str) -> list: #TODO do region search
+        """Get Creatives or ads by quering given Advertisor Id
+        If no Ad found return []"""
         data = {
             'f.req': '{"2":40,"3":{"12":{"1":"","2":true},"13":{"1":["' + advertiser_id + '"]}}, "7":{"1":1}}',
         }
         response = self.reqs.post(
             'https://adstransparency.google.com/anji/_/rpc/SearchService/SearchCreatives',
             params={'authuser': ''},
             data=data,
         )
         if ads := response.json().get("1"):
             return [ad["2"] for ad in ads]
         return []
 
-    def get_creative_Ids(self, keyword):
+    def get_creative_Ids(self, keyword: str) -> dict:
+        """Makes search for given keyword and gets the first Suggestion. Then gets the Creatives for that.
+        Returns Advertisor Name, Id, Ad count and List of Creatives"""
         if search := self.get_first_search_suggestion(keyword):
             print(search)
 
-            if search.get("2"): # TODO add domain  "Advertisor": advertisor, "Ad Count": Ad_count, 
+            if search.get("2"): 
                 if advertisor := self.get_advistisor_by_domain(domain=search["2"]["1"]):
                     suggestions = self.get_all_search_suggestions(advertisor["Name"])
                     search = next((suggestion for suggestion in suggestions if suggestion["1"]["1"] == advertisor["Name"] and suggestion["1"]["2"] == advertisor["Advertisor Id"]), None)
                 else:
                     return {"Advertisor": "", "Advertisor Id":"", "Ad Count": 0, "Creatives": []}
             advertisor = search["1"]["1"]
             Ad_count = search['1']['4']['2']['2'] if search["1"].get("4") else 0
             if Ad_count:
                 return {"Advertisor": advertisor, "Advertisor Id": search["1"]["2"], "Ad Count": Ad_count, "Creative_Ids": self.creative_search_by_advertiser_id(advertiser_id=search["1"]["2"])}
             return {"Advertisor": advertisor, "Advertisor Id":search["1"]["2"], "Ad Count": Ad_count, "Creative_Ids": []}
         return {"Advertisor": "", "Advertisor Id":"", "Ad Count": 0, "Creatives": []}
 
-    def get_link_to_video(self, link):
+    def get_link_to_video(self, link: str) -> str:
+        """Get the JS response from the link given and parse the Video/Image Link. Returns input Link if any error occurs"""
         response = requests.post(link)
         try:
             txt = next((x for x in response.text.split("CDATA[") if "googlevideo.com" in x))
             x = str(txt.split("]")[0]).encode("utf-8").decode("unicode_escape")
             return x.encode("utf-8").decode("unicode_escape")
         except:
             return link
 
-    def get_breif_ads(self, advertisor_id, creative_id):
+    def get_breif_ads(self, advertisor_id: str, creative_id: str) -> dict: # TODO do region search
+        """Takes the Advertisor Id and Creative ID and returns the breif details of that particular Ad"""
         data = {
             'f.req': '{"1":"' + advertisor_id + '","2":"' + creative_id + '","5":{"1":1}}',
         }
         response = self.reqs.post(
             'https://adstransparency.google.com/anji/_/rpc/LookupService/GetCreativeById',
             params={'authuser': '0'},
             data=data,
@@ -149,28 +170,30 @@
         date = datetime.datetime.fromtimestamp(int(response["4"]["1"])).strftime('%Y-%m-%d')
         return {"Adverisor Id" : advertisor_id,  # TODO Add Country
                 "Creative Id" : creative_id,
                 "Ad Format": format,
                 "Last Shown" : date,
                 "Ad Link" : link}
     
-    def parse_ad_link(self, html):
+    def parse_ad_link(self, html: str) -> dict:
+        """Parse the Ad Body and Ad title from the html"""
         page = soap(html, 'lxml')
         try:
             ad_body = page.find("div", {"data-highlight-id-inside":"36"}).text
         except:
             ad_body = ""
             #ad_body = page.find_all("div", recursive=False)[0].text
         try: 
             ad_title = page.find("div", {"aria-level":"3"}).text
         except:
             ad_title = ""
         return {"Ad Body":ad_body, "Ad Title": ad_title}
 
-    def get_detailed_ad(self, advertisor_id, creative_id):
+    def get_detailed_ad(self, advertisor_id: str, creative_id: str) -> dict:
+        """Takes the Advertisor Id and Creative ID and returns the details of that particular Ad"""
         ad_detail = self.get_breif_ads(advertisor_id, creative_id)
         response = self.reqs.get(
             ad_detail["Ad Link"],
         )
         ad_detail.update({"Ad Body":"", "Ad Title": "", "Image URL": "", "Video URL": ""})
         if ad_detail["Ad Format"] == "Text":
             ad_detail.update(self.parse_ad_link(response.text))
```

### Comparing `Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO` & `Google Ads Transparency Scraper-1.1/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Google-Ads-Transparency-Scraper
-Version: 1.0
+Version: 1.1
 Summary: A scraper for getting Ads from Google Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
 Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v0.1.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Trends,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scrapre
```

### Comparing `Google Ads Transparency Scraper-1.0/PKG-INFO` & `Google Ads Transparency Scraper-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Google Ads Transparency Scraper
-Version: 1.0
+Version: 1.1
 Summary: A scraper for getting Ads from Google Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
 Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v0.1.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Trends,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scrapre
```

### Comparing `Google Ads Transparency Scraper-1.0/setup.py` & `Google Ads Transparency Scraper-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 setup(
     name="Google Ads Transparency Scraper",
     author="Farhan Ahmed",
     author_email="jattfarhan10@gmail.com",
     url="https://github.com/faniAhmed/GoogleAdsTransparencyScraper",
     description="A scraper for getting Ads from Google Transparency",
-    version="1.0",
+    version="1.1",
     packages=find_packages(where=".", exclude=["tests"]),
     download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v0.1.tar.gz',
     keywords= ['Google', 'Trends', 'Scraper', 'API', 'Google Ads', 'Ads', 'Google Transparency', 'Google Transparency Scraper', 'Google Ads Scrapre'],
     license='Securely Incorporation',
     install_requires=[
         "setuptools>=45.0",
         "beautifulsoup4>=4.12.2",
```

