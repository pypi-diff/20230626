# Comparing `tmp/skillshare_dl-0.0.1.tar.gz` & `tmp/skillshare_dl-0.0.2.tar.gz`

## Comparing `skillshare_dl-0.0.1.tar` & `skillshare_dl-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 skillshare_dl-0.0.1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skillshare_dl-0.0.1/src/skillshare_dl/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 skillshare_dl-0.0.1/src/skillshare_dl/cli.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 skillshare_dl-0.0.1/src/skillshare_dl/main.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 skillshare_dl-0.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 skillshare_dl-0.0.1/LICENSE
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 skillshare_dl-0.0.1/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 skillshare_dl-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 skillshare_dl-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/src/skillshare_dl/__init__.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/src/skillshare_dl/cli.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/src/skillshare_dl/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 skillshare_dl-0.0.2/PKG-INFO
```

### Comparing `skillshare_dl-0.0.1/src/skillshare_dl/cli.py` & `skillshare_dl-0.0.2/src/skillshare_dl/cli.py`

 * *Files identical despite different names*

### Comparing `skillshare_dl-0.0.1/src/skillshare_dl/main.py` & `skillshare_dl-0.0.2/src/skillshare_dl/main.py`

 * *Files identical despite different names*

### Comparing `skillshare_dl-0.0.1/LICENSE` & `skillshare_dl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skillshare_dl-0.0.1/pyproject.toml` & `skillshare_dl-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "skillshare_dl"
-version = "0.0.1"
+version = "0.0.2"
 description = "A cli tool for downloading Skillshare lesson videos"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { text = 'MIT' }
 authors = [{ name = "Wayde Gilliam", email = "waydegilliam@gmail.com" }]
 keywords = ["python", "skillshare"]
 dependencies = ["httpx", "tqdm", "beautifulsoup4"]
```

