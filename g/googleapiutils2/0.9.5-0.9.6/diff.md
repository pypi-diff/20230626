# Comparing `tmp/googleapiutils2-0.9.5.tar.gz` & `tmp/googleapiutils2-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.9.5.tar", max compression
+gzip compressed data, was "googleapiutils2-0.9.6.tar", max compression
```

## Comparing `googleapiutils2-0.9.5.tar` & `googleapiutils2-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.9.5/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.9.5/README.md
--rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.9.5/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.9.5/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    22040 2023-06-09 19:21:45.977910 googleapiutils2-0.9.5/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-06-07 16:12:16.848980 googleapiutils2-0.9.5/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.9.5/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.9.5/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.9.5/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.9.5/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     9618 2023-06-02 19:09:36.958908 googleapiutils2-0.9.5/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    33736 2023-06-07 18:16:28.569445 googleapiutils2-0.9.5/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.9.5/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     9430 2023-06-07 18:49:59.814378 googleapiutils2-0.9.5/googleapiutils2/utils.py
--rw-r--r--   0        0        0     1089 2023-06-09 19:22:10.168691 googleapiutils2-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.9.6/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.9.6/README.md
+-rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.9.6/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.9.6/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    22040 2023-06-09 19:21:45.977910 googleapiutils2-0.9.6/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-06-07 16:12:16.848980 googleapiutils2-0.9.6/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.9.6/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.9.6/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.9.6/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.9.6/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     9618 2023-06-02 19:09:36.958908 googleapiutils2-0.9.6/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    33756 2023-06-26 15:13:33.966370 googleapiutils2-0.9.6/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.9.6/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     9430 2023-06-07 18:49:59.814378 googleapiutils2-0.9.6/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1089 2023-06-26 15:14:06.883891 googleapiutils2-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.9.6/PKG-INFO
```

### Comparing `googleapiutils2-0.9.5/LICENSE` & `googleapiutils2-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.5/README.md` & `googleapiutils2-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.5/googleapiutils2/drive/drive.py` & `googleapiutils2-0.9.6/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.5/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.9.6/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.5/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.9.6/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.5/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.9.6/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.5/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.9.6/googleapiutils2/sheets/sheets.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             )
             self._cache[(spreadsheet_id, sheet_name)] = list(header)
 
         frame = frame.reindex(columns=header)
         values = frame.fillna("").values.tolist()
 
         # insert the header if the range starts at the first row
-        if insert_header and row_slc.start == 1:
+        if not len(header) and insert_header and row_slc.start == 1:
             values.insert(0, header.tolist())
 
         return values
 
     def _process_sheets_values(
         self,
         spreadsheet_id: str,
```

### Comparing `googleapiutils2-0.9.5/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.9.6/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.5/googleapiutils2/utils.py` & `googleapiutils2-0.9.6/googleapiutils2/utils.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.5/pyproject.toml` & `googleapiutils2-0.9.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.9.5"
+version = "0.9.6"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.2"
-mypy = "^1.3.0"
+mypy = "^1.4.1"
 google-api-python-client-stubs = "^1.17.0"
-google-api-python-client = "^2.88.0"
+google-api-python-client = "^2.90.0"
 google-auth-oauthlib = "^1.0.0"
 requests = "^2.31.0"
 cachetools = "^5.3.1"
 google-auth-httplib2 = "^0.1.0"
-google-auth = "^2.19.1"
+google-auth = "^2.20.0"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.31.0.1"
 types-cachetools = "^5.3.0.5"
-pytest = "^7.3.1"
+pytest = "^7.4.0"
 pandas-stubs = "^2.0.2.230605"
 black = "^23.3.0"
 
 [tool.mypy]
 python_version = "3.10"
 warn_return_any = false
 warn_unused_configs = false
```

### Comparing `googleapiutils2-0.9.5/PKG-INFO` & `googleapiutils2-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.9.5
+Version: 0.9.6
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
-Requires-Dist: google-api-python-client (>=2.88.0,<3.0.0)
+Requires-Dist: google-api-python-client (>=2.90.0,<3.0.0)
 Requires-Dist: google-api-python-client-stubs (>=1.17.0,<2.0.0)
-Requires-Dist: google-auth (>=2.19.1,<3.0.0)
+Requires-Dist: google-auth (>=2.20.0,<3.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
 Requires-Dist: google-auth-oauthlib (>=1.0.0,<2.0.0)
-Requires-Dist: mypy (>=1.3.0,<2.0.0)
+Requires-Dist: mypy (>=1.4.1,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/mkbabb/googleapiutils2
 Description-Content-Type: text/markdown
 
 # googleapiutils2
```

