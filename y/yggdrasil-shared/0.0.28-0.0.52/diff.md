# Comparing `tmp/yggdrasil_shared-0.0.28.tar.gz` & `tmp/yggdrasil_shared-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yggdrasil_shared-0.0.28.tar", last modified: Wed Apr 20 09:29:12 2022, max compression
+gzip compressed data, was "yggdrasil_shared-0.0.52.tar", last modified: Mon Jun 26 12:12:13 2023, max compression
```

## Comparing `yggdrasil_shared-0.0.28.tar` & `yggdrasil_shared-0.0.52.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)        0 2022-04-20 09:29:12.779780 yggdrasil_shared-0.0.28/
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      190 2022-04-20 09:29:12.779780 yggdrasil_shared-0.0.28/PKG-INFO
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)       38 2022-04-20 09:29:12.779780 yggdrasil_shared-0.0.28/setup.cfg
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      558 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/setup.py
-drwxrwxr-x   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)        0 2022-04-20 09:29:12.779780 yggdrasil_shared-0.0.28/yggdrasil_shared/
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      256 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/__init__.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     1793 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/adapters.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      513 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/dependencies.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      187 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/encoders.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     4121 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/events.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     2062 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/exceptions.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      382 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/formatters.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     3899 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/handlers.py
-drwxrwxr-x   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)        0 2022-04-20 09:29:12.779780 yggdrasil_shared-0.0.28/yggdrasil_shared/i18n/
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)        0 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/i18n/__init__.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     6895 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/i18n/translate.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     1746 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/middlewares.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     1785 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/models.py
-drwxrwxr-x   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)        0 2022-04-20 09:29:12.779780 yggdrasil_shared-0.0.28/yggdrasil_shared/monkey_patch/
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)        0 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/monkey_patch/__init__.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      769 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/monkey_patch/werkzeug.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)    14403 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/permissions.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      883 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/responses.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     3295 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/s3_client.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     1479 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/schema.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     2528 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/test_utils.py
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)     6462 2022-04-20 09:22:25.000000 yggdrasil_shared-0.0.28/yggdrasil_shared/utils.py
-drwxrwxr-x   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)        0 2022-04-20 09:29:12.779780 yggdrasil_shared-0.0.28/yggdrasil_shared.egg-info/
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      190 2022-04-20 09:29:12.000000 yggdrasil_shared-0.0.28/yggdrasil_shared.egg-info/PKG-INFO
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      868 2022-04-20 09:29:12.000000 yggdrasil_shared-0.0.28/yggdrasil_shared.egg-info/SOURCES.txt
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)        1 2022-04-20 09:29:12.000000 yggdrasil_shared-0.0.28/yggdrasil_shared.egg-info/dependency_links.txt
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)      131 2022-04-20 09:29:12.000000 yggdrasil_shared-0.0.28/yggdrasil_shared.egg-info/requires.txt
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)       17 2022-04-20 09:29:12.000000 yggdrasil_shared-0.0.28/yggdrasil_shared.egg-info/top_level.txt
--rw-rw-r--   0 aabdolrazaghi  (1000) aabdolrazaghi  (1000)        1 2022-04-20 09:29:12.000000 yggdrasil_shared-0.0.28/yggdrasil_shared.egg-info/zip-safe
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-06-26 12:12:13.704753 yggdrasil_shared-0.0.52/
+-rw-rw-r--   0 sina      (1000) sina      (1000)      179 2023-06-26 12:12:13.704753 yggdrasil_shared-0.0.52/PKG-INFO
+-rw-rw-r--   0 sina      (1000) sina      (1000)      275 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/README.md
+-rw-rw-r--   0 sina      (1000) sina      (1000)       38 2023-06-26 12:12:13.704753 yggdrasil_shared-0.0.52/setup.cfg
+-rw-rw-r--   0 sina      (1000) sina      (1000)      558 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/setup.py
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-06-26 12:12:13.700753 yggdrasil_shared-0.0.52/yggdrasil_shared/
+-rw-rw-r--   0 sina      (1000) sina      (1000)      256 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/__init__.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     1793 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/adapters.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)      513 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/dependencies.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)      362 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/encoders.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     7734 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/entrypoints.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     5782 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/events.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     2062 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/exceptions.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)      382 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/formatters.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     3899 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/handlers.py
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-06-26 12:12:13.704753 yggdrasil_shared-0.0.52/yggdrasil_shared/i18n/
+-rw-rw-r--   0 sina      (1000) sina      (1000)        0 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/i18n/__init__.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     6895 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/i18n/translate.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     1746 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/middlewares.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     1785 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/models.py
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-06-26 12:12:13.704753 yggdrasil_shared-0.0.52/yggdrasil_shared/monkey_patch/
+-rw-rw-r--   0 sina      (1000) sina      (1000)        0 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/monkey_patch/__init__.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)      769 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/monkey_patch/werkzeug.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)    20797 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/permissions.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)      883 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/responses.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     3295 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/s3_client.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     1479 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/schema.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     2528 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/test_utils.py
+-rw-rw-r--   0 sina      (1000) sina      (1000)     6462 2023-06-26 12:11:36.000000 yggdrasil_shared-0.0.52/yggdrasil_shared/utils.py
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-06-26 12:12:13.700753 yggdrasil_shared-0.0.52/yggdrasil_shared.egg-info/
+-rw-rw-r--   0 sina      (1000) sina      (1000)      179 2023-06-26 12:12:13.000000 yggdrasil_shared-0.0.52/yggdrasil_shared.egg-info/PKG-INFO
+-rw-rw-r--   0 sina      (1000) sina      (1000)      910 2023-06-26 12:12:13.000000 yggdrasil_shared-0.0.52/yggdrasil_shared.egg-info/SOURCES.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-06-26 12:12:13.000000 yggdrasil_shared-0.0.52/yggdrasil_shared.egg-info/dependency_links.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)      131 2023-06-26 12:12:13.000000 yggdrasil_shared-0.0.52/yggdrasil_shared.egg-info/requires.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)       17 2023-06-26 12:12:13.000000 yggdrasil_shared-0.0.52/yggdrasil_shared.egg-info/top_level.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-06-26 12:12:13.000000 yggdrasil_shared-0.0.52/yggdrasil_shared.egg-info/zip-safe
```

### Comparing `yggdrasil_shared-0.0.28/setup.py` & `yggdrasil_shared-0.0.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 setup(
     name='yggdrasil_shared',
-    version='0.0.28',
+    version='0.0.52',
     description='Yggdrasil Shared library',
     packages=find_packages(exclude=['tests', 'tests.*']),
     zip_safe=True,
     install_requires=[
         'sqlalchemy~=1.4.0',
         'nameko>=3.0.0',
         'marshmallow==3.6.0',
```

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/adapters.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/adapters.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/dependencies.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/dependencies.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/exceptions.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/handlers.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/handlers.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/i18n/translate.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/i18n/translate.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/middlewares.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/middlewares.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/models.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/models.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/monkey_patch/werkzeug.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/monkey_patch/werkzeug.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/responses.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/responses.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/s3_client.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/s3_client.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/schema.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/schema.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/test_utils.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/test_utils.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared/utils.py` & `yggdrasil_shared-0.0.52/yggdrasil_shared/utils.py`

 * *Files identical despite different names*

### Comparing `yggdrasil_shared-0.0.28/yggdrasil_shared.egg-info/SOURCES.txt` & `yggdrasil_shared-0.0.52/yggdrasil_shared.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+README.md
 setup.py
 yggdrasil_shared/__init__.py
 yggdrasil_shared/adapters.py
 yggdrasil_shared/dependencies.py
 yggdrasil_shared/encoders.py
+yggdrasil_shared/entrypoints.py
 yggdrasil_shared/events.py
 yggdrasil_shared/exceptions.py
 yggdrasil_shared/formatters.py
 yggdrasil_shared/handlers.py
 yggdrasil_shared/middlewares.py
 yggdrasil_shared/models.py
 yggdrasil_shared/permissions.py
```

