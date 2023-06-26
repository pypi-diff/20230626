# Comparing `tmp/tendril-utils-core-0.5.8.tar.gz` & `tmp/tendril-utils-core-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tendril-utils-core-0.5.8.tar", last modified: Thu Mar 30 08:49:10 2023, max compression
+gzip compressed data, was "dist/tendril-utils-core-0.5.9.tar", last modified: Mon Apr  3 09:37:11 2023, max compression
```

## Comparing `tendril-utils-core-0.5.8.tar` & `tendril-utils-core-0.5.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3976 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2240 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.257694 tendril-utils-core-0.5.8/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      147 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/api/tendril.utils.colors.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/api/tendril.utils.config.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       92 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/api/tendril.utils.log.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/api/tendril.utils.versions.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13462 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      863 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1539 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3280 2022-11-25 15:15:56.000000 tendril-utils-core-0.5.8/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.257694 tendril-utils-core-0.5.8/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:11:50.000000 tendril-utils-core-0.5.8/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/src/tendril/utils/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:12:02.000000 tendril-utils-core-0.5.8/src/tendril/utils/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2422 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/src/tendril/utils/colors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    22013 2023-03-30 07:41:32.000000 tendril-utils-core-0.5.8/src/tendril/utils/config.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    12692 2023-03-30 08:45:28.000000 tendril-utils-core-0.5.8/src/tendril/utils/log.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      136 2022-12-15 17:03:07.000000 tendril-utils-core-0.5.8/src/tendril/utils/pydantic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/src/tendril/utils/versions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3976 2023-03-30 08:49:10.000000 tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1039 2023-03-30 08:49:10.000000 tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-03-30 08:49:10.000000 tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-30 08:49:10.000000 tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/entry_points.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      527 2023-03-30 08:49:10.000000 tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-03-30 08:49:10.000000 tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 08:49:10.261694 tendril-utils-core-0.5.8/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2039 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/tests/test_utils_log.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      826 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.8/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.528789 tendril-utils-core-0.5.9/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3976 2023-04-03 09:37:11.528789 tendril-utils-core-0.5.9/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2240 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.520789 tendril-utils-core-0.5.9/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.520789 tendril-utils-core-0.5.9/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.520789 tendril-utils-core-0.5.9/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.520789 tendril-utils-core-0.5.9/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      147 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/api/tendril.utils.colors.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/api/tendril.utils.config.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       92 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/api/tendril.utils.log.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/api/tendril.utils.versions.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13462 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      863 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1539 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.524789 tendril-utils-core-0.5.9/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-03 09:37:11.528789 tendril-utils-core-0.5.9/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3280 2022-11-25 15:15:56.000000 tendril-utils-core-0.5.9/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.516789 tendril-utils-core-0.5.9/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.524789 tendril-utils-core-0.5.9/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:11:50.000000 tendril-utils-core-0.5.9/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.524789 tendril-utils-core-0.5.9/src/tendril/utils/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:12:02.000000 tendril-utils-core-0.5.9/src/tendril/utils/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2422 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/src/tendril/utils/colors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    22266 2023-04-03 09:36:00.000000 tendril-utils-core-0.5.9/src/tendril/utils/config.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    12721 2023-03-30 09:05:59.000000 tendril-utils-core-0.5.9/src/tendril/utils/log.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      136 2022-12-15 17:03:07.000000 tendril-utils-core-0.5.9/src/tendril/utils/pydantic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/src/tendril/utils/versions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.524789 tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3976 2023-04-03 09:37:11.000000 tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1039 2023-04-03 09:37:11.000000 tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-03 09:37:11.000000 tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-04-03 09:37:11.000000 tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/entry_points.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      527 2023-04-03 09:37:11.000000 tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-03 09:37:11.000000 tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-03 09:37:11.524789 tendril-utils-core-0.5.9/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2039 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/tests/test_utils_log.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      826 2020-08-18 06:57:07.000000 tendril-utils-core-0.5.9/tox.ini
```

### Comparing `tendril-utils-core-0.5.8/.gitignore` & `tendril-utils-core-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/.readthedocs.yml` & `tendril-utils-core-0.5.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/.travis.yml` & `tendril-utils-core-0.5.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/LICENSE` & `tendril-utils-core-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/PKG-INFO` & `tendril-utils-core-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-core
-Version: 0.5.8
+Version: 0.5.9
 Summary: Core utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-core
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 License: UNKNOWN
 Project-URL: Documentation, https://tendril-utils-core.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-core/issues
