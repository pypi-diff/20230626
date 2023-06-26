# Comparing `tmp/lfinancial-0.0.5.tar.gz` & `tmp/lfinancial-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.0.5.tar", last modified: Mon Jun 26 03:37:17 2023, max compression
+gzip compressed data, was "lfinancial-0.0.6.tar", last modified: Mon Jun 26 14:01:25 2023, max compression
```

## Comparing `lfinancial-0.0.5.tar` & `lfinancial-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-26 03:37:17.513412 lfinancial-0.0.5/
--rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-26 03:37:17.513283 lfinancial-0.0.5/PKG-INFO
--rw-r--r--   0 lzy        (501) staff       (20)      340 2023-06-26 03:37:07.000000 lfinancial-0.0.5/README.md
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-26 03:37:17.512596 lfinancial-0.0.5/lfinancial/
--rw-r--r--   0 lzy        (501) staff       (20)       33 2023-06-21 09:04:34.000000 lfinancial-0.0.5/lfinancial/__init__.py
--rw-r--r--   0 lzy        (501) staff       (20)      604 2023-06-26 03:34:26.000000 lfinancial-0.0.5/lfinancial/financial.py
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-26 03:37:17.513048 lfinancial-0.0.5/lfinancial.egg-info/
--rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-26 03:37:17.000000 lfinancial-0.0.5/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 lzy        (501) staff       (20)      201 2023-06-26 03:37:17.000000 lfinancial-0.0.5/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 lzy        (501) staff       (20)        1 2023-06-26 03:37:17.000000 lfinancial-0.0.5/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 lzy        (501) staff       (20)       11 2023-06-26 03:37:17.000000 lfinancial-0.0.5/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 lzy        (501) staff       (20)       38 2023-06-26 03:37:17.513449 lfinancial-0.0.5/setup.cfg
--rw-r--r--   0 lzy        (501) staff       (20)      568 2023-06-26 03:37:07.000000 lfinancial-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:01:25.272941 lfinancial-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 14:01:25.272941 lfinancial-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-26 14:01:15.000000 lfinancial-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:01:25.272941 lfinancial-0.0.6/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 14:01:15.000000 lfinancial-0.0.6/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-26 14:01:15.000000 lfinancial-0.0.6/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:01:25.272941 lfinancial-0.0.6/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 14:01:25.000000 lfinancial-0.0.6/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-26 14:01:25.000000 lfinancial-0.0.6/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:01:25.000000 lfinancial-0.0.6/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 14:01:25.000000 lfinancial-0.0.6/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:01:25.272941 lfinancial-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 14:01:15.000000 lfinancial-0.0.6/setup.py
```

### Comparing `lfinancial-0.0.5/lfinancial/financial.py` & `lfinancial-0.0.6/lfinancial/financial.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.0.5/setup.py` & `lfinancial-0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from setuptools import find_packages, setup
+from setuptools import setup
 
 excluded_packages = ["docs", "tests", "tests.*"]
-
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+
 setup(
     name='lfinancial',
-    version='0.0.5',
+    version='0.0.6',
     author='zaneliu',
-    author_email='lzy291980138@163.com',
     description='Generate financial test data',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    readme="README.md",
+    author_email='lzy291980138@163.com',
     packages=['lfinancial'],
     install_requires=[],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

