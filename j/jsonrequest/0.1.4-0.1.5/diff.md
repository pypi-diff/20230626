# Comparing `tmp/jsonrequest-0.1.4.tar.gz` & `tmp/jsonrequest-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrequest-0.1.4.tar", last modified: Mon Jun 26 07:01:06 2023, max compression
+gzip compressed data, was "jsonrequest-0.1.5.tar", last modified: Mon Jun 26 08:02:14 2023, max compression
```

## Comparing `jsonrequest-0.1.4.tar` & `jsonrequest-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 07:01:06.944153 jsonrequest-0.1.4/
--rw-r--r--   0 JustinRWong   (502) staff       (20)    11357 2023-06-26 05:51:37.000000 jsonrequest-0.1.4/LICENSE
--rw-r--r--   0 JustinRWong   (502) staff       (20)     1610 2023-06-26 07:01:06.944025 jsonrequest-0.1.4/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)      979 2023-06-26 06:40:48.000000 jsonrequest-0.1.4/README.md
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 07:01:06.943872 jsonrequest-0.1.4/jsonrequest.egg-info/
--rw-r--r--   0 JustinRWong   (502) staff       (20)     1610 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)      215 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/SOURCES.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/dependency_links.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/requires.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/top_level.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)      597 2023-06-26 06:55:16.000000 jsonrequest-0.1.4/pyproject.toml
--rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 07:01:06.944193 jsonrequest-0.1.4/setup.cfg
--rw-r--r--   0 JustinRWong   (502) staff       (20)      621 2023-06-26 06:55:26.000000 jsonrequest-0.1.4/setup.py
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 08:02:14.167487 jsonrequest-0.1.5/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)     1734 2023-06-26 08:02:14.167326 jsonrequest-0.1.5/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)     1103 2023-06-26 07:12:08.000000 jsonrequest-0.1.5/README.md
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 08:02:14.166394 jsonrequest-0.1.5/jsonrequest/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      395 2023-06-26 08:01:51.000000 jsonrequest-0.1.5/jsonrequest/RequestModel.py
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       74 2023-06-26 07:59:32.000000 jsonrequest-0.1.5/jsonrequest/__init__.py
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      604 2023-06-26 07:59:30.000000 jsonrequest-0.1.5/jsonrequest/jsonrequest.py
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 08:02:14.167049 jsonrequest-0.1.5/jsonrequest.egg-info/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)     1734 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      286 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/SOURCES.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/dependency_links.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/requires.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       12 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/top_level.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      597 2023-06-26 08:00:35.000000 jsonrequest-0.1.5/pyproject.toml
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 08:02:14.167536 jsonrequest-0.1.5/setup.cfg
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      621 2023-06-26 07:59:59.000000 jsonrequest-0.1.5/setup.py
```

### Comparing `jsonrequest-0.1.4/pyproject.toml` & `jsonrequest-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jsonrequest"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Justin Wong", email="justinryanwong@berkeley.edu" },
 ]
 description = "Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content."
 readme = "README.md"
 requires-python = ">=3.2"
 classifiers = [
```

### Comparing `jsonrequest-0.1.4/setup.py` & `jsonrequest-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='jsonrequest',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pydantic',
     ],
     author='Justin Wong',
     description='Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.',
```

