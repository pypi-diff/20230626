# Comparing `tmp/otlmow_converter-0.8.tar.gz` & `tmp/otlmow_converter-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otlmow_converter-0.8.tar", last modified: Thu Feb  9 11:42:35 2023, max compression
+gzip compressed data, was "otlmow_converter-0.9.tar", last modified: Mon Mar  6 12:34:15 2023, max compression
```

## Comparing `otlmow_converter-0.8.tar` & `otlmow_converter-0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:42:35.900822 otlmow_converter-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-02-09 11:42:26.000000 otlmow_converter-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-09 11:42:26.000000 otlmow_converter-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43126 2023-02-09 11:42:35.900822 otlmow_converter-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-02-09 11:42:26.000000 otlmow_converter-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:42:35.896823 otlmow_converter-0.8/otlmow_converter/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/AssetFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/DotnotationHelper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:42:35.900822 otlmow_converter-0.8/otlmow_converter/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/Exceptions/BadTypeWarning.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/Exceptions/InvalidExtensionError.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/Exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileExporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:42:35.900822 otlmow_converter-0.8/otlmow_converter/FileFormats/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/CsvExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/CsvImporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/DictDecoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/ExcelExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/ExcelImporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/JsonDecoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/JsonExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/JsonImporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/JsonLdExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/OtlAssetJSONEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/RDFExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/TableExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/TtlExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileFormats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/FileImporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/HelperFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/OtlmowConverter.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/SettingsManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/SubsetTool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-02-09 11:42:26.000000 otlmow_converter-0.8/otlmow_converter/settings_otlmow_converter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 11:42:35.896823 otlmow_converter-0.8/otlmow_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43126 2023-02-09 11:42:35.000000 otlmow_converter-0.8/otlmow_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-02-09 11:42:35.000000 otlmow_converter-0.8/otlmow_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 11:42:35.000000 otlmow_converter-0.8/otlmow_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-09 11:42:35.000000 otlmow_converter-0.8/otlmow_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-09 11:42:35.000000 otlmow_converter-0.8/otlmow_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-02-09 11:42:26.000000 otlmow_converter-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 11:42:35.900822 otlmow_converter-0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.696233 otlmow_converter-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-03-06 12:34:06.000000 otlmow_converter-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-06 12:34:06.000000 otlmow_converter-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43126 2023-03-06 12:34:15.696233 otlmow_converter-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-06 12:34:06.000000 otlmow_converter-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.692233 otlmow_converter-0.9/otlmow_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/AssetFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/DotnotationHelper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.696233 otlmow_converter-0.9/otlmow_converter/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/Exceptions/BadTypeWarning.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/Exceptions/InvalidExtensionError.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/Exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileExporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.696233 otlmow_converter-0.9/otlmow_converter/FileFormats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/CsvExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/CsvImporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/DictDecoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/ExcelExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/ExcelImporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/JsonDecoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/JsonExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/JsonImporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/JsonLdExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/OtlAssetJSONEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/RDFExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/TableExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/TtlExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileFormats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/FileImporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/HelperFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/OtlmowConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/SettingsManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/SubsetTool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-06 12:34:06.000000 otlmow_converter-0.9/otlmow_converter/settings_otlmow_converter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:34:15.696233 otlmow_converter-0.9/otlmow_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43126 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-06 12:34:15.000000 otlmow_converter-0.9/otlmow_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-06 12:34:06.000000 otlmow_converter-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 12:34:15.696233 otlmow_converter-0.9/setup.cfg
```

### Comparing `otlmow_converter-0.8/LICENSE` & `otlmow_converter-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/PKG-INFO` & `otlmow_converter-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otlmow_converter
-Version: 0.8
+Version: 0.9
 Author-email: David Vlaminck <david.vlaminck@mow.vlaanderen.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `otlmow_converter-0.8/README.md` & `otlmow_converter-0.9/README.md`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/AssetFactory.py` & `otlmow_converter-0.9/otlmow_converter/AssetFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿from typing import Union, List
 
 from otlmow_model.Classes.ImplementatieElement.AIMObject import AIMObject
 from otlmow_model.Classes.ImplementatieElement.RelatieObject import RelatieObject
