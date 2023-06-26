# Comparing `tmp/galaxy-web-framework-23.0.2.tar.gz` & `tmp/galaxy-web-framework-23.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_framework/dist/.tmp-_1i9mkft/galaxy-web-framework-23.0.2.tar", last modified: Tue Jun 13 17:12:26 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_framework/dist/.tmp-rq26rzvo/galaxy-web-framework-23.0.3.tar", last modified: Mon Jun 26 09:55:53 2023, max compression
```

## Comparing `galaxy-web-framework-23.0.2.tar` & `galaxy-web-framework-23.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-web-framework-23.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/web/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/form_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21135 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/helpers/grids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/helpers/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/remoteuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/request_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/sqldebug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/translogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/xforwardedhost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/web/legacy_framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/legacy_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38893 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/legacy_framework/grids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/js/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/js/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/js/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/js/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/js/lib/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/js/lib/mapper.js
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/js/lib/proxy.js
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/proxy/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy/web/short_term_storage/
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/short_term_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/galaxy/web/statsd_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy_web_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy_web_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy_web_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy_web_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy_web_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/galaxy_web_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-13 17:12:26.000000 galaxy-web-framework-23.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-web-framework-23.0.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-26 09:48:32.000000 galaxy-web-framework-23.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/form_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21135 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/helpers/grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/helpers/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/remoteuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/sqldebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/translogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/xforwardedhost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/web/legacy_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/legacy_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38893 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/legacy_framework/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/js/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/js/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/js/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/js/lib/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/js/lib/mapper.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/js/lib/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/proxy/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy/web/short_term_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/short_term_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/galaxy/web/statsd_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy_web_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy_web_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy_web_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy_web_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy_web_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/galaxy_web_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 09:55:53.000000 galaxy-web-framework-23.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:48:33.000000 galaxy-web-framework-23.0.3/test-requirements.txt
```

### Comparing `galaxy-web-framework-23.0.2/HISTORY.rst` & `galaxy-web-framework-23.0.3/HISTORY.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-web-framework-23.0.2/LICENSE` & `galaxy-web-framework-23.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/PKG-INFO` & `galaxy-web-framework-23.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/__init__.py` & `galaxy-web-framework-23.0.3/galaxy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/__init__.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/base.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/base.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/decorators.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/decorators.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/helpers/__init__.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/helpers/grids.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/helpers/grids.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/helpers/tags.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/helpers/tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/error.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/error.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/profile.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/profile.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/remoteuser.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/remoteuser.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/sqldebug.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/sqldebug.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/static.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/static.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/statsd.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/statsd.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/translogger.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/translogger.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/framework/middleware/xforwardedhost.py` & `galaxy-web-framework-23.0.3/galaxy/web/framework/middleware/xforwardedhost.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/legacy_framework/grids.py` & `galaxy-web-framework-23.0.3/galaxy/web/legacy_framework/grids.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/proxy/__init__.py` & `galaxy-web-framework-23.0.3/galaxy/web/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/proxy/js/Dockerfile` & `galaxy-web-framework-23.0.3/galaxy/web/proxy/js/Dockerfile`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/proxy/js/lib/main.js` & `galaxy-web-framework-23.0.3/galaxy/web/proxy/js/lib/main.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/proxy/js/lib/mapper.js` & `galaxy-web-framework-23.0.3/galaxy/web/proxy/js/lib/mapper.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/proxy/js/lib/proxy.js` & `galaxy-web-framework-23.0.3/galaxy/web/proxy/js/lib/proxy.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/short_term_storage/__init__.py` & `galaxy-web-framework-23.0.3/galaxy/web/short_term_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy/web/statsd_client.py` & `galaxy-web-framework-23.0.3/galaxy/web/statsd_client.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/galaxy_web_framework.egg-info/PKG-INFO` & `galaxy-web-framework-23.0.3/galaxy_web_framework.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-web-framework-23.0.2/galaxy_web_framework.egg-info/SOURCES.txt` & `galaxy-web-framework-23.0.3/galaxy_web_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-23.0.2/setup.cfg` & `galaxy-web-framework-23.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-framework
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.2
+version = 23.0.3
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 	galaxy-web-stack
```

