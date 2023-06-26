# Comparing `tmp/pyegt-0.1.1.tar.gz` & `tmp/pyegt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyegt-0.1.1.tar", last modified: Mon Jun 26 12:59:53 2023, max compression
+gzip compressed data, was "pyegt-0.1.2.tar", last modified: Mon Jun 26 18:23:32 2023, max compression
```

## Comparing `pyegt-0.1.1.tar` & `pyegt-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 12:59:53.643580 pyegt-0.1.1/
--rw-r--r--   0 iannesbitt   (501) staff       (20)    11357 2023-06-15 22:22:38.000000 pyegt-0.1.1/LICENSE
--rw-r--r--   0 iannesbitt   (501) staff       (20)     2862 2023-06-26 12:59:53.641826 pyegt-0.1.1/PKG-INFO
--rw-r--r--   0 iannesbitt   (501) staff       (20)     2170 2023-06-26 12:56:15.000000 pyegt-0.1.1/README.md
-drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 12:59:53.640624 pyegt-0.1.1/pyegt/
--rw-r--r--   0 iannesbitt   (501) staff       (20)        0 2023-06-15 22:18:10.000000 pyegt-0.1.1/pyegt/__init__.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)       21 2023-06-26 12:58:32.000000 pyegt-0.1.1/pyegt/_version.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)     2853 2023-06-25 16:39:53.000000 pyegt-0.1.1/pyegt/defs.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)    12502 2023-06-25 18:11:54.000000 pyegt-0.1.1/pyegt/height.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)     1264 2023-06-25 18:10:51.000000 pyegt-0.1.1/pyegt/test.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)     8367 2023-06-25 17:58:50.000000 pyegt-0.1.1/pyegt/utils.py
-drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 12:59:53.641603 pyegt-0.1.1/pyegt.egg-info/
--rw-r--r--   0 iannesbitt   (501) staff       (20)     2862 2023-06-26 12:59:53.000000 pyegt-0.1.1/pyegt.egg-info/PKG-INFO
--rw-r--r--   0 iannesbitt   (501) staff       (20)      297 2023-06-26 12:59:53.000000 pyegt-0.1.1/pyegt.egg-info/SOURCES.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)        1 2023-06-26 12:59:53.000000 pyegt-0.1.1/pyegt.egg-info/dependency_links.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)       47 2023-06-26 12:59:53.000000 pyegt-0.1.1/pyegt.egg-info/entry_points.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)       23 2023-06-26 12:59:53.000000 pyegt-0.1.1/pyegt.egg-info/requires.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)        6 2023-06-26 12:59:53.000000 pyegt-0.1.1/pyegt.egg-info/top_level.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)       38 2023-06-26 12:59:53.643776 pyegt-0.1.1/setup.cfg
--rw-r--r--   0 iannesbitt   (501) staff       (20)     1163 2023-06-26 12:29:23.000000 pyegt-0.1.1/setup.py
+drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 18:23:32.706589 pyegt-0.1.2/
+-rw-r--r--   0 iannesbitt   (501) staff       (20)    11357 2023-06-15 22:22:38.000000 pyegt-0.1.2/LICENSE
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     2862 2023-06-26 18:23:32.706444 pyegt-0.1.2/PKG-INFO
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     2170 2023-06-26 12:56:15.000000 pyegt-0.1.2/README.md
+drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 18:23:32.705484 pyegt-0.1.2/pyegt/
+-rw-r--r--   0 iannesbitt   (501) staff       (20)        0 2023-06-15 22:18:10.000000 pyegt-0.1.2/pyegt/__init__.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)       21 2023-06-26 18:22:39.000000 pyegt-0.1.2/pyegt/_version.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     3809 2023-06-26 14:27:21.000000 pyegt-0.1.2/pyegt/defs.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)    12502 2023-06-25 18:11:54.000000 pyegt-0.1.2/pyegt/height.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     1264 2023-06-25 18:10:51.000000 pyegt-0.1.2/pyegt/test.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     9320 2023-06-26 15:55:21.000000 pyegt-0.1.2/pyegt/utils.py
+drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 18:23:32.706237 pyegt-0.1.2/pyegt.egg-info/
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     2862 2023-06-26 18:23:32.000000 pyegt-0.1.2/pyegt.egg-info/PKG-INFO
+-rw-r--r--   0 iannesbitt   (501) staff       (20)      297 2023-06-26 18:23:32.000000 pyegt-0.1.2/pyegt.egg-info/SOURCES.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)        1 2023-06-26 18:23:32.000000 pyegt-0.1.2/pyegt.egg-info/dependency_links.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)       47 2023-06-26 18:23:32.000000 pyegt-0.1.2/pyegt.egg-info/entry_points.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)       23 2023-06-26 18:23:32.000000 pyegt-0.1.2/pyegt.egg-info/requires.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)        6 2023-06-26 18:23:32.000000 pyegt-0.1.2/pyegt.egg-info/top_level.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)       38 2023-06-26 18:23:32.706630 pyegt-0.1.2/setup.cfg
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     1163 2023-06-26 12:29:23.000000 pyegt-0.1.2/setup.py
```

### Comparing `pyegt-0.1.1/LICENSE` & `pyegt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyegt-0.1.1/PKG-INFO` & `pyegt-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Look up geoid and tidal model heights relative to the ellipsoid
 Home-page: https://iannesbitt.github.io/pyegt
 Author: Ian Nesbitt
 Author-email: nesbitt@nceas.ucsb.edu
 License: Apache Software License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `pyegt-0.1.1/README.md` & `pyegt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyegt-0.1.1/pyegt/defs.py` & `pyegt-0.1.2/pyegt/defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,26 +57,48 @@
     'WGS84_TRANSIT', 'WGS84_G1762', 'WGS84_G2139'
 ]
 """.. |vdmodels| raw:: html
 
     <a href="https://vdatum.noaa.gov/docs/services.html#step160" target="_blank">VDatum API Vertical Reference Frames List</a>
 
 List of geoid and tidal models used in the VDatum API. From |vdmodels|.
+
+Definition::
+
+    VDATUM_MODELS = [
+        'NAVD88', 'NGVD29', 'ASVD02', 'W0_USGG2012', 'GUVD04', 'NMVD03', 'PRVD02',
+        'VIVD09', 'CRD', 'EGM2008', 'EGM1996', 'EGM1984', 'XGEOID16B', 'XGEOID17B',
+        'XGEOID18B', 'XGEOID19B', 'XGEOID20B', 'IGLD85', 'LWD_IGLD85',
+        'OHWM_IGLD85', 'CRD', 'LMSL', 'MLLW', 'MLW', 'MTL', 'DTL', 'MHW', 'MHHW',
+        'LWD', 'NAD27', 'NAD83_1986', 'NAD83_2011', 'NAD83_NSRS2007',
+        'NAD83_MARP00', 'NAD83_PACP00', 'WGS84_G1674', 'ITRF2014', 'IGS14',
+        'ITRF2008', 'IGS08', 'ITRF2005', 'IGS2005', 'WGS84_G1150', 'ITRF2000',
+        'IGS00', 'IGb00', 'ITRF96', 'WGS84_G873', 'ITRF94', 'ITRF93', 'ITRF92',
+        'SIOMIT92', 'WGS84_G730', 'ITRF91', 'ITRF90', 'ITRF89', 'ITRF88',
+        'WGS84_TRANSIT', 'WGS84_G1762', 'WGS84_G2139'
+    ]
+
 """
 
 REGIONS = [
     # VDatum regions (from https://vdatum.noaa.gov/docs/services.html#step140)
     'contiguous', 'ak', 'seak', 'as', 'chesapeak_delaware',
     'westcoast', 'gcnmi', 'hi', 'prvi', 'sgi', 'spi', 'sli'
 ]
 """.. |regions| raw:: html
 
     <a href="https://vdatum.noaa.gov/docs/services.html#step140" target="_blank">VDatum API Regions List</a>
 
 List of regions used in the VDatum API. From |regions|.
+
+Definition::
+
+    REGIONS = ['contiguous', 'ak', 'seak', 'as', 'chesapeak_delaware',
+               'westcoast', 'gcnmi', 'hi', 'prvi', 'sgi', 'spi', 'sli']
+
 """
 
 VDATUM_URL = 'https://vdatum.noaa.gov/vdatumweb/api/convert?s_x=%s&s_y=%s&s_h_frame=%s&s_v_frame=%s&s_v_geoid=%s&t_h_frame=%s&t_v_frame=%s&t_v_geoid=%s&region=%s'
 
 MODEL_LIST = []
 for m in NGS_MODELS:
     MODEL_LIST.append(m)
```

