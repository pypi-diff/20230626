# Comparing `tmp/mangorest-0.12100000000000002.tar.gz` & `tmp/mangorest-0.12200000000000003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mangorest-0.12100000000000002.tar", last modified: Sun Sep  4 05:53:17 2022, max compression
+gzip compressed data, was "dist/mangorest-0.12200000000000003.tar", last modified: Mon Jun 26 00:02:34 2023, max compression
```

## Comparing `mangorest-0.12100000000000002.tar` & `mangorest-0.12200000000000003.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2022-09-04 05:53:17.021332 mangorest-0.12100000000000002/
--rw-r--r--   0 snarayan   (501) wheel        (0)    11357 2020-09-20 16:46:27.000000 mangorest-0.12100000000000002/LICENSE
--rw-r--r--   0 snarayan   (501) wheel        (0)      826 2022-09-04 05:53:17.020976 mangorest-0.12100000000000002/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)     2449 2022-07-26 01:13:10.000000 mangorest-0.12100000000000002/README.md
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2022-09-04 05:53:17.018042 mangorest-0.12100000000000002/mangorest/
--rw-r--r--   0 snarayan   (501) wheel        (0)        0 2020-09-20 16:51:18.000000 mangorest-0.12100000000000002/mangorest/__init__.py
--rw-r--r--   0 snarayan   (501) wheel        (0)     1310 2020-09-26 18:35:34.000000 mangorest-0.12100000000000002/mangorest/dirlist.py
--rwxr-xr-x   0 snarayan   (501) wheel        (0)    10866 2022-09-04 05:24:44.000000 mangorest-0.12100000000000002/mangorest/mango.py
--rw-r--r--   0 snarayan   (501) wheel        (0)       27 2022-09-04 05:53:16.000000 mangorest-0.12100000000000002/mangorest/version.txt
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2022-09-04 05:53:17.020174 mangorest-0.12100000000000002/mangorest.egg-info/
--rw-r--r--   0 snarayan   (501) wheel        (0)      826 2022-09-04 05:53:16.000000 mangorest-0.12100000000000002/mangorest.egg-info/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)      319 2022-09-04 05:53:16.000000 mangorest-0.12100000000000002/mangorest.egg-info/SOURCES.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2022-09-04 05:53:16.000000 mangorest-0.12100000000000002/mangorest.egg-info/dependency_links.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2020-09-26 14:25:00.000000 mangorest-0.12100000000000002/mangorest.egg-info/not-zip-safe
--rw-r--r--   0 snarayan   (501) wheel        (0)        7 2022-09-04 05:53:16.000000 mangorest-0.12100000000000002/mangorest.egg-info/requires.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       10 2022-09-04 05:53:16.000000 mangorest-0.12100000000000002/mangorest.egg-info/top_level.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       38 2022-09-04 05:53:17.021443 mangorest-0.12100000000000002/setup.cfg
--rw-r--r--   0 snarayan   (501) wheel        (0)     1698 2022-09-04 05:53:16.000000 mangorest-0.12100000000000002/setup.py
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2022-09-04 05:53:17.020527 mangorest-0.12100000000000002/test/
--rwxrwxr-x   0 snarayan   (501) wheel        (0)      653 2022-07-20 11:34:26.000000 mangorest-0.12100000000000002/test/test.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:02:34.876291 mangorest-0.12200000000000003/
+-rw-r--r--   0 snarayan   (501) wheel        (0)    11357 2020-09-20 16:46:27.000000 mangorest-0.12200000000000003/LICENSE
+-rw-r--r--   0 snarayan   (501) wheel        (0)      798 2023-06-26 00:02:34.875980 mangorest-0.12200000000000003/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)     2449 2022-07-26 01:13:10.000000 mangorest-0.12200000000000003/README.md
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:02:34.872513 mangorest-0.12200000000000003/mangorest/
+-rw-r--r--   0 snarayan   (501) wheel        (0)        0 2020-09-20 16:51:18.000000 mangorest-0.12200000000000003/mangorest/__init__.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1310 2020-09-26 18:35:34.000000 mangorest-0.12200000000000003/mangorest/dirlist.py
+-rwxr-xr-x   0 snarayan   (501) wheel        (0)    11207 2023-06-26 00:02:08.000000 mangorest-0.12200000000000003/mangorest/mango.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)       27 2023-06-26 00:02:33.000000 mangorest-0.12200000000000003/mangorest/version.txt
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:02:34.875194 mangorest-0.12200000000000003/mangorest.egg-info/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      798 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)      319 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/SOURCES.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/dependency_links.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2020-09-26 14:25:00.000000 mangorest-0.12200000000000003/mangorest.egg-info/not-zip-safe
+-rw-r--r--   0 snarayan   (501) wheel        (0)        7 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/requires.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       10 2023-06-26 00:02:34.000000 mangorest-0.12200000000000003/mangorest.egg-info/top_level.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       38 2023-06-26 00:02:34.876396 mangorest-0.12200000000000003/setup.cfg
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1698 2023-06-26 00:02:33.000000 mangorest-0.12200000000000003/setup.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2023-06-26 00:02:34.875524 mangorest-0.12200000000000003/test/
+-rwxrwxr-x   0 snarayan   (501) wheel        (0)      653 2022-07-20 11:34:26.000000 mangorest-0.12200000000000003/test/test.py
```

### Comparing `mangorest-0.12100000000000002/LICENSE` & `mangorest-0.12200000000000003/LICENSE`

 * *Files identical despite different names*

### Comparing `mangorest-0.12100000000000002/README.md` & `mangorest-0.12200000000000003/README.md`

 * *Files identical despite different names*

### Comparing `mangorest-0.12100000000000002/mangorest/dirlist.py` & `mangorest-0.12200000000000003/mangorest/dirlist.py`

 * *Files identical despite different names*

### Comparing `mangorest-0.12100000000000002/mangorest/mango.py` & `mangorest-0.12200000000000003/mangorest/mango.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 from django.contrib.auth.decorators import login_required
 from django.core.serializers.json import DjangoJSONEncoder
 from django.conf import settings
 from django.core.management import execute_from_command_line
 import numpy as np
 from proxy.views import proxy_view
 
