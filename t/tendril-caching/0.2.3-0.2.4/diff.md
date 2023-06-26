# Comparing `tmp/tendril-caching-0.2.3.tar.gz` & `tmp/tendril-caching-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tendril-caching-0.2.3.tar", last modified: Tue Mar 28 18:19:25 2023, max compression
+gzip compressed data, was "tendril-caching-0.2.4.tar", last modified: Mon Jun 26 13:08:55 2023, max compression
```

## Comparing `tendril-caching-0.2.3.tar` & `tendril-caching-0.2.4.tar`

### file list

```diff
@@ -1,51 +1,57 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3921 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.630817 tendril-caching-0.2.3/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-caching-0.2.3/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      903 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3133 2022-11-29 09:11:32.000000 tendril-caching-0.2.3/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.630817 tendril-caching-0.2.3/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/src/tendril/caching/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      449 2022-11-29 14:28:12.000000 tendril-caching-0.2.3/src/tendril/caching/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/src/tendril/caching/providers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:53:59.000000 tendril-caching-0.2.3/src/tendril/caching/providers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      272 2022-11-29 13:57:11.000000 tendril-caching-0.2.3/src/tendril/caching/providers/dummy.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1910 2022-11-29 14:11:44.000000 tendril-caching-0.2.3/src/tendril/caching/providers/redis.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2185 2023-03-15 16:37:56.000000 tendril-caching-0.2.3/src/tendril/caching/transit.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-caching-0.2.3/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1104 2023-03-28 18:17:59.000000 tendril-caching-0.2.3/src/tendril/config/caching.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/src/tendril_caching.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3921 2023-03-28 18:19:25.000000 tendril-caching-0.2.3/src/tendril_caching.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      889 2023-03-28 18:19:25.000000 tendril-caching-0.2.3/src/tendril_caching.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-03-28 18:19:25.000000 tendril-caching-0.2.3/src/tendril_caching.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      503 2023-03-28 18:19:25.000000 tendril-caching-0.2.3/src/tendril_caching.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-03-28 18:19:25.000000 tendril-caching-0.2.3/src/tendril_caching.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:19:25.634817 tendril-caching-0.2.3/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-11-29 08:29:31.000000 tendril-caching-0.2.3/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.846445 tendril-caching-0.2.4/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-06-26 13:08:55.846445 tendril-caching-0.2.4/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.838445 tendril-caching-0.2.4/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.842445 tendril-caching-0.2.4/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.842445 tendril-caching-0.2.4/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-caching-0.2.4/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.842445 tendril-caching-0.2.4/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      903 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.842445 tendril-caching-0.2.4/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-06-26 13:08:55.846445 tendril-caching-0.2.4/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3133 2022-11-29 09:11:32.000000 tendril-caching-0.2.4/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.834445 tendril-caching-0.2.4/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.842445 tendril-caching-0.2.4/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.842445 tendril-caching-0.2.4/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:20.000000 tendril-caching-0.2.4/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.842445 tendril-caching-0.2.4/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-caching-0.2.4/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      862 2023-06-26 11:34:05.000000 tendril-caching-0.2.4/src/tendril/apiserver/routers/tokens.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.842445 tendril-caching-0.2.4/src/tendril/caching/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      449 2022-11-29 14:28:12.000000 tendril-caching-0.2.4/src/tendril/caching/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.842445 tendril-caching-0.2.4/src/tendril/caching/providers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:53:59.000000 tendril-caching-0.2.4/src/tendril/caching/providers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      272 2022-11-29 13:57:11.000000 tendril-caching-0.2.4/src/tendril/caching/providers/dummy.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1910 2022-11-29 14:11:44.000000 tendril-caching-0.2.4/src/tendril/caching/providers/redis.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4514 2023-06-26 13:06:24.000000 tendril-caching-0.2.4/src/tendril/caching/tokens.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2349 2023-06-25 19:47:22.000000 tendril-caching-0.2.4/src/tendril/caching/transit.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.846445 tendril-caching-0.2.4/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-caching-0.2.4/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1689 2023-06-26 10:43:35.000000 tendril-caching-0.2.4/src/tendril/config/caching.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.846445 tendril-caching-0.2.4/src/tendril_caching.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3481 2023-06-26 13:08:55.000000 tendril-caching-0.2.4/src/tendril_caching.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1035 2023-06-26 13:08:55.000000 tendril-caching-0.2.4/src/tendril_caching.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-06-26 13:08:55.000000 tendril-caching-0.2.4/src/tendril_caching.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      503 2023-06-26 13:08:55.000000 tendril-caching-0.2.4/src/tendril_caching.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-06-26 13:08:55.000000 tendril-caching-0.2.4/src/tendril_caching.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 13:08:55.846445 tendril-caching-0.2.4/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-11-29 08:29:31.000000 tendril-caching-0.2.4/tox.ini
```

### Comparing `tendril-caching-0.2.3/.gitignore` & `tendril-caching-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/.readthedocs.yml` & `tendril-caching-0.2.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/.travis.yml` & `tendril-caching-0.2.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/LICENSE` & `tendril-caching-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/PKG-INFO` & `tendril-caching-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-caching
-Version: 0.2.3
+Version: 0.2.4
 Summary: Caching Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-caching
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-caching.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-caching/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-caching
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-caching.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-caching
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-caching.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-caching
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-caching.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-caching
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-caching.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-caching
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-caching
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-caching.svg
-            :target: https://requires.io/github/tendril-framework/tendril-caching/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-caching.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-caching.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-caching>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-caching`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-caching`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-caching.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-caching
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-caching.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-caching
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-caching.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-caching
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-caching.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-caching
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-caching
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-caching.svg
+    :target: https://requires.io/github/tendril-framework/tendril-caching/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-caching.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-caching.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-caching>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-caching`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-caching`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-caching-0.2.3/README.rst` & `tendril-caching-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/docs/Makefile` & `tendril-caching-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/docs/_static/custom.css` & `tendril-caching-0.2.4/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/docs/_static/favicon.ico` & `tendril-caching-0.2.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/docs/_static/logo.png` & `tendril-caching-0.2.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/docs/_static/logo_packed.png` & `tendril-caching-0.2.4/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/docs/_templates/about.html` & `tendril-caching-0.2.4/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/docs/conf.py` & `tendril-caching-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/docs/index.rst` & `tendril-caching-0.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/docs/installation.rst` & `tendril-caching-0.2.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/setup.py` & `tendril-caching-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/src/tendril/caching/providers/redis.py` & `tendril-caching-0.2.4/src/tendril/caching/providers/redis.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/src/tendril/caching/transit.py` & `tendril-caching-0.2.4/src/tendril/caching/transit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 
 
 import json
 
