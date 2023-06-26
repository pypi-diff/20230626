# Comparing `tmp/pypomes-0.1.8.tar.gz` & `tmp/pypomes-0.1.9.tar.gz`

## Comparing `pypomes-0.1.8.tar` & `pypomes-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.8/requirements.txt
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/__init__.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/azure_pomes.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/crypto_pomes.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/datetime_pomes.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/db_pomes.py
--rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/dict_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/encoding_pomes.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/file_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/json_pomes.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/list_pomes.py
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/logging_pomes.py
--rw-r--r--   0        0        0    10498 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/minio_pomes.py
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/soap_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/str_pomes.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/xml_pomes.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.8/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.9/requirements.txt
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/__init__.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/azure_pomes.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/crypto_pomes.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/datetime_pomes.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/db_pomes.py
+-rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/dict_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/encoding_pomes.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/file_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/json_pomes.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/list_pomes.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/logging_pomes.py
+-rw-r--r--   0        0        0    10498 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/minio_pomes.py
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/soap_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/str_pomes.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/xml_pomes.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.9/README.md
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 pypomes-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pypomes-0.1.9/PKG-INFO
```

### Comparing `pypomes-0.1.8/src/pypomes/__init__.py` & `pypomes-0.1.9/src/pypomes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,9 +100,9 @@
     soap_post, soap_post_zeep, soap_get_attachment, soap_get_dict, soap_get_cids, soap_build_envelope,
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.8"
-__version_info__ = (0, 1, 8)
+__version__ = "0.1.9"
+__version_info__ = (0, 1, 9)
```

### Comparing `pypomes-0.1.8/src/pypomes/azure_pomes.py` & `pypomes-0.1.9/src/pypomes/azure_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/crypto_pomes.py` & `pypomes-0.1.9/src/pypomes/crypto_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/datetime_pomes.py` & `pypomes-0.1.9/src/pypomes/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/db_pomes.py` & `pypomes-0.1.9/src/pypomes/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/dict_pomes.py` & `pypomes-0.1.9/src/pypomes/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/encoding_pomes.py` & `pypomes-0.1.9/src/pypomes/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/env_pomes.py` & `pypomes-0.1.9/src/pypomes/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/exception_pomes.py` & `pypomes-0.1.9/src/pypomes/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/file_pomes.py` & `pypomes-0.1.9/src/pypomes/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/json_pomes.py` & `pypomes-0.1.9/src/pypomes/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/list_pomes.py` & `pypomes-0.1.9/src/pypomes/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/logging_pomes.py` & `pypomes-0.1.9/src/pypomes/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/minio_pomes.py` & `pypomes-0.1.9/src/pypomes/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/soap_pomes.py` & `pypomes-0.1.9/src/pypomes/soap_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/str_pomes.py` & `pypomes-0.1.9/src/pypomes/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/src/pypomes/xml_pomes.py` & `pypomes-0.1.9/src/pypomes/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/LICENSE` & `pypomes-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.8/pyproject.toml` & `pypomes-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 [build-system]
 requires = [
-    "hatchling",
+    "hatchling"
+]
+build-backend = "hatchling.build"
+
+[project]
+name = "pypomes"
+version = "0.1.9"
+authors = [
+  { name="GT Nunes", email="wisecoder01@gmail.com" },
+]
+description = "A collection of Python pomes, pennyeach"
+readme = "README.md"
+requires-python = ">=3.10"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
     "asn1crypto>=1.5.1",
     "azure-common>=1.1.28",
     "azure-core>=1.26.4",
     "azure-identity>=1.13.0",
     "azure-storage-blob>=12.16.0",
     "cryptography>=41.0.1",
     "Flask>=2.3.2",
@@ -17,27 +35,10 @@
     "setuptools>=67.8.0",
     "Unidecode>=1.3.6",
     "Werkzeug>=2.3.6",
     "wheel>=0.40.0",
     "xmltodict3>=0.0.4",
     "zeep>=4.2.1"
 ]
-build-backend = "hatchling.build"
-
-[project]
-name = "pypomes"
-version = "0.1.8"
-authors = [
-  { name="GT Nunes", email="wisecoder01@gmail.com" },
-]
-description = "A collection of Python pomes, pennyeach"
-readme = "README.md"
-requires-python = ">=3.10"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes/issues"
```

