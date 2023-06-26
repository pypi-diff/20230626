# Comparing `tmp/astropandas-1.1.3.tar.gz` & `tmp/astropandas-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astropandas-1.1.3.tar", last modified: Sat May 28 19:19:44 2022, max compression
+gzip compressed data, was "astropandas-1.2.tar", last modified: Mon Jun 26 14:58:56 2023, max compression
```

## Comparing `astropandas-1.1.3.tar` & `astropandas-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 janluca   (1000) janluca   (1000)        0 2022-05-28 19:19:44.867453 astropandas-1.1.3/
--rw-rw-r--   0 janluca   (1000) janluca   (1000)    35148 2022-05-25 08:28:02.000000 astropandas-1.1.3/LICENSE
--rw-rw-r--   0 janluca   (1000) janluca   (1000)     1501 2022-05-28 19:19:44.867453 astropandas-1.1.3/PKG-INFO
--rw-rw-r--   0 janluca   (1000) janluca   (1000)     1064 2022-05-25 08:28:02.000000 astropandas-1.1.3/README.md
-drwxrwxr-x   0 janluca   (1000) janluca   (1000)        0 2022-05-28 19:19:44.867453 astropandas-1.1.3/astropandas/
--rw-rw-r--   0 janluca   (1000) janluca   (1000)      113 2022-05-25 08:32:23.000000 astropandas-1.1.3/astropandas/__init__.py
--rw-rw-r--   0 janluca   (1000) janluca   (1000)     7186 2022-05-28 19:14:00.000000 astropandas-1.1.3/astropandas/io.py
--rw-rw-r--   0 janluca   (1000) janluca   (1000)    16090 2022-05-25 08:28:02.000000 astropandas-1.1.3/astropandas/match.py
--rw-rw-r--   0 janluca   (1000) janluca   (1000)       21 2022-05-28 19:19:03.000000 astropandas-1.1.3/astropandas/version.py
-drwxrwxr-x   0 janluca   (1000) janluca   (1000)        0 2022-05-28 19:19:44.867453 astropandas-1.1.3/astropandas.egg-info/
--rw-rw-r--   0 janluca   (1000) janluca   (1000)     1501 2022-05-28 19:19:44.000000 astropandas-1.1.3/astropandas.egg-info/PKG-INFO
--rw-rw-r--   0 janluca   (1000) janluca   (1000)      286 2022-05-28 19:19:44.000000 astropandas-1.1.3/astropandas.egg-info/SOURCES.txt
--rw-rw-r--   0 janluca   (1000) janluca   (1000)        1 2022-05-28 19:19:44.000000 astropandas-1.1.3/astropandas.egg-info/dependency_links.txt
--rw-rw-r--   0 janluca   (1000) janluca   (1000)       37 2022-05-28 19:19:44.000000 astropandas-1.1.3/astropandas.egg-info/requires.txt
--rw-rw-r--   0 janluca   (1000) janluca   (1000)       12 2022-05-28 19:19:44.000000 astropandas-1.1.3/astropandas.egg-info/top_level.txt
--rw-rw-r--   0 janluca   (1000) janluca   (1000)       38 2022-05-28 19:19:44.867453 astropandas-1.1.3/setup.cfg
--rw-rw-r--   0 janluca   (1000) janluca   (1000)      877 2022-05-25 08:50:32.000000 astropandas-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:58:56.237604 astropandas-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-26 14:58:44.000000 astropandas-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-26 14:58:56.237604 astropandas-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 14:58:44.000000 astropandas-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:58:56.237604 astropandas-1.2/astropandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 14:58:44.000000 astropandas-1.2/astropandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-26 14:58:44.000000 astropandas-1.2/astropandas/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16090 2023-06-26 14:58:44.000000 astropandas-1.2/astropandas/match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:58:56.237604 astropandas-1.2/astropandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 14:58:44.000000 astropandas-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-26 14:58:56.237604 astropandas-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 14:58:44.000000 astropandas-1.2/setup.py
```

### Comparing `astropandas-1.1.3/LICENSE` & `astropandas-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astropandas-1.1.3/PKG-INFO` & `astropandas-1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: astropandas
-Version: 1.1.3
+Version: 1.2
 Summary: Tools to expand on pandas functionality for astronomical operations.
-Home-page: https://github.com/jlvdb/astropandas
 Author: Jan Luca van den Busch
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+License: GPLv3
+Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # astropandas
 
 Tools to expand on pandas functionality for astronomical applications.
 
