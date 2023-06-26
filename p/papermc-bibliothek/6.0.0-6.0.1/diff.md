# Comparing `tmp/papermc_bibliothek-6.0.0.tar.gz` & `tmp/papermc_bibliothek-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papermc_bibliothek-6.0.0.tar", max compression
+gzip compressed data, was "papermc_bibliothek-6.0.1.tar", max compression
```

## Comparing `papermc_bibliothek-6.0.0.tar` & `papermc_bibliothek-6.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2022-04-11 10:22:56.963000 papermc_bibliothek-6.0.0/LICENSE
--rw-r--r--   0        0        0      922 2023-06-26 01:17:34.738999 papermc_bibliothek-6.0.0/README.md
--rw-r--r--   0        0        0       26 2023-06-26 01:48:16.672464 papermc_bibliothek-6.0.0/bibliothek/__init__.py
--rw-r--r--   0        0        0    11472 2023-06-26 01:44:30.731748 papermc_bibliothek-6.0.0/bibliothek/bibliothek.py
--rw-r--r--   0        0        0      601 2023-06-26 01:15:07.289117 papermc_bibliothek-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 papermc_bibliothek-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-04-11 10:22:56.963000 papermc_bibliothek-6.0.1/LICENSE
+-rw-r--r--   0        0        0      922 2023-06-26 01:17:34.738999 papermc_bibliothek-6.0.1/README.md
+-rw-r--r--   0        0        0       26 2023-06-26 01:48:16.672464 papermc_bibliothek-6.0.1/bibliothek/__init__.py
+-rw-r--r--   0        0        0    11572 2023-06-26 11:40:35.202335 papermc_bibliothek-6.0.1/bibliothek/bibliothek.py
+-rw-r--r--   0        0        0      601 2023-06-26 11:41:36.989218 papermc_bibliothek-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 papermc_bibliothek-6.0.1/PKG-INFO
```

### Comparing `papermc_bibliothek-6.0.0/LICENSE` & `papermc_bibliothek-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `papermc_bibliothek-6.0.0/README.md` & `papermc_bibliothek-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `papermc_bibliothek-6.0.0/bibliothek/bibliothek.py` & `papermc_bibliothek-6.0.1/bibliothek/bibliothek.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,18 @@
         download_bytesio = BytesIO()
         while True:
             data = request.read(2 ** 16)  # 64kb
             if not data:
                 break
             download_bytesio.write(data)
             if progress_callback:
-                progress_callback(download_bytesio.getbuffer().nbytes, request.headers.get("Content-Length"))
+                length = request.headers.get("Content-Length")
+                if length:
+                    length = int(length)
+                progress_callback(download_bytesio.getbuffer().nbytes, length)
 
         request.release_conn()
 
         if request.status != 200:
             raise UnexpectedResponseBibliothekException(request)
 
         return download_bytesio
```

### Comparing `papermc_bibliothek-6.0.0/pyproject.toml` & `papermc_bibliothek-6.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "papermc-bibliothek"
 packages = [{ include = "bibliothek" }]
-version = "6.0.0"
+version = "6.0.1"
 description = "bibliothek API client with CLI"
 authors = ["Oskar <56176746+OskarZyg@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/OskarsMC-Network/papermc-bibliothek"
 homepage = "https://github.com/OskarsMC-Network/papermc-bibliothek"
```

### Comparing `papermc_bibliothek-6.0.0/PKG-INFO` & `papermc_bibliothek-6.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papermc-bibliothek
-Version: 6.0.0
+Version: 6.0.1
 Summary: bibliothek API client with CLI
 Home-page: https://github.com/OskarsMC-Network/papermc-bibliothek
 License: MIT
 Author: Oskar
 Author-email: 56176746+OskarZyg@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

