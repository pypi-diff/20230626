# Comparing `tmp/pymultigit-0.0.85.tar.gz` & `tmp/pymultigit-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultigit-0.0.85.tar", last modified: Mon Jun 26 09:13:59 2023, max compression
+gzip compressed data, was "pymultigit-0.0.86.tar", last modified: Mon Jun 26 11:01:10 2023, max compression
```

## Comparing `pymultigit-0.0.85.tar` & `pymultigit-0.0.86.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-26 09:13:59.037600 pymultigit-0.0.85/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-06-26 09:13:51.000000 pymultigit-0.0.85/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1411 2023-06-26 09:13:59.037600 pymultigit-0.0.85/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      427 2023-06-26 09:13:31.000000 pymultigit-0.0.85/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-26 09:13:59.037600 pymultigit-0.0.85/pymultigit/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:34:03.000000 pymultigit-0.0.85/pymultigit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2662 2023-05-02 09:28:38.000000 pymultigit-0.0.85/pymultigit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     8946 2023-06-26 09:13:12.000000 pymultigit-0.0.85/pymultigit/core.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5359 2023-05-02 11:04:28.000000 pymultigit-0.0.85/pymultigit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      208 2023-06-26 09:13:31.000000 pymultigit-0.0.85/pymultigit/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-26 09:13:59.037600 pymultigit-0.0.85/pymultigit/utils/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-05-02 09:28:38.000000 pymultigit-0.0.85/pymultigit/utils/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      797 2023-05-02 09:28:38.000000 pymultigit-0.0.85/pymultigit/utils/subprocess.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-26 09:13:59.037600 pymultigit-0.0.85/pymultigit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1411 2023-06-26 09:13:59.000000 pymultigit-0.0.85/pymultigit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      407 2023-06-26 09:13:59.000000 pymultigit-0.0.85/pymultigit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-06-26 09:13:59.000000 pymultigit-0.0.85/pymultigit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-06-26 09:13:59.000000 pymultigit-0.0.85/pymultigit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       47 2023-06-26 09:13:59.000000 pymultigit-0.0.85/pymultigit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-06-26 09:13:59.000000 pymultigit-0.0.85/pymultigit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-06-26 09:13:59.037600 pymultigit-0.0.85/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1652 2023-06-26 09:13:31.000000 pymultigit-0.0.85/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-26 11:01:09.997213 pymultigit-0.0.86/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-06-26 11:00:59.000000 pymultigit-0.0.86/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1411 2023-06-26 11:01:09.997213 pymultigit-0.0.86/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      427 2023-06-26 11:00:57.000000 pymultigit-0.0.86/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-26 11:01:09.997213 pymultigit-0.0.86/pymultigit/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:34:03.000000 pymultigit-0.0.86/pymultigit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2662 2023-05-02 09:28:38.000000 pymultigit-0.0.86/pymultigit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     8952 2023-06-26 11:00:26.000000 pymultigit-0.0.86/pymultigit/core.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5359 2023-05-02 11:04:28.000000 pymultigit-0.0.86/pymultigit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      208 2023-06-26 11:00:57.000000 pymultigit-0.0.86/pymultigit/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-26 11:01:09.997213 pymultigit-0.0.86/pymultigit/utils/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-05-02 09:28:38.000000 pymultigit-0.0.86/pymultigit/utils/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      797 2023-05-02 09:28:38.000000 pymultigit-0.0.86/pymultigit/utils/subprocess.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-26 11:01:09.997213 pymultigit-0.0.86/pymultigit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1411 2023-06-26 11:01:09.000000 pymultigit-0.0.86/pymultigit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      407 2023-06-26 11:01:09.000000 pymultigit-0.0.86/pymultigit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-06-26 11:01:09.000000 pymultigit-0.0.86/pymultigit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-06-26 11:01:09.000000 pymultigit-0.0.86/pymultigit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       47 2023-06-26 11:01:09.000000 pymultigit-0.0.86/pymultigit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-06-26 11:01:09.000000 pymultigit-0.0.86/pymultigit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-06-26 11:01:09.997213 pymultigit-0.0.86/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1652 2023-06-26 11:00:57.000000 pymultigit-0.0.86/setup.py
```

### Comparing `pymultigit-0.0.85/LICENSE` & `pymultigit-0.0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.85/PKG-INFO` & `pymultigit-0.0.86/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultigit
-Version: 0.0.85
+Version: 0.0.86
 Summary: Pymultigit helps you deal with multiple git repositories
 Home-page: https://veltzer.github.io/pymultigit
 Download-URL: https://github.com/veltzer/pymultigit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pymultigit
 
 author: Mark Veltzer
 
-version: 0.0.85
+version: 0.0.86
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pymultigit-0.0.85/pymultigit/configs.py` & `pymultigit-0.0.86/pymultigit/configs.py`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.85/pymultigit/core.py` & `pymultigit-0.0.86/pymultigit/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 def do_build_make() -> None:
     if disable():
         return
     if not os.path.isfile("Makefile"):
         if ConfigOutput.print_not:
             print("not a make folder (Makefile not there)")
         return
-    subprocess.call(["make"])
+    subprocess.check_call(["make"])
 
 
 def do_pull() -> int:
     args = ["git", "pull"]
     if ConfigDebug.git_verbose:
         args.append("--verbose")
     if ConfigPull.pull_quiet:
```

### Comparing `pymultigit-0.0.85/pymultigit/main.py` & `pymultigit-0.0.86/pymultigit/main.py`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.85/pymultigit/utils/subprocess.py` & `pymultigit-0.0.86/pymultigit/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.85/pymultigit.egg-info/PKG-INFO` & `pymultigit-0.0.86/pymultigit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultigit
-Version: 0.0.85
+Version: 0.0.86
 Summary: Pymultigit helps you deal with multiple git repositories
 Home-page: https://veltzer.github.io/pymultigit
 Download-URL: https://github.com/veltzer/pymultigit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pymultigit
 
 author: Mark Veltzer
 
-version: 0.0.85
+version: 0.0.86
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pymultigit-0.0.85/setup.py` & `pymultigit-0.0.86/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pymultigit",
-    version="0.0.85",
+    version="0.0.86",
     packages=[
         "pymultigit",
         "pymultigit.utils",
     ],
     # from here all is optional
     description="Pymultigit helps you deal with multiple git repositories",
     long_description=get_readme(),
```

