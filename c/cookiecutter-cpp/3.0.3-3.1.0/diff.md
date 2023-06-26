# Comparing `tmp/cookiecutter-cpp-3.0.3.tar.gz` & `tmp/cookiecutter-cpp-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter-cpp-3.0.3.tar", last modified: Mon Mar 27 17:42:07 2023, max compression
+gzip compressed data, was "cookiecutter-cpp-3.1.0.tar", last modified: Mon Jun 26 21:32:05 2023, max compression
```

## Comparing `cookiecutter-cpp-3.0.3.tar` & `cookiecutter-cpp-3.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:42:07.229573 cookiecutter-cpp-3.0.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1551 2023-03-27 17:42:03.000000 cookiecutter-cpp-3.0.3/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5517 2023-03-27 17:42:07.229573 cookiecutter-cpp-3.0.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4524 2023-03-27 17:42:03.000000 cookiecutter-cpp-3.0.3/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:42:07.229573 cookiecutter-cpp-3.0.3/cookiecutter_cpp.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5517 2023-03-27 17:42:07.000000 cookiecutter-cpp-3.0.3/cookiecutter_cpp.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      197 2023-03-27 17:42:07.000000 cookiecutter-cpp-3.0.3/cookiecutter_cpp.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-27 17:42:07.000000 cookiecutter-cpp-3.0.3/cookiecutter_cpp.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-27 17:42:07.000000 cookiecutter-cpp-3.0.3/cookiecutter_cpp.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      245 2023-03-27 17:42:07.229573 cookiecutter-cpp-3.0.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1259 2023-03-27 17:42:03.000000 cookiecutter-cpp-3.0.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 21:32:05.468337 cookiecutter-cpp-3.1.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1551 2023-06-26 21:32:02.000000 cookiecutter-cpp-3.1.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5517 2023-06-26 21:32:05.468337 cookiecutter-cpp-3.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4524 2023-06-26 21:32:02.000000 cookiecutter-cpp-3.1.0/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 21:32:05.468337 cookiecutter-cpp-3.1.0/cookiecutter_cpp.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5517 2023-06-26 21:32:05.000000 cookiecutter-cpp-3.1.0/cookiecutter_cpp.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      197 2023-06-26 21:32:05.000000 cookiecutter-cpp-3.1.0/cookiecutter_cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-26 21:32:05.000000 cookiecutter-cpp-3.1.0/cookiecutter_cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-26 21:32:05.000000 cookiecutter-cpp-3.1.0/cookiecutter_cpp.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      245 2023-06-26 21:32:05.468337 cookiecutter-cpp-3.1.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1259 2023-06-26 21:32:02.000000 cookiecutter-cpp-3.1.0/setup.py
```

### Comparing `cookiecutter-cpp-3.0.3/LICENSE` & `cookiecutter-cpp-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter-cpp-3.0.3/PKG-INFO` & `cookiecutter-cpp-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-cpp
-Version: 3.0.3
+Version: 3.1.0
 Summary: Cookiecutter template for C++ with several libs ready to be used.
 Home-page: https://github.com/grhawk/cookiecutter-cpp.git
 Author: Riccardo Petraglia (forked from https://github.com/audreyr/cookiecutter-pypackage)
 Author-email: riccardo.petraglia@gmail.com
 License: BSD
 Keywords: cookiecutter,template,package,c++,cpp,gtest,spdlog
 Platform: UNKNOWN
```

### Comparing `cookiecutter-cpp-3.0.3/README.rst` & `cookiecutter-cpp-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `cookiecutter-cpp-3.0.3/cookiecutter_cpp.egg-info/PKG-INFO` & `cookiecutter-cpp-3.1.0/cookiecutter_cpp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-cpp
-Version: 3.0.3
+Version: 3.1.0
 Summary: Cookiecutter template for C++ with several libs ready to be used.
 Home-page: https://github.com/grhawk/cookiecutter-cpp.git
 Author: Riccardo Petraglia (forked from https://github.com/audreyr/cookiecutter-pypackage)
 Author-email: riccardo.petraglia@gmail.com
 License: BSD
 Keywords: cookiecutter,template,package,c++,cpp,gtest,spdlog
 Platform: UNKNOWN
```

### Comparing `cookiecutter-cpp-3.0.3/setup.py` & `cookiecutter-cpp-3.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 from pathlib import Path
 this_folder = Path(__file__).parent
 
 setup(
     name='cookiecutter-cpp',
     packages=[],
-    version='3.0.3',
+    version='3.1.0',
     description='Cookiecutter template for C++ with several libs ready to be used.',
     long_description=(this_folder / 'README.rst').read_text(),
     long_description_content_type='text/x-rst',
     author='Riccardo Petraglia (forked from https://github.com/audreyr/cookiecutter-pypackage)',
     license='BSD',
     author_email='riccardo.petraglia@gmail.com',
     url='https://github.com/grhawk/cookiecutter-cpp.git',
```

