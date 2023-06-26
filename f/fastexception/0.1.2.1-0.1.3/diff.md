# Comparing `tmp/fastexception-0.1.2.1.tar.gz` & `tmp/fastexception-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastexception-0.1.2.1.tar", last modified: Mon Jun 26 08:50:07 2023, max compression
+gzip compressed data, was "fastexception-0.1.3.tar", last modified: Mon Jun 26 08:57:12 2023, max compression
```

## Comparing `fastexception-0.1.2.1.tar` & `fastexception-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 08:50:07.139729 fastexception-0.1.2.1/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1062 2023-06-25 19:31:43.000000 fastexception-0.1.2.1/LICENSE.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      296 2023-06-26 08:50:07.139729 fastexception-0.1.2.1/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1015 2023-06-26 07:08:25.000000 fastexception-0.1.2.1/README.md
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 08:50:07.139729 fastexception-0.1.2.1/fastexception.egg-info/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      296 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      214 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/SOURCES.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/dependency_links.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/requires.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/top_level.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-06-26 08:50:07.139729 fastexception-0.1.2.1/setup.cfg
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      547 2023-06-26 08:50:05.000000 fastexception-0.1.2.1/setup.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 08:57:12.713100 fastexception-0.1.3/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1062 2023-06-25 19:31:43.000000 fastexception-0.1.3/LICENSE.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1300 2023-06-26 08:57:12.713100 fastexception-0.1.3/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1015 2023-06-26 07:08:25.000000 fastexception-0.1.3/README.md
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 08:57:12.713100 fastexception-0.1.3/fastexception.egg-info/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1300 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      214 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/SOURCES.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/dependency_links.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/requires.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/top_level.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-06-26 08:57:12.713100 fastexception-0.1.3/setup.cfg
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      581 2023-06-26 08:57:07.000000 fastexception-0.1.3/setup.py
```

### Comparing `fastexception-0.1.2.1/LICENSE.txt` & `fastexception-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastexception-0.1.2.1/README.md` & `fastexception-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fastexception-0.1.2.1/setup.py` & `fastexception-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
-# this_directory = Path(__file__)
-long_description = "README.md"
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 setup(
     name='fastexception',
-    version='0.1.2.1',
+    version='0.1.3',
     license='MIT',
     author='Mojtaba',
     author_email='mojtabapaso@gamil.com',
     packages=find_packages(),
     url='https://github.com/mojtabapaso/fastexception',
     keywords='FastAPI Tools Fast Exception',
     install_requires=[
```

