# Comparing `tmp/pydefillama-1.0.8.tar.gz` & `tmp/pydefillama-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydefillama-1.0.8.tar", last modified: Wed Apr 26 19:10:17 2023, max compression
+gzip compressed data, was "pydefillama-1.0.9.tar", last modified: Mon Jun 26 18:59:44 2023, max compression
```

## Comparing `pydefillama-1.0.8.tar` & `pydefillama-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.583180 pydefillama-1.0.8/
--rw-r--r--   0 nirmal     (501) staff       (20)     1064 2023-04-25 14:06:51.000000 pydefillama-1.0.8/LICENSE
--rw-r--r--   0 nirmal     (501) staff       (20)     2307 2023-04-26 19:10:17.583050 pydefillama-1.0.8/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)     2011 2023-04-26 19:10:13.000000 pydefillama-1.0.8/README.md
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.580437 pydefillama-1.0.8/pydefillama/
--rw-r--r--   0 nirmal     (501) staff       (20)       41 2023-04-25 15:59:53.000000 pydefillama-1.0.8/pydefillama/__init__.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.582426 pydefillama-1.0.8/pydefillama/src/
--rw-r--r--   0 nirmal     (501) staff       (20)       23 2023-04-25 16:01:08.000000 pydefillama-1.0.8/pydefillama/src/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)     5910 2023-04-26 19:10:13.000000 pydefillama-1.0.8/pydefillama/src/fetcher.py
--rw-r--r--   0 nirmal     (501) staff       (20)      110 2023-04-25 14:30:17.000000 pydefillama-1.0.8/pydefillama/src/utils.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.582849 pydefillama-1.0.8/pydefillama/tests/
--rw-r--r--   0 nirmal     (501) staff       (20)       29 2023-04-25 16:07:05.000000 pydefillama-1.0.8/pydefillama/tests/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)     3658 2023-04-26 19:10:13.000000 pydefillama-1.0.8/pydefillama/tests/fetcher_tests.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.581805 pydefillama-1.0.8/pydefillama.egg-info/
--rw-r--r--   0 nirmal     (501) staff       (20)     2307 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)      403 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/SOURCES.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/dependency_links.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-25 14:46:30.000000 pydefillama-1.0.8/pydefillama.egg-info/not-zip-safe
--rw-r--r--   0 nirmal     (501) staff       (20)       28 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/requires.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       12 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/top_level.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       38 2023-04-26 19:10:17.583219 pydefillama-1.0.8/setup.cfg
--rw-r--r--   0 nirmal     (501) staff       (20)      717 2023-04-26 19:10:13.000000 pydefillama-1.0.8/setup.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-26 18:59:44.416916 pydefillama-1.0.9/
+-rw-r--r--   0 nirmal     (501) staff       (20)     1064 2023-04-25 14:06:51.000000 pydefillama-1.0.9/LICENSE
+-rw-r--r--   0 nirmal     (501) staff       (20)     2307 2023-06-26 18:59:44.416790 pydefillama-1.0.9/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)     2011 2023-04-26 19:10:13.000000 pydefillama-1.0.9/README.md
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-26 18:59:44.414728 pydefillama-1.0.9/pydefillama/
+-rw-r--r--   0 nirmal     (501) staff       (20)       41 2023-04-25 15:59:53.000000 pydefillama-1.0.9/pydefillama/__init__.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-26 18:59:44.416096 pydefillama-1.0.9/pydefillama/src/
+-rw-r--r--   0 nirmal     (501) staff       (20)       23 2023-04-25 16:01:08.000000 pydefillama-1.0.9/pydefillama/src/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)     6443 2023-06-26 18:58:34.000000 pydefillama-1.0.9/pydefillama/src/fetcher.py
+-rw-r--r--   0 nirmal     (501) staff       (20)      110 2023-04-25 14:30:17.000000 pydefillama-1.0.9/pydefillama/src/utils.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-26 18:59:44.416552 pydefillama-1.0.9/pydefillama/tests/
+-rw-r--r--   0 nirmal     (501) staff       (20)       29 2023-04-25 16:07:05.000000 pydefillama-1.0.9/pydefillama/tests/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)     3658 2023-04-26 19:10:13.000000 pydefillama-1.0.9/pydefillama/tests/fetcher_tests.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-26 18:59:44.415584 pydefillama-1.0.9/pydefillama.egg-info/
+-rw-r--r--   0 nirmal     (501) staff       (20)     2307 2023-06-26 18:59:44.000000 pydefillama-1.0.9/pydefillama.egg-info/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)      403 2023-06-26 18:59:44.000000 pydefillama-1.0.9/pydefillama.egg-info/SOURCES.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-06-26 18:59:44.000000 pydefillama-1.0.9/pydefillama.egg-info/dependency_links.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-25 14:46:30.000000 pydefillama-1.0.9/pydefillama.egg-info/not-zip-safe
+-rw-r--r--   0 nirmal     (501) staff       (20)       28 2023-06-26 18:59:44.000000 pydefillama-1.0.9/pydefillama.egg-info/requires.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       12 2023-06-26 18:59:44.000000 pydefillama-1.0.9/pydefillama.egg-info/top_level.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       38 2023-06-26 18:59:44.416951 pydefillama-1.0.9/setup.cfg
+-rw-r--r--   0 nirmal     (501) staff       (20)      717 2023-06-26 18:59:28.000000 pydefillama-1.0.9/setup.py
```

### Comparing `pydefillama-1.0.8/LICENSE` & `pydefillama-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydefillama-1.0.8/PKG-INFO` & `pydefillama-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydefillama
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Wrapper for DefiLlama endpoints
 Home-page: https://github.com/Artemis-xyz/DefiLlama-Python-Client
 Author: Artemis.xyz
 Author-email: team@artemis.xyz
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pydefillama-1.0.8/README.md` & `pydefillama-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pydefillama-1.0.8/pydefillama/src/fetcher.py` & `pydefillama-1.0.9/pydefillama/src/fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import numpy as np
 import pandas as pd
 import requests
 
 from .utils import FEE_TYPE
 
