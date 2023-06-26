# Comparing `tmp/ctd-python-0.1.2.tar.gz` & `tmp/ctd-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctd-python-0.1.2.tar", last modified: Mon Jun 26 01:55:21 2023, max compression
+gzip compressed data, was "ctd-python-0.1.3.tar", last modified: Mon Jun 26 02:00:00 2023, max compression
```

## Comparing `ctd-python-0.1.2.tar` & `ctd-python-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:55:21.564485 ctd-python-0.1.2/
--rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 01:55:21.563845 ctd-python-0.1.2/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      887 2023-06-26 01:02:36.000000 ctd-python-0.1.2/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:55:21.555886 ctd-python-0.1.2/ctd/
--rw-r--r--   0 john       (501) staff       (20)       31 2023-06-26 00:20:15.000000 ctd-python-0.1.2/ctd/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     3379 2023-06-26 01:55:04.000000 ctd-python-0.1.2/ctd/get_data.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:55:21.557504 ctd-python-0.1.2/ctd/unzipped_data/
--rw-r--r--   0 john       (501) staff       (20)        0 2023-06-25 23:36:26.000000 ctd-python-0.1.2/ctd/unzipped_data/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     1072 2023-06-26 00:49:30.000000 ctd-python-0.1.2/ctd/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:55:21.563220 ctd-python-0.1.2/ctd_python.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      262 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       21 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        4 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-06-26 01:55:21.564628 ctd-python-0.1.2/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      544 2023-06-26 01:55:19.000000 ctd-python-0.1.2/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 02:00:00.430099 ctd-python-0.1.3/
+-rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 02:00:00.429691 ctd-python-0.1.3/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      887 2023-06-26 01:02:36.000000 ctd-python-0.1.3/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 02:00:00.425668 ctd-python-0.1.3/ctd/
+-rw-r--r--   0 john       (501) staff       (20)       31 2023-06-26 00:20:15.000000 ctd-python-0.1.3/ctd/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     3333 2023-06-26 01:59:46.000000 ctd-python-0.1.3/ctd/get_data.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 02:00:00.426596 ctd-python-0.1.3/ctd/unzipped_data/
+-rw-r--r--   0 john       (501) staff       (20)        0 2023-06-25 23:36:26.000000 ctd-python-0.1.3/ctd/unzipped_data/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     1072 2023-06-26 00:49:30.000000 ctd-python-0.1.3/ctd/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 02:00:00.429084 ctd-python-0.1.3/ctd_python.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      262 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       21 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        4 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-06-26 02:00:00.430351 ctd-python-0.1.3/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      544 2023-06-26 01:59:57.000000 ctd-python-0.1.3/setup.py
```

### Comparing `ctd-python-0.1.2/PKG-INFO` & `ctd-python-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.1.2/README.md` & `ctd-python-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ctd-python-0.1.2/ctd/get_data.py` & `ctd-python-0.1.3/ctd/get_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import os
+import io
 import gzip
 import shutil
 import logging
 import requests
 from tqdm import tqdm
 import pandas as pd
 
 PACKAGE_DIR = os.path.dirname(__file__)
 RAW_DATA_DIR = os.path.join(PACKAGE_DIR, 'unzipped_data')
 
-from tqdm import tqdm
-
-from tqdm import tqdm
-import io
 
 def download_resource(resource: str) -> str:
     url_dl_pattern = 'http://ctdbase.org/reports/{resource}.csv.gz'
     url = url_dl_pattern.format(resource=resource)
 
     logging.info('[download_resource]: downloading: %s', resource)
-    local_filename = os.path.join(RAW_DATA_DIR, url.split('/')[-1])
+    local_filename = os.path.join(RAW_DATA_DIR, f"{resource}.csv")
 
     ## TODO - make this a config to refresh
     ## perhaps even add the date of the file created so we can dl new
     ## files when they come in
     if os.path.isfile(local_filename):
         return local_filename
```

### Comparing `ctd-python-0.1.2/ctd/utils.py` & `ctd-python-0.1.3/ctd/utils.py`

 * *Files identical despite different names*

### Comparing `ctd-python-0.1.2/ctd_python.egg-info/PKG-INFO` & `ctd-python-0.1.3/ctd_python.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.1.2/setup.py` & `ctd-python-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='ctd-python',
-    version='0.1.2',
+    version='0.1.3',
     description='Python interface to access data from The Comparative Toxicogenomics Database (CTD)',
     packages=['ctd'],
     install_requires=[
         'requests',
         'pandas',
         'tqdm'
     ],
```

