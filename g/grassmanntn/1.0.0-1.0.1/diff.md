# Comparing `tmp/grassmanntn-1.0.0.tar.gz` & `tmp/grassmanntn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.0.0.tar", last modified: Mon Jun 26 03:46:43 2023, max compression
+gzip compressed data, was "grassmanntn-1.0.1.tar", last modified: Mon Jun 26 04:07:39 2023, max compression
```

## Comparing `grassmanntn-1.0.0.tar` & `grassmanntn-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 03:46:43.185673 grassmanntn-1.0.0/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.0.0/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      731 2023-06-26 03:46:43.185673 grassmanntn-1.0.0/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     4373 2023-06-26 02:27:00.000000 grassmanntn-1.0.0/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 03:46:43.185673 grassmanntn-1.0.0/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      107 2023-06-26 02:11:32.000000 grassmanntn-1.0.0/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132612 2023-06-26 03:15:27.000000 grassmanntn-1.0.0/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109253 2023-06-26 03:34:21.000000 grassmanntn-1.0.0/grassmanntn/grassmanntn.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.0.0/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 03:46:43.185673 grassmanntn-1.0.0/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      731 2023-06-26 03:46:43.000000 grassmanntn-1.0.0/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      309 2023-06-26 03:46:43.000000 grassmanntn-1.0.0/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-06-26 03:46:43.000000 grassmanntn-1.0.0/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-06-26 03:46:43.000000 grassmanntn-1.0.0/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-06-26 03:46:43.000000 grassmanntn-1.0.0/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-06-26 03:46:43.189673 grassmanntn-1.0.0/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1681 2023-06-26 03:46:33.000000 grassmanntn-1.0.0/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 04:07:39.310927 grassmanntn-1.0.1/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.0.1/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-06-26 04:07:39.310927 grassmanntn-1.0.1/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.0.1/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 04:07:39.310927 grassmanntn-1.0.1/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      107 2023-06-26 02:11:32.000000 grassmanntn-1.0.1/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132612 2023-06-26 03:15:27.000000 grassmanntn-1.0.1/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109253 2023-06-26 03:34:21.000000 grassmanntn-1.0.1/grassmanntn/grassmanntn.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.0.1/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 04:07:39.310927 grassmanntn-1.0.1/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-06-26 04:07:39.000000 grassmanntn-1.0.1/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      309 2023-06-26 04:07:39.000000 grassmanntn-1.0.1/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-06-26 04:07:39.000000 grassmanntn-1.0.1/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-06-26 04:07:39.000000 grassmanntn-1.0.1/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-06-26 04:07:39.000000 grassmanntn-1.0.1/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-06-26 04:07:39.310927 grassmanntn-1.0.1/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-06-26 04:06:37.000000 grassmanntn-1.0.1/setup.py
```

### Comparing `grassmanntn-1.0.0/LICENSE.txt` & `grassmanntn-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.0.0/grassmanntn/gauge2d.py` & `grassmanntn-1.0.1/grassmanntn/gauge2d.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.0.0/grassmanntn/grassmanntn.py` & `grassmanntn-1.0.1/grassmanntn/grassmanntn.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.0.0/grassmanntn/param.py` & `grassmanntn-1.0.1/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.0.0/setup.py` & `grassmanntn-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from distutils.core import setup
+
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.0.0',      # Start with a small number and increase it with every change you make
+  version = '1.0.1',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
+  long_description=long_description,
+  long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_100.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_101.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