#### html2text {}

```diff
@@ -18,16 +18,27 @@
 'MLW', 'MTL', 'DTL', 'MHW', 'MHHW', 'LWD', 'NAD27', 'NAD83_1986', 'NAD83_2011',
 'NAD83_NSRS2007', 'NAD83_MARP00', 'NAD83_PACP00', 'WGS84_G1674', 'ITRF2014',
 'IGS14', 'ITRF2008', 'IGS08', 'ITRF2005', 'IGS2005', 'WGS84_G1150', 'ITRF2000',
 'IGS00', 'IGb00', 'ITRF96', 'WGS84_G873', 'ITRF94', 'ITRF93', 'ITRF92',
 'SIOMIT92', 'WGS84_G730', 'ITRF91', 'ITRF90', 'ITRF89', 'ITRF88',
 'WGS84_TRANSIT', 'WGS84_G1762', 'WGS84_G2139' ] """.. |vdmodels| raw:: html
 VDatum_API_Vertical_Reference_Frames_List List of geoid and tidal models used
-in the VDatum API. From |vdmodels|. """ REGIONS = [ # VDatum regions (from
-https://vdatum.noaa.gov/docs/services.html#step140) 'contiguous', 'ak', 'seak',
-'as', 'chesapeak_delaware', 'westcoast', 'gcnmi', 'hi', 'prvi', 'sgi', 'spi',
-'sli' ] """.. |regions| raw:: html VDatum_API_Regions_List List of regions used
-in the VDatum API. From |regions|. """ VDATUM_URL = 'https://vdatum.noaa.gov/
+in the VDatum API. From |vdmodels|. Definition:: VDATUM_MODELS = [ 'NAVD88',
+'NGVD29', 'ASVD02', 'W0_USGG2012', 'GUVD04', 'NMVD03', 'PRVD02', 'VIVD09',
+'CRD', 'EGM2008', 'EGM1996', 'EGM1984', 'XGEOID16B', 'XGEOID17B', 'XGEOID18B',
+'XGEOID19B', 'XGEOID20B', 'IGLD85', 'LWD_IGLD85', 'OHWM_IGLD85', 'CRD', 'LMSL',
+'MLLW', 'MLW', 'MTL', 'DTL', 'MHW', 'MHHW', 'LWD', 'NAD27', 'NAD83_1986',
+'NAD83_2011', 'NAD83_NSRS2007', 'NAD83_MARP00', 'NAD83_PACP00', 'WGS84_G1674',
+'ITRF2014', 'IGS14', 'ITRF2008', 'IGS08', 'ITRF2005', 'IGS2005', 'WGS84_G1150',
+'ITRF2000', 'IGS00', 'IGb00', 'ITRF96', 'WGS84_G873', 'ITRF94', 'ITRF93',
+'ITRF92', 'SIOMIT92', 'WGS84_G730', 'ITRF91', 'ITRF90', 'ITRF89', 'ITRF88',
+'WGS84_TRANSIT', 'WGS84_G1762', 'WGS84_G2139' ] """ REGIONS = [ # VDatum
+regions (from https://vdatum.noaa.gov/docs/services.html#step140) 'contiguous',
+'ak', 'seak', 'as', 'chesapeak_delaware', 'westcoast', 'gcnmi', 'hi', 'prvi',
+'sgi', 'spi', 'sli' ] """.. |regions| raw:: html VDatum_API_Regions_List List
+of regions used in the VDatum API. From |regions|. Definition:: REGIONS =
+['contiguous', 'ak', 'seak', 'as', 'chesapeak_delaware', 'westcoast', 'gcnmi',
+'hi', 'prvi', 'sgi', 'spi', 'sli'] """ VDATUM_URL = 'https://vdatum.noaa.gov/
 vdatumweb/api/
 convert?s_x=%s&s_y=%s&s_h_frame=%s&s_v_frame=%s&s_v_geoid=%s&t_h_frame=%s&t_v_frame=%s&t_v_geoid=%s&region=%s'
 MODEL_LIST = [] for m in NGS_MODELS: MODEL_LIST.append(m) for m in
 VDATUM_MODELS: MODEL_LIST.append(m)
```

