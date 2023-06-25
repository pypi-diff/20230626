# Comparing `tmp/ctd-python-0.0.5.tar.gz` & `tmp/ctd-python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctd-python-0.0.5.tar", last modified: Sun Jun 25 21:15:04 2023, max compression
+gzip compressed data, was "ctd-python-0.0.6.tar", last modified: Sun Jun 25 21:19:25 2023, max compression
```

## Comparing `ctd-python-0.0.5.tar` & `ctd-python-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 21:15:04.753329 ctd-python-0.0.5/
--rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 21:15:04.752810 ctd-python-0.0.5/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      974 2023-06-25 21:03:16.000000 ctd-python-0.0.5/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 21:15:04.747812 ctd-python-0.0.5/ctd/
--rw-r--r--   0 john       (501) staff       (20)     2396 2023-06-25 21:04:11.000000 ctd-python-0.0.5/ctd/__init__.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 21:15:04.751706 ctd-python-0.0.5/ctd_python.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 21:15:04.000000 ctd-python-0.0.5/ctd_python.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      203 2023-06-25 21:15:04.000000 ctd-python-0.0.5/ctd_python.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-06-25 21:15:04.000000 ctd-python-0.0.5/ctd_python.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       16 2023-06-25 21:15:04.000000 ctd-python-0.0.5/ctd_python.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        4 2023-06-25 21:15:04.000000 ctd-python-0.0.5/ctd_python.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-06-25 21:15:04.753539 ctd-python-0.0.5/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      498 2023-06-25 21:14:45.000000 ctd-python-0.0.5/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 21:19:25.987390 ctd-python-0.0.6/
+-rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 21:19:25.986341 ctd-python-0.0.6/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      974 2023-06-25 21:03:16.000000 ctd-python-0.0.6/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 21:19:25.979106 ctd-python-0.0.6/ctd/
+-rw-r--r--   0 john       (501) staff       (20)     2396 2023-06-25 21:04:11.000000 ctd-python-0.0.6/ctd/__init__.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-25 21:19:25.984769 ctd-python-0.0.6/ctd_python.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     1604 2023-06-25 21:19:25.000000 ctd-python-0.0.6/ctd_python.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      203 2023-06-25 21:19:25.000000 ctd-python-0.0.6/ctd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-06-25 21:19:25.000000 ctd-python-0.0.6/ctd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       16 2023-06-25 21:19:25.000000 ctd-python-0.0.6/ctd_python.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        4 2023-06-25 21:19:25.000000 ctd-python-0.0.6/ctd_python.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-06-25 21:19:25.987657 ctd-python-0.0.6/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      498 2023-06-25 21:19:16.000000 ctd-python-0.0.6/setup.py
```

### Comparing `ctd-python-0.0.5/PKG-INFO` & `ctd-python-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.0.5/README.md` & `ctd-python-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ctd-python-0.0.5/ctd/__init__.py` & `ctd-python-0.0.6/ctd/__init__.py`

 * *Files identical despite different names*

### Comparing `ctd-python-0.0.5/ctd_python.egg-info/PKG-INFO` & `ctd-python-0.0.6/ctd_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

