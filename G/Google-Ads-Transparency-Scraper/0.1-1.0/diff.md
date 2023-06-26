# Comparing `tmp/Google Ads Transparency Scraper-0.1.tar.gz` & `tmp/Google Ads Transparency Scraper-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Google Ads Transparency Scraper-0.1.tar", last modified: Mon Jun 26 05:27:48 2023, max compression
+gzip compressed data, was "Google Ads Transparency Scraper-1.0.tar", last modified: Mon Jun 26 05:41:34 2023, max compression
```

## Comparing `Google Ads Transparency Scraper-0.1.tar` & `Google Ads Transparency Scraper-1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 05:27:48.888665 Google Ads Transparency Scraper-0.1/
-drwxrwxrwx   0        0        0        0 2023-06-26 05:27:48.864591 Google Ads Transparency Scraper-0.1/GoogleAds/
--rw-rw-rw-   0        0        0       38 2023-06-26 01:03:05.000000 Google Ads Transparency Scraper-0.1/GoogleAds/__init__.py
--rw-rw-rw-   0        0        0     8302 2023-06-26 00:31:39.000000 Google Ads Transparency Scraper-0.1/GoogleAds/main.py
-drwxrwxrwx   0        0        0        0 2023-06-26 05:27:48.887668 Google Ads Transparency Scraper-0.1/Google_Ads_Transparency_Scraper.egg-info/
--rw-rw-rw-   0        0        0      863 2023-06-26 05:27:48.000000 Google Ads Transparency Scraper-0.1/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-06-26 05:27:48.000000 Google Ads Transparency Scraper-0.1/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 05:27:48.000000 Google Ads Transparency Scraper-0.1/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-26 05:27:48.000000 Google Ads Transparency Scraper-0.1/Google_Ads_Transparency_Scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 05:27:48.000000 Google Ads Transparency Scraper-0.1/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      863 2023-06-26 05:27:48.888665 Google Ads Transparency Scraper-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-06-26 05:27:48.890660 Google Ads Transparency Scraper-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-06-26 05:27:33.000000 Google Ads Transparency Scraper-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 05:41:34.638880 Google Ads Transparency Scraper-1.0/
+drwxrwxrwx   0        0        0        0 2023-06-26 05:41:34.628000 Google Ads Transparency Scraper-1.0/GoogleAdsTransparency/
+-rw-rw-rw-   0        0        0       50 2023-06-26 05:30:53.000000 Google Ads Transparency Scraper-1.0/GoogleAdsTransparency/__init__.py
+-rw-rw-rw-   0        0        0     8302 2023-06-26 00:31:39.000000 Google Ads Transparency Scraper-1.0/GoogleAdsTransparency/main.py
+drwxrwxrwx   0        0        0        0 2023-06-26 05:41:34.637879 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/
+-rw-rw-rw-   0        0        0      849 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-26 05:41:34.000000 Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      849 2023-06-26 05:41:34.638880 Google Ads Transparency Scraper-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-06-26 05:37:43.000000 Google Ads Transparency Scraper-1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-26 05:41:34.640874 Google Ads Transparency Scraper-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-06-26 05:34:58.000000 Google Ads Transparency Scraper-1.0/setup.py
```

### Comparing `Google Ads Transparency Scraper-0.1/GoogleAds/main.py` & `Google Ads Transparency Scraper-1.0/GoogleAdsTransparency/main.py`

 * *Files identical despite different names*

### Comparing `Google Ads Transparency Scraper-0.1/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO` & `Google Ads Transparency Scraper-1.0/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: Google-Ads-Transparency-Scraper
-Version: 0.1
-Summary: A scraper for getting Ads from Google Trends
+Version: 1.0
+Summary: A scraper for getting Ads from Google Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v0.1.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v0.1.tar.gz
-Keywords: Google,Trends,Scraper,API,Google Ads,Ads,Google Trends,Google Trends Scraper,Google Ads Scrapre
-Platform: UNKNOWN
+Keywords: Google,Trends,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scrapre
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: Urdu
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
-
-UNKNOWN
-
```

### Comparing `Google Ads Transparency Scraper-0.1/PKG-INFO` & `Google Ads Transparency Scraper-1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: Google Ads Transparency Scraper
-Version: 0.1
-Summary: A scraper for getting Ads from Google Trends
+Version: 1.0
+Summary: A scraper for getting Ads from Google Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v0.1.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v0.1.tar.gz
-Keywords: Google,Trends,Scraper,API,Google Ads,Ads,Google Trends,Google Trends Scraper,Google Ads Scrapre
-Platform: UNKNOWN
+Keywords: Google,Trends,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scrapre
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: Urdu
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
-
-UNKNOWN
-
```

### Comparing `Google Ads Transparency Scraper-0.1/setup.py` & `Google Ads Transparency Scraper-1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Google Ads Transparency Scraper",
     author="Farhan Ahmed",
     author_email="jattfarhan10@gmail.com",
     url="https://github.com/faniAhmed/GoogleAdsTransparencyScraper",
-    description="A scraper for getting Ads from Google Trends",
-    version="0.1",
+    description="A scraper for getting Ads from Google Transparency",
+    version="1.0",
     packages=find_packages(where=".", exclude=["tests"]),
     download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v0.1.tar.gz',
-    keywords= ['Google', 'Trends', 'Scraper', 'API', 'Google Ads', 'Ads', 'Google Trends', 'Google Trends Scraper', 'Google Ads Scrapre'],
+    keywords= ['Google', 'Trends', 'Scraper', 'API', 'Google Ads', 'Ads', 'Google Transparency', 'Google Transparency Scraper', 'Google Ads Scrapre'],
     license='Securely Incorporation',
     install_requires=[
         "setuptools>=45.0",
         "beautifulsoup4>=4.12.2",
         "Requests>=2.31.0",
     ],
     classifiers=[
```