-from otlmow_model.Helpers.AssetCreator import AssetCreator
+from otlmow_model.Helpers.AssetCreator import dynamic_create_instance_from_uri
 
 from otlmow_converter.FileFormats.DictDecoder import DictDecoder
 
 
 class AssetFactory:
     @staticmethod
     def create_aimObject_using_other_aimObject_as_template(orig_aim_object: Union[AIMObject, RelatieObject], 
@@ -28,15 +28,15 @@
 
         if typeURI != '':
             if typeURI != orig_aim_object.typeURI and (fields_to_copy == [] or fields_to_copy is None):
                 raise ValueError("parameter typeURI is different from orig_aim_object. parameter fields_to_copy cannot be empty")
 
         if typeURI == '':
             typeURI = orig_aim_object.typeURI
-        new_asset = AssetCreator.dynamic_create_instance_from_uri(typeURI, directory=directory)
+        new_asset = dynamic_create_instance_from_uri(typeURI, directory=directory)
 
         if len(fields_to_copy) == 0:
             fields_to_copy = AssetFactory.get_attribute_list_from_object(orig_aim_object)
 
         if 'typeURI' in fields_to_copy:
             fields_to_copy.remove('typeURI')
         if 'assetId' in fields_to_copy:
```

### Comparing `otlmow_converter-0.8/otlmow_converter/DotnotationHelper.py` & `otlmow_converter-0.9/otlmow_converter/DotnotationHelper.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileExporter.py` & `otlmow_converter-0.9/otlmow_converter/FileExporter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/CsvExporter.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/CsvExporter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/CsvImporter.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/CsvImporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import os
 from pathlib import Path
 
-from otlmow_model.Helpers.AssetCreator import AssetCreator
+from otlmow_model.Helpers.AssetCreator import dynamic_create_instance_from_uri
 
-from otlmow_converter.AssetFactory import AssetFactory
 from otlmow_converter.DotnotationHelper import DotnotationHelper
 
 
 class CsvImporter:
     def __init__(self, settings=None):
         if settings is None:
             settings = {}
@@ -57,15 +56,15 @@
 
         try:
             type_index = self.headers.index('typeURI')
         except ValueError:
             raise ValueError('The data is missing essential typeURI data')
 
         for record in self.data:
-            instance = AssetCreator.dynamic_create_instance_from_uri(record[type_index], directory=class_directory)
+            instance = dynamic_create_instance_from_uri(record[type_index], directory=class_directory)
             list_of_objects.append(instance)
             for index, row in enumerate(record):
                 if index == type_index:
                     continue
                 if row == '':
                     continue
```

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/DictDecoder.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/DictDecoder.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/ExcelExporter.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/ExcelExporter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/ExcelImporter.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/ExcelImporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 import os
 from pathlib import Path
 from typing import Dict, List
 
 import openpyxl
-from otlmow_model.Helpers.AssetCreator import AssetCreator
+from otlmow_model.Helpers.AssetCreator import dynamic_create_instance_from_uri
 
-from otlmow_converter.AssetFactory import AssetFactory
 from otlmow_converter.DotnotationHelper import DotnotationHelper
 
 
 class ExcelImporter:
     def __init__(self, settings=None):
         if settings is None:
             settings = {}
@@ -56,15 +55,15 @@
 
         cardinality_indicator = self.settings['dotnotation']['cardinality indicator']
 
         for sheet, data in self.data.items():
             headers = data[0]
             type_index = headers.index('typeURI')
             for row in data[1:]:
-                instance = AssetCreator.dynamic_create_instance_from_uri(row[type_index], directory=class_directory)
+                instance = dynamic_create_instance_from_uri(row[type_index], directory=class_directory)
                 list_of_objects.append(instance)
                 for index, row_value in enumerate(row):
                     if index == type_index:
                         continue
 
                     header = headers[index]
```

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/JsonDecoder.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/JsonDecoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 
-from otlmow_model.Helpers.AssetCreator import AssetCreator
+from otlmow_model.Helpers.AssetCreator import dynamic_create_instance_from_uri
 
-from otlmow_converter.AssetFactory import AssetFactory
 from otlmow_converter.FileFormats.DictDecoder import DictDecoder
 
 
 class JsonDecoder:
     def __init__(self, settings=None):
         if settings is None:
             settings = {}
@@ -26,15 +25,15 @@
         for obj in dict_list:
             try:
                 typeURI = next(value for key, value in obj.items() if 'typeURI' in key)
 
                 if 'https://wegenenverkeer.data.vlaanderen.be/ns' not in typeURI:
                     raise ValueError('typeURI should start with "https://wegenenverkeer.data.vlaanderen.be/ns" to use this decoder')
 
-                instance = AssetCreator.dynamic_create_instance_from_uri(typeURI, directory=classes_directory)
+                instance = dynamic_create_instance_from_uri(typeURI, directory=classes_directory)
                 lijst.append(instance)
 
                 for key, value in obj.items():
                     if 'typeURI' in key or value == '' or value == [] or key == 'bron' or key == 'doel':
                         continue
 
                     DictDecoder.set_value_by_dictitem(instance, key, value, self.settings['dotnotation']['waarde_shortcut_applicable'])
```

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/JsonImporter.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/JsonImporter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/JsonLdExporter.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/JsonLdExporter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/OtlAssetJSONEncoder.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/OtlAssetJSONEncoder.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/RDFExporter.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/RDFExporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Dict, Iterable
 
 from otlmow_model.BaseClasses.FloatOrDecimalField import FloatOrDecimalField
 from otlmow_model.BaseClasses.KeuzelijstField import KeuzelijstField
+from otlmow_model.Classes.ImplementatieElement.RelatieObject import RelatieObject
 from rdflib import Graph, FOAF, URIRef, BNode, Literal, RDF, XSD
 
 
 class RDFExporter:
     def __init__(self, dotnotation_settings: Dict = None):
 
         if dotnotation_settings is None:
@@ -21,14 +22,16 @@
         for ns, namespace in {'foaf': FOAF,
                               'imel': 'https://wegenenverkeer.data.vlaanderen.be/ns/implementatieelement#',
                               'asset': 'https://data.awvvlaanderen.be/id/asset/',
                               'assetrelatie': 'https://data.awvvlaanderen.be/id/assetrelatie/',
                               'onderdeel': 'https://wegenenverkeer.data.vlaanderen.be/ns/onderdeel#',
                               'installatie': 'https://wegenenverkeer.data.vlaanderen.be/ns/installatie#',
                               'keuzelijst': 'https://wegenenverkeer.data.vlaanderen.be/id/concept/',
+                              'abs': 'https://wegenenverkeer.data.vlaanderen.be/ns/abstracten#',
+                              'pem': 'https://wegenenverkeer.data.vlaanderen.be/ns/proefenmeting#',
                               'loc': 'https://loc.data.wegenenverkeer.be/ns/implementatieelement#'}.items():
             g.bind(ns, namespace)
 
         for instance in list_of_objects:
             if instance.assetId is None or instance.assetId.identificator is None or \
                     instance.assetId.identificator == '':
                 raise ValueError('Can not export assets without a valid assetId')
@@ -36,19 +39,19 @@
             if not hasattr(instance, 'typeURI') or instance.typeURI is None or instance.typeURI == '':
                 raise ValueError(f'Can not export invalid objects: {instance}')
 
             asset = URIRef('https://data.awvvlaanderen.be/id/asset/' + instance.assetId.identificator)
             type_node = URIRef(instance.typeURI)
             g.add((asset, RDF.type, type_node))
 
-            # if isinstance(instance, RelatieObject):
-            #     g.add((asset, URIRef('https://wegenenverkeer.data.vlaanderen.be/ns/implementatieelement#bron'),
-            #            URIRef('https://data.awvvlaanderen.be/id/asset/' + instance.bronAssetId.identificator)))
-            #     g.add((asset, URIRef('https://wegenenverkeer.data.vlaanderen.be/ns/implementatieelement#doel'),
-            #            URIRef('https://data.awvvlaanderen.be/id/asset/' + instance.doelAssetId.identificator)))
+            if isinstance(instance, RelatieObject):
+                g.add((asset, URIRef('https://wegenenverkeer.data.vlaanderen.be/ns/implementatieelement#bron'),
+                       URIRef('https://data.awvvlaanderen.be/id/asset/' + instance.bronAssetId.identificator)))
+                g.add((asset, URIRef('https://wegenenverkeer.data.vlaanderen.be/ns/implementatieelement#doel'),
+                       URIRef('https://data.awvvlaanderen.be/id/asset/' + instance.doelAssetId.identificator)))
 
             self._add_attributes_to_graph(graph=g, asset_or_attribute=instance, asset_attribute_ref=asset)
 
         return g
 
     def _add_attributes_to_graph(self, graph, asset_or_attribute, asset_attribute_ref):
         keys = list(filter(lambda k: k[0] == '_', vars(asset_or_attribute).keys()))
@@ -73,15 +76,15 @@
                     graph.add((asset_attribute_ref, URIRef(attribute.objectUri), waarde_object))
                     self._add_attributes_to_graph(graph=graph, asset_or_attribute=attribute.waarde,
                                                   asset_attribute_ref=waarde_object)
                 continue
 
             if attribute.kardinaliteit_max != '1':
                 for waarde_item in attribute.waarde:
-                    if issubclass(attribute.field, KeuzelijstField):
+                    if waarde_item is not None and issubclass(attribute.field, KeuzelijstField):
                         graph.add((asset_attribute_ref, URIRef(attribute.objectUri),
                                    URIRef(attribute.field.options[waarde_item].objectUri)))
                     elif issubclass(attribute.field, FloatOrDecimalField):
                         graph.add((asset_attribute_ref, URIRef(attribute.objectUri), Literal(waarde_item, datatype=XSD.decimal)))
                     else:
                         graph.add((asset_attribute_ref, URIRef(attribute.objectUri), Literal(waarde_item)))
             else:
```

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/TableExporter.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/TableExporter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileFormats/TtlExporter.py` & `otlmow_converter-0.9/otlmow_converter/FileFormats/TtlExporter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/FileImporter.py` & `otlmow_converter-0.9/otlmow_converter/FileImporter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/OtlmowConverter.py` & `otlmow_converter-0.9/otlmow_converter/OtlmowConverter.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/SettingsManager.py` & `otlmow_converter-0.9/otlmow_converter/SettingsManager.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/SubsetTool.py` & `otlmow_converter-0.9/otlmow_converter/SubsetTool.py`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter/settings_otlmow_converter.json` & `otlmow_converter-0.9/otlmow_converter/settings_otlmow_converter.json`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/otlmow_converter.egg-info/PKG-INFO` & `otlmow_converter-0.9/otlmow_converter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otlmow-converter
-Version: 0.8
+Version: 0.9
 Author-email: David Vlaminck <david.vlaminck@mow.vlaanderen.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `otlmow_converter-0.8/otlmow_converter.egg-info/SOURCES.txt` & `otlmow_converter-0.9/otlmow_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otlmow_converter-0.8/pyproject.toml` & `otlmow_converter-0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otlmow_converter"
-version = "0.8"
+version = "0.9"
 authors = [{name = "David Vlaminck", email = "david.vlaminck@mow.vlaanderen.be"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.7"
 dependencies = [
-  'openpyxl >= 3.0',
-  'otlmow_model >= 2.6.4',
-  'rdflib >= 6.0.0',
+    'openpyxl >= 3.0',
+    'otlmow_model >= 2.6.7',
+    'rdflib >= 6.0.0',
+    'PyLD>=2.0.0',
+    'prettytable>=3.6.0'
 ]
 
 [tool.setuptools.packages.find]
 include = ["otlmow_converter*"]
 
 [project.urls]
 "Homepage" = "https://github.com/davidvlaminck/OTLMOW-Converter"
```

