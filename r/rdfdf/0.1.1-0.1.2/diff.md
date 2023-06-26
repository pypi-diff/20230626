# Comparing `tmp/rdfdf-0.1.1.tar.gz` & `tmp/rdfdf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfdf-0.1.1.tar", max compression
+gzip compressed data, was "rdfdf-0.1.2.tar", max compression
```

## Comparing `rdfdf-0.1.1.tar` & `rdfdf-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.1/LICENSE
--rw-r--r--   0        0        0     8588 2023-05-24 07:20:23.215813 rdfdf-0.1.1/README.md
--rw-r--r--   0        0        0      459 2023-06-26 08:40:11.261587 rdfdf-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      918 2023-05-15 09:40:40.000000 rdfdf-0.1.1/rdfdf/examples/example_1.py
--rw-r--r--   0        0        0     1154 2023-05-15 09:40:40.000000 rdfdf-0.1.1/rdfdf/examples/example_2.py
--rw-r--r--   0        0        0     1517 2023-05-15 09:40:40.000000 rdfdf-0.1.1/rdfdf/examples/example_3.py
--rw-r--r--   0        0        0     1373 2023-05-15 09:40:40.000000 rdfdf-0.1.1/rdfdf/examples/example_4.py
--rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.1/rdfdf/helpers/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.1/rdfdf/helpers/importers.py
--rw-r--r--   0        0        0      969 2023-05-22 07:07:02.000000 rdfdf-0.1.1/rdfdf/helpers/rdfdf_utils.py
--rw-r--r--   0        0        0     3998 2023-06-20 14:36:07.754829 rdfdf-0.1.1/rdfdf/rdfdf.py
--rw-r--r--   0        0        0     9145 1970-01-01 00:00:00.000000 rdfdf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8588 2023-05-24 07:20:23.215813 rdfdf-0.1.2/README.md
+-rw-r--r--   0        0        0      459 2023-06-26 10:19:50.105222 rdfdf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.2/rdfdf/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-15 09:40:40.000000 rdfdf-0.1.2/rdfdf/examples/example_1.py
+-rw-r--r--   0        0        0     1154 2023-05-15 09:40:40.000000 rdfdf-0.1.2/rdfdf/examples/example_2.py
+-rw-r--r--   0        0        0     1517 2023-05-15 09:40:40.000000 rdfdf-0.1.2/rdfdf/examples/example_3.py
+-rw-r--r--   0        0        0     1373 2023-05-15 09:40:40.000000 rdfdf-0.1.2/rdfdf/examples/example_4.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.2/rdfdf/helpers/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.2/rdfdf/helpers/importers.py
+-rw-r--r--   0        0        0      969 2023-05-22 07:07:02.000000 rdfdf-0.1.2/rdfdf/helpers/rdfdf_utils.py
+-rw-r--r--   0        0        0     3998 2023-06-20 14:36:07.754829 rdfdf-0.1.2/rdfdf/rdfdf.py
+-rw-r--r--   0        0        0     9145 1970-01-01 00:00:00.000000 rdfdf-0.1.2/PKG-INFO
```

### Comparing `rdfdf-0.1.1/LICENSE` & `rdfdf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.1/README.md` & `rdfdf-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.1/rdfdf/examples/example_1.py` & `rdfdf-0.1.2/rdfdf/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.1/rdfdf/examples/example_2.py` & `rdfdf-0.1.2/rdfdf/examples/example_2.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.1/rdfdf/examples/example_3.py` & `rdfdf-0.1.2/rdfdf/examples/example_3.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.1/rdfdf/examples/example_4.py` & `rdfdf-0.1.2/rdfdf/examples/example_4.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.1/rdfdf/helpers/importers.py` & `rdfdf-0.1.2/rdfdf/helpers/importers.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.1/rdfdf/helpers/rdfdf_utils.py` & `rdfdf-0.1.2/rdfdf/helpers/rdfdf_utils.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.1/rdfdf/rdfdf.py` & `rdfdf-0.1.2/rdfdf/rdfdf.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.1/PKG-INFO` & `rdfdf-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfdf
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: GPL3
 Author: Lukas Plank
 Author-email: lupl@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