-# TODO: Add docstrings
-
 
 def _convert_df_column_to_date(
     df, date_column="date", format=None, unit=None
 ) -> pd.DataFrame:
     if unit is not None:
         df[date_column] = pd.to_datetime(df[date_column], unit=unit)
     elif format is not None:
@@ -40,25 +38,40 @@
     r = requests.get(url)
     raw_protocols = r.json()
     protocols_keys_kept = [
         _transform_raw_protocol(raw_protocol) for raw_protocol in raw_protocols
     ]
     return protocols_keys_kept
 
+# DefiLlama API sometimes has missing dates in their data
+# This function fills in the missing dates with the previous date's value
+def _forward_fill_missing_dates(df: pd.DataFrame, date_column: str) -> pd.DataFrame:
+    all_columns = df.columns
+    df = df.sort_values(date_column)
+    df = df.set_index(date_column)
+    min_date = df.index.min()
+    max_date = df.index.max()
+    date_range = pd.date_range(min_date, max_date)
+    df = df.reindex(date_range)
+    df = df.ffill().reset_index()
+    df.columns = all_columns
+    return df
+
+
 
 def fetch_protocol_tvl(protocol_slug: str) -> pd.DataFrame:
     url = f"https://api.llama.fi/protocol/{protocol_slug}"
     r = requests.get(url)
     data = r.json()
     df = pd.DataFrame(data["tvl"])
     df.columns = ["date", "tvl"]
     df = _convert_df_column_to_date(df, unit="s")
     # get latest for each date
     df = df.groupby("date").max().reset_index()
-    df = df.sort_values("date")
+    df = _forward_fill_missing_dates(df, "date")
     return df
 
 
 def fetch_all_chains() -> list[dict]:
     def _transform_raw_chain(raw_chain):
         return {
             "gecko_id": raw_chain.get("gecko_id"),
```

### Comparing `pydefillama-1.0.8/pydefillama/tests/fetcher_tests.py` & `pydefillama-1.0.9/pydefillama/tests/fetcher_tests.py`

 * *Files identical despite different names*

### Comparing `pydefillama-1.0.8/pydefillama.egg-info/PKG-INFO` & `pydefillama-1.0.9/pydefillama.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydefillama
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Wrapper for DefiLlama endpoints
 Home-page: https://github.com/Artemis-xyz/DefiLlama-Python-Client
 Author: Artemis.xyz
 Author-email: team@artemis.xyz
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pydefillama-1.0.8/setup.py` & `pydefillama-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("requirements.txt", "r") as requirements_file:
     requirements_text = requirements_file.read()
 
 requirements = requirements_text.split()
 
 setuptools.setup(
     name="pydefillama",
-    version="1.0.8",
+    version="1.0.9",
     description="Python Wrapper for DefiLlama endpoints",
     url="https://github.com/Artemis-xyz/DefiLlama-Python-Client",
     author="Artemis.xyz",
     author_email="team@artemis.xyz",
     license="MIT",
     packages=setuptools.find_packages(exclude="tests"),
     zip_safe=False,
```

