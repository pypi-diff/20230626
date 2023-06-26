# Comparing `tmp/mangorest-0.12200000000000003.tar.gz` & `tmp/mangorest-0.12300000000000003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mangorest-0.12200000000000003.tar", last modified: Mon Jun 26 00:02:34 2023, max compression
+gzip compressed data, was "dist/mangorest-0.12300000000000003.tar", last modified: Mon Jun 26 00:10:12 2023, max compression
```

## Comparing `mangorest-0.12200000000000003.tar` & `mangorest-0.12300000000000003.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:02:34.876291 mangorest-0.12200000000000003/
--rw-r--r--   0 snarayan   (501) wheel        (0)    11357 2020-09-20 16:46:27.000000 mangorest-0.12200000000000003/LICENSE
--rw-r--r--   0 snarayan   (501) wheel        (0)      798 2023-06-26 00:02:34.875980 mangorest-0.12200000000000003/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)     2449 2022-07-26 01:13:10.000000 mangorest-0.12200000000000003/README.md
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:02:34.872513 mangorest-0.12200000000000003/mangorest/
--rw-r--r--   0 snarayan   (501) wheel        (0)        0 2020-09-20 16:51:18.000000 mangorest-0.12200000000000003/mangorest/__init__.py
--rw-r--r--   0 snarayan   (501) wheel        (0)     1310 2020-09-26 18:35:34.000000 mangorest-0.12200000000000003/mangorest/dirlist.py
--rwxr-xr-x   0 snarayan   (501) wheel        (0)    11207 2023-06-26 00:02:08.000000 mangorest-0.12200000000000003/mangorest/mango.py
--rw-r--r--   0 snarayan   (501) wheel        (0)       27 2023-06-26 00:02:33.000000 mangorest-0.12200000000000003/mangorest/version.txt
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:02:34.875194 mangorest-0.12200000000000003/mangorest.egg-info/
--rw-r--r--   0 snarayan   (501) wheel        (0)      798 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)      319 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/SOURCES.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/dependency_links.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2020-09-26 14:25:00.000000 mangorest-0.12200000000000003/mangorest.egg-info/not-zip-safe
--rw-r--r--   0 snarayan   (501) wheel        (0)        7 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/requires.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       10 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/top_level.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       38 2023-06-26 00:02:34.876396 mangorest-0.12200000000000003/setup.cfg
--rw-r--r--   0 snarayan   (501) wheel        (0)     1698 2023-06-26 00:02:33.000000 mangorest-0.12200000000000003/setup.py
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:02:34.875524 mangorest-0.12200000000000003/test/
--rwxrwxr-x   0 snarayan   (501) wheel        (0)      653 2022-07-20 11:34:26.000000 mangorest-0.12200000000000003/test/test.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:10:12.096194 mangorest-0.12300000000000003/
+-rw-r--r--   0 snarayan   (501) wheel        (0)    11357 2020-09-20 16:46:27.000000 mangorest-0.12300000000000003/LICENSE
+-rw-r--r--   0 snarayan   (501) wheel        (0)      798 2023-06-26 00:10:12.095989 mangorest-0.12300000000000003/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)     2449 2022-07-26 01:13:10.000000 mangorest-0.12300000000000003/README.md
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:10:12.093321 mangorest-0.12300000000000003/mangorest/
+-rw-r--r--   0 snarayan   (501) wheel        (0)        0 2020-09-20 16:51:18.000000 mangorest-0.12300000000000003/mangorest/__init__.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1310 2020-09-26 18:35:34.000000 mangorest-0.12300000000000003/mangorest/dirlist.py
+-rwxr-xr-x   0 snarayan   (501) wheel        (0)    11302 2023-06-26 00:07:46.000000 mangorest-0.12300000000000003/mangorest/mango.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)       27 2023-06-26 00:10:11.000000 mangorest-0.12300000000000003/mangorest/version.txt
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:10:12.095258 mangorest-0.12300000000000003/mangorest.egg-info/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      798 2023-06-26 00:10:11.000000 mangorest-0.12300000000000003/mangorest.egg-info/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)      319 2023-06-26 00:10:12.000000 mangorest-0.12300000000000003/mangorest.egg-info/SOURCES.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2023-06-26 00:10:11.000000 mangorest-0.12300000000000003/mangorest.egg-info/dependency_links.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2020-09-26 14:25:00.000000 mangorest-0.12300000000000003/mangorest.egg-info/not-zip-safe
+-rw-r--r--   0 snarayan   (501) wheel        (0)        7 2023-06-26 00:10:11.000000 mangorest-0.12300000000000003/mangorest.egg-info/requires.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       10 2023-06-26 00:10:11.000000 mangorest-0.12300000000000003/mangorest.egg-info/top_level.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       38 2023-06-26 00:10:12.096259 mangorest-0.12300000000000003/setup.cfg
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1698 2023-06-26 00:10:11.000000 mangorest-0.12300000000000003/setup.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:10:12.095563 mangorest-0.12300000000000003/test/
+-rwxrwxr-x   0 snarayan   (501) wheel        (0)      653 2022-07-20 11:34:26.000000 mangorest-0.12300000000000003/test/test.py
```

### Comparing `mangorest-0.12200000000000003/LICENSE` & `mangorest-0.12300000000000003/LICENSE`

 * *Files identical despite different names*

### Comparing `mangorest-0.12200000000000003/PKG-INFO` & `mangorest-0.12300000000000003/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangorest
-Version: 0.12200000000000003
+Version: 0.12300000000000003
 Summary: Very simple quick way to deploy Django Webservices
 Home-page: https://github.com/meyers007/mangorest.git
 Author: Wan Bae, Seattle University
 Author-email: baew@seattleu.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mangorest-0.12200000000000003/README.md` & `mangorest-0.12300000000000003/README.md`

 * *Files identical despite different names*

### Comparing `mangorest-0.12200000000000003/mangorest/dirlist.py` & `mangorest-0.12300000000000003/mangorest/dirlist.py`

 * *Files identical despite different names*

### Comparing `mangorest-0.12200000000000003/mangorest/mango.py` & `mangorest-0.12300000000000003/mangorest/mango.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,21 @@
 DEBUG=0
 def logp(*args, **kwargs):
     if not DEBUG:
         return;
     
     logger.info(f'==> MANGO: {args} {kwargs}')
 
