# Comparing `tmp/pandas_money-0.2.1.tar.gz` & `tmp/pandas_money-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_money-0.2.1.tar", max compression
+gzip compressed data, was "pandas_money-0.2.2.tar", max compression
```

## Comparing `pandas_money-0.2.1.tar` & `pandas_money-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-06-09 03:17:36.171096 pandas_money-0.2.1/LICENSE
--rw-r--r--   0        0        0      859 2023-06-12 22:53:26.115878 pandas_money-0.2.1/README.md
--rw-r--r--   0        0        0      207 2023-06-13 19:32:02.941024 pandas_money-0.2.1/pandas_money/__init__.py
--rw-r--r--   0        0        0     8652 2023-06-13 20:29:44.806189 pandas_money-0.2.1/pandas_money/money_dtype.py
--rw-r--r--   0        0        0        0 2023-06-12 04:25:47.563979 pandas_money-0.2.1/pandas_money/tests/__init__.py
--rw-r--r--   0        0        0    13160 2023-06-13 20:23:58.449518 pandas_money-0.2.1/pandas_money/tests/test_money_dtype.py
--rw-r--r--   0        0        0     1434 2023-06-13 20:31:03.509546 pandas_money-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 pandas_money-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 03:17:36.171096 pandas_money-0.2.2/LICENSE
+-rw-r--r--   0        0        0      859 2023-06-12 22:53:26.115878 pandas_money-0.2.2/README.md
+-rw-r--r--   0        0        0      207 2023-06-16 17:48:47.618208 pandas_money-0.2.2/pandas_money/__init__.py
+-rw-r--r--   0        0        0     9019 2023-06-26 05:54:45.243155 pandas_money-0.2.2/pandas_money/money_dtype.py
+-rw-r--r--   0        0        0        0 2023-06-16 17:48:47.622207 pandas_money-0.2.2/pandas_money/tests/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-26 05:54:45.243155 pandas_money-0.2.2/pandas_money/tests/test_indexing.py
+-rw-r--r--   0        0        0    13160 2023-06-16 17:48:47.622207 pandas_money-0.2.2/pandas_money/tests/test_money_dtype.py
+-rw-r--r--   0        0        0     1434 2023-06-26 05:54:45.243155 pandas_money-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 pandas_money-0.2.2/PKG-INFO
```

### Comparing `pandas_money-0.2.1/LICENSE` & `pandas_money-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_money-0.2.1/README.md` & `pandas_money-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pandas_money-0.2.1/pandas_money/money_dtype.py` & `pandas_money-0.2.2/pandas_money/money_dtype.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     ExtensionArray,
     ExtensionScalarOpsMixin,
     register_extension_dtype,
 )
 from pandas.core.dtypes.base import ExtensionDtype
 from pandas.core.dtypes.common import is_dtype_equal, pandas_dtype
 from pandas.core.dtypes.dtypes import PandasExtensionDtype
+from pandas.core.dtypes.inference import is_integer
 
 money_decimals = 2
 money_factor = 10**money_decimals
 decimal_quantize = Decimal(f".{'0'*(money_decimals-1)}1")
 
 
 @register_extension_dtype
@@ -97,14 +98,23 @@
             val = self.values[item]
             if pd.isna(val):
                 return val
             return Money(val, USD) / money_factor
         else:
             return MoneyArray(self.values[item], to_cents=False)
 
+    def __setitem__(self, key, value) -> None:
+        """Set one or more values inplace."""
+        try:
+            value = self._clean_value(value, to_cents=True)
+        except TypeError:
+            pass
+        value = value if pd.isna(value) else np.int64(value)
+        self.values.__setitem__(key, value)
+
     def __eq__(self, other):
         if isinstance(other, (pd.Index, pd.Series, pd.DataFrame)):
             return NotImplemented
         if not isinstance(other, MoneyArray):
             other = MoneyArray(other)
         return self.values == other.values
```

### Comparing `pandas_money-0.2.1/pandas_money/tests/test_money_dtype.py` & `pandas_money-0.2.2/pandas_money/tests/test_money_dtype.py`

 * *Files identical despite different names*

### Comparing `pandas_money-0.2.1/pyproject.toml` & `pandas_money-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-money"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Pandas ArrayExtension for handling currency with int64 performance"
 authors = ["Rod Morison <rmorison@users.noreply.github.com>"]
 repository = "https://github.com/rmorison/pandas-money"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandas_money"}]
```

### Comparing `pandas_money-0.2.1/PKG-INFO` & `pandas_money-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-money
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Pandas ArrayExtension for handling currency with int64 performance
 Home-page: https://github.com/rmorison/pandas-money
 License: MIT
 Author: Rod Morison
 Author-email: rmorison@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

