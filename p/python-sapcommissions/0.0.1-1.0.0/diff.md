# Comparing `tmp/python-sapcommissions-0.0.1.tar.gz` & `tmp/python-sapcommissions-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sapcommissions-0.0.1.tar", last modified: Mon Jun 26 21:00:40 2023, max compression
+gzip compressed data, was "python-sapcommissions-1.0.0.tar", last modified: Mon Jun 26 21:16:31 2023, max compression
```

## Comparing `python-sapcommissions-0.0.1.tar` & `python-sapcommissions-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 21:00:40.602370 python-sapcommissions-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-26 20:02:48.000000 python-sapcommissions-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    17698 2023-06-26 21:00:40.590370 python-sapcommissions-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 21:00:40.484371 python-sapcommissions-0.0.1/docs/
--rw-rw-rw-   0        0        0    16952 2023-06-26 20:34:26.000000 python-sapcommissions-0.0.1/docs/README.md
--rw-rw-rw-   0        0        0     1265 2023-06-26 21:00:15.000000 python-sapcommissions-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-26 21:00:40.557372 python-sapcommissions-0.0.1/python_sapcommissions.egg-info/
--rw-rw-rw-   0        0        0    17698 2023-06-26 21:00:40.000000 python-sapcommissions-0.0.1/python_sapcommissions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-06-26 21:00:40.000000 python-sapcommissions-0.0.1/python_sapcommissions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 21:00:40.000000 python-sapcommissions-0.0.1/python_sapcommissions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-26 21:00:40.000000 python-sapcommissions-0.0.1/python_sapcommissions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-26 21:00:40.000000 python-sapcommissions-0.0.1/python_sapcommissions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 21:00:40.575370 python-sapcommissions-0.0.1/sapcommissions/
--rw-rw-rw-   0        0        0      922 2023-06-26 20:08:46.000000 python-sapcommissions-0.0.1/sapcommissions/__init__.py
--rw-rw-rw-   0        0        0    25310 2023-06-26 19:40:12.000000 python-sapcommissions-0.0.1/sapcommissions/endpoints.py
--rw-rw-rw-   0        0        0      469 2023-06-26 10:08:08.000000 python-sapcommissions-0.0.1/sapcommissions/exceptions.py
--rw-rw-rw-   0        0        0   114226 2023-06-26 11:52:36.000000 python-sapcommissions-0.0.1/sapcommissions/resources.py
--rw-rw-rw-   0        0        0       42 2023-06-26 21:00:40.602370 python-sapcommissions-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-05-17 08:27:22.000000 python-sapcommissions-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 21:00:40.588369 python-sapcommissions-0.0.1/tests/
--rw-rw-rw-   0        0        0     2411 2023-06-26 20:01:52.000000 python-sapcommissions-0.0.1/tests/test_base.py
--rw-rw-rw-   0        0        0    11948 2023-06-26 19:35:30.000000 python-sapcommissions-0.0.1/tests/test_endpoints.py
--rw-rw-rw-   0        0        0     4560 2023-06-26 19:50:02.000000 python-sapcommissions-0.0.1/tests/test_resources.py
+drwxrwxrwx   0        0        0        0 2023-06-26 21:16:31.051707 python-sapcommissions-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-26 20:02:48.000000 python-sapcommissions-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    17535 2023-06-26 21:16:31.038609 python-sapcommissions-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 21:16:30.922087 python-sapcommissions-1.0.0/docs/
+-rw-rw-rw-   0        0        0    16952 2023-06-26 20:34:26.000000 python-sapcommissions-1.0.0/docs/README.md
+-rw-rw-rw-   0        0        0     1118 2023-06-26 21:15:12.000000 python-sapcommissions-1.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-26 21:16:30.946088 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/
+-rw-rw-rw-   0        0        0    17535 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-26 21:16:30.000000 python-sapcommissions-1.0.0/python_sapcommissions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 21:16:30.993292 python-sapcommissions-1.0.0/sapcommissions/
+-rw-rw-rw-   0        0        0      922 2023-06-26 20:08:46.000000 python-sapcommissions-1.0.0/sapcommissions/__init__.py
+-rw-rw-rw-   0        0        0    25310 2023-06-26 19:40:12.000000 python-sapcommissions-1.0.0/sapcommissions/endpoints.py
+-rw-rw-rw-   0        0        0      469 2023-06-26 10:08:08.000000 python-sapcommissions-1.0.0/sapcommissions/exceptions.py
+-rw-rw-rw-   0        0        0   114226 2023-06-26 11:52:36.000000 python-sapcommissions-1.0.0/sapcommissions/resources.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 21:16:31.051707 python-sapcommissions-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-05-17 08:27:22.000000 python-sapcommissions-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 21:16:31.035611 python-sapcommissions-1.0.0/tests/
+-rw-rw-rw-   0        0        0     2411 2023-06-26 20:01:52.000000 python-sapcommissions-1.0.0/tests/test_base.py
+-rw-rw-rw-   0        0        0    11948 2023-06-26 19:35:30.000000 python-sapcommissions-1.0.0/tests/test_endpoints.py
+-rw-rw-rw-   0        0        0     4560 2023-06-26 19:50:02.000000 python-sapcommissions-1.0.0/tests/test_resources.py
```

### Comparing `python-sapcommissions-0.0.1/LICENSE` & `python-sapcommissions-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-0.0.1/PKG-INFO` & `python-sapcommissions-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-sapcommissions
-Version: 0.0.1
+Version: 1.0.0
 Summary: A Python wrapper for the SAP Commissions API
 Author-email: Niels Perfors <niels.perfors1987@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