@@ -45,9 +45,7 @@
 apd.match(
     left=data1, right=data2,
     ra="RA", dec="DEC",
     threshold=1/3600)
 # If no threshold is provided, it is computed automatically by finding the
 # distance at which the number of matches is almost stationary.
 ```
-
-
```

### Comparing `astropandas-1.1.3/README.md` & `astropandas-1.2/README.md`

 * *Files identical despite different names*

### Comparing `astropandas-1.1.3/astropandas/io.py` & `astropandas-1.2/astropandas/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+from __future__ import annotations
+
 import os
 import sys
 import warnings
+from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 try:
     import fitsio
     _FITSIO = True
 except ImportError:
     import astropy.io.fits
     _FITSIO = False
-    warnings.warn(
-        "astropy.io.fits implementation does not support string type columns")
     # set up data type conversion
     from astropy.io.fits.column import FITS2NUMPY as format_FITS2NUMPY
     format_NUMPY2FITS = dict((v, k) for k, v in format_FITS2NUMPY.items())
 
+if TYPE_CHECKING:
+    from numpy.typing import NDArray
+
 
-def _convert_byteorder(data):
+def _convert_byteorder(data: NDArray) -> NDArray:
     dtype = data.dtype
     # check if the byte order matches the native order, identified by the
     # numpy dtype string representation: little endian = "<" and
     # big endian = ">"
     if dtype.str.startswith(("<", ">")):
         if sys.byteorder == "little":
             dtype = np.dtype("<" + dtype.base.str.strip("><"))
         elif sys.byteorder == "big":
             dtype = np.dtype(">" + dtype.base.str.strip("><"))
     return data.astype(dtype, casting="equiv", copy=False)
 
 
-def get_FITS_format(data):
+def get_FITS_format(data: NDArray) -> str:
     """
     Get a FITS data format string for given a numpy.ndarray.
 
     Parameters:
     -----------
     data : numpy.ndarray
         Data to generate a format string for.
@@ -50,15 +55,20 @@
     except KeyError:
         raise TypeError(
             "cannot convert data of type '{:}' to FITS binary".format(
                 data.dtype))
     return fmt_str
 
 
-def read_fits(fpath, columns=None, hdu=1):
+def read_fits(
+    fpath: str,
+    columns: Sequence[str] | None = None,
+    hdu: int = 1,
+    use_fitsio: bool = _FITSIO
+) -> pd.DataFrame:
     """
     Read a FITS data table into a pandas.DataFrame.
 
     Parameters:
     -----------
     fpath : str
         Path to the FITS file.
