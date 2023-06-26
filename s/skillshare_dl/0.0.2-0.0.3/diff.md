# Comparing `tmp/skillshare_dl-0.0.2.tar.gz` & `tmp/skillshare_dl-0.0.3.tar.gz`

## Comparing `skillshare_dl-0.0.2.tar` & `skillshare_dl-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/src/skillshare_dl/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/src/skillshare_dl/cli.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/src/skillshare_dl/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/LICENSE
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 skillshare_dl-0.0.3/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skillshare_dl-0.0.3/src/skillshare_dl/__init__.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 skillshare_dl-0.0.3/src/skillshare_dl/cli.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 skillshare_dl-0.0.3/src/skillshare_dl/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 skillshare_dl-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 skillshare_dl-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 skillshare_dl-0.0.3/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 skillshare_dl-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 skillshare_dl-0.0.3/PKG-INFO
```

### Comparing `skillshare_dl-0.0.2/src/skillshare_dl/cli.py` & `skillshare_dl-0.0.3/src/skillshare_dl/cli.py`

 * *Files identical despite different names*

### Comparing `skillshare_dl-0.0.2/src/skillshare_dl/main.py` & `skillshare_dl-0.0.3/src/skillshare_dl/main.py`

 * *Files identical despite different names*

### Comparing `skillshare_dl-0.0.2/LICENSE` & `skillshare_dl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skillshare_dl-0.0.2/README.md` & `skillshare_dl-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -42,7 +42,10 @@
 A complete example of this can look like:
 
 ```bash
 skillshare-dl \
   "https://www.skillshare.com/en/classes/Motion-Graphics-with-Kurzgesagt-%E2%80%93-Part-1/631970755/projects?via=Selected-SearchSuggestion" \
   "eyJhbGciOi98y1yCho98y112Cl8Ga21dac3usImtpZCI6IldC..."
 ```
+
+If you're getting 401 errors, refresh the page and use the new access token that was
+generated.
```

### Comparing `skillshare_dl-0.0.2/pyproject.toml` & `skillshare_dl-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "skillshare_dl"
-version = "0.0.2"
+version = "0.0.3"
 description = "A cli tool for downloading Skillshare lesson videos"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { text = 'MIT' }
 authors = [{ name = "Wayde Gilliam", email = "waydegilliam@gmail.com" }]
 keywords = ["python", "skillshare"]
 dependencies = ["httpx", "tqdm", "beautifulsoup4"]
```

### Comparing `skillshare_dl-0.0.2/PKG-INFO` & `skillshare_dl-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillshare_dl
-Version: 0.0.2
+Version: 0.0.3
 Summary: A cli tool for downloading Skillshare lesson videos
 Project-URL: Homepage, https://github.com/waydegg/skillshare-dl
 Project-URL: Source, https://github.com/waydegg/skillshare-dl
 Author-email: Wayde Gilliam <waydegilliam@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: python,skillshare
@@ -61,7 +61,10 @@
 A complete example of this can look like:
 
 ```bash
 skillshare-dl \
   "https://www.skillshare.com/en/classes/Motion-Graphics-with-Kurzgesagt-%E2%80%93-Part-1/631970755/projects?via=Selected-SearchSuggestion" \
   "eyJhbGciOi98y1yCho98y112Cl8Ga21dac3usImtpZCI6IldC..."
 ```
+
+If you're getting 401 errors, refresh the page and use the new access token that was
+generated.
```

