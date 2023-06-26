# Comparing `tmp/recurtx-0.0.3.tar.gz` & `tmp/recurtx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurtx-0.0.3.tar", last modified: Sun Jun 25 15:37:14 2023, max compression
+gzip compressed data, was "recurtx-0.0.4.tar", last modified: Mon Jun 26 05:02:58 2023, max compression
```

## Comparing `recurtx-0.0.3.tar` & `recurtx-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 15:37:14.530000 recurtx-0.0.3/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-20 00:32:16.000000 recurtx-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-25 15:37:14.530000 recurtx-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5715 2023-06-25 15:32:39.000000 recurtx-0.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-20 00:32:16.000000 recurtx-0.0.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 15:37:14.530000 recurtx-0.0.3/recurtx/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 01:35:17.000000 recurtx-0.0.3/recurtx/__init__.py
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-25 14:34:01.000000 recurtx-0.0.3/recurtx/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6437 2023-06-25 09:06:46.000000 recurtx-0.0.3/recurtx/pandas.py
--rw-r--r--   0 root         (0) root         (0)     4440 2023-06-25 09:08:00.000000 recurtx-0.0.3/recurtx/polars.py
--rw-r--r--   0 root         (0) root         (0)     3775 2023-06-25 11:34:26.000000 recurtx-0.0.3/recurtx/recur.py
--rw-r--r--   0 root         (0) root         (0)     3000 2023-06-25 12:35:43.000000 recurtx-0.0.3/recurtx/search.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-06-25 11:35:32.000000 recurtx-0.0.3/recurtx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 15:37:14.530000 recurtx-0.0.3/recurtx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      252 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-25 15:37:14.530000 recurtx-0.0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1562 2023-06-25 14:33:22.000000 recurtx-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:02:58.920000 recurtx-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-25 15:44:44.000000 recurtx-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-26 05:02:58.920000 recurtx-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5715 2023-06-25 15:44:44.000000 recurtx-0.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-25 15:44:44.000000 recurtx-0.0.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:02:58.910000 recurtx-0.0.4/recurtx/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 15:44:44.000000 recurtx-0.0.4/recurtx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-25 15:44:44.000000 recurtx-0.0.4/recurtx/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6686 2023-06-26 04:47:34.000000 recurtx-0.0.4/recurtx/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-06-26 04:53:15.000000 recurtx-0.0.4/recurtx/polars.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2023-06-25 15:44:44.000000 recurtx-0.0.4/recurtx/recur.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-26 03:53:38.000000 recurtx-0.0.4/recurtx/search.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-25 15:44:45.000000 recurtx-0.0.4/recurtx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:02:58.920000 recurtx-0.0.4/recurtx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      252 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-26 05:02:58.920000 recurtx-0.0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1562 2023-06-25 15:44:45.000000 recurtx-0.0.4/setup.py
```

### Comparing `recurtx-0.0.3/LICENSE` & `recurtx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.3/PKG-INFO` & `recurtx-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.3/README.md` & `recurtx-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.3/recurtx/__main__.py` & `recurtx-0.0.4/recurtx/__main__.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.3/recurtx/pandas.py` & `recurtx-0.0.4/recurtx/pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 def pandas(
     *paths: str,
     package: str = "pandas",
     read_type: str = None,
     columns: List[str] = None,
     excluding_columns: List[str] = None,
+    filepath_column: str = None,
     join: str = None,
     merge: str = None,
     on: str = None,
     left_on: str = None,
     right_on: str = None,
     left_index: bool = False,
     right_index: bool = False,
@@ -57,14 +58,18 @@
     write_path: str = None,
     **kwargs,
 ):
     """Read and transform tabular files using pandas."""
 
     """Workaround for unexpected behavior of Fire"""
     kwargs.pop("package", None)
+    kwargs.pop("read_type", None)
+    kwargs.pop("columns", None)
+    kwargs.pop("excluding_columns", None)
+    kwargs.pop("filepath_column", None)
     kwargs.pop("join", None)
     kwargs.pop("merge", None)
     kwargs.pop("on", None)
     kwargs.pop("left_on", None)
     kwargs.pop("right_on", None)
     kwargs.pop("left_index", False)
     kwargs.pop("right_index", False)
@@ -119,14 +124,17 @@
         if columns:
             df = df[columns]
         if excluding_columns:
             _columns = df.columns
             _columns = [c for c in _columns if c not in excluding_columns]
             df = df[_columns]
 
+        if filepath_column:
+            df[filepath_column] = path
+
         if query:
             df = df.query(query)
         ls.append(df)
 
     if not ls:
         return
     elif len(ls) == 1:
```

### Comparing `recurtx-0.0.3/recurtx/polars.py` & `recurtx-0.0.4/recurtx/polars.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     "json",
     "ndjson",
     "avro",
     "excel",
     "delta",
 }
 