+from tendril.config import TRANSIT_CACHING_PROVIDER
 from tendril.config import PLATFORM_CACHING_PROVIDER
 
+
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
+if not TRANSIT_CACHING_PROVIDER:
+    TRANSIT_CACHING_PROVIDER = PLATFORM_CACHING_PROVIDER
 
-if PLATFORM_CACHING_PROVIDER == 'redis':
-    logger.info("Using Redis for the platform level cache.")
+if TRANSIT_CACHING_PROVIDER == 'redis':
+    logger.info("Using Redis for the transit cache.")
     import redis
     from tendril.config import REDIS_HOST
     from tendril.config import REDIS_PORT
     from tendril.config import REDIS_DB
     from tendril.config import REDIS_PASSWORD
 else:
-    raise Exception("A valid PLATFORM_CACHING_PROVIDER is not configured "
+    raise Exception("A valid TRANSIT_CACHING_PROVIDER is not configured "
                     "and a fallback is not presently implemented.")
 
 
 redis_connection: redis.Redis = None
 
 
 def _create_redis_connection():
@@ -42,14 +46,15 @@
             "Redis transit caching requires a literal "
             "key to be provided."
         )
 
     if not namespace:
         logger.warn(f"No transit caching namespace was provided for "
                     f"key {key}. Using 'transit' instead.")
+        namespace = 'transit'
 
     cache_key = "{}:{}".format(namespace, key)
     return cache_key
 
 
 def write(value=None, namespace=None, ttl=None, key=None, ser=json.dumps):
     cache_key = _common(namespace=namespace, key=key)
```

### Comparing `tendril-caching-0.2.3/src/tendril/config/__init__.py` & `tendril-caching-0.2.4/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/src/tendril_caching.egg-info/PKG-INFO` & `tendril-caching-0.2.4/src/tendril_caching.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-caching
-Version: 0.2.3
+Version: 0.2.4
 Summary: Caching Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-caching
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-caching.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-caching/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-caching
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-caching.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-caching
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-caching.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-caching
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-caching.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-caching
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-caching.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-caching
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-caching
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-caching.svg
-            :target: https://requires.io/github/tendril-framework/tendril-caching/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-caching.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-caching.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-caching>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-caching`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-caching`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-caching.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-caching
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-caching.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-caching
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-caching.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-caching
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-caching.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-caching
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-caching
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-caching.svg
+    :target: https://requires.io/github/tendril-framework/tendril-caching/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-caching.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-caching.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-caching>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-caching`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-caching`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-caching-0.2.3/src/tendril_caching.egg-info/SOURCES.txt` & `tendril-caching-0.2.4/src/tendril_caching.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 docs/_static/logo.png
 docs/_static/logo_packed.png
 docs/_templates/about.html
 docs/api/index.rst
 docs/usage/standalone.rst
 docs/usage/tendril.rst
 src/tendril/__init__.py
+src/tendril/apiserver/__init__.py
+src/tendril/apiserver/routers/__init__.py
+src/tendril/apiserver/routers/tokens.py
 src/tendril/caching/__init__.py
+src/tendril/caching/tokens.py
 src/tendril/caching/transit.py
 src/tendril/caching/providers/__init__.py
 src/tendril/caching/providers/dummy.py
 src/tendril/caching/providers/redis.py
 src/tendril/config/__init__.py
 src/tendril/config/caching.py
 src/tendril_caching.egg-info/PKG-INFO
```

### Comparing `tendril-caching-0.2.3/tests/coveralls.py` & `tendril-caching-0.2.4/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-caching-0.2.3/tox.ini` & `tendril-caching-0.2.4/tox.ini`

 * *Files identical despite different names*

