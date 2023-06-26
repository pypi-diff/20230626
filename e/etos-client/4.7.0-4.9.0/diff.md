# Comparing `tmp/etos_client-4.7.0.tar.gz` & `tmp/etos_client-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_client-4.7.0.tar", last modified: Wed Mar 22 12:47:01 2023, max compression
+gzip compressed data, was "etos_client-4.9.0.tar", last modified: Mon Jun 26 06:34:57 2023, max compression
```

## Comparing `etos_client-4.7.0.tar` & `etos_client-4.9.0.tar`

### file list

```diff
@@ -1,42 +1,56 @@
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-03-22 12:47:01.254519 etos_client-4.7.0/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      594 2023-03-09 08:23:53.000000 etos_client-4.7.0/.coveragerc
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1581 2023-03-22 12:47:01.254519 etos_client-4.7.0/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      986 2023-03-09 08:23:53.000000 etos_client-4.7.0/README.rst
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-03-22 12:47:01.254519 etos_client-4.7.0/docs/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7616 2023-03-09 08:23:53.000000 etos_client-4.7.0/docs/Makefile
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-03-22 12:47:01.254519 etos_client-4.7.0/docs/_static/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-03-09 08:23:53.000000 etos_client-4.7.0/docs/_static/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-03-09 08:23:53.000000 etos_client-4.7.0/docs/authors.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-03-09 08:23:53.000000 etos_client-4.7.0/docs/changelog.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     9184 2023-03-09 08:23:53.000000 etos_client-4.7.0/docs/conf.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      452 2023-03-09 08:23:53.000000 etos_client-4.7.0/docs/index.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-03-09 08:23:53.000000 etos_client-4.7.0/docs/license.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-03-09 08:23:53.000000 etos_client-4.7.0/docs/readme.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-03-09 08:23:53.000000 etos_client-4.7.0/docs/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       38 2023-03-09 08:23:53.000000 etos_client-4.7.0/pylintrc
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      696 2023-03-09 08:23:53.000000 etos_client-4.7.0/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1464 2023-03-22 12:47:01.254519 etos_client-4.7.0/setup.cfg
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      555 2023-03-09 08:23:53.000000 etos_client-4.7.0/setup.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-03-22 12:47:01.254519 etos_client-4.7.0/src/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-03-22 12:47:01.254519 etos_client-4.7.0/src/etos_client/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1066 2023-03-09 08:23:53.000000 etos_client-4.7.0/src/etos_client/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10424 2023-03-10 12:27:18.000000 etos_client-4.7.0/src/etos_client/__main__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5097 2023-03-22 11:22:41.000000 etos_client-4.7.0/src/etos_client/client.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-03-22 12:47:01.254519 etos_client-4.7.0/src/etos_client/lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      802 2023-03-09 08:23:53.000000 etos_client-4.7.0/src/etos_client/lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7933 2023-03-09 08:23:53.000000 etos_client-4.7.0/src/etos_client/lib/graphql.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3110 2023-03-09 08:23:53.000000 etos_client-4.7.0/src/etos_client/lib/graphql_queries.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7195 2023-03-09 08:23:53.000000 etos_client-4.7.0/src/etos_client/lib/log_handler.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     9523 2023-03-09 08:23:53.000000 etos_client-4.7.0/src/etos_client/lib/test_result_handler.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-03-22 12:47:01.254519 etos_client-4.7.0/src/etos_client.egg-info/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1581 2023-03-22 12:47:01.000000 etos_client-4.7.0/src/etos_client.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      804 2023-03-22 12:47:01.000000 etos_client-4.7.0/src/etos_client.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-03-22 12:47:01.000000 etos_client-4.7.0/src/etos_client.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       58 2023-03-22 12:47:01.000000 etos_client-4.7.0/src/etos_client.egg-info/entry_points.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-03-10 12:24:03.000000 etos_client-4.7.0/src/etos_client.egg-info/not-zip-safe
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       83 2023-03-22 12:47:01.000000 etos_client-4.7.0/src/etos_client.egg-info/requires.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       12 2023-03-22 12:47:01.000000 etos_client-4.7.0/src/etos_client.egg-info/top_level.txt
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-03-22 12:47:01.254519 etos_client-4.7.0/tests/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      691 2023-03-09 08:23:53.000000 etos_client-4.7.0/tests/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      199 2023-03-09 08:23:53.000000 etos_client-4.7.0/tests/conftest.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      268 2023-03-09 08:23:53.000000 etos_client-4.7.0/tox.ini
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.255956 etos_client-4.9.0/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      594 2023-06-21 06:23:58.000000 etos_client-4.9.0/.coveragerc
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1581 2023-06-26 06:34:57.255956 etos_client-4.9.0/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      986 2023-06-21 06:23:58.000000 etos_client-4.9.0/README.rst
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.251956 etos_client-4.9.0/docs/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7616 2023-06-21 06:23:58.000000 etos_client-4.9.0/docs/Makefile
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.251956 etos_client-4.9.0/docs/_static/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-06-21 06:23:58.000000 etos_client-4.9.0/docs/_static/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-06-21 06:23:58.000000 etos_client-4.9.0/docs/authors.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-06-21 06:23:58.000000 etos_client-4.9.0/docs/changelog.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     9184 2023-06-21 06:23:58.000000 etos_client-4.9.0/docs/conf.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      452 2023-06-21 06:23:58.000000 etos_client-4.9.0/docs/index.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-06-21 06:23:58.000000 etos_client-4.9.0/docs/license.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-06-21 06:23:58.000000 etos_client-4.9.0/docs/readme.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-06-21 06:23:58.000000 etos_client-4.9.0/docs/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       38 2023-06-21 06:23:58.000000 etos_client-4.9.0/pylintrc
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      683 2023-06-21 07:07:16.000000 etos_client-4.9.0/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1450 2023-06-26 06:34:57.255956 etos_client-4.9.0/setup.cfg
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      555 2023-06-21 06:23:58.000000 etos_client-4.9.0/setup.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.251956 etos_client-4.9.0/src/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.251956 etos_client-4.9.0/src/etos_client/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1061 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7661 2023-06-21 09:43:30.000000 etos_client-4.9.0/src/etos_client/__main__.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.255956 etos_client-4.9.0/src/etos_client/announcer/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      718 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/announcer/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2633 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/announcer/announcer.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.255956 etos_client-4.9.0/src/etos_client/etos/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      710 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/etos/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4028 2023-06-21 07:07:16.000000 etos_client-4.9.0/src/etos_client/etos/etos.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3433 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/etos/schema.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.255956 etos_client-4.9.0/src/etos_client/event_repository/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      726 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/event_repository/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     6926 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/event_repository/graphql.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2953 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/event_repository/graphql_queries.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.255956 etos_client-4.9.0/src/etos_client/events/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      694 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/events/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7525 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/events/collector.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1765 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/events/events.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.255956 etos_client-4.9.0/src/etos_client/logs/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      734 2023-06-21 07:07:16.000000 etos_client-4.9.0/src/etos_client/logs/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7091 2023-06-21 07:07:16.000000 etos_client-4.9.0/src/etos_client/logs/logs.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.255956 etos_client-4.9.0/src/etos_client/test_results/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      731 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/test_results/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2791 2023-06-21 06:23:58.000000 etos_client-4.9.0/src/etos_client/test_results/test_results.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.251956 etos_client-4.9.0/src/etos_client.egg-info/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1581 2023-06-26 06:34:57.000000 etos_client-4.9.0/src/etos_client.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1161 2023-06-26 06:34:57.000000 etos_client-4.9.0/src/etos_client.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-26 06:34:57.000000 etos_client-4.9.0/src/etos_client.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       58 2023-06-26 06:34:57.000000 etos_client-4.9.0/src/etos_client.egg-info/entry_points.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-21 06:32:29.000000 etos_client-4.9.0/src/etos_client.egg-info/not-zip-safe
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       70 2023-06-26 06:34:57.000000 etos_client-4.9.0/src/etos_client.egg-info/requires.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       12 2023-06-26 06:34:57.000000 etos_client-4.9.0/src/etos_client.egg-info/top_level.txt
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-26 06:34:57.255956 etos_client-4.9.0/tests/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      686 2023-06-21 06:23:58.000000 etos_client-4.9.0/tests/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      199 2023-06-21 06:23:58.000000 etos_client-4.9.0/tests/conftest.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      286 2023-06-21 06:23:58.000000 etos_client-4.9.0/tox.ini
```

### Comparing `etos_client-4.7.0/.coveragerc` & `etos_client-4.9.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_client-4.7.0/PKG-INFO` & `etos_client-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_client
-Version: 4.7.0
+Version: 4.9.0
 Summary: Test suite execution client for ETOS.
 Home-page: https://github.com/eiffel-community/etos-suite-starter
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_client-4.7.0/README.rst` & `etos_client-4.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_client-4.7.0/docs/Makefile` & `etos_client-4.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_client-4.7.0/docs/conf.py` & `etos_client-4.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_client-4.7.0/requirements.txt` & `etos_client-4.9.0/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,10 +11,9 @@
 # Add your pinned requirements so that they can be easily installed with:
 # pip install -r requirements.txt
 # Remember to also add them in setup.cfg but unpinned.
 # Example:
 # numpy==1.13.3
 # scipy==1.0
 #