+import logging
+logging.basicConfig( level=logging.INFO,
+        format='%(asctime)s %(name)s %(levelname)s: %(message)s',
+        handlers=[ logging.FileHandler("/tmp/geoapp.log"), logging.StreamHandler()],
+        #handlers=[ logging.StreamHandler()],
+)
+logger = logging.getLogger( "geoapp")
 
 '''
 References: 
 https://blog.miguelgrinberg.com/post/the-ultimate-guide-to-python-decorators-part-iii-decorators-with-arguments
 https://simpleisbetterthancomplex.com/article/2017/08/07/a-minimal-django-application.html
 
 '''
@@ -30,14 +37,16 @@
     return showroutes(request)    
 #--------------------------------------------------------------------------------
 DEBUG=0
 def logp(*args, **kwargs):
     if not DEBUG:
         return;
     
+    logger.info(f'==> MANGO: {args} {kwargs}')
+
     for c in kwargs:
         print(kwargs[c], end=" ")
     for c in args:
         print(c, end=" ")
     print()
 #--------------------------------------------------------------------------------
 def Debug(request, APPNAME=''):
```

### Comparing `mangorest-0.12100000000000002/setup.py` & `mangorest-0.12200000000000003/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version=0.12100000000000002
+version=0.12200000000000003
 
 setup(name='mangorest', 
       version=str(version), 
       description='Very simple quick way to deploy Django Webservices',
       url='https://github.com/meyers007/mangorest.git',
       author='Wan Bae, Seattle University',
       author_email='baew@seattleu.edu',
```

### Comparing `mangorest-0.12100000000000002/test/test.py` & `mangorest-0.12200000000000003/test/test.py`

 * *Files identical despite different names*

