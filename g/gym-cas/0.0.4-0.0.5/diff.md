# Comparing `tmp/gym_cas-0.0.4.tar.gz` & `tmp/gym_cas-0.0.5.tar.gz`

## Comparing `gym_cas-0.0.4.tar` & `gym_cas-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,19 @@
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gym_cas-0.0.4/src/gym_cas/__about__.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 gym_cas-0.0.4/src/gym_cas/__init__.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 gym_cas-0.0.4/src/gym_cas/trigonometry.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 gym_cas-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gym_cas-0.0.4/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gym_cas-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 gym_cas-0.0.4/README.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gym_cas-0.0.4/hatch.toml
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 gym_cas-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 gym_cas-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gym_cas-0.0.5/bitbucket-pipelines.yml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 gym_cas-0.0.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gym_cas-0.0.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 gym_cas-0.0.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 gym_cas-0.0.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gym_cas-0.0.5/src/gym_cas/__about__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 gym_cas-0.0.5/src/gym_cas/__init__.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 gym_cas-0.0.5/src/gym_cas/trigonometry.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 gym_cas-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 gym_cas-0.0.5/tests/test_abc.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 gym_cas-0.0.5/tests/test_trigonometry.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gym_cas-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gym_cas-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 gym_cas-0.0.5/README.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gym_cas-0.0.5/hatch.toml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 gym_cas-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 gym_cas-0.0.5/PKG-INFO
```

### Comparing `gym_cas-0.0.4/src/gym_cas/trigonometry.py` & `gym_cas-0.0.5/src/gym_cas/trigonometry.py`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.4/LICENSE.txt` & `gym_cas-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.4/hatch.toml` & `gym_cas-0.0.5/hatch.toml`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.4/pyproject.toml` & `gym_cas-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,33 +5,39 @@
 [project]
 name = "gym-cas"
 dynamic = ["version"]
 description = "Tools to aid the use of Python as CAS in danish high schools."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
-keywords = ["matematik, math, gymnasie, HTX, sympy"]
+keywords = ["matematik, math, gymnasium, HTX, sympy"]
 authors = [
   { name = "JACS", email = "jacs@zbc.dk" },
 ]
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["sympy>=1.12"]
 
 [project.urls]
 "Homepage" = "https://jacs-mat.bitbucket.io/"
 
 [tool.black]
 target-version = ["py37"]
 line-length = 120
 skip-string-normalization = true
 
+[tool.pyright]
+reportWildcardImportFromLibrary = false
+
 [tool.ruff]
 target-version = "py37"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
@@ -79,14 +85,17 @@
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
+[tool.pytest.ini_options]
+python_functions = "test_"
+
 [tool.coverage.run]
 source_pkgs = ["gym_cas", "tests"]
 branch = true
 parallel = true
 omit = [
   "src/gym_cas/__about__.py",
 ]
```

### Comparing `gym_cas-0.0.4/PKG-INFO` & `gym_cas-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: gym-cas
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools to aid the use of Python as CAS in danish high schools.
 Project-URL: Homepage, https://jacs-mat.bitbucket.io/
 Author-email: JACS <jacs@zbc.dk>
 License-Expression: MIT
 License-File: LICENSE.txt
-Keywords: matematik, math, gymnasie, HTX, sympy
+Keywords: matematik, math, gymnasium, HTX, sympy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: sympy>=1.12
 Description-Content-Type: text/markdown
 
 # GYM CAS
 
 [![PyPI - Version](https://img.shields.io/pypi/v/gym-cas.svg)](https://pypi.org/project/gym-cas)
@@ -24,7 +27,12 @@
 ## Installation
 
 ```console
 pip install gym-cas
 ```
 
 ## Eksempler
+
+```py
+from gym_cas import *
+print(Sin(80))
+```
```