+    '''
     for c in kwargs:
         print(kwargs[c], end=" ")
     for c in args:
         print(c, end=" ")
     print()
+    '''
 #--------------------------------------------------------------------------------
 def Debug(request, APPNAME=''):
     rpath = request.path.split('/')[-2] #en(APPNAME)+2:-1]
     template = "/templates/" + rpath;
     pyModule = rpath;
     
     logp(f"{template} Requested")
@@ -195,14 +197,15 @@
     try:
         response = proxy_view(request, url)
     except Exception as e:
         return HttpResponse(f"ERROR: while getting '{url}' {e}")
     
     return response
 #--------------------------------------------------------------------------------
+LOG_NUM=1;
 def Common(request):
     path = request.path[:-1] if request.path.endswith("/") else request.path
     if ( path.endswith("favicon.ico")):
         return HttpResponse(f"{path}!!");
     
     rpaths = [c for c in request.path.split("/") if (c) ];
     if len(rpaths) and rpaths[0] == "proxy":
@@ -210,15 +213,18 @@
     
     # Check for authorizaton and version request
     authError = AUTH_METHOD(request)
     if ( authError ):
         return HttpResponse(f"{path} -- {authError}!!");
 
     # Next STEP 1: check with registered URLS
-    logp(f'*Check: {path} registered URLS: {_WEBAPI_ROUTES.keys()}')
+    global LOG_NUM
+    if ( LOG_NUM > 0 ):
+        logp(f'*Check: {path} registered URLS: {_WEBAPI_ROUTES.keys()}')
+        LOG_NUM -= 1
     
     if (path == "/SHOW_ROUTES" ):
         return showroutes(request)
     
     if (path in _WEBAPI_ROUTES.keys() ):
         f, args, auth, opts = _WEBAPI_ROUTES[path]
         if ( auth ):
```

### Comparing `mangorest-0.12200000000000003/mangorest.egg-info/PKG-INFO` & `mangorest-0.12300000000000003/mangorest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangorest
-Version: 0.12200000000000003
+Version: 0.12300000000000003
 Summary: Very simple quick way to deploy Django Webservices
 Home-page: https://github.com/meyers007/mangorest.git
 Author: Wan Bae, Seattle University
 Author-email: baew@seattleu.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mangorest-0.12200000000000003/setup.py` & `mangorest-0.12300000000000003/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version=0.12200000000000003
+version=0.12300000000000003
 
 setup(name='mangorest', 
       version=str(version), 
       description='Very simple quick way to deploy Django Webservices',
       url='https://github.com/meyers007/mangorest.git',
       author='Wan Bae, Seattle University',
       author_email='baew@seattleu.edu',
```

### Comparing `mangorest-0.12200000000000003/test/test.py` & `mangorest-0.12300000000000003/test/test.py`

 * *Files identical despite different names*

