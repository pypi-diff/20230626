# Comparing `tmp/dargus-1.1.0.tar.gz` & `tmp/dargus-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dapregi/dev/argus/dist/.tmp-6fj1dhkr/dargus-1.1.0.tar", last modified: Mon Jun 19 16:05:29 2023, max compression
+gzip compressed data, was "/home/dapregi/dev/argus/dist/.tmp-92zwxa0a/dargus-1.1.1.tar", last modified: Mon Jun 26 16:14:49 2023, max compression
```

## Comparing `dargus-1.1.0.tar` & `dargus-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-06-19 16:05:29.000000 dargus-1.1.0/
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)    11357 2020-07-29 10:38:30.000000 dargus-1.1.0/LICENSE
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-06-19 16:05:29.000000 dargus-1.1.0/PKG-INFO
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       73 2023-06-01 15:53:34.000000 dargus-1.1.0/README.md
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus/
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        0 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/__init__.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13373 2023-06-19 16:04:17.000000 dargus-1.1.0/dargus/argus.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1940 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/argus_cli.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     2350 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/argus_config.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       43 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/argus_exceptions.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      928 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/commons.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1577 2023-06-19 16:04:17.000000 dargus-1.1.0/dargus/utils.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      889 2023-06-01 15:53:34.000000 dargus-1.1.0/dargus/validation_result.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     7180 2023-06-19 16:04:17.000000 dargus-1.1.0/dargus/validator.py
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/PKG-INFO
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      410 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/SOURCES.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        1 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/dependency_links.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       49 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/entry_points.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       29 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/requires.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        7 2023-06-19 16:05:29.000000 dargus-1.1.0/dargus.egg-info/top_level.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1042 2023-06-19 16:04:17.000000 dargus-1.1.0/pyproject.toml
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       38 2023-06-19 16:05:29.000000 dargus-1.1.0/setup.cfg
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       92 2023-06-01 15:53:34.000000 dargus-1.1.0/setup.py
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-06-26 16:14:49.000000 dargus-1.1.1/
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)    11357 2020-07-29 10:38:30.000000 dargus-1.1.1/LICENSE
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-06-26 16:14:49.000000 dargus-1.1.1/PKG-INFO
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       73 2023-06-01 15:53:34.000000 dargus-1.1.1/README.md
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-06-26 16:14:49.000000 dargus-1.1.1/dargus/
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        0 2023-06-01 15:53:34.000000 dargus-1.1.1/dargus/__init__.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13373 2023-06-26 15:21:21.000000 dargus-1.1.1/dargus/argus.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1940 2023-06-01 15:53:34.000000 dargus-1.1.1/dargus/argus_cli.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     2350 2023-06-01 15:53:34.000000 dargus-1.1.1/dargus/argus_config.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       43 2023-06-01 15:53:34.000000 dargus-1.1.1/dargus/argus_exceptions.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      928 2023-06-01 15:53:34.000000 dargus-1.1.1/dargus/commons.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1760 2023-06-26 16:12:05.000000 dargus-1.1.1/dargus/utils.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      889 2023-06-01 15:53:34.000000 dargus-1.1.1/dargus/validation_result.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     7180 2023-06-26 15:54:00.000000 dargus-1.1.1/dargus/validator.py
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-06-26 16:14:49.000000 dargus-1.1.1/dargus.egg-info/
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-06-26 16:14:49.000000 dargus-1.1.1/dargus.egg-info/PKG-INFO
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      410 2023-06-26 16:14:49.000000 dargus-1.1.1/dargus.egg-info/SOURCES.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        1 2023-06-26 16:14:49.000000 dargus-1.1.1/dargus.egg-info/dependency_links.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       49 2023-06-26 16:14:49.000000 dargus-1.1.1/dargus.egg-info/entry_points.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       29 2023-06-26 16:14:49.000000 dargus-1.1.1/dargus.egg-info/requires.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        7 2023-06-26 16:14:49.000000 dargus-1.1.1/dargus.egg-info/top_level.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1042 2023-06-26 15:58:41.000000 dargus-1.1.1/pyproject.toml
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       38 2023-06-26 16:14:49.000000 dargus-1.1.1/setup.cfg
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       92 2023-06-01 15:53:34.000000 dargus-1.1.1/setup.py
```

### Comparing `dargus-1.1.0/LICENSE` & `dargus-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dargus-1.1.0/PKG-INFO` & `dargus-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargus
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python engine for testing and benchmarking REST web services
 Author-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 Maintainer-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dargus-1.1.0/dargus/argus.py` & `dargus-1.1.1/dargus/argus.py`

 * *Files identical despite different names*

### Comparing `dargus-1.1.0/dargus/argus_cli.py` & `dargus-1.1.1/dargus/argus_cli.py`

 * *Files identical despite different names*

### Comparing `dargus-1.1.0/dargus/argus_config.py` & `dargus-1.1.1/dargus/argus_config.py`

 * *Files identical despite different names*

### Comparing `dargus-1.1.0/dargus/commons.py` & `dargus-1.1.1/dargus/commons.py`

 * *Files identical despite different names*

### Comparing `dargus-1.1.0/dargus/validation_result.py` & `dargus-1.1.1/dargus/validation_result.py`

 * *Files identical despite different names*

### Comparing `dargus-1.1.0/dargus/validator.py` & `dargus-1.1.1/dargus/validator.py`

 * *Files identical despite different names*

### Comparing `dargus-1.1.0/dargus.egg-info/PKG-INFO` & `dargus-1.1.1/dargus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargus
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python engine for testing and benchmarking REST web services
 Author-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 Maintainer-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dargus-1.1.0/pyproject.toml` & `dargus-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["dargus"]
 
 [project]
 name = "dargus"
-version = "1.1.0"
+version = "1.1.1"
 description = "A Python engine for testing and benchmarking REST web services"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 authors = [
   {name="Daniel Perez-Gil", email="daniel.perez@zettagenomics.com"}
 ]
```

