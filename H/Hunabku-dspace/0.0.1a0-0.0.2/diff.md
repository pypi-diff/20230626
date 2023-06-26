# Comparing `tmp/Hunabku_dspace-0.0.1a0.tar.gz` & `tmp/Hunabku_dspace-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_dspace-0.0.1a0.tar", last modified: Tue May 30 00:49:26 2023, max compression
+gzip compressed data, was "Hunabku_dspace-0.0.2.tar", last modified: Mon Jun 26 16:14:21 2023, max compression
```

## Comparing `Hunabku_dspace-0.0.1a0.tar` & `Hunabku_dspace-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:49:26.064857 Hunabku_dspace-0.0.1a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:49:26.064857 Hunabku_dspace-0.0.1a0/Hunabku_dspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-30 00:49:26.000000 Hunabku_dspace-0.0.1a0/Hunabku_dspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 00:49:26.000000 Hunabku_dspace-0.0.1a0/Hunabku_dspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:49:26.000000 Hunabku_dspace-0.0.1a0/Hunabku_dspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:49:26.000000 Hunabku_dspace-0.0.1a0/Hunabku_dspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 00:49:26.000000 Hunabku_dspace-0.0.1a0/Hunabku_dspace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 00:49:09.000000 Hunabku_dspace-0.0.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-30 00:49:26.064857 Hunabku_dspace-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-30 00:49:09.000000 Hunabku_dspace-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:49:26.064857 Hunabku_dspace-0.0.1a0/hunabku_dspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:49:09.000000 Hunabku_dspace-0.0.1a0/hunabku_dspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 00:49:09.000000 Hunabku_dspace-0.0.1a0/hunabku_dspace/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:49:26.064857 Hunabku_dspace-0.0.1a0/hunabku_dspace/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-05-30 00:49:09.000000 Hunabku_dspace-0.0.1a0/hunabku_dspace/endpoints/DSpace.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:49:26.064857 Hunabku_dspace-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-30 00:49:09.000000 Hunabku_dspace-0.0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:21.272706 Hunabku_dspace-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:21.272706 Hunabku_dspace-0.0.2/Hunabku_dspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-26 16:14:21.000000 Hunabku_dspace-0.0.2/Hunabku_dspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-26 16:14:21.000000 Hunabku_dspace-0.0.2/Hunabku_dspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:14:21.000000 Hunabku_dspace-0.0.2/Hunabku_dspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:14:21.000000 Hunabku_dspace-0.0.2/Hunabku_dspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 16:14:21.000000 Hunabku_dspace-0.0.2/Hunabku_dspace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 16:14:04.000000 Hunabku_dspace-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-26 16:14:21.272706 Hunabku_dspace-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-26 16:14:04.000000 Hunabku_dspace-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:21.272706 Hunabku_dspace-0.0.2/hunabku_dspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:04.000000 Hunabku_dspace-0.0.2/hunabku_dspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 16:14:04.000000 Hunabku_dspace-0.0.2/hunabku_dspace/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:21.272706 Hunabku_dspace-0.0.2/hunabku_dspace/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-06-26 16:14:04.000000 Hunabku_dspace-0.0.2/hunabku_dspace/endpoints/DSpace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:14:21.272706 Hunabku_dspace-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-26 16:14:04.000000 Hunabku_dspace-0.0.2/setup.py
```

### Comparing `Hunabku_dspace-0.0.1a0/Hunabku_dspace.egg-info/PKG-INFO` & `Hunabku_dspace-0.0.2/Hunabku_dspace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku-dspace
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: Hunabku plugin for dspace
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_dspace-0.0.1a0/PKG-INFO` & `Hunabku_dspace-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku_dspace
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: Hunabku plugin for dspace
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_dspace-0.0.1a0/README.md` & `Hunabku_dspace-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Hunabku_dspace-0.0.1a0/hunabku_dspace/endpoints/DSpace.py` & `Hunabku_dspace-0.0.2/hunabku_dspace/endpoints/DSpace.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         if a required parameter is not found, returns error code 400 (Bad Request)
         """
         institution = req_args.get('institution')
 
         if not institution:
             # institution required
             data = {"error": "Bad Request",
-                    "message": "institution parameter is required, it was not provided. options are: udea, unaula, uec"}
+                    "message": "institution parameter is required, it was not provided. options are: udea, unaula, uec, univalle"}
             response = self.app.response_class(
                 response=self.json.dumps(data),
                 status=400,
                 mimetype='application/json'
             )
             return response
         return None
@@ -75,15 +75,15 @@
         @apiName product
         @apiGroup DSpace
         @apiDescription Allows to perform queries for products on DSpace,
                         institution is mandatory parameter.
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} id  DSpace id of the product
-        @apiParam {String} institution Institution initials. supported example: udea, uec, unaula
+        @apiParam {String} institution Institution initials. supported example: udea, uec, unaula, univalle
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
@@ -152,15 +152,15 @@
         @api {get} /dspace/info DSpace info endpoint
         @apiName Info
         @apiGroup DSpace
         @apiDescription Allows to perform queries for information,
                         about avialable institution and ids.
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} get Options are resume and ids, ids require additional parameter institution
-        @apiParam {String} institution Institution initials. supported example: udea, uec, unaula
+        @apiParam {String} institution Institution initials. supported example: udea, uec, unaula, univalle
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
```

### Comparing `Hunabku_dspace-0.0.1a0/setup.py` & `Hunabku_dspace-0.0.2/setup.py`

 * *Files identical despite different names*