@@ -69,45 +79,75 @@
     
     Returns:
     -------
     df : pandas.DataFrame
         Table data converted to a DataFrame instance.
     """
     # load the FITS data
-    if _FITSIO:
+    if use_fitsio:
         fits = fitsio.FITS(fpath)
-        if columns is None:
-            data = fits[hdu][:]
-        else:
-            data = fits[hdu][columns][:]
-        fits.close()
+        try:
+            if columns is None:
+                data = fits[hdu][:]
+            else:
+                data = fits[hdu][columns][:]
+        finally:
+            fits.close()
+
+        # construct the data frame
+        coldata = {}
+        for colname, (dt, _) in data.dtype.fields.items():
+            if len(dt.shape) > 0:
+                warnings.warn(
+                    "dropping multidimensional column '{:}'".format(colname))
+            else:
+                coldata[colname] = _convert_byteorder(data[colname])
+        dataframe = pd.DataFrame(coldata)
+
     else:
         with astropy.io.fits.open(fpath) as fits:
             if columns is None:
-                data = fits[hdu].data
+                # probably better to read data at once but I did not find a good
+                # way to identify and convert string columns correctly to fixed
+                # width
+                columns = fits[hdu].data.dtype.names
+            nrows = fits[hdu].data.shape[0]
+            vals = [fits[hdu].data[c] for c in columns]
+            dtype = np.dtype([
+                (c, v.dtype.str) for c, v in zip(columns, vals)])
+            data = np.empty(nrows, dtype=dtype)
+            for c, v in zip(columns, vals):
+                data[c] = v
+
+        # construct the data frame
+        coldata = {}
+        for colname, (dt, _) in data.dtype.fields.items():
+            if dt.kind == "O":
+                coldata[colname] = np.array([
+                    "".join(chars) for chars in data[colname]]).astype("|S")
+            elif len(dt.shape) > 0:
+                warnings.warn(
+                    "dropping multidimensional column '{:}'".format(colname))
             else:
-                nrows = fits[hdu].data.shape[0]
-                vals = [fits[hdu].data[c] for c in columns]
-                dtype = np.dtype([
-                    (c, v.dtype.str) for c, v in zip(columns, vals)])
-                data = np.empty(nrows, dtype=dtype)
-                for c, v in zip(columns, vals):
-                    data[c] = v
-    # construct the data frame
-    coldata = {}
-    for colname, (dt, _) in data.dtype.fields.items():
-        if len(dt.shape) > 0:
-            warnings.warn(
-                "dropping multidimensional column '{:}'".format(colname))
-        else:
-            coldata[colname] = _convert_byteorder(data[colname])
-    return pd.DataFrame(coldata)
+                coldata[colname] = _convert_byteorder(data[colname])
+        dataframe = pd.DataFrame(coldata)
 
+    # convert string types to fixed width (pandas default are py str objects)
+    for colname, values in coldata.items():
+        if values.dtype.kind in "SU":
+            # FITS does not support unicode, use bytes array instead
+            dataframe[colname] = values.astype("|S")
+    return dataframe
 
-def read_auto(fpath, columns=None, ext=None, **kwargs):
+
+def read_auto(
+    fpath: str,
+    columns: Sequence[str] | None = None,
+    **kwargs
+) -> pd.DataFrame:
     """
     Read a file by guessing its type from the extension. Standard parameters
     are used for the pandas.read_xxx() method.
 
     Parameters:
     -----------
     fpath : str
@@ -155,27 +195,31 @@
         return pd.read_pickle(fpath, **kwargs)
     elif ext in (".fits", ".cat"):
         return read_fits(fpath, **kwargs)
     else:
         raise ValueError("unrecognized file extesion '{:}'".format(ext))
 
 
-def to_fits(df, fpath):
+def to_fits(
+    df: pd.DataFrame,
+    fpath: str,
+    use_fitsio: bool = _FITSIO
+) -> None:
     """
     Write a pandas.DataFrame as FITS table file.
 
     Parameters:
     -----------
     df : pandas.DataFrame
         Data frame to write as FITS table.
     fpath : str
         Path to the FITS file.
     """
     # load the FITS data
-    if _FITSIO:
+    if use_fitsio:
         dtype = np.dtype(list(df.dtypes.items()))
         array = np.empty(len(df), dtype=dtype)
         for column in df.columns:
             array[column] = df[column]
         if os.path.exists(fpath):
             os.remove(fpath)
         with fitsio.FITS(fpath, "rw") as fits:
@@ -193,15 +237,20 @@
                 warnings.warn(
                     "dropping column '{:}' with unsuppored type '{:}'".format(
                         col, df[col].dtype))
         hdu = astropy.io.fits.BinTableHDU.from_columns(columns)
         hdu.writeto(fpath, overwrite=True)
 
 
-def to_auto(df, fpath, ext=None, **kwargs):
+def to_auto(
+    df: pd.DataFrame,
+    fpath: str,
+    ext: int | None = None,
+    **kwargs
+) -> None:
     """
     Write a file to a file format using standard parameters for the
     pandas.to_xxx() method.
 
     Parameters:
     -----------
     df : pandas.DataFrame
```

### Comparing `astropandas-1.1.3/astropandas/match.py` & `astropandas-1.2/astropandas/match.py`

 * *Files identical despite different names*

### Comparing `astropandas-1.1.3/astropandas.egg-info/PKG-INFO` & `astropandas-1.2/astropandas.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: astropandas
-Version: 1.1.3
+Version: 1.2
 Summary: Tools to expand on pandas functionality for astronomical operations.
-Home-page: https://github.com/jlvdb/astropandas
 Author: Jan Luca van den Busch
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+License: GPLv3
+Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # astropandas
 
 Tools to expand on pandas functionality for astronomical applications.
 
@@ -45,9 +45,7 @@
 apd.match(
     left=data1, right=data2,
     ra="RA", dec="DEC",
     threshold=1/3600)
 # If no threshold is provided, it is computed automatically by finding the
 # distance at which the number of matches is almost stationary.
 ```
-
-
```

