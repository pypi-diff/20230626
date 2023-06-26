# Comparing `tmp/eodc_faas_sen2like-2023.6.3rc6.tar.gz` & `tmp/eodc_faas_sen2like-2023.6.3rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_sen2like-2023.6.3rc6.tar", max compression
+gzip compressed data, was "eodc_faas_sen2like-2023.6.3rc7.tar", max compression
```

## Comparing `eodc_faas_sen2like-2023.6.3rc6.tar` & `eodc_faas_sen2like-2023.6.3rc7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.6.3rc6/README.md
--rw-r--r--   0        0        0      624 2023-06-19 08:15:46.164000 eodc_faas_sen2like-2023.6.3rc6/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-19 08:15:46.164000 eodc_faas_sen2like-2023.6.3rc6/sen2like_processor_bindings/__init__.py
--rw-r--r--   0        0        0     2970 2023-06-15 14:21:56.444000 eodc_faas_sen2like-2023.6.3rc6/sen2like_processor_bindings/model.py
--rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.6.3rc6/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.6.3rc7/README.md
+-rw-r--r--   0        0        0      642 2023-06-26 09:00:02.472000 eodc_faas_sen2like-2023.6.3rc7/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-26 09:00:02.472000 eodc_faas_sen2like-2023.6.3rc7/sen2like_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     2970 2023-06-15 14:21:56.444000 eodc_faas_sen2like-2023.6.3rc7/sen2like_processor_bindings/model.py
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.6.3rc7/PKG-INFO
```

### Comparing `eodc_faas_sen2like-2023.6.3rc6/pyproject.toml` & `eodc_faas_sen2like-2023.6.3rc7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "eodc-faas-sen2like"
-version = "2023.6.3-rc.6"
+version = "2023.6.3-rc.7"
 description = "Bindings for the sen2like processor exposed at EODC"
 authors = ["Valentina Hutter <valentina.hutter@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "sen2like_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.7"
+pyproj = "^3.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.1"
 pytest = "^7.2.2"
 ruff = "^0.0.259"
 ipykernel = "^6.22.0"
```

### Comparing `eodc_faas_sen2like-2023.6.3rc6/sen2like_processor_bindings/model.py` & `eodc_faas_sen2like-2023.6.3rc7/sen2like_processor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_sen2like-2023.6.3rc6/PKG-INFO` & `eodc_faas_sen2like-2023.6.3rc7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: eodc-faas-sen2like
-Version: 2023.6.3rc6
+Version: 2023.6.3rc7
 Summary: Bindings for the sen2like processor exposed at EODC
 Author: Valentina Hutter
 Author-email: valentina.hutter@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pyproj (>=3.6.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Sen2like Python Bindings
```

