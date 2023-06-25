# Comparing `tmp/ngitl_common_py-0.4.2.tar.gz` & `tmp/ngitl_common_py-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngitl_common_py-0.4.2.tar", last modified: Sun Jun 25 22:37:16 2023, max compression
+gzip compressed data, was "ngitl_common_py-0.4.3.tar", last modified: Sun Jun 25 22:59:09 2023, max compression
```

## Comparing `ngitl_common_py-0.4.2.tar` & `ngitl_common_py-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/ngitl_common_py/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/ngitl_common_py/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/autostart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/file_viewer_starter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/log.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/ngitl_common_py/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 22:37:16.000000 ngitl_common_py-0.4.2/ngitl_common_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:37:16.361214 ngitl_common_py-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/tests/test_autostart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    83436 2023-06-25 22:36:59.000000 ngitl_common_py-0.4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:59:09.345339 ngitl_common_py-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 22:59:09.345339 ngitl_common_py-0.4.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:59:09.349339 ngitl_common_py-0.4.3/ngitl_common_py/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/ngitl_common_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-25 22:59:09.349339 ngitl_common_py-0.4.3/ngitl_common_py/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/ngitl_common_py/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/ngitl_common_py/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/ngitl_common_py/file_viewer_starter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/ngitl_common_py/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/ngitl_common_py/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:59:09.345339 ngitl_common_py-0.4.3/ngitl_common_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 22:59:09.000000 ngitl_common_py-0.4.3/ngitl_common_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-25 22:59:09.000000 ngitl_common_py-0.4.3/ngitl_common_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:59:09.000000 ngitl_common_py-0.4.3/ngitl_common_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 22:59:09.000000 ngitl_common_py-0.4.3/ngitl_common_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 22:59:09.000000 ngitl_common_py-0.4.3/ngitl_common_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-25 22:59:09.349339 ngitl_common_py-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:59:09.345339 ngitl_common_py-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/tests/test_autostart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83436 2023-06-25 22:58:59.000000 ngitl_common_py-0.4.3/versioneer.py
```

### Comparing `ngitl_common_py-0.4.2/ngitl_common_py/autostart.py` & `ngitl_common_py-0.4.3/ngitl_common_py/autostart.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.4.2/ngitl_common_py/config.py` & `ngitl_common_py-0.4.3/ngitl_common_py/config.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.4.2/ngitl_common_py/file_viewer_starter.py` & `ngitl_common_py-0.4.3/ngitl_common_py/file_viewer_starter.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.4.2/ngitl_common_py/log.py` & `ngitl_common_py-0.4.3/ngitl_common_py/log.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.4.2/setup.py` & `ngitl_common_py-0.4.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,8 +13,9 @@
     long_description="Helper classes and functions for common python problems",
     author="NG:ITL",
     license="GPLv3",
     author_email="torsten.wylegala@volkswagen.de",
     url="https://github.com/vw-wob-it-edu-ngitl/ngitl_common_py/",
     packages=find_packages("."),
     install_requires=["pywin32==306"],
+    include_package_data=True,
 )
```

### Comparing `ngitl_common_py-0.4.2/tests/test_autostart.py` & `ngitl_common_py-0.4.3/tests/test_autostart.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.4.2/tests/test_log.py` & `ngitl_common_py-0.4.3/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `ngitl_common_py-0.4.2/versioneer.py` & `ngitl_common_py-0.4.3/versioneer.py`

 * *Files identical despite different names*

