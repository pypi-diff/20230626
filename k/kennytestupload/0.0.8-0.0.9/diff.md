# Comparing `tmp/kennytestupload-0.0.8.tar.gz` & `tmp/kennytestupload-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kennytestupload-0.0.8.tar", last modified: Mon Jun 26 21:46:21 2023, max compression
+gzip compressed data, was "dist/kennytestupload-0.0.9.tar", last modified: Mon Jun 26 21:49:56 2023, max compression
```

## Comparing `kennytestupload-0.0.8.tar` & `kennytestupload-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:46:21.455167 kennytestupload-0.0.8/
--rw-r--r--   0 kenny      (501) staff       (20)      348 2023-06-26 21:46:21.454966 kennytestupload-0.0.8/PKG-INFO
--rw-r--r--   0 kenny      (501) staff       (20)       22 2023-06-26 19:38:53.000000 kennytestupload-0.0.8/README
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:46:21.453787 kennytestupload-0.0.8/kennytestupload/
--rw-r--r--   0 kenny      (501) staff       (20)      582 2023-06-12 20:55:20.000000 kennytestupload-0.0.8/kennytestupload/BasicDemo.py
--rw-r--r--   0 kenny      (501) staff       (20)     1543 2023-06-12 21:21:01.000000 kennytestupload-0.0.8/kennytestupload/ClassUsage.py
--rw-r--r--   0 kenny      (501) staff       (20)     1895 2023-06-20 00:05:55.000000 kennytestupload-0.0.8/kennytestupload/Collision.py
--rw-r--r--   0 kenny      (501) staff       (20)      989 2023-06-12 23:31:16.000000 kennytestupload-0.0.8/kennytestupload/Features.py
--rw-r--r--   0 kenny      (501) staff       (20)    11451 2023-06-26 19:31:00.000000 kennytestupload-0.0.8/kennytestupload/Main.py
--rw-r--r--   0 kenny      (501) staff       (20)     3075 2023-06-26 21:18:01.000000 kennytestupload-0.0.8/kennytestupload/SpaceInvader.py
--rw-r--r--   0 kenny      (501) staff       (20)     1613 2023-06-13 00:24:31.000000 kennytestupload-0.0.8/kennytestupload/Tets.py
--rw-r--r--   0 kenny      (501) staff       (20)      131 2023-06-26 20:29:08.000000 kennytestupload-0.0.8/kennytestupload/__init__.py
--rw-r--r--   0 kenny      (501) staff       (20)      816 2023-06-26 21:18:37.000000 kennytestupload-0.0.8/kennytestupload/__init__.spec
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:46:21.454753 kennytestupload-0.0.8/kennytestupload.egg-info/
--rw-r--r--   0 kenny      (501) staff       (20)      348 2023-06-26 21:46:21.000000 kennytestupload-0.0.8/kennytestupload.egg-info/PKG-INFO
--rw-r--r--   0 kenny      (501) staff       (20)      425 2023-06-26 21:46:21.000000 kennytestupload-0.0.8/kennytestupload.egg-info/SOURCES.txt
--rw-r--r--   0 kenny      (501) staff       (20)        1 2023-06-26 21:46:21.000000 kennytestupload-0.0.8/kennytestupload.egg-info/dependency_links.txt
--rw-r--r--   0 kenny      (501) staff       (20)       16 2023-06-26 21:46:21.000000 kennytestupload-0.0.8/kennytestupload.egg-info/top_level.txt
--rw-r--r--   0 kenny      (501) staff       (20)       38 2023-06-26 21:46:21.455224 kennytestupload-0.0.8/setup.cfg
--rw-r--r--   0 kenny      (501) staff       (20)      918 2023-06-26 21:46:15.000000 kennytestupload-0.0.8/setup.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:49:56.555455 kennytestupload-0.0.9/
+-rw-r--r--   0 kenny      (501) staff       (20)      348 2023-06-26 21:49:56.555221 kennytestupload-0.0.9/PKG-INFO
+-rw-r--r--   0 kenny      (501) staff       (20)       22 2023-06-26 19:38:53.000000 kennytestupload-0.0.9/README
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:49:56.554034 kennytestupload-0.0.9/kennytestupload/
+-rw-r--r--   0 kenny      (501) staff       (20)      582 2023-06-12 20:55:20.000000 kennytestupload-0.0.9/kennytestupload/BasicDemo.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1543 2023-06-12 21:21:01.000000 kennytestupload-0.0.9/kennytestupload/ClassUsage.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1895 2023-06-20 00:05:55.000000 kennytestupload-0.0.9/kennytestupload/Collision.py
+-rw-r--r--   0 kenny      (501) staff       (20)      989 2023-06-12 23:31:16.000000 kennytestupload-0.0.9/kennytestupload/Features.py
+-rw-r--r--   0 kenny      (501) staff       (20)    11451 2023-06-26 19:31:00.000000 kennytestupload-0.0.9/kennytestupload/Main.py
+-rw-r--r--   0 kenny      (501) staff       (20)     3075 2023-06-26 21:18:01.000000 kennytestupload-0.0.9/kennytestupload/SpaceInvader.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1613 2023-06-13 00:24:31.000000 kennytestupload-0.0.9/kennytestupload/Tets.py
+-rw-r--r--   0 kenny      (501) staff       (20)      131 2023-06-26 20:29:08.000000 kennytestupload-0.0.9/kennytestupload/__init__.py
+-rw-r--r--   0 kenny      (501) staff       (20)      816 2023-06-26 21:18:37.000000 kennytestupload-0.0.9/kennytestupload/__init__.spec
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:49:56.554930 kennytestupload-0.0.9/kennytestupload.egg-info/
+-rw-r--r--   0 kenny      (501) staff       (20)      348 2023-06-26 21:49:56.000000 kennytestupload-0.0.9/kennytestupload.egg-info/PKG-INFO
+-rw-r--r--   0 kenny      (501) staff       (20)      425 2023-06-26 21:49:56.000000 kennytestupload-0.0.9/kennytestupload.egg-info/SOURCES.txt
+-rw-r--r--   0 kenny      (501) staff       (20)        1 2023-06-26 21:49:56.000000 kennytestupload-0.0.9/kennytestupload.egg-info/dependency_links.txt
+-rw-r--r--   0 kenny      (501) staff       (20)       16 2023-06-26 21:49:56.000000 kennytestupload-0.0.9/kennytestupload.egg-info/top_level.txt
+-rw-r--r--   0 kenny      (501) staff       (20)       38 2023-06-26 21:49:56.555515 kennytestupload-0.0.9/setup.cfg
+-rw-r--r--   0 kenny      (501) staff       (20)      951 2023-06-26 21:49:54.000000 kennytestupload-0.0.9/setup.py
```

### Comparing `kennytestupload-0.0.8/kennytestupload/BasicDemo.py` & `kennytestupload-0.0.9/kennytestupload/BasicDemo.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.8/kennytestupload/ClassUsage.py` & `kennytestupload-0.0.9/kennytestupload/ClassUsage.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.8/kennytestupload/Collision.py` & `kennytestupload-0.0.9/kennytestupload/Collision.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.8/kennytestupload/Features.py` & `kennytestupload-0.0.9/kennytestupload/Features.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.8/kennytestupload/Main.py` & `kennytestupload-0.0.9/kennytestupload/Main.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.8/kennytestupload/SpaceInvader.py` & `kennytestupload-0.0.9/kennytestupload/SpaceInvader.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.8/kennytestupload/Tets.py` & `kennytestupload-0.0.9/kennytestupload/Tets.py`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.8/kennytestupload/__init__.spec` & `kennytestupload-0.0.9/kennytestupload/__init__.spec`

 * *Files identical despite different names*

### Comparing `kennytestupload-0.0.8/setup.py` & `kennytestupload-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "kennytestupload",
-    version = "0.0.8",
+    version = "0.0.9",
     author = "Kenny C",
     author_email = "kennycheung388@yahoo.com.hk",
     description = ("An demonstration of how to upload project to pypi."),
     license = "MIT License",
     keywords = "tutorial",
     url = "",
+    include_package_data = True,
     packages=['kennytestupload'],
     package_data={'kennytestupload':['*']},
     long_description=read('README'),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
     ],
```

