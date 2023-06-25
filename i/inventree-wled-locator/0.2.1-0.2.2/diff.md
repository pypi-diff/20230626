# Comparing `tmp/inventree-wled-locator-0.2.1.tar.gz` & `tmp/inventree-wled-locator-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/inventree-wled-locator/inventree-wled-locator/dist/.tmp-4m9_h04n/inventree-wled-locator-0.2.1.tar", last modified: Sun Jun 25 19:56:32 2023, max compression
+gzip compressed data, was "/home/runner/work/inventree-wled-locator/inventree-wled-locator/dist/.tmp-hzf9p968/inventree-wled-locator-0.2.2.tar", last modified: Sun Jun 25 22:30:52 2023, max compression
```

## Comparing `inventree-wled-locator-0.2.1.tar` & `inventree-wled-locator-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator/
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator/WledPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:30:52.000000 inventree-wled-locator-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 22:30:28.000000 inventree-wled-locator-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 22:30:28.000000 inventree-wled-locator-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-25 22:30:52.000000 inventree-wled-locator-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 22:30:28.000000 inventree-wled-locator-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-25 22:30:28.000000 inventree-wled-locator-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-25 22:30:52.000000 inventree-wled-locator-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:30:52.000000 inventree-wled-locator-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:30:52.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator/
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-25 22:30:28.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator/WledPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 22:30:28.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:30:52.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-25 22:30:51.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-25 22:30:52.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:30:51.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 22:30:51.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-25 22:30:52.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 22:30:52.000000 inventree-wled-locator-0.2.2/src/inventree_wled_locator.egg-info/top_level.txt
```

### Comparing `inventree-wled-locator-0.2.1/LICENSE` & `inventree-wled-locator-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-wled-locator-0.2.1/PKG-INFO` & `inventree-wled-locator-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wled-locator
-Version: 0.2.1
+Version: 0.2.2
 Summary: Use WLED to locate InvenTree StockLocations.
 Author-email: Matthias Mair <code@mjmair.com>
 License: MIT license
 Project-URL: Repository, https://github.com/matmair/inventree-wled-locator
 Project-URL: Bug Tracker, https://github.com/matmair/inventree-wled-locator/issues
 Keywords: inventree,inventree-plugin,inventree-wled-locator
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inventree-wled-locator-0.2.1/README.md` & `inventree-wled-locator-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `inventree-wled-locator-0.2.1/pyproject.toml` & `inventree-wled-locator-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel", "pyyaml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inventree-wled-locator"
-version =  "0.2.1"
+version =  "0.2.2"
 description="Use WLED to locate InvenTree StockLocations."
 readme = "README.md"
 license = {text = "MIT license"}
 keywords = ["inventree", "inventree-plugin", "inventree-wled-locator"]
 authors = [
     {name = "Matthias Mair", email =  "code@mjmair.com"}
 ]
```

### Comparing `inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/PKG-INFO` & `inventree-wled-locator-0.2.2/src/inventree_wled_locator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wled-locator
-Version: 0.2.1
+Version: 0.2.2
 Summary: Use WLED to locate InvenTree StockLocations.
 Author-email: Matthias Mair <code@mjmair.com>
 License: MIT license
 Project-URL: Repository, https://github.com/matmair/inventree-wled-locator
 Project-URL: Bug Tracker, https://github.com/matmair/inventree-wled-locator/issues
 Keywords: inventree,inventree-plugin,inventree-wled-locator
 Classifier: Programming Language :: Python :: 3
```

