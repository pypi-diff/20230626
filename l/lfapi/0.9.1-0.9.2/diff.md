# Comparing `tmp/lfapi-0.9.1.tar.gz` & `tmp/lfapi-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfapi-0.9.1.tar", last modified: Fri Mar 17 13:23:16 2023, max compression
+gzip compressed data, was "lfapi-0.9.2.tar", last modified: Mon Jun 26 17:00:51 2023, max compression
```

## Comparing `lfapi-0.9.1.tar` & `lfapi-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:23:16.961215 lfapi-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-17 13:22:59.000000 lfapi-0.9.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-03-17 13:23:16.961215 lfapi-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-03-17 13:22:59.000000 lfapi-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:23:16.961215 lfapi-0.9.1/lfapi/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-17 13:22:59.000000 lfapi-0.9.1/lfapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 13:22:59.000000 lfapi-0.9.1/lfapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-17 13:22:59.000000 lfapi-0.9.1/lfapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-03-17 13:22:59.000000 lfapi-0.9.1/lfapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-17 13:22:59.000000 lfapi-0.9.1/lfapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-03-17 13:22:59.000000 lfapi-0.9.1/lfapi/http_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-03-17 13:22:59.000000 lfapi-0.9.1/lfapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:23:16.961215 lfapi-0.9.1/lfapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-03-17 13:23:16.000000 lfapi-0.9.1/lfapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-17 13:23:16.000000 lfapi-0.9.1/lfapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 13:23:16.000000 lfapi-0.9.1/lfapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-17 13:23:16.000000 lfapi-0.9.1/lfapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-17 13:23:16.000000 lfapi-0.9.1/lfapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 13:23:16.965215 lfapi-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-17 13:22:59.000000 lfapi-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:23:16.961215 lfapi-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-17 13:22:59.000000 lfapi-0.9.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-03-17 13:22:59.000000 lfapi-0.9.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:00:51.646525 lfapi-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-26 17:00:27.000000 lfapi-0.9.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-26 17:00:51.646525 lfapi-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-26 17:00:27.000000 lfapi-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:00:51.642525 lfapi-0.9.2/lfapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 17:00:27.000000 lfapi-0.9.2/lfapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 17:00:27.000000 lfapi-0.9.2/lfapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-26 17:00:27.000000 lfapi-0.9.2/lfapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-26 17:00:27.000000 lfapi-0.9.2/lfapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 17:00:27.000000 lfapi-0.9.2/lfapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-26 17:00:27.000000 lfapi-0.9.2/lfapi/http_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-26 17:00:27.000000 lfapi-0.9.2/lfapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:00:51.642525 lfapi-0.9.2/lfapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-26 17:00:51.000000 lfapi-0.9.2/lfapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-26 17:00:51.000000 lfapi-0.9.2/lfapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:00:51.000000 lfapi-0.9.2/lfapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 17:00:51.000000 lfapi-0.9.2/lfapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 17:00:51.000000 lfapi-0.9.2/lfapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:00:51.646525 lfapi-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-26 17:00:27.000000 lfapi-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:00:51.646525 lfapi-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-26 17:00:27.000000 lfapi-0.9.2/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-26 17:00:27.000000 lfapi-0.9.2/tests/test_client.py
```

### Comparing `lfapi-0.9.1/LICENSE.md` & `lfapi-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lfapi-0.9.1/PKG-INFO` & `lfapi-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfapi
-Version: 0.9.1
+Version: 0.9.2
 Summary: The Python library for the ListenFirst API
 Home-page: https://github.com/ListenFirstMedia/lf-python-sdk
 Download-URL: https://pypi.org/project/lfapi
 Author: Joseph Masom
 Author-email: joseph.masom@listenfirstmedia.com
 License: MIT
 Keywords: listenfirst api sdk
```

### Comparing `lfapi-0.9.1/README.md` & `lfapi-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `lfapi-0.9.1/lfapi/auth.py` & `lfapi-0.9.2/lfapi/auth.py`

 * *Files identical despite different names*

### Comparing `lfapi-0.9.1/lfapi/client.py` & `lfapi-0.9.2/lfapi/client.py`

 * *Files identical despite different names*

### Comparing `lfapi-0.9.1/lfapi/errors.py` & `lfapi-0.9.2/lfapi/errors.py`

 * *Files identical despite different names*

### Comparing `lfapi-0.9.1/lfapi/http_utils.py` & `lfapi-0.9.2/lfapi/http_utils.py`

 * *Files identical despite different names*

### Comparing `lfapi-0.9.1/lfapi/models.py` & `lfapi-0.9.2/lfapi/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,18 @@
       setattr(self, attr, getattr(other, attr))
 
 
   @property
   def record(self):
     return self.body.get("record")
 
+  @property
+  def attrs(self):
+    return sorted(self.as_dict().keys())
+
 
 class FetchJob(Model):
   """Wrapper for ListenFirst API Fetch Jobs."""
   _required = ["id", "state", "created_at", "updated_at", "client_context",
                "schedule_config_id"]
 
   @requires_client
@@ -162,14 +166,19 @@
     """Return the model as a list of models."""
     return self.records
 
   def as_dict_list(self):
     """Return the model as a list of dictionaries."""
     return [rec.as_dict() for rec in self.records]
 
+  @property
+  def _labels(self):
+    base_labels = set(self._item_class._required)
+    return sorted(base_labels.union(*[rec.attrs for rec in self.records]))
+
   def to_csv(self, fp=None, delimiter=','):
     """Send the model to a CSV file or string object.
 
     Arguments:
     fp
       the file object or filename; if None, this method returns a string
       containing the data in CSV format
@@ -181,30 +190,30 @@
     # Convert filename to file pointer
     if isinstance(fp, str):
       with open(fp, 'w') as fp:
         return self.to_csv(fp, delimiter=delimiter)
 
     # Write to fp
     rows = self.as_dict_list()
-    writer = csv.DictWriter(fp, delimiter=delimiter, fieldnames=rows[0].keys())
+    writer = csv.DictWriter(fp, delimiter=delimiter, fieldnames=self._labels)
     writer.writeheader()
     writer.writerows(rows)
 
     return fp.getvalue() if isinstance(fp, io.StringIO) else None
 
   def to_pandas(self):
     """Convert the model to a Pandas DataFrame. Not implemented if Pandas is
     not installed.
     """
     if pd is None:
-      raise NotImplementedError('pandas is not installed.')
+      raise NotImplementedError('Pandas is not installed.')
 
     rows = self.as_dict_list()
     return pd.DataFrame(
-      columns=rows[0].keys(),
+      columns=self._labels,
       data=rows
     )
 
   # List-like dunder methods
   def __len__(self):
     return len(self.records)
```

### Comparing `lfapi-0.9.1/lfapi.egg-info/PKG-INFO` & `lfapi-0.9.2/lfapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfapi
-Version: 0.9.1
+Version: 0.9.2
 Summary: The Python library for the ListenFirst API
 Home-page: https://github.com/ListenFirstMedia/lf-python-sdk
 Download-URL: https://pypi.org/project/lfapi
 Author: Joseph Masom
 Author-email: joseph.masom@listenfirstmedia.com
 License: MIT
 Keywords: listenfirst api sdk
```

### Comparing `lfapi-0.9.1/setup.py` & `lfapi-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `lfapi-0.9.1/tests/test_auth.py` & `lfapi-0.9.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `lfapi-0.9.1/tests/test_client.py` & `lfapi-0.9.2/tests/test_client.py`

 * *Files identical despite different names*

