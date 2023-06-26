# Comparing `tmp/thothlibrary-0.9.0.tar.gz` & `tmp/thothlibrary-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thothlibrary-0.9.0.tar", last modified: Tue Feb  1 15:27:25 2022, max compression
+gzip compressed data, was "thothlibrary-0.9.1.tar", last modified: Wed Feb  2 09:32:56 2022, max compression
```

## Comparing `thothlibrary-0.9.0.tar` & `thothlibrary-0.9.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.563183 thothlibrary-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    12539 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6776 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6383 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-01 15:27:25.563183 thothlibrary-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.555183 thothlibrary-0.9.0/thothdjango/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothdjango/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothdjango/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothdjango/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothlibrary/
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    43222 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7007 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2582 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/graphql.py
--rw-r--r--   0 runner    (1001) docker     (121)    10078 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothlibrary/thoth-0_4_2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_4_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31901 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_4_2/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothlibrary/thoth-0_4_2/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)    18384 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_4_2/fixtures/QUERIES
--rw-r--r--   0 runner    (1001) docker     (121)    10793 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_4_2/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothlibrary/thoth-0_5_0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_5_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31901 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_5_0/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothlibrary/thoth-0_5_0/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)    18482 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_5_0/fixtures/QUERIES
--rw-r--r--   0 runner    (1001) docker     (121)    10793 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_5_0/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothlibrary/thoth-0_6_0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_6_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31952 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_6_0/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothlibrary/thoth-0_6_0/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)    18849 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_6_0/fixtures/QUERIES
--rw-r--r--   0 runner    (1001) docker     (121)    10808 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothlibrary/thoth-0_6_0/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothlibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6776 2022-02-01 15:27:25.000000 thothlibrary-0.9.0/thothlibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-02-01 15:27:25.000000 thothlibrary-0.9.0/thothlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-01 15:27:25.000000 thothlibrary-0.9.0/thothlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-01 15:27:25.000000 thothlibrary-0.9.0/thothlibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-02-01 15:27:25.000000 thothlibrary-0.9.0/thothlibrary.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothrest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothrest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothrest/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothrest/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothrest/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:25.559183 thothlibrary-0.9.0/thothrest/thoth-0_4_2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothrest/thoth-0_4_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothrest/thoth-0_4_2/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-02-01 15:27:12.000000 thothlibrary-0.9.0/thothrest/thoth-0_4_2/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    12539 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6776 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6383 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.042241 thothlibrary-0.9.1/thothdjango/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothdjango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothdjango/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothdjango/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.042241 thothlibrary-0.9.1/thothlibrary/
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43222 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7007 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2582 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10078 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/query.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/thothlibrary/thoth-0_4_2/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_4_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31901 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_4_2/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/thothlibrary/thoth-0_4_2/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)    18384 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_4_2/fixtures/QUERIES
+-rw-r--r--   0 runner    (1001) docker     (121)    10793 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_4_2/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/thothlibrary/thoth-0_5_0/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_5_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31901 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_5_0/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/thothlibrary/thoth-0_5_0/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)    18482 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_5_0/fixtures/QUERIES
+-rw-r--r--   0 runner    (1001) docker     (121)    10793 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_5_0/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/thothlibrary/thoth-0_6_0/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_6_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31952 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_6_0/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/thothlibrary/thoth-0_6_0/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)    19035 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_6_0/fixtures/QUERIES
+-rw-r--r--   0 runner    (1001) docker     (121)    10808 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothlibrary/thoth-0_6_0/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.042241 thothlibrary-0.9.1/thothlibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6776 2022-02-02 09:32:55.000000 thothlibrary-0.9.1/thothlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-02-02 09:32:55.000000 thothlibrary-0.9.1/thothlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-02 09:32:55.000000 thothlibrary-0.9.1/thothlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-02 09:32:55.000000 thothlibrary-0.9.1/thothlibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-02-02 09:32:55.000000 thothlibrary-0.9.1/thothlibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/thothrest/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothrest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothrest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothrest/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothrest/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:56.046241 thothlibrary-0.9.1/thothrest/thoth-0_4_2/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothrest/thoth-0_4_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothrest/thoth-0_4_2/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-02-02 09:32:34.000000 thothlibrary-0.9.1/thothrest/thoth-0_4_2/structures.py
```

### Comparing `thothlibrary-0.9.0/LICENSE` & `thothlibrary-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/PKG-INFO` & `thothlibrary-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thothlibrary
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for Thoth's APIs
 Home-page: UNKNOWN
 Author: Javier Arias, Martin Paul Eve
 Author-email: javier@arias.re
 License: Apache 2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 ## Usage
 
 ### Install
 Install is either via pip or cloning the repository.
 
 From pip:
 ```sh
-python3 -m pip install thothlibrary==0.9.0
+python3 -m pip install thothlibrary==0.9.1
 ```
 
 Or from the repo:
 ```sh
 git clone git@github.com:dqprogramming/thoth-client.git
 cd thoth-client
 pip3 install -r ./requirements.txt
```

