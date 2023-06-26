# Comparing `tmp/metal_sdk-1.0.8.tar.gz` & `tmp/metal_sdk-1.0.9.tar.gz`

## Comparing `metal_sdk-1.0.8.tar` & `metal_sdk-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/motorhead.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/motorhead_async.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/test_metal.py
--rw-r--r--   0        0        0     9962 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/test_metal_async.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/test_motorhead.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/test_motorhead_async.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/fixtures/sample.csv
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/motorhead.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/motorhead_async.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/test_metal.py
+-rw-r--r--   0        0        0     9962 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/test_metal_async.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/test_motorhead.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/test_motorhead_async.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/LICENSE
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 metal_sdk-1.0.9/PKG-INFO
```

### Comparing `metal_sdk-1.0.8/.github/workflows/publish.yml` & `metal_sdk-1.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/.github/workflows/test.yml` & `metal_sdk-1.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/examples/example.py` & `metal_sdk-1.0.9/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/examples/example_async.py` & `metal_sdk-1.0.9/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/src/metal_sdk/metal.py` & `metal_sdk-1.0.9/src/metal_sdk/metal.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,25 +143,27 @@
         if index is None:
             raise TypeError("index_id required")
 
         url = "/v1/indexes/" + index + "/documents/" + id
 
         res = self.request("delete", url)
         res.raise_for_status()
-        return res.json()
+
+        return None
 
     def delete_many(self, ids: List[str], index_id=None):
         if ids is None:
             raise TypeError("ids required")
 
         url = "/v1/documents/bulk"
 
         res = self.request("delete", url, json={"ids": ids})
         res.raise_for_status()
-        return res.json()
+
+        return None
 
     def __sanitize_filename(self, filename):
         """
         Implement your filename sanitation method here.
         """
         sanitized_filename = filename.replace(' ', '_')  # Simplified example
         return sanitized_filename
```

### Comparing `metal_sdk-1.0.8/src/metal_sdk/metal_async.py` & `metal_sdk-1.0.9/src/metal_sdk/metal_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,25 +143,25 @@
         if index is None:
             raise TypeError("index_id required")
 
         url = "/v1/indexes/" + index + "/documents/" + id
 
         res = await self.request("delete", url)
         res.raise_for_status()
-        return res.json()
+        return None
 
     async def delete_many(self, ids: List[str]):
         if ids is None:
             raise TypeError("ids required")
 
         url = "/v1/documents/bulk"
 
         res = await self.request("delete", url, json={"ids": ids})
         res.raise_for_status()
-        return res.json()
+        return None
 
     def __sanitize_filename(self, filename):
         """
         Implement your filename sanitation method here.
         """
         sanitized_filename = filename.replace(' ', '_')  # Simplified example
         return sanitized_filename
```

### Comparing `metal_sdk-1.0.8/src/metal_sdk/motorhead.py` & `metal_sdk-1.0.9/src/metal_sdk/motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/src/metal_sdk/motorhead_async.py` & `metal_sdk-1.0.9/src/metal_sdk/motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/src/metal_sdk/typings.py` & `metal_sdk-1.0.9/src/metal_sdk/typings.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/tests/test_metal.py` & `metal_sdk-1.0.9/tests/test_metal.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/tests/test_metal_async.py` & `metal_sdk-1.0.9/tests/test_metal_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/tests/test_motorhead.py` & `metal_sdk-1.0.9/tests/test_motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/tests/test_motorhead_async.py` & `metal_sdk-1.0.9/tests/test_motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/.gitignore` & `metal_sdk-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/LICENSE` & `metal_sdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.8/pyproject.toml` & `metal_sdk-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

