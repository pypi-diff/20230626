# Comparing `tmp/ctd-python-0.0.8.tar.gz` & `tmp/ctd-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctd-python-0.0.8.tar", last modified: Sun Jun 25 23:31:43 2023, max compression
+gzip compressed data, was "ctd-python-0.0.9.tar", last modified: Sun Jun 25 23:33:21 2023, max compression
```

## Comparing `ctd-python-0.0.8.tar` & `ctd-python-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 23:31:43.759652 ctd-python-0.0.8/
--rw-r--r--   0 john       (501) staff       (20)       54 2023-06-25 23:29:12.000000 ctd-python-0.0.8/MANIFEST.in
--rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 23:31:43.758803 ctd-python-0.0.8/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      974 2023-06-25 21:03:16.000000 ctd-python-0.0.8/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 23:31:43.754612 ctd-python-0.0.8/ctd/
--rw-r--r--   0 john       (501) staff       (20)     2326 2023-06-25 23:31:25.000000 ctd-python-0.0.8/ctd/__init__.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 23:31:43.757701 ctd-python-0.0.8/ctd_python.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 23:31:43.000000 ctd-python-0.0.8/ctd_python.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      215 2023-06-25 23:31:43.000000 ctd-python-0.0.8/ctd_python.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-06-25 23:31:43.000000 ctd-python-0.0.8/ctd_python.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       16 2023-06-25 23:31:43.000000 ctd-python-0.0.8/ctd_python.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        4 2023-06-25 23:31:43.000000 ctd-python-0.0.8/ctd_python.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-06-25 23:31:43.759815 ctd-python-0.0.8/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      506 2023-06-25 23:31:36.000000 ctd-python-0.0.8/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 23:33:21.790214 ctd-python-0.0.9/
+-rw-r--r--   0 john       (501) staff       (20)       54 2023-06-25 23:29:12.000000 ctd-python-0.0.9/MANIFEST.in
+-rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 23:33:21.789801 ctd-python-0.0.9/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      974 2023-06-25 21:03:16.000000 ctd-python-0.0.9/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 23:33:21.785617 ctd-python-0.0.9/ctd/
+-rw-r--r--   0 john       (501) staff       (20)     2326 2023-06-25 23:31:25.000000 ctd-python-0.0.9/ctd/__init__.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 23:33:21.786400 ctd-python-0.0.9/ctd/unzipped_data/
+-rw-r--r--   0 john       (501) staff       (20)        0 2023-06-25 23:33:07.000000 ctd-python-0.0.9/ctd/unzipped_data/__init__.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 23:33:21.786822 ctd-python-0.0.9/ctd/zipped_data/
+-rw-r--r--   0 john       (501) staff       (20)        0 2023-06-25 23:33:02.000000 ctd-python-0.0.9/ctd/zipped_data/__init__.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 23:33:21.789348 ctd-python-0.0.9/ctd_python.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 23:33:21.000000 ctd-python-0.0.9/ctd_python.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      273 2023-06-25 23:33:21.000000 ctd-python-0.0.9/ctd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-06-25 23:33:21.000000 ctd-python-0.0.9/ctd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       16 2023-06-25 23:33:21.000000 ctd-python-0.0.9/ctd_python.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        4 2023-06-25 23:33:21.000000 ctd-python-0.0.9/ctd_python.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-06-25 23:33:21.790377 ctd-python-0.0.9/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      506 2023-06-25 23:33:19.000000 ctd-python-0.0.9/setup.py
```

### Comparing `ctd-python-0.0.8/PKG-INFO` & `ctd-python-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.0.8/README.md` & `ctd-python-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ctd-python-0.0.8/ctd/__init__.py` & `ctd-python-0.0.9/ctd/__init__.py`

 * *Files identical despite different names*

### Comparing `ctd-python-0.0.8/ctd_python.egg-info/PKG-INFO` & `ctd-python-0.0.9/ctd_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

