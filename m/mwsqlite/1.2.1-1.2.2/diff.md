# Comparing `tmp/mwsqlite-1.2.1.tar.gz` & `tmp/mwsqlite-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mwsqlite-1.2.1.tar", last modified: Wed May 31 05:59:36 2023, max compression
+gzip compressed data, was "dist\mwsqlite-1.2.2.tar", last modified: Mon Jun 26 20:58:46 2023, max compression
```

## Comparing `mwsqlite-1.2.1.tar` & `mwsqlite-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 05:59:36.539919 mwsqlite-1.2.1/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     3172 2023-05-31 05:59:36.539919 mwsqlite-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 05:59:36.526284 mwsqlite-1.2.1/mwsqlite/
--rw-rw-rw-   0        0        0      186 2022-12-19 10:39:07.000000 mwsqlite-1.2.1/mwsqlite/__init__.py
--rw-rw-rw-   0        0        0     1513 2022-12-23 17:48:52.000000 mwsqlite-1.2.1/mwsqlite/_types.py
--rw-rw-rw-   0        0        0    14614 2023-05-31 05:56:49.000000 mwsqlite-1.2.1/mwsqlite/mw_sql.py
--rw-rw-rw-   0        0        0     3388 2022-12-23 15:06:08.000000 mwsqlite-1.2.1/mwsqlite/sql_compile.py
--rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.2.1/mwsqlite/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:59:36.538904 mwsqlite-1.2.1/mwsqlite.egg-info/
--rw-rw-rw-   0        0        0     3172 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 05:59:36.540919 mwsqlite-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1666 2023-05-31 05:59:17.000000 mwsqlite-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:58:46.077516 mwsqlite-1.2.2/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3172 2023-06-26 20:58:46.078517 mwsqlite-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 20:58:46.064513 mwsqlite-1.2.2/mwsqlite/
+-rw-rw-rw-   0        0        0      186 2022-12-19 10:39:07.000000 mwsqlite-1.2.2/mwsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1513 2022-12-23 17:48:52.000000 mwsqlite-1.2.2/mwsqlite/_types.py
+-rw-rw-rw-   0        0        0    14773 2023-06-26 20:56:30.000000 mwsqlite-1.2.2/mwsqlite/mw_sql.py
+-rw-rw-rw-   0        0        0     3388 2022-12-23 15:06:08.000000 mwsqlite-1.2.2/mwsqlite/sql_compile.py
+-rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.2.2/mwsqlite/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:58:46.076516 mwsqlite-1.2.2/mwsqlite.egg-info/
+-rw-rw-rw-   0        0        0     3172 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:58:46.079516 mwsqlite-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1666 2023-06-26 20:52:20.000000 mwsqlite-1.2.2/setup.py
```

### Comparing `mwsqlite-1.2.1/LICENSE` & `mwsqlite-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.1/PKG-INFO` & `mwsqlite-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.1.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.2.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.2.1/README.md` & `mwsqlite-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.1/mwsqlite/_types.py` & `mwsqlite-1.2.2/mwsqlite/_types.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.1/mwsqlite/mw_sql.py` & `mwsqlite-1.2.2/mwsqlite/mw_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 import json
 # This Python file uses the following encoding: utf-8
 import sqlite3
+from typing import List
 
 try:
     from ._types import Struct, Where, Order, InvalidColumnNameError, DESC, ASC, Limit
     from .utils import tuple_to_dict
     from .sql_compile import SQLCompile
 except:
     from _types import Struct, Where, Order, InvalidColumnNameError, DESC, ASC, Limit
@@ -50,15 +51,15 @@
     return dct
 
 def check_kwargs(kwargs: dict):
     kwargs = check_dict(kwargs)
 
     for k, v in kwargs.items():
         if isinstance(v, list) or isinstance(v, dict):
-            kwargs[k] = json.dumps(v)
+            kwargs[k] = json.dumps(v, separators = (',', ':'))
     
     return kwargs
     
     
 class MWBase():
     @ensure_connection
     def __init__(self, filename: str, tables: str, cursor=None):
@@ -77,14 +78,16 @@
 
     def table(self, table: str) -> Table:
         """
         Get table object.
         """
         return self.__getattribute__(table)
 
+    def __getattribute__(self, __name: str) -> Table:
+        return object.__getattribute__(self, __name)
 
 
 class Table:
     """
     Table class for working with sqlite3 databases.
     """
     def __init__(self, table: str, columns: dict, base: MWBase):
@@ -116,15 +119,15 @@
         kwargs = check_kwargs(kwargs)
 
         cmd = SQLCompile.insert(self.table, kwargs.keys())
         values = tuple(map(str, kwargs.values()))
         cursor.execute(cmd, values)
     
     @ensure_connection
-    def get_all(self, order: Order = Order(), cursor=None) -> list[Row]:
+    def get_all(self, order: Order = Order(), cursor=None) -> List[Row]:
         """
         Get all rows from table.
         """
         if order:
             return self.get(order=order)
 
         cmd = SQLCompile.select(self.table)
@@ -137,15 +140,15 @@
         resp = []
         for item in items:
             resp.append(Row(self, **tuple_to_dict(item, self.columns)))
 
         return resp
 
     @ensure_connection
-    def get(self, order: Order = Order(), where: Where = Where(), distinct: bool=False, cursor=None, **kwargs) -> list[Row]:
+    def get(self, order: Order = Order(), where: Where = Where(), distinct: bool=False, cursor=None, **kwargs) -> List[Row]:
         """
         Get rows from table.
         ```python
         base.test_table.get(Order(id=DESC), Where(id=1, name="test"))
         ```
 
         or 
@@ -263,15 +266,15 @@
     @ensure_connection
     def get_last(self, cursor=None, **kwargs) -> Row | None:
         """
         Get last row with parameters from table.
         """
         return self.get_one(default_index=-1, **kwargs)
     @ensure_connection
-    def get_like(self, where: Where = Where(), order: Order = Order(), return_index: int = None, cursor=None, **kwargs) -> list[Row]:
+    def get_like(self, where: Where = Where(), order: Order = Order(), return_index: int = None, cursor=None, **kwargs) -> List[Row]:
         
         if isinstance(order, Where) and isinstance(where, Order):
             order, where = where, order
 
         elif isinstance(order, Where) and isinstance(where, Where): 
             where.update(order)
             order = Order()
```

### Comparing `mwsqlite-1.2.1/mwsqlite/sql_compile.py` & `mwsqlite-1.2.2/mwsqlite/sql_compile.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.1/mwsqlite/utils.py` & `mwsqlite-1.2.2/mwsqlite/utils.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.1/mwsqlite.egg-info/PKG-INFO` & `mwsqlite-1.2.2/mwsqlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.1.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.2.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.2.1/setup.py` & `mwsqlite-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.2.1'
+version = '1.2.2'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mwsqlite",
     version=version,
```

