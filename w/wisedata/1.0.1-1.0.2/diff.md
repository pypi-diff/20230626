# Comparing `tmp/wisedata-1.0.1.tar.gz` & `tmp/wisedata-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisedata-1.0.1.tar", max compression
+gzip compressed data, was "wisedata-1.0.2.tar", max compression
```

## Comparing `wisedata-1.0.1.tar` & `wisedata-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.1/LICENSE
--rw-r--r--   0        0        0     6743 2023-06-26 13:59:59.003655 wisedata-1.0.1/README.md
--rw-r--r--   0        0        0      588 2023-06-26 14:00:27.109458 wisedata-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8384 2023-06-26 12:19:30.469356 wisedata-1.0.1/wisedata/__init__.py
--rw-r--r--   0        0        0      704 2023-06-26 12:18:32.144558 wisedata-1.0.1/wisedata/exceptions.py
--rw-r--r--   0        0        0     7300 1970-01-01 00:00:00.000000 wisedata-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.2/LICENSE
+-rw-r--r--   0        0        0     9983 2023-06-26 15:21:51.504859 wisedata-1.0.2/README.md
+-rw-r--r--   0        0        0      588 2023-06-26 15:22:34.215462 wisedata-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8361 2023-06-26 15:18:56.202009 wisedata-1.0.2/wisedata/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-26 12:18:32.144558 wisedata-1.0.2/wisedata/exceptions.py
+-rw-r--r--   0        0        0    10540 1970-01-01 00:00:00.000000 wisedata-1.0.2/PKG-INFO
```

### Comparing `wisedata-1.0.1/LICENSE` & `wisedata-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.1/pyproject.toml` & `wisedata-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wisedata"
-version = "1.0.1"
+version = "1.0.2"
 description = "AI Assistant for Python Data Analytics"
 authors = ["WiseData Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `wisedata-1.0.1/wisedata/__init__.py` & `wisedata-1.0.2/wisedata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     import pandas as pd
     import numpy as np
     globals = { "np": np, "pd": pd }
     locals = dataframes.copy()
     try:
       exec(python_code, globals, locals)
       if isinstance(locals["return_df"], pd.DataFrame):
-        return_df=locals["return_df"].reset_index(drop=True)
+        return_df=locals["return_df"]
         if code: logging.info(f"Given prompt: \n{prompt} \nOutput code: \n{python_code}\n")
       else:
         num_retries += 1
         data["error"] = "Is not a pandas dataframe. Please return dataframe."
         return_df = self._transform(prompt, dataframes, error=data["error"], code=code, num_retries=num_retries, prev_code=python_code)
     except Exception as e:
       num_retries += 1
```

### Comparing `wisedata-1.0.1/wisedata/exceptions.py` & `wisedata-1.0.2/wisedata/exceptions.py`

 * *Files identical despite different names*

