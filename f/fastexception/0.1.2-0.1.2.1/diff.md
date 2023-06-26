# Comparing `tmp/fastexception-0.1.2.tar.gz` & `tmp/fastexception-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastexception-0.1.2.tar", last modified: Mon Jun 26 06:44:51 2023, max compression
+gzip compressed data, was "fastexception-0.1.2.1.tar", last modified: Mon Jun 26 08:50:07 2023, max compression
```

## Comparing `fastexception-0.1.2.tar` & `fastexception-0.1.2.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 06:44:51.380868 fastexception-0.1.2/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1274 2023-06-26 06:44:51.380868 fastexception-0.1.2/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1174 2023-06-25 19:34:30.000000 fastexception-0.1.2/README.rst
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 06:44:51.380868 fastexception-0.1.2/fastexception.egg-info/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1274 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      213 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/SOURCES.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/dependency_links.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/requires.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 06:44:51.000000 fastexception-0.1.2/fastexception.egg-info/top_level.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      107 2023-06-26 06:44:51.380868 fastexception-0.1.2/setup.cfg
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      581 2023-06-26 06:44:37.000000 fastexception-0.1.2/setup.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 08:50:07.139729 fastexception-0.1.2.1/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1062 2023-06-25 19:31:43.000000 fastexception-0.1.2.1/LICENSE.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      296 2023-06-26 08:50:07.139729 fastexception-0.1.2.1/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1015 2023-06-26 07:08:25.000000 fastexception-0.1.2.1/README.md
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 08:50:07.139729 fastexception-0.1.2.1/fastexception.egg-info/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      296 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      214 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/SOURCES.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/dependency_links.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/requires.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 08:50:07.000000 fastexception-0.1.2.1/fastexception.egg-info/top_level.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-06-26 08:50:07.139729 fastexception-0.1.2.1/setup.cfg
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      547 2023-06-26 08:50:05.000000 fastexception-0.1.2.1/setup.py
```

### Comparing `fastexception-0.1.2/setup.py` & `fastexception-0.1.2.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+# this_directory = Path(__file__)
+long_description = "README.md"
 setup(
     name='fastexception',
-    version='0.1.2',
+    version='0.1.2.1',
     license='MIT',
     author='Mojtaba',
     author_email='mojtabapaso@gamil.com',
     packages=find_packages(),
     url='https://github.com/mojtabapaso/fastexception',
     keywords='FastAPI Tools Fast Exception',
     install_requires=[
```

