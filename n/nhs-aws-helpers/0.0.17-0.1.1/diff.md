# Comparing `tmp/nhs_aws_helpers-0.0.17.tar.gz` & `tmp/nhs_aws_helpers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_aws_helpers-0.0.17.tar", max compression
+gzip compressed data, was "nhs_aws_helpers-0.1.1.tar", max compression
```

## Comparing `nhs_aws_helpers-0.0.17.tar` & `nhs_aws_helpers-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1078 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/LICENSE.md
--rw-r--r--   0        0        0      666 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/README.md
--rw-r--r--   0        0        0    39862 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/nhs_aws_helpers/__init__.py
--rw-r--r--   0        0        0     7980 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/nhs_aws_helpers/async_s3_object_reader.py
--rw-r--r--   0        0        0     6673 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/nhs_aws_helpers/async_s3_object_writer.py
--rw-r--r--   0        0        0      674 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/nhs_aws_helpers/common.py
--rw-r--r--   0        0        0     4095 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/nhs_aws_helpers/fixtures.py
--rw-r--r--   0        0        0        0 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/nhs_aws_helpers/py.typed
--rw-r--r--   0        0        0     7916 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/nhs_aws_helpers/s3_object_reader.py
--rw-r--r--   0        0        0     6681 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/nhs_aws_helpers/s3_object_writer.py
--rw-r--r--   0        0        0     3060 2023-06-25 21:15:33.310167 nhs_aws_helpers-0.0.17/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/tests/__init__.py
--rw-r--r--   0        0        0    10996 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/tests/async_s3_object_buffer_tests.py
--rw-r--r--   0        0        0     7558 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/tests/aws_tests.py
--rw-r--r--   0        0        0      280 2023-06-25 21:15:08.997875 nhs_aws_helpers-0.0.17/tests/conftest.py
--rw-r--r--   0        0        0    10316 2023-06-25 21:15:09.001875 nhs_aws_helpers-0.0.17/tests/s3_object_buffer_tests.py
--rw-r--r--   0        0        0      518 2023-06-25 21:15:09.001875 nhs_aws_helpers-0.0.17/tests/utils.py
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-26 09:25:33.545862 nhs_aws_helpers-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      666 2023-06-26 09:25:33.545862 nhs_aws_helpers-0.1.1/README.md
+-rw-r--r--   0        0        0    39862 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/nhs_aws_helpers/__init__.py
+-rw-r--r--   0        0        0     7980 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/nhs_aws_helpers/async_s3_object_reader.py
+-rw-r--r--   0        0        0     6673 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/nhs_aws_helpers/async_s3_object_writer.py
+-rw-r--r--   0        0        0      674 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/nhs_aws_helpers/common.py
+-rw-r--r--   0        0        0     4095 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/nhs_aws_helpers/fixtures.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/nhs_aws_helpers/py.typed
+-rw-r--r--   0        0        0     7916 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/nhs_aws_helpers/s3_object_reader.py
+-rw-r--r--   0        0        0     6681 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/nhs_aws_helpers/s3_object_writer.py
+-rw-r--r--   0        0        0     3059 2023-06-26 09:25:54.786357 nhs_aws_helpers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    10996 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/tests/async_s3_object_buffer_tests.py
+-rw-r--r--   0        0        0     7558 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/tests/aws_tests.py
+-rw-r--r--   0        0        0      280 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    10316 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/tests/s3_object_buffer_tests.py
+-rw-r--r--   0        0        0      518 2023-06-26 09:25:33.549862 nhs_aws_helpers-0.1.1/tests/utils.py
+-rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.1.1/PKG-INFO
```

### Comparing `nhs_aws_helpers-0.0.17/LICENSE.md` & `nhs_aws_helpers-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/README.md` & `nhs_aws_helpers-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/nhs_aws_helpers/__init__.py` & `nhs_aws_helpers-0.1.1/nhs_aws_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/nhs_aws_helpers/async_s3_object_reader.py` & `nhs_aws_helpers-0.1.1/nhs_aws_helpers/async_s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/nhs_aws_helpers/async_s3_object_writer.py` & `nhs_aws_helpers-0.1.1/nhs_aws_helpers/async_s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/nhs_aws_helpers/common.py` & `nhs_aws_helpers-0.1.1/nhs_aws_helpers/common.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/nhs_aws_helpers/fixtures.py` & `nhs_aws_helpers-0.1.1/nhs_aws_helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/nhs_aws_helpers/s3_object_reader.py` & `nhs_aws_helpers-0.1.1/nhs_aws_helpers/s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/nhs_aws_helpers/s3_object_writer.py` & `nhs_aws_helpers-0.1.1/nhs_aws_helpers/s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/pyproject.toml` & `nhs_aws_helpers-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhs_aws_helpers"
-version = "0.0.17"
+version = "0.1.1"
 description = ""
 authors = ["spinecore"]
 license = "MIT"
 packages = [
     { include = "nhs_aws_helpers" },
     { include = "tests", format = "sdist" },
 ]
```

### Comparing `nhs_aws_helpers-0.0.17/tests/async_s3_object_buffer_tests.py` & `nhs_aws_helpers-0.1.1/tests/async_s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/tests/aws_tests.py` & `nhs_aws_helpers-0.1.1/tests/aws_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/tests/s3_object_buffer_tests.py` & `nhs_aws_helpers-0.1.1/tests/s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/tests/utils.py` & `nhs_aws_helpers-0.1.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.0.17/PKG-INFO` & `nhs_aws_helpers-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhs-aws-helpers
-Version: 0.0.17
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: spinecore
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