### Comparing `pyegt-0.1.1/pyegt/height.py` & `pyegt-0.1.2/pyegt/height.py`

 * *Files identical despite different names*

### Comparing `pyegt-0.1.1/pyegt/test.py` & `pyegt-0.1.2/pyegt/test.py`

 * *Files identical despite different names*

### Comparing `pyegt-0.1.1/pyegt/utils.py` & `pyegt-0.1.2/pyegt/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,107 @@
 import time
 import requests
 from typing import Union, Literal
 
 from . import defs
 
-def get_ngs_url(lat: float, lon: float, ngs_model: int):
+def model_search(vrs: str=None) -> Union[str, Literal[None]]:
+    """
+    Get a model name from a search term containing that name.
+
+    Example::
+
+        >>> egm = "EGM2008 height"
+        >>> model_search(vrs=egm)
+        "EGM2008"
+        >>> navd88 = "NAVD88 (US Survey Feet)"
+        >>> model_search(vrs=navd88)
+        "NAVD88"
+        >>> bad_name = "NAVD 88"
+        >>> model_search(vrs=bad_name)
+        None
+
+    :param str vrs: The search term containing the model name
+    :return: A verified model name or ``None`` if none is found
+    :rtype: str or None
+    """
+    for m in defs.MODEL_LIST:
+        if m in vrs:
+            # sometimes vrs from WKT will be formatted like "EGM2008 height" and this should catch that
+            return m
+    return None
+
+def get_ngs_url(lat: float, lon: float, ngs_model: int) -> str:
     """
     :param float lat: Decimal latitude
     :param float lon: Decimal longitude
     :param str ngs_model: The NGS geoid model to use for lookup `(see list) <https://www.ngs.noaa.gov/web_services/geoid.shtml>`_
     :return: The query url to use in lookup
     :rtype: str
     """
     return defs.NGS_URL % (lat, lon, ngs_model)
 