-Project-URL: Bug Tracker, https://github.com/niro1987/python-sapcommissions/issues
-Project-URL: Documentation, https://github.com/niro1987/python-sapcommissions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `python-sapcommissions-0.0.1/docs/README.md` & `python-sapcommissions-1.0.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-0.0.1/pyproject.toml` & `python-sapcommissions-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "python-sapcommissions"
 description = "A Python wrapper for the SAP Commissions API"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
     {name = "Niels Perfors", email = "niels.perfors1987@gmail.com"},
 ]
 license = {text = "MIT"}
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -22,16 +22,14 @@
     "requests ~= 2.31.0",
 ]
 readme = "docs/README.md"
 
 
 [project.urls]
 "Homepage" = "https://github.com/niro1987/python-sapcommissions"
-"Bug Tracker" = "https://github.com/niro1987/python-sapcommissions/issues"
-"Documentation" = "https://github.com/niro1987/python-sapcommissions"
 
 
 [tool.setuptools.packages.find]
 exclude = [
     "tests",
 ]
```

### Comparing `python-sapcommissions-0.0.1/python_sapcommissions.egg-info/PKG-INFO` & `python-sapcommissions-1.0.0/python_sapcommissions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-sapcommissions
-Version: 0.0.1
+Version: 1.0.0
 Summary: A Python wrapper for the SAP Commissions API
 Author-email: Niels Perfors <niels.perfors1987@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
-Project-URL: Bug Tracker, https://github.com/niro1987/python-sapcommissions/issues
-Project-URL: Documentation, https://github.com/niro1987/python-sapcommissions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `python-sapcommissions-0.0.1/sapcommissions/__init__.py` & `python-sapcommissions-1.0.0/sapcommissions/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-0.0.1/sapcommissions/endpoints.py` & `python-sapcommissions-1.0.0/sapcommissions/endpoints.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-0.0.1/sapcommissions/resources.py` & `python-sapcommissions-1.0.0/sapcommissions/resources.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-0.0.1/tests/test_base.py` & `python-sapcommissions-1.0.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-0.0.1/tests/test_endpoints.py` & `python-sapcommissions-1.0.0/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-0.0.1/tests/test_resources.py` & `python-sapcommissions-1.0.0/tests/test_resources.py`

 * *Files identical despite different names*

