# Comparing `tmp/cstore-0.3.3.tar.gz` & `tmp/cstore-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cstore-0.3.3.tar", last modified: Wed Jun 14 13:21:36 2023, max compression
+gzip compressed data, was "cstore-0.6.0.tar", last modified: Sun Jun 25 23:12:10 2023, max compression
```

## Comparing `cstore-0.3.3.tar` & `cstore-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 13:21:36.627845 cstore-0.3.3/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.3.3/LICENSE
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-14 13:21:36.627845 cstore-0.3.3/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      115 2023-06-14 08:22:10.000000 cstore-0.3.3/README.md
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 13:21:36.623845 cstore-0.3.3/cstore/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:12:45.000000 cstore-0.3.3/cstore/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      592 2023-06-14 13:19:04.000000 cstore-0.3.3/cstore/cli.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 13:21:36.627845 cstore-0.3.3/cstore.egg-info/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-14 13:21:36.000000 cstore-0.3.3/cstore.egg-info/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      247 2023-06-14 13:21:36.000000 cstore-0.3.3/cstore.egg-info/SOURCES.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-14 13:21:36.000000 cstore-0.3.3/cstore.egg-info/dependency_links.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-06-14 13:21:36.000000 cstore-0.3.3/cstore.egg-info/entry_points.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       11 2023-06-14 13:21:36.000000 cstore-0.3.3/cstore.egg-info/requires.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-06-14 13:21:36.000000 cstore-0.3.3/cstore.egg-info/top_level.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      716 2023-06-14 13:21:24.000000 cstore-0.3.3/pyproject.toml
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-14 13:21:36.627845 cstore-0.3.3/setup.cfg
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:12:10.754381 cstore-0.6.0/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.6.0/LICENSE
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-25 23:12:10.754381 cstore-0.6.0/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      115 2023-06-14 08:22:10.000000 cstore-0.6.0/README.md
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:12:10.754381 cstore-0.6.0/cstore/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:12:45.000000 cstore-0.6.0/cstore/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)    15194 2023-06-25 22:35:01.000000 cstore-0.6.0/cstore/cli.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      180 2023-06-25 12:51:24.000000 cstore-0.6.0/cstore/constants.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      393 2023-06-21 10:01:53.000000 cstore-0.6.0/cstore/database.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1000 2023-06-25 21:35:45.000000 cstore-0.6.0/cstore/models.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:12:10.754381 cstore-0.6.0/cstore/repo/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-20 15:21:29.000000 cstore-0.6.0/cstore/repo/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     2887 2023-06-25 20:48:02.000000 cstore-0.6.0/cstore/repo/repo_command.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1300 2023-06-25 12:38:12.000000 cstore-0.6.0/cstore/repo/repo_tag.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1758 2023-06-25 21:19:40.000000 cstore-0.6.0/cstore/schemes.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      529 2023-06-25 14:04:16.000000 cstore-0.6.0/cstore/verbose.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:12:10.754381 cstore-0.6.0/cstore.egg-info/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      415 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/SOURCES.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/dependency_links.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/entry_points.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       74 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/requires.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/top_level.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      821 2023-06-25 22:53:45.000000 cstore-0.6.0/pyproject.toml
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-25 23:12:10.754381 cstore-0.6.0/setup.cfg
```

### Comparing `cstore-0.3.3/LICENSE` & `cstore-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cstore-0.3.3/PKG-INFO` & `cstore-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.3.3
+Version: 0.6.0
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cstore-0.3.3/cstore.egg-info/PKG-INFO` & `cstore-0.6.0/cstore.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.3.3
+Version: 0.6.0
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