+TRUE_VALUES = {"", "True", "true", "T", "t", "1"}
+
 
 def activate(
     df,
     fetch: int = None,
     streaming: bool = None,
 ):
     df = (
@@ -31,14 +33,15 @@
 
 
 def polars(
     *paths: str,
     read_type: str = None,
     columns: List[str] = None,
     excluding_columns: List[str] = None,
+    filepath_column: str = None,
     streaming: str = None,  # actually bool
     fetch: int = None,
     join: str = None,
     on: str = None,
     left_on: str = None,
     right_on: str = None,
     suffix: str = "_right",
@@ -53,14 +56,15 @@
 ):
     """Read and transform tabular files using polars."""
 
     """Workaround for unexpected behavior of Fire"""
     kwargs.pop("read_type", None)
     kwargs.pop("columns", None)
     kwargs.pop("excluding_columns", None)
+    kwargs.pop("filepath_column", None)
     kwargs.pop("streaming", None)
     kwargs.pop("fetch", None)
     kwargs.pop("join", None)
     kwargs.pop("on", None)
     kwargs.pop("left_on", None)
     kwargs.pop("right_on", None)
     kwargs.pop("suffix", "_right")
@@ -73,15 +77,15 @@
     kwargs.pop("write_path", None)
 
     _write_type = (
         infer_type(write_type, write_path, DATA_TYPES.union({"markdown"}), polars=True)
         or "csv"
     )
 
-    streaming = streaming in {"", "True", "true", "T", "t", "1"}
+    streaming = streaming in TRUE_VALUES
 
     import polars as pl
 
     ls = []
     for path in paths:
         _read_type = infer_type(read_type, path, DATA_TYPES, polars=True)
         if not _read_type:
@@ -104,14 +108,17 @@
         if excluding_columns:
             if isinstance(excluding_columns, str):
                 excluding_columns = [excluding_columns]
             _columns = df.columns
             _columns = [c for c in _columns if c not in excluding_columns]
             df = df.select(_columns)
 
+        if filepath_column:
+            df = df.with_columns(pl.lit(path).alias(filepath_column))
+
         ls.append(df)
 
     if not ls:
         return
     elif len(ls) == 1:
         df = ls[0]
     elif join is not None:
```

### Comparing `recurtx-0.0.3/recurtx/recur.py` & `recurtx-0.0.4/recurtx/recur.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.3/recurtx/search.py` & `recurtx-0.0.4/recurtx/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 from pathlib import Path
 
 
 def run_search(
+    text: str,
     target: str,
     path: Path,
-    text: str,
     sub: str = None,
     wildcard: str = "*",
+    separator: str = "/",
     verbose: int = 1,
 ):
-    separator: str = ";;"
     assert isinstance(separator, str), str(separator) + ": " + str(type(separator))
 
     if isinstance(target, (list, tuple, set, dict)):
         targets = target
     else:
         assert isinstance(target, str), str(type(target))
         if separator:
@@ -70,55 +70,59 @@
 
 
 def search(
     target: str,
     path: str,
     sub: str = None,
     wildcard: str = "*",
+    separator: str = "/",
     verbose: int = 1,
 ):
     """Search a keyword, which may include wildcards, in the text file content, and optionally substitute (replace)."""
 
     path = Path(path)
     try:
         text = path.read_text()
     except Exception:
         if verbose >= 3:
             raise
         return
 
     text = run_search(
-        target,
-        path,
-        text,
-        sub,
-        wildcard,
-        verbose,
+        text=text,
+        target=target,
+        path=path,
+        sub=sub,
+        wildcard=wildcard,
+        separator=separator,
+        verbose=verbose,
     )
 
     if sub is not None:
         path.write_text(text)
 
 
 def find(
     target: str,
     path: str,
     sub: str = None,
     wildcard: str = "*",
+    separator: str = "/",
     verbose: int = 1,
 ):
     """Find a keyword, which may include wildcards, in the file path, and optionally substitute (replace)."""
 
     text = path
     path = Path(path)
 
     text = run_search(
-        target,
-        path,
-        text,
-        sub,
-        wildcard,
-        verbose,
+        text=text,
+        target=target,
+        path=path,
+        sub=sub,
+        wildcard=wildcard,
+        separator=separator,
+        verbose=verbose,
     )
 
     if sub is not None:
         path.rename(text)
```

### Comparing `recurtx-0.0.3/recurtx/utils.py` & `recurtx-0.0.4/recurtx/utils.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.3/recurtx.egg-info/PKG-INFO` & `recurtx-0.0.4/recurtx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.3/setup.py` & `recurtx-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 long_description = """
 Please see:
 https://github.com/Minyus/recurtx
 """
 
 setup(
     name="recurtx",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(exclude=["tests"]),
     entry_points={"console_scripts": console_scripts},
     install_requires=requires,
     description="CLI to transform text files recursively",
     license="Apache Software License (Apache 2.0)",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

