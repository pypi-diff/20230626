# Comparing `tmp/incantoos-1.0.1.tar.gz` & `tmp/incantoos-1.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incantoos-1.0.1.tar", last modified: Mon Jun 26 16:57:56 2023, max compression
+gzip compressed data, was "incantoos-1.0.1.2.tar", last modified: Mon Jun 26 17:39:42 2023, max compression
```

## Comparing `incantoos-1.0.1.tar` & `incantoos-1.0.1.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:57:56.608469 incantoos-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 16:57:44.000000 incantoos-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 16:57:56.608469 incantoos-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-26 16:57:44.000000 incantoos-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:57:56.608469 incantoos-1.0.1/incantoos/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-26 16:57:44.000000 incantoos-1.0.1/incantoos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:57:56.608469 incantoos-1.0.1/incantoos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 16:57:56.000000 incantoos-1.0.1/incantoos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 16:57:56.000000 incantoos-1.0.1/incantoos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:57:56.000000 incantoos-1.0.1/incantoos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 16:57:56.000000 incantoos-1.0.1/incantoos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 16:57:56.000000 incantoos-1.0.1/incantoos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:57:56.608469 incantoos-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-26 16:57:44.000000 incantoos-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:39:42.758455 incantoos-1.0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 17:39:29.000000 incantoos-1.0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-26 17:39:42.758455 incantoos-1.0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-26 17:39:29.000000 incantoos-1.0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:39:42.754455 incantoos-1.0.1.2/incantoos/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-26 17:39:29.000000 incantoos-1.0.1.2/incantoos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:39:42.758455 incantoos-1.0.1.2/incantoos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-26 17:39:42.000000 incantoos-1.0.1.2/incantoos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-26 17:39:42.000000 incantoos-1.0.1.2/incantoos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:39:42.000000 incantoos-1.0.1.2/incantoos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 17:39:42.000000 incantoos-1.0.1.2/incantoos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:39:42.758455 incantoos-1.0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-26 17:39:29.000000 incantoos-1.0.1.2/setup.py
```

### Comparing `incantoos-1.0.1/LICENSE` & `incantoos-1.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `incantoos-1.0.1/setup.py` & `incantoos-1.0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup_info = {
     "name": "incantoos",
-    "version": "1.0.1",
+    "version": "1.0.1.2",
     "author": "NinoTheMeano",
     "author_email": "ninosdeveloping@gmail.com",
     "description": "IncantoOS Is intended to give ",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     "url": "https://github.com/NinoTheMeano/incantoos",
     "packages": setuptools.find_packages(),
@@ -21,14 +21,12 @@
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries",
         "Topic :: Software Development :: Libraries"
     ],
     "project_urls": {
         "Discord": "https://discord.com/users/255125932447236096"
     },
     "python_requires": '>=3.7',
-    "install_requires": [
-        "python-datetime"
-    ]
+    "install_requires": []
 }
 
 
 setuptools.setup(**setup_info)
```

