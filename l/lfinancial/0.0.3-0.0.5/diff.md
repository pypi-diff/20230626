# Comparing `tmp/lfinancial-0.0.3.tar.gz` & `tmp/lfinancial-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.0.3.tar", last modified: Sun Jun 25 09:50:29 2023, max compression
+gzip compressed data, was "lfinancial-0.0.5.tar", last modified: Mon Jun 26 03:37:17 2023, max compression
```

## Comparing `lfinancial-0.0.3.tar` & `lfinancial-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-25 09:50:29.996655 lfinancial-0.0.3/
--rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-25 09:50:29.996537 lfinancial-0.0.3/PKG-INFO
--rw-r--r--   0 lzy        (501) staff       (20)       68 2023-06-21 09:04:34.000000 lfinancial-0.0.3/README.md
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-25 09:50:29.995993 lfinancial-0.0.3/lfinancial/
--rw-r--r--   0 lzy        (501) staff       (20)       33 2023-06-21 09:04:34.000000 lfinancial-0.0.3/lfinancial/__init__.py
--rw-r--r--   0 lzy        (501) staff       (20)      328 2023-06-25 09:43:45.000000 lfinancial-0.0.3/lfinancial/financial.py
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-25 09:50:29.996391 lfinancial-0.0.3/lfinancial.egg-info/
--rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-25 09:50:29.000000 lfinancial-0.0.3/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 lzy        (501) staff       (20)      201 2023-06-25 09:50:29.000000 lfinancial-0.0.3/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 lzy        (501) staff       (20)        1 2023-06-25 09:50:29.000000 lfinancial-0.0.3/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 lzy        (501) staff       (20)       11 2023-06-25 09:50:29.000000 lfinancial-0.0.3/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 lzy        (501) staff       (20)       38 2023-06-25 09:50:29.996690 lfinancial-0.0.3/setup.cfg
--rw-r--r--   0 lzy        (501) staff       (20)      568 2023-06-25 09:50:21.000000 lfinancial-0.0.3/setup.py
+drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-26 03:37:17.513412 lfinancial-0.0.5/
+-rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-26 03:37:17.513283 lfinancial-0.0.5/PKG-INFO
+-rw-r--r--   0 lzy        (501) staff       (20)      340 2023-06-26 03:37:07.000000 lfinancial-0.0.5/README.md
+drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-26 03:37:17.512596 lfinancial-0.0.5/lfinancial/
+-rw-r--r--   0 lzy        (501) staff       (20)       33 2023-06-21 09:04:34.000000 lfinancial-0.0.5/lfinancial/__init__.py
+-rw-r--r--   0 lzy        (501) staff       (20)      604 2023-06-26 03:34:26.000000 lfinancial-0.0.5/lfinancial/financial.py
+drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-26 03:37:17.513048 lfinancial-0.0.5/lfinancial.egg-info/
+-rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-26 03:37:17.000000 lfinancial-0.0.5/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 lzy        (501) staff       (20)      201 2023-06-26 03:37:17.000000 lfinancial-0.0.5/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 lzy        (501) staff       (20)        1 2023-06-26 03:37:17.000000 lfinancial-0.0.5/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 lzy        (501) staff       (20)       11 2023-06-26 03:37:17.000000 lfinancial-0.0.5/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 lzy        (501) staff       (20)       38 2023-06-26 03:37:17.513449 lfinancial-0.0.5/setup.cfg
+-rw-r--r--   0 lzy        (501) staff       (20)      568 2023-06-26 03:37:07.000000 lfinancial-0.0.5/setup.py
```

### Comparing `lfinancial-0.0.3/setup.py` & `lfinancial-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 excluded_packages = ["docs", "tests", "tests.*"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.0.3',
+    version='0.0.5',
     author='zaneliu',
     author_email='lzy291980138@163.com',
     description='Generate financial test data',
     packages=['lfinancial'],
     install_requires=[],
     classifiers=[
         'Programming Language :: Python :: 3',
```

