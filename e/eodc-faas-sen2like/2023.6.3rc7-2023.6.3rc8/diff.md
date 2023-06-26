# Comparing `tmp/eodc_faas_sen2like-2023.6.3rc7.tar.gz` & `tmp/eodc_faas_sen2like-2023.6.3rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_sen2like-2023.6.3rc7.tar", max compression
+gzip compressed data, was "eodc_faas_sen2like-2023.6.3rc8.tar", max compression
```

## Comparing `eodc_faas_sen2like-2023.6.3rc7.tar` & `eodc_faas_sen2like-2023.6.3rc8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.6.3rc7/README.md
--rw-r--r--   0        0        0      642 2023-06-26 09:00:02.472000 eodc_faas_sen2like-2023.6.3rc7/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-26 09:00:02.472000 eodc_faas_sen2like-2023.6.3rc7/sen2like_processor_bindings/__init__.py
--rw-r--r--   0        0        0     2970 2023-06-15 14:21:56.444000 eodc_faas_sen2like-2023.6.3rc7/sen2like_processor_bindings/model.py
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.6.3rc7/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.6.3rc8/README.md
+-rw-r--r--   0        0        0      642 2023-06-26 10:14:49.500000 eodc_faas_sen2like-2023.6.3rc8/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-26 10:14:49.500000 eodc_faas_sen2like-2023.6.3rc8/sen2like_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-26 12:59:11.464000 eodc_faas_sen2like-2023.6.3rc8/sen2like_processor_bindings/model.py
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.6.3rc8/PKG-INFO
```

### Comparing `eodc_faas_sen2like-2023.6.3rc7/pyproject.toml` & `eodc_faas_sen2like-2023.6.3rc8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-sen2like"
-version = "2023.6.3-rc.7"
+version = "2023.6.3-rc.8"
 description = "Bindings for the sen2like processor exposed at EODC"
 authors = ["Valentina Hutter <valentina.hutter@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "sen2like_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_sen2like-2023.6.3rc7/sen2like_processor_bindings/model.py` & `eodc_faas_sen2like-2023.6.3rc8/sen2like_processor_bindings/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import pyproj
 from pydantic import BaseModel, Field, validator
 
 logger = logging.getLogger(__name__)
 
 
-DEFAULT_CRS = pyproj.CRS.from_user_input("EPSG:4326").to_wkt()
+DEFAULT_CRS = pyproj.CRS.from_user_input("EPSG:4326")
 
 
 def parse_crs(v) -> pyproj.CRS:
     if v is None or v.strip() == "":
-        return DEFAULT_CRS
+        return str(DEFAULT_CRS)
     else:
         try:
             # Check that the crs can be parsed and store as WKT
             crs_obj = pyproj.CRS.from_user_input(v)
-            return crs_obj.to_wkt()
+            return str(crs_obj)
         except pyproj.exceptions.CRSError as e:
             logger.error(
                 f"Provided CRS {v} could not be parsed, defaulting to EPSG:4326"
             )
             raise e
```

### Comparing `eodc_faas_sen2like-2023.6.3rc7/PKG-INFO` & `eodc_faas_sen2like-2023.6.3rc8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-sen2like
-Version: 2023.6.3rc7
+Version: 2023.6.3rc8
 Summary: Bindings for the sen2like processor exposed at EODC
 Author: Valentina Hutter
 Author-email: valentina.hutter@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

