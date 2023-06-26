# Comparing `tmp/biosimulators_amici-0.1.8.tar.gz` & `tmp/biosimulators_amici-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biosimulators_amici-0.1.8.tar", last modified: Wed Mar 24 19:29:37 2021, max compression
+gzip compressed data, was "dist/biosimulators_amici-0.1.9.tar", last modified: Thu Mar 25 07:48:55 2021, max compression
```

## Comparing `biosimulators_amici-0.1.8.tar` & `biosimulators_amici-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5808 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3943 2021-03-24 19:29:31.000000 biosimulators_amici-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/biosimulators_amici/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/biosimulators_amici/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/biosimulators_amici/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/biosimulators_amici/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    12556 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/biosimulators_amici/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/biosimulators_amici/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/biosimulators_amici.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5808 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/biosimulators_amici.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/biosimulators_amici.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/biosimulators_amici.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/biosimulators_amici.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/biosimulators_amici.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/biosimulators_amici.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/requirements.optional.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-03-24 19:29:37.000000 biosimulators_amici-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2021-03-24 19:15:27.000000 biosimulators_amici-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-25 07:48:55.000000 biosimulators_amici-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5808 2021-03-25 07:48:55.000000 biosimulators_amici-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3943 2021-03-25 07:48:50.000000 biosimulators_amici-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-25 07:48:55.000000 biosimulators_amici-0.1.9/biosimulators_amici/
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/biosimulators_amici/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/biosimulators_amici/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/biosimulators_amici/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12556 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/biosimulators_amici/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/biosimulators_amici/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-25 07:48:55.000000 biosimulators_amici-0.1.9/biosimulators_amici.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5808 2021-03-25 07:48:54.000000 biosimulators_amici-0.1.9/biosimulators_amici.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-03-25 07:48:54.000000 biosimulators_amici-0.1.9/biosimulators_amici.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-25 07:48:54.000000 biosimulators_amici-0.1.9/biosimulators_amici.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-03-25 07:48:54.000000 biosimulators_amici-0.1.9/biosimulators_amici.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-03-25 07:48:54.000000 biosimulators_amici-0.1.9/biosimulators_amici.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-25 07:48:54.000000 biosimulators_amici-0.1.9/biosimulators_amici.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/requirements.optional.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-03-25 07:48:55.000000 biosimulators_amici-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1973 2021-03-25 07:38:44.000000 biosimulators_amici-0.1.9/setup.py
```

### Comparing `biosimulators_amici-0.1.8/LICENSE` & `biosimulators_amici-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biosimulators_amici-0.1.8/PKG-INFO` & `biosimulators_amici-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosimulators_amici
-Version: 0.1.8
+Version: 0.1.9
 Summary: BioSimulators-compliant command-line interface to the AMICI simulation program <https://github.com/AMICI-dev/amici>.
 Home-page: https://github.com/biosimulators/Biosimulators_AMICI>
 Author: Center for Reproducible Biomedical Modeling
 Author-email: info@biosimulators.org
 License: MIT
 Download-URL: https://github.com/biosimulators/Biosimulators_AMICI
 Description: |Latest release| |PyPI| |CI status| |Test coverage|
```

### Comparing `biosimulators_amici-0.1.8/README.rst` & `biosimulators_amici-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `biosimulators_amici-0.1.8/biosimulators_amici/__main__.py` & `biosimulators_amici-0.1.9/biosimulators_amici/__main__.py`

 * *Files identical despite different names*

### Comparing `biosimulators_amici-0.1.8/biosimulators_amici/core.py` & `biosimulators_amici-0.1.9/biosimulators_amici/core.py`

 * *Files identical despite different names*

### Comparing `biosimulators_amici-0.1.8/biosimulators_amici/data_model.py` & `biosimulators_amici-0.1.9/biosimulators_amici/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_amici-0.1.8/biosimulators_amici.egg-info/PKG-INFO` & `biosimulators_amici-0.1.9/biosimulators_amici.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosimulators-amici
-Version: 0.1.8
+Version: 0.1.9
 Summary: BioSimulators-compliant command-line interface to the AMICI simulation program <https://github.com/AMICI-dev/amici>.
 Home-page: https://github.com/biosimulators/Biosimulators_AMICI>
 Author: Center for Reproducible Biomedical Modeling
 Author-email: info@biosimulators.org
 License: MIT
 Download-URL: https://github.com/biosimulators/Biosimulators_AMICI
 Description: |Latest release| |PyPI| |CI status| |Test coverage|
```

### Comparing `biosimulators_amici-0.1.8/setup.py` & `biosimulators_amici-0.1.9/setup.py`

 * *Files identical despite different names*

