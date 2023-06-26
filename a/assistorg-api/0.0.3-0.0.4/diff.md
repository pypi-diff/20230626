# Comparing `tmp/assistorg-api-0.0.3.tar.gz` & `tmp/assistorg_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistorg-api-0.0.3.tar", last modified: Mon Jun 26 03:48:49 2023, max compression
+gzip compressed data, was "assistorg_api-0.0.4.tar", last modified: Mon Jun 26 03:58:44 2023, max compression
```

## Comparing `assistorg-api-0.0.3.tar` & `assistorg_api-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:48:49.962809 assistorg-api-0.0.3/
--rw-r--r--   0 monte      (501) staff       (20)      188 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/AUTHORS.rst
--rw-r--r--   0 monte      (501) staff       (20)     3707 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/CONTRIBUTING.rst
--rw-r--r--   0 monte      (501) staff       (20)     1086 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/LICENSE
--rw-r--r--   0 monte      (501) staff       (20)      262 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/MANIFEST.in
--rw-r--r--   0 monte      (501) staff       (20)     1479 2023-06-26 03:48:49.962870 assistorg-api-0.0.3/PKG-INFO
--rw-r--r--   0 monte      (501) staff       (20)      670 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/README.md
-drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:48:49.960985 assistorg-api-0.0.3/assistorg_api.egg-info/
--rw-r--r--   0 monte      (501) staff       (20)     1479 2023-06-26 03:48:49.000000 assistorg-api-0.0.3/assistorg_api.egg-info/PKG-INFO
--rw-r--r--   0 monte      (501) staff       (20)      477 2023-06-26 03:48:49.000000 assistorg-api-0.0.3/assistorg_api.egg-info/SOURCES.txt
--rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 03:48:49.000000 assistorg-api-0.0.3/assistorg_api.egg-info/dependency_links.txt
--rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 03:43:23.000000 assistorg-api-0.0.3/assistorg_api.egg-info/not-zip-safe
--rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 03:48:49.000000 assistorg-api-0.0.3/assistorg_api.egg-info/top_level.txt
-drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:48:49.962409 assistorg-api-0.0.3/docs/
--rw-r--r--   0 monte      (501) staff       (20)      619 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/Makefile
--rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/authors.rst
--rw-r--r--   0 monte      (501) staff       (20)     4966 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/conf.py
--rw-r--r--   0 monte      (501) staff       (20)       33 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/contributing.rst
--rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/history.rst
--rw-r--r--   0 monte      (501) staff       (20)      315 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/index.rst
--rw-r--r--   0 monte      (501) staff       (20)     1270 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/installation.rst
--rw-r--r--   0 monte      (501) staff       (20)      780 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/make.bat
--rw-r--r--   0 monte      (501) staff       (20)       27 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/readme.rst
--rw-r--r--   0 monte      (501) staff       (20)       91 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/usage.rst
--rw-r--r--   0 monte      (501) staff       (20)      385 2023-06-26 03:48:49.963088 assistorg-api-0.0.3/setup.cfg
--rw-r--r--   0 monte      (501) staff       (20)     1378 2023-06-26 03:46:16.000000 assistorg-api-0.0.3/setup.py
-drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:48:49.962678 assistorg-api-0.0.3/tests/
--rw-r--r--   0 monte      (501) staff       (20)       48 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/tests/__init__.py
--rw-r--r--   0 monte      (501) staff       (20)      442 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/tests/test_assist_api_wrapper.py
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:58:44.756152 assistorg_api-0.0.4/
+-rw-r--r--   0 monte      (501) staff       (20)      188 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/AUTHORS.rst
+-rw-r--r--   0 monte      (501) staff       (20)     3707 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 monte      (501) staff       (20)     1086 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/LICENSE
+-rw-r--r--   0 monte      (501) staff       (20)      262 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/MANIFEST.in
+-rw-r--r--   0 monte      (501) staff       (20)     1479 2023-06-26 03:58:44.756223 assistorg_api-0.0.4/PKG-INFO
+-rw-r--r--   0 monte      (501) staff       (20)      670 2023-06-26 03:52:34.000000 assistorg_api-0.0.4/README.md
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:58:44.754410 assistorg_api-0.0.4/assistorg_api.egg-info/
+-rw-r--r--   0 monte      (501) staff       (20)     1479 2023-06-26 03:58:44.000000 assistorg_api-0.0.4/assistorg_api.egg-info/PKG-INFO
+-rw-r--r--   0 monte      (501) staff       (20)      477 2023-06-26 03:58:44.000000 assistorg_api-0.0.4/assistorg_api.egg-info/SOURCES.txt
+-rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 03:58:44.000000 assistorg_api-0.0.4/assistorg_api.egg-info/dependency_links.txt
+-rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 03:43:23.000000 assistorg_api-0.0.4/assistorg_api.egg-info/not-zip-safe
+-rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 03:58:44.000000 assistorg_api-0.0.4/assistorg_api.egg-info/top_level.txt
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:58:44.755755 assistorg_api-0.0.4/docs/
+-rw-r--r--   0 monte      (501) staff       (20)      619 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/Makefile
+-rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/authors.rst
+-rw-r--r--   0 monte      (501) staff       (20)     4966 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/conf.py
+-rw-r--r--   0 monte      (501) staff       (20)       33 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/contributing.rst
+-rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/history.rst
+-rw-r--r--   0 monte      (501) staff       (20)      315 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/index.rst
+-rw-r--r--   0 monte      (501) staff       (20)     1270 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/installation.rst
+-rw-r--r--   0 monte      (501) staff       (20)      780 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/make.bat
+-rw-r--r--   0 monte      (501) staff       (20)       27 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/readme.rst
+-rw-r--r--   0 monte      (501) staff       (20)       91 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/docs/usage.rst
+-rw-r--r--   0 monte      (501) staff       (20)      385 2023-06-26 03:58:44.756551 assistorg_api-0.0.4/setup.cfg
+-rw-r--r--   0 monte      (501) staff       (20)     1378 2023-06-26 03:58:20.000000 assistorg_api-0.0.4/setup.py
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:58:44.756002 assistorg_api-0.0.4/tests/
+-rw-r--r--   0 monte      (501) staff       (20)       48 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/tests/__init__.py
+-rw-r--r--   0 monte      (501) staff       (20)      442 2023-06-26 03:31:11.000000 assistorg_api-0.0.4/tests/test_assist_api_wrapper.py
```

### Comparing `assistorg-api-0.0.3/CONTRIBUTING.rst` & `assistorg_api-0.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.3/LICENSE` & `assistorg_api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.3/PKG-INFO` & `assistorg_api-0.0.4/assistorg_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistorg-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unofficial API wrapper for ASSIST.org's API.
 Home-page: https://github.com/montesclarosglennbenedict/assistapi-org
 Author: Glenn Benedict Montesclaros
 Author-email: montesclarosglennbenedict@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assistorg-api-0.0.3/README.md` & `assistorg_api-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.3/assistorg_api.egg-info/PKG-INFO` & `assistorg_api-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: assistorg-api
-Version: 0.0.3
+Name: assistorg_api
+Version: 0.0.4
 Summary: Unofficial API wrapper for ASSIST.org's API.
 Home-page: https://github.com/montesclarosglennbenedict/assistapi-org
 Author: Glenn Benedict Montesclaros
 Author-email: montesclarosglennbenedict@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assistorg-api-0.0.3/docs/Makefile` & `assistorg_api-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.3/docs/conf.py` & `assistorg_api-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.3/docs/installation.rst` & `assistorg_api-0.0.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.3/docs/make.bat` & `assistorg_api-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `assistorg-api-0.0.3/setup.py` & `assistorg_api-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 history = "there is no history, test"
 
 requirements = []
 
 test_requirements = []
 
 setup(
-    name='assistorg-api',
-    version='0.0.3',
+    name='assistorg_api',
+    version='0.0.4',
     description="Unofficial API wrapper for ASSIST.org's API.",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author="Glenn Benedict Montesclaros",
     author_email='montesclarosglennbenedict@gmail.com',
     url='https://github.com/montesclarosglennbenedict/assistapi-org',
     packages=find_packages(include=['assistapi-org', 'assistapi.*']),
```