### Comparing `thothlibrary-0.9.0/README.md` & `thothlibrary-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## Usage
 
 ### Install
 Install is either via pip or cloning the repository.
 
 From pip:
 ```sh
-python3 -m pip install thothlibrary==0.9.0
+python3 -m pip install thothlibrary==0.9.1
 ```
 
 Or from the repo:
 ```sh
 git clone git@github.com:dqprogramming/thoth-client.git
 cd thoth-client
 pip3 install -r ./requirements.txt
```

### Comparing `thothlibrary-0.9.0/setup.py` & `thothlibrary-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothdjango/admin.py` & `thothlibrary-0.9.1/thothdjango/admin.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothdjango/models.py` & `thothlibrary-0.9.1/thothdjango/models.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/auth.py` & `thothlibrary-0.9.1/thothlibrary/auth.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/cli.py` & `thothlibrary-0.9.1/thothlibrary/cli.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/client.py` & `thothlibrary-0.9.1/thothlibrary/client.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/graphql.py` & `thothlibrary-0.9.1/thothlibrary/graphql.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/mutation.py` & `thothlibrary-0.9.1/thothlibrary/mutation.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/query.py` & `thothlibrary-0.9.1/thothlibrary/query.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/thoth-0_4_2/endpoints.py` & `thothlibrary-0.9.1/thothlibrary/thoth-0_4_2/endpoints.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/thoth-0_4_2/fixtures/QUERIES` & `thothlibrary-0.9.1/thothlibrary/thoth-0_4_2/fixtures/QUERIES`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/thoth-0_4_2/structures.py` & `thothlibrary-0.9.1/thothlibrary/thoth-0_4_2/structures.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/thoth-0_5_0/endpoints.py` & `thothlibrary-0.9.1/thothlibrary/thoth-0_5_0/endpoints.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/thoth-0_5_0/fixtures/QUERIES` & `thothlibrary-0.9.1/thothlibrary/thoth-0_5_0/fixtures/QUERIES`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/thoth-0_5_0/structures.py` & `thothlibrary-0.9.1/thothlibrary/thoth-0_5_0/structures.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/thoth-0_6_0/endpoints.py` & `thothlibrary-0.9.1/thothlibrary/thoth-0_6_0/endpoints.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary/thoth-0_6_0/fixtures/QUERIES` & `thothlibrary-0.9.1/thothlibrary/thoth-0_6_0/fixtures/QUERIES`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998828125%*

 * *Differences: {"'institutions'": "{'fields': {insert: [(3, 'ror'), (4, 'countryCode'), (6, 'affiliations { "*

 * *                   'affiliationOrdinal position contribution { fullName contributionType '*

 * *                   "mainContribution contributionOrdinal } }')]}}"}*

```diff
@@ -183,15 +183,18 @@
         ]
     },
     "institutions": {
         "fields": [
             "institutionId",
             "institutionName",
             "institutionDoi",
+            "ror",
+            "countryCode",
             "fundings { grantNumber program projectName jurisdiction work { workId fullTitle doi publicationDate place contributions { fullName contributionType mainContribution contributionOrdinal } imprint { publisher { publisherName publisherId } } } }",
+            "affiliations { affiliationOrdinal position contribution { fullName contributionType mainContribution contributionOrdinal } }",
             "__typename"
         ],
         "parameters": [
             "limit",
             "offset",
             "filter",
             "order"
```

### Comparing `thothlibrary-0.9.0/thothlibrary/thoth-0_6_0/structures.py` & `thothlibrary-0.9.1/thothlibrary/thoth-0_6_0/structures.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothlibrary.egg-info/PKG-INFO` & `thothlibrary-0.9.1/thothlibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thothlibrary
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for Thoth's APIs
 Home-page: UNKNOWN
 Author: Javier Arias, Martin Paul Eve
 Author-email: javier@arias.re
 License: Apache 2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 ## Usage
 
 ### Install
 Install is either via pip or cloning the repository.
 
 From pip:
 ```sh
-python3 -m pip install thothlibrary==0.9.0
+python3 -m pip install thothlibrary==0.9.1
 ```
 
 Or from the repo:
 ```sh
 git clone git@github.com:dqprogramming/thoth-client.git
 cd thoth-client
 pip3 install -r ./requirements.txt
```

### Comparing `thothlibrary-0.9.0/thothlibrary.egg-info/SOURCES.txt` & `thothlibrary-0.9.1/thothlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothrest/cli.py` & `thothlibrary-0.9.1/thothrest/cli.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothrest/client.py` & `thothlibrary-0.9.1/thothrest/client.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothrest/thoth-0_4_2/endpoints.py` & `thothlibrary-0.9.1/thothrest/thoth-0_4_2/endpoints.py`

 * *Files identical despite different names*

### Comparing `thothlibrary-0.9.0/thothrest/thoth-0_4_2/structures.py` & `thothlibrary-0.9.1/thothrest/thoth-0_4_2/structures.py`

 * *Files identical despite different names*