```

### Comparing `tendril-utils-core-0.5.8/README.rst` & `tendril-utils-core-0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/docs/Makefile` & `tendril-utils-core-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/docs/_static/custom.css` & `tendril-utils-core-0.5.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/docs/_static/favicon.ico` & `tendril-utils-core-0.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/docs/_static/logo.png` & `tendril-utils-core-0.5.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/docs/_static/logo_packed.png` & `tendril-utils-core-0.5.9/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/docs/_templates/about.html` & `tendril-utils-core-0.5.9/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/docs/conf.py` & `tendril-utils-core-0.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/docs/index.rst` & `tendril-utils-core-0.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/docs/installation.rst` & `tendril-utils-core-0.5.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/setup.py` & `tendril-utils-core-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/src/tendril/utils/colors.py` & `tendril-utils-core-0.5.9/src/tendril/utils/colors.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/src/tendril/utils/config.py` & `tendril-utils-core-0.5.9/src/tendril/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 """
 
 import os
 import json
 import importlib
 import logging
 from runpy import run_path
+from distutils.util import strtobool
 from tendril.utils.versions import get_namespace_package_names
 from tendril.utils.files import yml
 
 logger = logging.getLogger(__name__)
 
 
 class ConfigElement(object):
@@ -81,14 +82,21 @@
             return value
 
         v_len = len(value)
         m_len = int(min(v_len/8, 8))
         return f"{value[:m_len]}...{value[-m_len:]}"
 
 
+def bool_parser(value):
+    if isinstance(value, str):
+        return strtobool(value)
+    else:
+        return bool(value)
+
+
 class ConfigConstant(ConfigElement):
     """
     A configuration `constant`. This is fully specified in the core
     configuration module and cannot be changed by the user or the instance
     administrator without modifying the code.
 
     The value itself is constructed using ``eval()``.
@@ -117,15 +125,15 @@
             self.source = 'environment_override'
             return rv
         except KeyError:
             pass
 
         try:
             rv = self.ctx['_local_config'][self.name]
-            self.source = 'local_override'
+            self.source = 'localboo_override'
             return rv
         except KeyError:
             pass
 
         try:
             rv = self.ctx['_instance_config'][self.name]
             self.source = 'instance_config'
@@ -157,14 +165,16 @@
         If a parser is defined, the value returned is the result of
         applying the parser to the raw value of the property. Otherwise,
         the raw value is returned.
 
         (doc generated mostly by GitHub Copilot)
         """
         if self.parser:
+            if self.parser == bool:
+                return bool_parser(self.raw_value)
             return self.parser(self.raw_value)
         else:
             return self.raw_value
 
 
 class ConfigOptionConstruct(ConfigElement):
     def __init__(self, name, parameters, doc):
```

### Comparing `tendril-utils-core-0.5.8/src/tendril/utils/log.py` & `tendril-utils-core-0.5.9/src/tendril/utils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     DEFAULT = config.LOG_LEVEL
     logging.root.setLevel(config.LOG_LEVEL)
 
     patcher = _config(config)
 
     fmt = "<green>" + _time_fmt(config) + _hostname_fmt(config) + "</green> | " \
           "<level>" + _level_fmt(config) + "</level> | " \
-          "<cyan>" + _source_fmt(config) + "</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> " \
+          "<cyan><i>" + _source_fmt(config) + "</i></cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> " \
           "- <level><n>{message}</n></level>"
 
     params = {
         'handlers': [{"sink": sys.stdout, "serialize": False, "format": fmt}],
     }
     if patcher:
         params['patcher'] = patcher
@@ -178,15 +178,15 @@
     logdir = os.path.split(config.LOG_PATH)[0]
     if not os.path.exists(logdir):
         os.makedirs(logdir)
 
     fmt = "<green>" + _time_fmt(config) + _hostname_fmt(config) + "</green> | " \
           "<level>" + _level_fmt(config) + "</level> | " \
           "<cyan>" + _source_fmt(config) + "</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> " \
-          "- {message}"
+          "- <level><n>{message}</n></level>"
 
     logger.add(config.LOG_PATH, level="INFO", serialize=config.JSON_LOGS, enqueue=True,
                rotation="1 week", retention="14 days", format=fmt,
                catch=True, backtrace=True, diagnose=True)
     logging.info("Logging to: {}".format(config.LOG_PATH))
```

### Comparing `tendril-utils-core-0.5.8/src/tendril/utils/versions.py` & `tendril-utils-core-0.5.9/src/tendril/utils/versions.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/PKG-INFO` & `tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-core
-Version: 0.5.8
+Version: 0.5.9
 Summary: Core utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-core
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 License: UNKNOWN
 Project-URL: Documentation, https://tendril-utils-core.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-core/issues
```

### Comparing `tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/SOURCES.txt` & `tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/src/tendril_utils_core.egg-info/requires.txt` & `tendril-utils-core-0.5.9/src/tendril_utils_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/tests/coveralls.py` & `tendril-utils-core-0.5.9/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/tests/test_utils_log.py` & `tendril-utils-core-0.5.9/tests/test_utils_log.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-core-0.5.8/tox.ini` & `tendril-utils-core-0.5.9/tox.ini`

 * *Files identical despite different names*