-def get_ngs_json(ngs_url: str):
+def get_ngs_json(ngs_url: str) -> dict:
     """
-    :param str ngs_url: Decimal latitude
+    :param str ngs_url: The NGS query URL
     :return: The returned json (if applicable)
     :rtype: json
+    :raises AttributeError: if geoidHeight is not in returned json
+    :raises ConnectionError: if no NGS json is returned in 3 tries
     """
     i = 0
     while True:
         print('Querying %s' % (ngs_url))
         response = requests.get(ngs_url)
         json_data = response.json() if response and response.status_code == 200 else None
         if json_data and 'geoidHeight' in json_data:
             return json_data
         if json_data and (not 'geoidHeight' in json_data):
-            print('Json data request returned in error: %s' % (json_data))
-            exit(1)
+            raise AttributeError('geoidHeight not in returned json:\n%s' % (json_data))
         if i < 3:
             i += 1
             time.sleep(1)
         else:
-            print('Could not complete request for NGS API in %s tries.' % (i  ))
-            exit(1)
+            raise ConnectionError('Could not get NGS json in %s tries.' % (i))
 
-def get_vdatum_url(lat: float, lon: float, vdatum_model: str, region: str):
+def get_vdatum_url(lat: float, lon: float, vdatum_model: str, region: str) -> str:
     """
     .. |vdatum| raw:: html
 
         <a href="https://vdatum.noaa.gov/docs/services.html#step160" target="_blank">see list</a>
 
     
     :param float lat: Decimal latitude
     :param float lon: Decimal longitude
     :param str vdatum_model: The VDatum geoid, tidal, or potential model to use for lookup (|vdatum|)
     :param str region: The region to search
+    :return: The VDatum query URL
+    :rtype: str
     """
     wgs = 'WGS84_G1674'
     return defs.VDATUM_URL % (
             lon, # s_x
             lat, # s_y
             wgs, # s_h_frame
             vdatum_model, # s_v_frame
             vdatum_model, # s_v_geoid
             wgs, # t_h_frame
             wgs, # t_v_frame
             vdatum_model, # t_v_geoid
             region # region
             )
 
-def get_vdatum_json(vdatum_url, region):
+def get_vdatum_json(vdatum_url, region) -> dict:
     """
     
-    :param float lat: Decimal latitude
-    :param float lon: Decimal longitude
-    :param str vdatum_model: The VDatum geoid, tidal, or potential model to use for lookup (|vdatum|)
+    :param str vdatum_url: The VDatum query URL
     :param str region: The region to search
+    :return: JSON response from VDatum API
+    :rtype: dict
+    :raises AttributeError: if the returned JSON has an error code
     """
     while True:
         print('Querying %s' % (vdatum_url))
         response = requests.get(vdatum_url)
         json_data = response.json() if response and response.status_code == 200 else None
         if json_data and ('t_z' in json_data):
             return json_data
```

### Comparing `pyegt-0.1.1/pyegt.egg-info/PKG-INFO` & `pyegt-0.1.2/pyegt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Look up geoid and tidal model heights relative to the ellipsoid
 Home-page: https://iannesbitt.github.io/pyegt
 Author: Ian Nesbitt
 Author-email: nesbitt@nceas.ucsb.edu
 License: Apache Software License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `pyegt-0.1.1/setup.py` & `pyegt-0.1.2/setup.py`

 * *Files identical despite different names*

