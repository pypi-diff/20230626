# Comparing `tmp/Hunabku_scienti-0.0.5.tar.gz` & `tmp/Hunabku_scienti-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_scienti-0.0.5.tar", last modified: Mon May 29 22:23:55 2023, max compression
+gzip compressed data, was "Hunabku_scienti-0.0.6.tar", last modified: Mon Jun 26 15:56:30 2023, max compression
```

## Comparing `Hunabku_scienti-0.0.5.tar` & `Hunabku_scienti-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/hunabku_scienti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/hunabku_scienti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/hunabku_scienti/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/hunabku_scienti/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)    32842 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/hunabku_scienti/endpoints/Scienti.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:30.136212 Hunabku_scienti-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:30.132212 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-26 15:56:30.132212 Hunabku_scienti-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:30.132212 Hunabku_scienti-0.0.6/hunabku_scienti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/hunabku_scienti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/hunabku_scienti/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:30.132212 Hunabku_scienti-0.0.6/hunabku_scienti/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)    32902 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/hunabku_scienti/endpoints/Scienti.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:56:30.136212 Hunabku_scienti-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/setup.py
```

### Comparing `Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/PKG-INFO` & `Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku-scienti
-Version: 0.0.5
+Version: 0.0.6
 Summary: Hunabku scienti plugin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Hunabku_scienti-0.0.5/LICENSE` & `Hunabku_scienti-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Hunabku_scienti-0.0.5/PKG-INFO` & `Hunabku_scienti-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku_scienti
-Version: 0.0.5
+Version: 0.0.6
 Summary: Hunabku scienti plugin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Hunabku_scienti-0.0.5/README.md` & `Hunabku_scienti-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Hunabku_scienti-0.0.5/hunabku_scienti/endpoints/Scienti.py` & `Hunabku_scienti-0.0.6/hunabku_scienti/endpoints/Scienti.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                         parameter passed, the endpoint returns all the dump of the database.
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_PRODUCTO  Product key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  Category of the product
         @apiParam {String} model_year  Year of the scienti model, example: 2022
-        @apiParam {String} institution Institution initials. supported example: udea, uec, unaula
+        @apiParam {String} institution Institution initials. supported example: udea, uec, unaula, univalle
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
@@ -190,15 +190,15 @@
                         parameter passed, the endpoint returns all the dump of the database.
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_RED  network key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  category of the network
         @apiParam {String} model_year  year of the scienti model, example: 2022
-        @apiParam {String} institution institution initials. supported example: udea, uec, unaula
+        @apiParam {String} institution institution initials. supported example: udea, uec, unaula, univalle
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
@@ -295,15 +295,15 @@
                         parameter passed, the endpoint returns all the dump of the database.
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_PROYECTO  project key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  category of the network
         @apiParam {String} model_year  year of the scienti model, example: 2022
-        @apiParam {String} institution institution initials. supported example: udea, uec, unaula
+        @apiParam {String} institution institution initials. supported example: udea, uec, unaula, univalle
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
@@ -399,15 +399,15 @@
                         parameter passed, the endpoint returns all the dump of the database.
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_EVENTO  event key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  category of the network
         @apiParam {String} model_year  year of the scienti model, example: 2022
-        @apiParam {String} institution institution initials. supported example: udea, uec, unaula
+        @apiParam {String} institution institution initials. supported example: udea, uec, unaula, univalle
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
@@ -502,15 +502,15 @@
                         parameter passed, the endpoint returns all the dump of the database.
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_PATENTE  patent key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  category of the network
         @apiParam {String} model_year  year of the scienti model, example: 2022
-        @apiParam {String} institution institution initials. supported example: udea, uec, unaula
+        @apiParam {String} institution institution initials. supported example: udea, uec, unaula, univalle
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
@@ -601,15 +601,15 @@
         @apiName Info
         @apiGroup Scienti
         @apiDescription Allows to perform queries for information,
                         about avialable institution and ids.
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} get Options are resume and ids, ids require additional parameters model_year and institution
         @apiParam {String} model_year  Year of the scienti model, example: 2022
-        @apiParam {String} institution Institution initials. supported example: udea, uec, unaula
+        @apiParam {String} institution Institution initials. supported example: udea, uec, unaula, univalle
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
```

### Comparing `Hunabku_scienti-0.0.5/setup.py` & `Hunabku_scienti-0.0.6/setup.py`

 * *Files identical despite different names*

