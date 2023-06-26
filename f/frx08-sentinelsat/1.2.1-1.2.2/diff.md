# Comparing `tmp/frx08-sentinelsat-1.2.1.tar.gz` & `tmp/frx08-sentinelsat-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frx08-sentinelsat-1.2.1.tar", last modified: Mon Jun 26 09:27:03 2023, max compression
+gzip compressed data, was "frx08-sentinelsat-1.2.2.tar", last modified: Mon Jun 26 09:30:45 2023, max compression
```

## Comparing `frx08-sentinelsat-1.2.1.tar` & `frx08-sentinelsat-1.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:27:03.714208 frx08-sentinelsat-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-26 09:27:03.714208 frx08-sentinelsat-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:27:03.710208 frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-26 09:27:03.000000 frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 09:27:03.000000 frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:27:03.000000 frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 09:27:03.000000 frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 09:27:03.000000 frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 09:27:03.000000 frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:27:03.000000 frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:27:03.710208 frx08-sentinelsat-1.2.1/sentinelsat/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/sentinelsat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/sentinelsat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31813 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/sentinelsat/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/sentinelsat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/sentinelsat/products.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:27:03.710208 frx08-sentinelsat-1.2.1/sentinelsat/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/sentinelsat/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/sentinelsat/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    57113 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/sentinelsat/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 09:27:03.714208 frx08-sentinelsat-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-26 09:26:53.000000 frx08-sentinelsat-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:27:03.714208 frx08-sentinelsat-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21441 2023-06-26 09:26:54.000000 frx08-sentinelsat-1.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-26 09:26:54.000000 frx08-sentinelsat-1.2.1/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-06-26 09:26:54.000000 frx08-sentinelsat-1.2.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-26 09:26:54.000000 frx08-sentinelsat-1.2.1/tests/test_geographic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-26 09:26:54.000000 frx08-sentinelsat-1.2.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-26 09:26:54.000000 frx08-sentinelsat-1.2.1/tests/test_odata.py
--rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-06-26 09:26:54.000000 frx08-sentinelsat-1.2.1/tests/test_opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-26 09:26:54.000000 frx08-sentinelsat-1.2.1/tests/test_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:30:45.469917 frx08-sentinelsat-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-26 09:30:45.469917 frx08-sentinelsat-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:30:45.465917 frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-26 09:30:45.000000 frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 09:30:45.000000 frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:30:45.000000 frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 09:30:45.000000 frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 09:30:45.000000 frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 09:30:45.000000 frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:30:45.000000 frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:30:45.469917 frx08-sentinelsat-1.2.2/sentinelsat/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/sentinelsat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/sentinelsat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31813 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/sentinelsat/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/sentinelsat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/sentinelsat/products.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:30:45.469917 frx08-sentinelsat-1.2.2/sentinelsat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/sentinelsat/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/sentinelsat/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57113 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/sentinelsat/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 09:30:45.473917 frx08-sentinelsat-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:30:45.469917 frx08-sentinelsat-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21441 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/tests/test_geographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/tests/test_odata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/tests/test_opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-26 09:30:28.000000 frx08-sentinelsat-1.2.2/tests/test_pandas.py
```

### Comparing `frx08-sentinelsat-1.2.1/AUTHORS.rst` & `frx08-sentinelsat-1.2.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/LICENSE` & `frx08-sentinelsat-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/PKG-INFO` & `frx08-sentinelsat-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frx08-sentinelsat
-Version: 1.2.1
+Version: 1.2.2
 Summary: Utility to search and download Copernicus Sentinel satellite images
 Home-page: https://github.com/sentinelsat/sentinelsat
 Author: Kersten Clauss
 Author-email: sentinelsat@krstn.eu
 License: GPLv3+
 Keywords: copernicus,sentinel,esa,satellite,download,GIS
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `frx08-sentinelsat-1.2.1/README.rst` & `frx08-sentinelsat-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/PKG-INFO` & `frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frx08-sentinelsat
-Version: 1.2.1
+Version: 1.2.2
 Summary: Utility to search and download Copernicus Sentinel satellite images
 Home-page: https://github.com/sentinelsat/sentinelsat
 Author: Kersten Clauss
 Author-email: sentinelsat@krstn.eu
 License: GPLv3+
 Keywords: copernicus,sentinel,esa,satellite,download,GIS
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `frx08-sentinelsat-1.2.1/frx08_sentinelsat.egg-info/SOURCES.txt` & `frx08-sentinelsat-1.2.2/frx08_sentinelsat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/sentinelsat/__init__.py` & `frx08-sentinelsat-1.2.2/sentinelsat/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 # Import for backwards-compatibility
 from . import sentinel
 from .exceptions import (
     SentinelAPIError,
     LTAError,
     LTATriggered,
```

### Comparing `frx08-sentinelsat-1.2.1/sentinelsat/download.py` & `frx08-sentinelsat-1.2.2/sentinelsat/download.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/sentinelsat/exceptions.py` & `frx08-sentinelsat-1.2.2/sentinelsat/exceptions.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/sentinelsat/products.py` & `frx08-sentinelsat-1.2.2/sentinelsat/products.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/sentinelsat/scripts/cli.py` & `frx08-sentinelsat-1.2.2/sentinelsat/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/sentinelsat/sentinel.py` & `frx08-sentinelsat-1.2.2/sentinelsat/sentinel.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/setup.py` & `frx08-sentinelsat-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/tests/test_cli.py` & `frx08-sentinelsat-1.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/tests/test_docs.py` & `frx08-sentinelsat-1.2.2/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/tests/test_download.py` & `frx08-sentinelsat-1.2.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/tests/test_geographic.py` & `frx08-sentinelsat-1.2.2/tests/test_geographic.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/tests/test_misc.py` & `frx08-sentinelsat-1.2.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/tests/test_odata.py` & `frx08-sentinelsat-1.2.2/tests/test_odata.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/tests/test_opensearch.py` & `frx08-sentinelsat-1.2.2/tests/test_opensearch.py`

 * *Files identical despite different names*

### Comparing `frx08-sentinelsat-1.2.1/tests/test_pandas.py` & `frx08-sentinelsat-1.2.2/tests/test_pandas.py`

 * *Files identical despite different names*