-halo==0.0.26
 packageurl-python==0.9.1
 etos_lib==2.1.0
```

### Comparing `etos_client-4.7.0/setup.cfg` & `etos_client-4.9.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
-	halo==0.0.26
 	packageurl-python==0.9.1
 	etos_lib==2.1.0
 python_requires = >=3.4
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `etos_client-4.7.0/setup.py` & `etos_client-4.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_client-4.7.0/src/etos_client/__init__.py` & `etos_client-4.9.0/src/etos_client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Axis Communications AB.
+# Copyright Axis Communications AB.
 #
 # For a full list of individual contributors, please see the commit history.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `etos_client-4.7.0/src/etos_client/lib/__init__.py` & `etos_client-4.9.0/src/etos_client/event_repository/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# Copyright 2020 Axis Communications AB.
+# Copyright Axis Communications AB.
 #
 # For a full list of individual contributors, please see the commit history.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ETOS client common helpers module."""
-from .log_handler import ETOSLogHandler
-from .test_result_handler import ETOSTestResultHandler
+"""ETOS client graphql helpers module."""
+from .graphql import *
```

### Comparing `etos_client-4.7.0/src/etos_client/lib/graphql_queries.py` & `etos_client-4.9.0/src/etos_client/event_repository/graphql_queries.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020-2022 Axis Communications AB.
+# Copyright Axis Communications AB.
 #
 # For a full list of individual contributors, please see the commit history.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -13,89 +13,108 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """GraphQL queries."""
 
 TEST_SUITE = """
 {
-  testExecutionRecipeCollectionCreated(search: "{'meta.id': '%s'}") {
+  testExecutionRecipeCollectionCreated(%s) {
     edges {
       node {
         data {
           batchesUri
         }
       }
     }
   }
 }
 """
 
 
 ACTIVITY_TRIGGERED = """
 {
-  activityTriggered(search: "{'links.type': 'CAUSE', 'links.target': '%s'}") {
+  activityTriggered(%s) {
     edges {
       node {
         meta {
           id
         }
       }
     }
   }
 }
 """
 
