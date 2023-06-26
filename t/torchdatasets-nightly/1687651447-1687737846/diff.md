# Comparing `tmp/torchdatasets-nightly-1687651447.tar.gz` & `tmp/torchdatasets-nightly-1687737846.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchdatasets-nightly-1687651447.tar", last modified: Sun Jun 25 00:04:11 2023, max compression
+gzip compressed data, was "dist/torchdatasets-nightly-1687737846.tar", last modified: Mon Jun 26 00:04:18 2023, max compression
```

## Comparing `torchdatasets-nightly-1687651447.tar` & `torchdatasets-nightly-1687737846.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/tests/cachers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/tests/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/tests/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/tests/maps_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/tests/modifiers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/tests/samplers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/tests/torchdata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/torchdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/_dev_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/cachers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24308 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-06-25 00:04:07.000000 torchdatasets-nightly-1687651447/torchdatasets/samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/torchdatasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/torchdatasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/torchdatasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/torchdatasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/torchdatasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 00:04:11.000000 torchdatasets-nightly-1687651447/torchdatasets_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:04:18.000000 torchdatasets-nightly-1687737846/
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-26 00:04:18.000000 torchdatasets-nightly-1687737846/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 00:04:18.000000 torchdatasets-nightly-1687737846/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:04:18.000000 torchdatasets-nightly-1687737846/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/tests/cachers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/tests/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/tests/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/tests/maps_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/tests/modifiers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/tests/samplers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/tests/torchdata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:04:18.000000 torchdatasets-nightly-1687737846/torchdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/_dev_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/cachers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24308 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-06-26 00:04:06.000000 torchdatasets-nightly-1687737846/torchdatasets/samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:04:18.000000 torchdatasets-nightly-1687737846/torchdatasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-26 00:04:17.000000 torchdatasets-nightly-1687737846/torchdatasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-26 00:04:18.000000 torchdatasets-nightly-1687737846/torchdatasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:04:17.000000 torchdatasets-nightly-1687737846/torchdatasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 00:04:17.000000 torchdatasets-nightly-1687737846/torchdatasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 00:04:17.000000 torchdatasets-nightly-1687737846/torchdatasets_nightly.egg-info/top_level.txt
```

### Comparing `torchdatasets-nightly-1687651447/PKG-INFO` & `torchdatasets-nightly-1687737846/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchdatasets-nightly
-Version: 1687651447
+Version: 1687737846
 Summary: PyTorch based library focused on data processing and input pipelines in general.
 Home-page: https://github.com/szymonmaszke/torchdatasets
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchdatasets
 Project-URL: Documentation, https://szymonmaszke.github.io/torchdatasets/#torchdatasets
```

### Comparing `torchdatasets-nightly-1687651447/README.md` & `torchdatasets-nightly-1687737846/README.md`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/setup.py` & `torchdatasets-nightly-1687737846/setup.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/tests/cachers_test.py` & `torchdatasets-nightly-1687737846/tests/cachers_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/tests/datasets.py` & `torchdatasets-nightly-1687737846/tests/datasets.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/tests/datasets_test.py` & `torchdatasets-nightly-1687737846/tests/datasets_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/tests/maps_test.py` & `torchdatasets-nightly-1687737846/tests/maps_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/tests/modifiers_test.py` & `torchdatasets-nightly-1687737846/tests/modifiers_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/tests/samplers_test.py` & `torchdatasets-nightly-1687737846/tests/samplers_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/tests/torchdata_test.py` & `torchdatasets-nightly-1687737846/tests/torchdata_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/tests/utils.py` & `torchdatasets-nightly-1687737846/tests/utils.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/torchdatasets/__init__.py` & `torchdatasets-nightly-1687737846/torchdatasets/__init__.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/torchdatasets/_base.py` & `torchdatasets-nightly-1687737846/torchdatasets/_base.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/torchdatasets/cachers.py` & `torchdatasets-nightly-1687737846/torchdatasets/cachers.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/torchdatasets/datasets.py` & `torchdatasets-nightly-1687737846/torchdatasets/datasets.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/torchdatasets/maps.py` & `torchdatasets-nightly-1687737846/torchdatasets/maps.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/torchdatasets/modifiers.py` & `torchdatasets-nightly-1687737846/torchdatasets/modifiers.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/torchdatasets/samplers.py` & `torchdatasets-nightly-1687737846/torchdatasets/samplers.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1687651447/torchdatasets_nightly.egg-info/PKG-INFO` & `torchdatasets-nightly-1687737846/torchdatasets_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchdatasets-nightly
-Version: 1687651447
+Version: 1687737846
 Summary: PyTorch based library focused on data processing and input pipelines in general.
 Home-page: https://github.com/szymonmaszke/torchdatasets
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchdatasets
 Project-URL: Documentation, https://szymonmaszke.github.io/torchdatasets/#torchdatasets
```

### Comparing `torchdatasets-nightly-1687651447/torchdatasets_nightly.egg-info/SOURCES.txt` & `torchdatasets-nightly-1687737846/torchdatasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

