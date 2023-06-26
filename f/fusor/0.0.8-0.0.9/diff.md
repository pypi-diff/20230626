# Comparing `tmp/fusor-0.0.8.tar.gz` & `tmp/fusor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusor-0.0.8.tar", last modified: Sun Sep 19 18:49:16 2021, max compression
+gzip compressed data, was "fusor-0.0.9.tar", last modified: Thu Sep 30 18:21:23 2021, max compression
```

## Comparing `fusor-0.0.8.tar` & `fusor-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 18:49:16.853318 fusor-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-09-19 18:49:03.000000 fusor-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-09-19 18:49:16.853318 fusor-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-09-19 18:49:03.000000 fusor-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 18:49:16.849318 fusor-0.0.8/fusor/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-09-19 18:49:03.000000 fusor-0.0.8/fusor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14332 2021-09-19 18:49:03.000000 fusor-0.0.8/fusor/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 18:49:16.853318 fusor-0.0.8/fusor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-09-19 18:49:16.000000 fusor-0.0.8/fusor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-09-19 18:49:16.000000 fusor-0.0.8/fusor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-19 18:49:16.000000 fusor-0.0.8/fusor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-19 18:49:16.000000 fusor-0.0.8/fusor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-09-19 18:49:16.000000 fusor-0.0.8/fusor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-19 18:49:16.000000 fusor-0.0.8/fusor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      650 2021-09-19 18:49:16.853318 fusor-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-09-19 18:49:03.000000 fusor-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 18:21:23.439025 fusor-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-09-30 18:21:11.000000 fusor-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-09-30 18:21:23.439025 fusor-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-09-30 18:21:11.000000 fusor-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 18:21:23.435025 fusor-0.0.9/fusor/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-09-30 18:21:11.000000 fusor-0.0.9/fusor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17125 2021-09-30 18:21:11.000000 fusor-0.0.9/fusor/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 18:21:23.435025 fusor-0.0.9/fusor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-09-30 18:21:23.000000 fusor-0.0.9/fusor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2021-09-30 18:21:23.000000 fusor-0.0.9/fusor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-30 18:21:23.000000 fusor-0.0.9/fusor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-30 18:21:23.000000 fusor-0.0.9/fusor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-09-30 18:21:23.000000 fusor-0.0.9/fusor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-30 18:21:23.000000 fusor-0.0.9/fusor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2021-09-30 18:21:23.439025 fusor-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-09-30 18:21:11.000000 fusor-0.0.9/setup.py
```

### Comparing `fusor-0.0.8/LICENSE` & `fusor-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fusor-0.0.8/PKG-INFO` & `fusor-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provide computable object representation and validation for gene fusions
 Home-page: https://github.com/cancervariants/fusor
 Author: Wagner Lab, Nationwide Childrens Hospital
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fusor-0.0.8/README.md` & `fusor-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fusor-0.0.8/fusor.egg-info/PKG-INFO` & `fusor-0.0.9/fusor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provide computable object representation and validation for gene fusions
 Home-page: https://github.com/cancervariants/fusor
 Author: Wagner Lab, Nationwide Childrens Hospital
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fusor-0.0.8/setup.cfg` & `fusor-0.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 include_package_data = True
 install_requires = 
 	pydantic
 	ga4gh.vrsatile.pydantic
+	ga4gh.vrs[extras] == 0.7.0rc3
+	jsonschema >=2.3, <4.0
 tests_require = 
 	pytest
 	pytest-cov
 
 [tool:pytest]
 addopts = --ignore setup.py --doctest-modules --cov-report term-missing --disable-warnings --cov .
```

