# Comparing `tmp/PVNet-2.0.0.tar.gz` & `tmp/PVNet-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-2.0.0.tar", last modified: Mon Jun 26 08:33:46 2023, max compression
+gzip compressed data, was "PVNet-2.1.0.tar", last modified: Mon Jun 26 08:36:47 2023, max compression
```

## Comparing `PVNet-2.0.0.tar` & `PVNet-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:33:46.130437 PVNet-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-26 08:33:34.000000 PVNet-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 08:33:34.000000 PVNet-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-26 08:33:46.130437 PVNet-2.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:33:46.126438 PVNet-2.0.0/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-26 08:33:46.000000 PVNet-2.0.0/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 08:33:46.000000 PVNet-2.0.0/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:33:46.000000 PVNet-2.0.0/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 08:33:46.000000 PVNet-2.0.0/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 08:33:46.000000 PVNet-2.0.0/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-26 08:33:34.000000 PVNet-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:33:46.130437 PVNet-2.0.0/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 08:33:34.000000 PVNet-2.0.0/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-26 08:33:34.000000 PVNet-2.0.0/pvnet/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-26 08:33:34.000000 PVNet-2.0.0/pvnet/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-26 08:33:34.000000 PVNet-2.0.0/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 08:33:34.000000 PVNet-2.0.0/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-26 08:33:34.000000 PVNet-2.0.0/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-26 08:33:34.000000 PVNet-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 08:33:34.000000 PVNet-2.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-26 08:33:34.000000 PVNet-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:33:46.130437 PVNet-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-26 08:33:34.000000 PVNet-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:33:46.130437 PVNet-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:33:34.000000 PVNet-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-26 08:33:34.000000 PVNet-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 08:33:34.000000 PVNet-2.0.0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:36:47.659182 PVNet-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-26 08:36:35.000000 PVNet-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 08:36:35.000000 PVNet-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-26 08:36:47.659182 PVNet-2.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:36:47.659182 PVNet-2.1.0/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-26 08:36:47.000000 PVNet-2.1.0/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 08:36:47.000000 PVNet-2.1.0/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:36:47.000000 PVNet-2.1.0/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 08:36:47.000000 PVNet-2.1.0/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 08:36:47.000000 PVNet-2.1.0/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-26 08:36:35.000000 PVNet-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:36:47.659182 PVNet-2.1.0/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 08:36:35.000000 PVNet-2.1.0/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-26 08:36:35.000000 PVNet-2.1.0/pvnet/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-26 08:36:35.000000 PVNet-2.1.0/pvnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-26 08:36:35.000000 PVNet-2.1.0/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 08:36:35.000000 PVNet-2.1.0/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-26 08:36:35.000000 PVNet-2.1.0/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-26 08:36:35.000000 PVNet-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 08:36:35.000000 PVNet-2.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-26 08:36:35.000000 PVNet-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:36:47.659182 PVNet-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-26 08:36:35.000000 PVNet-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:36:47.659182 PVNet-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:36:35.000000 PVNet-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-26 08:36:35.000000 PVNet-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 08:36:35.000000 PVNet-2.1.0/tests/test_app.py
```

### Comparing `PVNet-2.0.0/LICENSE` & `PVNet-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-2.0.0/pvnet/app.py` & `PVNet-2.1.0/pvnet/app.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.0.0/pvnet/callbacks.py` & `PVNet-2.1.0/pvnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.0.0/pvnet/optimizers.py` & `PVNet-2.1.0/pvnet/optimizers.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.0.0/pvnet/training.py` & `PVNet-2.1.0/pvnet/training.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.0.0/pvnet/utils.py` & `PVNet-2.1.0/pvnet/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.0.0/setup.py` & `PVNet-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.0.0/tests/conftest.py` & `PVNet-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.0.0/tests/test_app.py` & `PVNet-2.1.0/tests/test_app.py`

 * *Files identical despite different names*

