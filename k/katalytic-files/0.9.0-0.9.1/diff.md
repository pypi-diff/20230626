# Comparing `tmp/katalytic_files-0.9.0.tar.gz` & `tmp/katalytic_files-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic_files-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "katalytic_files-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic_files-0.9.0.tar` & `katalytic_files-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-13 15:48:09.439894 katalytic_files-0.9.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_files-0.9.0/.gitignore
--rw-r--r--   0        0        0     3242 2023-05-05 03:59:34.970335 katalytic_files-0.9.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     2614 2023-05-22 16:52:04.391944 katalytic_files-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-10 04:00:05.979612 katalytic_files-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     1900 2023-05-14 08:37:32.778688 katalytic_files-0.9.0/README.md
--rw-r--r--   0        0        0     1378 2023-05-22 16:52:04.367944 katalytic_files-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    35693 2023-05-22 16:47:01.078578 katalytic_files-0.9.0/src/katalytic/files.py
--rw-r--r--   0        0        0    45211 2023-05-20 16:40:59.258168 katalytic_files-0.9.0/tests/test_files.py
--rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 katalytic_files-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-13 15:48:09.439894 katalytic_files-0.9.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_files-0.9.1/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:34.970335 katalytic_files-0.9.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2805 2023-05-31 06:35:59.524828 katalytic_files-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-10 04:00:05.979612 katalytic_files-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     1959 2023-05-31 06:33:32.907622 katalytic_files-0.9.1/README.md
+-rw-r--r--   0        0        0     1378 2023-05-31 06:35:59.524828 katalytic_files-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    35699 2023-05-31 06:32:42.787371 katalytic_files-0.9.1/src/katalytic/files.py
+-rw-r--r--   0        0        0    45211 2023-05-20 16:40:59.258168 katalytic_files-0.9.1/tests/test_files.py
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 katalytic_files-0.9.1/PKG-INFO
```

### Comparing `katalytic_files-0.9.0/.gitignore` & `katalytic_files-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic_files-0.9.0/.gitlab-ci.yml` & `katalytic_files-0.9.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic_files-0.9.0/CHANGELOG.md` & `katalytic_files-0.9.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.9.1 (2023-05-31)
+### fix
+- [[`7cdb066`](https://gitlab.com/katalytic/katalytic-files/commit/7cdb066ac2833fb9977ddffafb8f843d066ce1e8)] use the latest signature for sort_dict_by_keys()
+
+
 ## 0.9.0 (2023-05-22)
 ### feat
 - [[`e339626`](https://gitlab.com/katalytic/katalytic-files/commit/e33962652287c979406ecc533da7a55e9cb58e50)] add ujson as optional dependency and try using it instead of the stdlib json for faster load/save
 ### refactor
 - [[`00d80e2`](https://gitlab.com/katalytic/katalytic-files/commit/00d80e2b4b273e595a6f174750a0e69f29540387)] remove unused private function
 - [[`69bd62b`](https://gitlab.com/katalytic/katalytic-files/commit/69bd62be521ca9cf2628eb36b79d327995b5509f)] replace private functions with the ones from katalytic.data
 - [[`7ecef41`](https://gitlab.com/katalytic/katalytic-files/commit/7ecef418d0cd93f92da959c0c16d2ecdfd6c2218)] use is_none_of, is_any_of from katalytic-data
```

### Comparing `katalytic_files-0.9.0/LICENSE.txt` & `katalytic_files-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic_files-0.9.0/README.md` & `katalytic_files-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Not fit for public use yet
+- I will probably introduce backwards incompatible changes
 
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-files)](https://pypi.org/project/katalytic-files/)
 [![tests](https://gitlab.com/katalytic/katalytic-files/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-files/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-files/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-files/-/commits/main)
```

### Comparing `katalytic_files-0.9.0/pyproject.toml` & `katalytic_files-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-files"
-version = "0.9.0"
+version = "0.9.1"
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic_files-0.9.0/src/katalytic/files.py` & `katalytic_files-0.9.1/src/katalytic/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     for func_name, f, groups in get_functions_in_group(group):
         for g in groups:
             ext = g.rpartition('::')[2]
             loaders[ext] = f
 
     # sort the dict with the most specific extension at the beginning
     # this makes it easier to pick ".tar.gz" over ".gz"
-    return sort_dict_by_keys(loaders, key=len, reverse=True)
+    return sort_dict_by_keys(loaders, condition=len, reverse=True)
 
 
 def _setup_load():
     """
     Set up a load function based on the available grouped load functions.
 
     Returns:
```

### Comparing `katalytic_files-0.9.0/tests/test_files.py` & `katalytic_files-0.9.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `katalytic_files-0.9.0/PKG-INFO` & `katalytic_files-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.9.0
+Version: 0.9.1
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Keywords: automation,filesystem
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,14 +26,15 @@
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-files.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-files.git
 Provides-Extra: all
 Provides-Extra: dev
 
 # Not fit for public use yet
+- I will probably introduce backwards incompatible changes
 
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-files)](https://pypi.org/project/katalytic-files/)
 [![tests](https://gitlab.com/katalytic/katalytic-files/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-files/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-files/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-files/-/commits/main)
```

