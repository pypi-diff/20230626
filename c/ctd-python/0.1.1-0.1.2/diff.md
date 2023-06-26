# Comparing `tmp/ctd-python-0.1.1.tar.gz` & `tmp/ctd-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctd-python-0.1.1.tar", last modified: Mon Jun 26 01:50:56 2023, max compression
+gzip compressed data, was "ctd-python-0.1.2.tar", last modified: Mon Jun 26 01:55:21 2023, max compression
```

## Comparing `ctd-python-0.1.1.tar` & `ctd-python-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:50:56.654168 ctd-python-0.1.1/
--rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 01:50:56.653684 ctd-python-0.1.1/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      887 2023-06-26 01:02:36.000000 ctd-python-0.1.1/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:50:56.645205 ctd-python-0.1.1/ctd/
--rw-r--r--   0 john       (501) staff       (20)       31 2023-06-26 00:20:15.000000 ctd-python-0.1.1/ctd/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     3384 2023-06-26 01:48:32.000000 ctd-python-0.1.1/ctd/get_data.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:50:56.648832 ctd-python-0.1.1/ctd/unzipped_data/
--rw-r--r--   0 john       (501) staff       (20)        0 2023-06-25 23:36:26.000000 ctd-python-0.1.1/ctd/unzipped_data/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     1072 2023-06-26 00:49:30.000000 ctd-python-0.1.1/ctd/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:50:56.653111 ctd-python-0.1.1/ctd_python.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 01:50:56.000000 ctd-python-0.1.1/ctd_python.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      262 2023-06-26 01:50:56.000000 ctd-python-0.1.1/ctd_python.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-06-26 01:50:56.000000 ctd-python-0.1.1/ctd_python.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       21 2023-06-26 01:50:56.000000 ctd-python-0.1.1/ctd_python.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        4 2023-06-26 01:50:56.000000 ctd-python-0.1.1/ctd_python.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-06-26 01:50:56.654459 ctd-python-0.1.1/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      544 2023-06-26 01:50:36.000000 ctd-python-0.1.1/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:55:21.564485 ctd-python-0.1.2/
+-rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 01:55:21.563845 ctd-python-0.1.2/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      887 2023-06-26 01:02:36.000000 ctd-python-0.1.2/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:55:21.555886 ctd-python-0.1.2/ctd/
+-rw-r--r--   0 john       (501) staff       (20)       31 2023-06-26 00:20:15.000000 ctd-python-0.1.2/ctd/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     3379 2023-06-26 01:55:04.000000 ctd-python-0.1.2/ctd/get_data.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:55:21.557504 ctd-python-0.1.2/ctd/unzipped_data/
+-rw-r--r--   0 john       (501) staff       (20)        0 2023-06-25 23:36:26.000000 ctd-python-0.1.2/ctd/unzipped_data/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     1072 2023-06-26 00:49:30.000000 ctd-python-0.1.2/ctd/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 01:55:21.563220 ctd-python-0.1.2/ctd_python.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      262 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       21 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        4 2023-06-26 01:55:21.000000 ctd-python-0.1.2/ctd_python.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-06-26 01:55:21.564628 ctd-python-0.1.2/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      544 2023-06-26 01:55:19.000000 ctd-python-0.1.2/setup.py
```

### Comparing `ctd-python-0.1.1/PKG-INFO` & `ctd-python-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.1.1/README.md` & `ctd-python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ctd-python-0.1.1/ctd/get_data.py` & `ctd-python-0.1.2/ctd/get_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     resource_name = RESOURCES.get(resource)
     if not resource_name:
         raise Exception(f"The resource '{resource}' is not available. Please check https://ctdbase.org/downloads/ for available resources.")
 
     download_resource(resource_name)
 
     line_number = 27  # files have the same header, TODO need to make dynamic
-    the_file = os.path.join(UNZIPPED_DATA_DIR, f"{resource_name}.csv")
+    the_file = os.path.join(RAW_DATA_DIR, f"{resource_name}.csv")
 
     with open(the_file, 'r') as reader:
         for i, row in enumerate(reader):
             if i == line_number:
                 header = row.replace("# ", "").split(",")
 
     df = pd.read_csv(the_file, skiprows=29, names=header)
```

### Comparing `ctd-python-0.1.1/ctd/utils.py` & `ctd-python-0.1.2/ctd/utils.py`

 * *Files identical despite different names*

### Comparing `ctd-python-0.1.1/ctd_python.egg-info/PKG-INFO` & `ctd-python-0.1.2/ctd_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.1.1/setup.py` & `ctd-python-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='ctd-python',
-    version='0.1.1',
+    version='0.1.2',
     description='Python interface to access data from The Comparative Toxicogenomics Database (CTD)',
     packages=['ctd'],
     install_requires=[
         'requests',
         'pandas',
         'tqdm'
     ],
```