+
+ACTIVITY_FINISHED = """
+{
+  activityFinished(%s) {
+    edges {
+      node {
+        data {
+          activityOutcome {
+            description
+            conclusion
+          }
+        }
+      }
+    }
+  }
+}
+"""
+
+
 ACTIVITY_CANCELED = """
 {
-  activityCanceled(search: "{'links.type': 'ACTIVITY_EXECUTION', 'links.target': '%s'}") {
+  activityCanceled(%s) {
     edges {
       node {
         data {
           reason
         }
       }
     }
   }
 }
 """
 
 
 TEST_SUITE_STARTED = """
 {
-  testSuiteStarted(search:"{'links.type': 'CAUSE', 'links.target': '%s'}") {
+  testSuiteStarted(%s) {
     edges {
       node {
         meta {
           id
         }
       }
     }
   }
 }
 """
 
 
 MAIN_TEST_SUITES_STARTED = """
 {
-  testSuiteStarted(search:"{'links.type': 'CONTEXT', 'links.target': '%s', 'data.categories': {'$ne': 'Sub suite'}}") {
+  testSuiteStarted(%s) {
     edges {
       node {
         meta {
           id
         }
       }
     }
   }
 }
 """
 
 
 TEST_SUITE_FINISHED = """
 {
-  testSuiteFinished(search: "{'links.type': 'TEST_SUITE_EXECUTION', 'links.target': '%s'}" last: 1) {
+  testSuiteFinished(%s) {
     edges {
       node {
         data {
           testSuitePersistentLogs {
             name
             uri
           }
@@ -108,15 +127,15 @@
   }
 }
 """
 
 
 ANNOUNCEMENTS = """
 {
-  announcementPublished(search: "%s") {
+  announcementPublished(%s) {
     edges {
       node {
         data {
           heading
           body
         }
       }
@@ -124,38 +143,44 @@
   }
 }
 """
 
 
 ENVIRONMENTS = """
 {
-  environmentDefined(search: "%s") {
+  environmentDefined(%s) {
     edges {
       node {
         data {
           name
           uri
         }
+        meta {
+          time
+        }
       }
     }
   }
 }
 """
 
 
 ARTIFACTS = """
 {
-  artifactCreated(search: "{'links.type': 'CONTEXT', 'links.target': '%s'}") {
+  artifactCreated(%s) {
     edges {
       node {
         data {
           fileInformation {
             name
           }
         }
+        meta {
+          time
+        }
         links {
           ... on Cause {
             links {
               ... on TestSuiteStarted {
                 data {
                   name
                 }
```

### Comparing `etos_client-4.7.0/src/etos_client.egg-info/PKG-INFO` & `etos_client-4.9.0/src/etos_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos-client
-Version: 4.7.0
+Version: 4.9.0
 Summary: Test suite execution client for ETOS.
 Home-page: https://github.com/eiffel-community/etos-suite-starter
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_client-4.7.0/src/etos_client.egg-info/SOURCES.txt` & `etos_client-4.9.0/src/etos_client.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,22 +12,31 @@
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 src/etos_client/__init__.py
 src/etos_client/__main__.py
-src/etos_client/client.py
 src/etos_client.egg-info/PKG-INFO
 src/etos_client.egg-info/SOURCES.txt
 src/etos_client.egg-info/dependency_links.txt
 src/etos_client.egg-info/entry_points.txt
 src/etos_client.egg-info/not-zip-safe
 src/etos_client.egg-info/requires.txt
 src/etos_client.egg-info/top_level.txt
-src/etos_client/lib/__init__.py
-src/etos_client/lib/graphql.py
-src/etos_client/lib/graphql_queries.py
-src/etos_client/lib/log_handler.py
-src/etos_client/lib/test_result_handler.py
+src/etos_client/announcer/__init__.py
+src/etos_client/announcer/announcer.py
+src/etos_client/etos/__init__.py
+src/etos_client/etos/etos.py
+src/etos_client/etos/schema.py
+src/etos_client/event_repository/__init__.py
+src/etos_client/event_repository/graphql.py
+src/etos_client/event_repository/graphql_queries.py
+src/etos_client/events/__init__.py
+src/etos_client/events/collector.py
+src/etos_client/events/events.py
+src/etos_client/logs/__init__.py
+src/etos_client/logs/logs.py
+src/etos_client/test_results/__init__.py
+src/etos_client/test_results/test_results.py
 tests/__init__.py
 tests/conftest.py
```

### Comparing `etos_client-4.7.0/tests/__init__.py` & `etos_client-4.9.0/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Axis Communications AB.
+# Copyright Axis Communications AB.
 #
 # For a full list of individual contributors, please see the commit history.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

