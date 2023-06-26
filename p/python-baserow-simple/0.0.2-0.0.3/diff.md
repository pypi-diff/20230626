# Comparing `tmp/python_baserow_simple-0.0.2.tar.gz` & `tmp/python_baserow_simple-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_baserow_simple-0.0.2.tar", last modified: Thu Jun 22 15:28:57 2023, max compression
+gzip compressed data, was "python_baserow_simple-0.0.3.tar", last modified: Mon Jun 26 15:21:19 2023, max compression
```

## Comparing `python_baserow_simple-0.0.2.tar` & `python_baserow_simple-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:28:57.800408 python_baserow_simple-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-22 15:28:57.800408 python_baserow_simple-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:28:57.800408 python_baserow_simple-0.0.2/python_baserow_simple/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/python_baserow_simple/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/python_baserow_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/python_baserow_simple/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/python_baserow_simple/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/python_baserow_simple/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:28:57.800408 python_baserow_simple-0.0.2/python_baserow_simple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-22 15:28:57.000000 python_baserow_simple-0.0.2/python_baserow_simple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-22 15:28:57.000000 python_baserow_simple-0.0.2/python_baserow_simple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:28:57.000000 python_baserow_simple-0.0.2/python_baserow_simple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 15:28:57.000000 python_baserow_simple-0.0.2/python_baserow_simple.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-22 15:28:57.000000 python_baserow_simple-0.0.2/python_baserow_simple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 15:28:57.000000 python_baserow_simple-0.0.2/python_baserow_simple.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 15:28:57.800408 python_baserow_simple-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:28:57.800408 python_baserow_simple-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 15:28:44.000000 python_baserow_simple-0.0.2/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:21:19.590090 python_baserow_simple-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-26 15:21:19.590090 python_baserow_simple-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:21:19.590090 python_baserow_simple-0.0.3/python_baserow_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/python_baserow_simple/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/python_baserow_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/python_baserow_simple/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/python_baserow_simple/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/python_baserow_simple/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:21:19.590090 python_baserow_simple-0.0.3/python_baserow_simple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-26 15:21:19.000000 python_baserow_simple-0.0.3/python_baserow_simple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 15:21:19.000000 python_baserow_simple-0.0.3/python_baserow_simple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:21:19.000000 python_baserow_simple-0.0.3/python_baserow_simple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 15:21:19.000000 python_baserow_simple-0.0.3/python_baserow_simple.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 15:21:19.000000 python_baserow_simple-0.0.3/python_baserow_simple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 15:21:19.000000 python_baserow_simple-0.0.3/python_baserow_simple.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:21:19.590090 python_baserow_simple-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:21:19.590090 python_baserow_simple-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 15:21:10.000000 python_baserow_simple-0.0.3/tests/test_base.py
```

### Comparing `python_baserow_simple-0.0.2/LICENSE` & `python_baserow_simple-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_baserow_simple-0.0.2/PKG-INFO` & `python_baserow_simple-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_baserow_simple
-Version: 0.0.2
+Version: 0.0.3
 Summary: Awesome python_baserow_simple created by xiamaz
 Home-page: https://github.com/xiamaz/python-baserow-simple/
 Author: xiamaz
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `python_baserow_simple-0.0.2/README.md` & `python_baserow_simple-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python_baserow_simple-0.0.2/python_baserow_simple/__init__.py` & `python_baserow_simple-0.0.3/python_baserow_simple/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,44 @@
                 "Authorization": f"Token {self._token}",
                 "Content-Type": "application/json",
             },
             json=data,
         )
         resp.raise_for_status()
 
+    def _update_rows(self, table_id, datas):
+        url = f"https://phenotips.charite.de/api/database/rows/table/{table_id}/batch/?user_field_names=true"  # noqa: E501
+        resp = requests.patch(
+            url,
+            headers={
+                "Authorization": f"Token {self._token}",
+                "Content-Type": "application/json",
+            },
+            json={"items": datas},
+        )
+        resp.raise_for_status()
+        data = resp.json()
+        ids = [e["id"] for e in data["items"]]
+        return ids
+
+    def _create_rows(self, table_id, datas):
+        url = f"https://phenotips.charite.de/api/database/rows/table/{table_id}/batch/?user_field_names=true"  # noqa: E501
+        resp = requests.post(
+            url,
+            headers={
+                "Authorization": f"Token {self._token}",
+                "Content-Type": "application/json",
+            },
+            json={"items": datas},
+        )
+        resp.raise_for_status()
+        data = resp.json()
+        ids = [e["id"] for e in data["items"]]
+        return ids
+
     def _convert_selects(self, data, fields):
         data_conv = deepcopy(data)
 
         def convert_option(v, opts):
             if isinstance(v, int):
                 return v
 
@@ -86,14 +116,29 @@
         if row_id:
             self._update_row(table_id, row_id, data_conv)
         else:
             row_id = self._create_row(table_id, data_conv)
 
         return row_id
 
+    def add_data_batch(self, table_id, entries):
+        """Add multiple entries."""
+        entries_update = []
+        entries_new = []
+        for entry in entries:
+            if entry.get("id") is not None:
+                entries_update.append(entry)
+            else:
+                entries_new.append(entry)
+
+        if entries_new:
+            self._create_rows(table_id, entries_new)
+        if entries_update:
+            self._update_rows(table_id, entries_update)
+
 
 def load_token(token_path):
     with open(token_path) as tokenfile:
         token = tokenfile.readline().strip()
     return token
```

### Comparing `python_baserow_simple-0.0.2/python_baserow_simple/cli.py` & `python_baserow_simple-0.0.3/python_baserow_simple/cli.py`

 * *Files identical despite different names*

### Comparing `python_baserow_simple-0.0.2/python_baserow_simple.egg-info/PKG-INFO` & `python_baserow_simple-0.0.3/python_baserow_simple.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-baserow-simple
-Version: 0.0.2
+Version: 0.0.3
 Summary: Awesome python_baserow_simple created by xiamaz
 Home-page: https://github.com/xiamaz/python-baserow-simple/
 Author: xiamaz
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `python_baserow_simple-0.0.2/python_baserow_simple.egg-info/SOURCES.txt` & `python_baserow_simple-0.0.3/python_baserow_simple.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_baserow_simple-0.0.2/setup.py` & `python_baserow_simple-0.0.3/setup.py`

 * *Files identical despite different names*

