# Comparing `tmp/atlaspy-0.0.8.tar.gz` & `tmp/atlaspy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlaspy-0.0.8.tar", last modified: Fri Jun 23 21:15:03 2023, max compression
+gzip compressed data, was "atlaspy-0.0.9.tar", last modified: Fri Jun 23 21:24:47 2023, max compression
```

## Comparing `atlaspy-0.0.8.tar` & `atlaspy-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:15:03.227590 atlaspy-0.0.8/
--rw-r--r--   0 allucas    (501) staff       (20)       40 2023-06-23 20:00:41.000000 atlaspy-0.0.8/MANIFEST.in
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 21:15:03.227451 atlaspy-0.0.8/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)     1988 2023-06-23 02:28:30.000000 atlaspy-0.0.8/README.md
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:15:03.216434 atlaspy-0.0.8/atlaspy/
--rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.8/atlaspy/__init__.py
--rw-r--r--   0 allucas    (501) staff       (20)    30454 2023-06-23 20:11:36.000000 atlaspy-0.0.8/atlaspy/core.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:15:03.217280 atlaspy-0.0.8/atlaspy/source_data/
--rwxrwxr-x   0 allucas    (501) staff       (20)     8196 2023-06-23 02:01:21.000000 atlaspy-0.0.8/atlaspy/source_data/.DS_Store
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:15:03.217560 atlaspy-0.0.8/atlaspy/source_data/atlases/
--rwxrwxr-x   0 allucas    (501) staff       (20)    10244 2023-06-23 18:03:18.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/.DS_Store
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:15:03.219370 atlaspy-0.0.8/atlaspy/source_data/atlases/luts/
--rw-r--r--   0 allucas    (501) staff       (20)     6148 2023-06-22 23:19:38.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/luts/.DS_Store
--rw-r--r--   0 allucas    (501) staff       (20)     2382 2023-06-22 23:19:38.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/luts/aal.csv
--rw-r--r--   0 allucas    (501) staff       (20)     3635 2023-06-23 18:01:47.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/luts/bna.csv
--rw-r--r--   0 allucas    (501) staff       (20)     3132 2023-06-23 02:00:02.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/luts/dkt.csv
--rw-r--r--   0 allucas    (501) staff       (20)     3497 2023-06-23 17:56:10.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/luts/ho.csv
--rw-r--r--   0 allucas    (501) staff       (20)     8374 2023-06-23 17:58:25.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/luts/sch400.csv
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:15:03.226654 atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/
--rw-r--r--   0 allucas    (501) staff       (20)     6148 2023-06-23 17:32:07.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/.DS_Store
--rwxr-xr-x   0 allucas    (501) staff       (20)   197670 2023-06-23 17:46:28.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/aal.nii.gz
--rwxrwxr-x   0 allucas    (501) staff       (20)   176321 2021-10-29 17:28:35.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/bna.nii.gz
--rwxrwxr-x   0 allucas    (501) staff       (20)   359072 2023-06-23 17:32:12.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/dkt.nii.gz
--rwxr-xr-x   0 allucas    (501) staff       (20)   183758 2023-06-23 17:34:18.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/ho.nii.gz
--rw-rw-r--   0 allucas    (501) staff       (20)   213076 2023-06-23 17:35:27.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/sch400.nii.gz
--rwxrwxr-x   0 allucas    (501) staff       (20)   373298 2023-06-23 17:32:54.000000 atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/vep.nii.gz
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:15:03.217146 atlaspy-0.0.8/atlaspy.egg-info/
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 21:15:03.000000 atlaspy-0.0.8/atlaspy.egg-info/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      861 2023-06-23 21:15:03.000000 atlaspy-0.0.8/atlaspy.egg-info/SOURCES.txt
--rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-23 21:15:03.000000 atlaspy-0.0.8/atlaspy.egg-info/dependency_links.txt
--rw-r--r--   0 allucas    (501) staff       (20)       50 2023-06-23 21:15:03.000000 atlaspy-0.0.8/atlaspy.egg-info/requires.txt
--rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-23 21:15:03.000000 atlaspy-0.0.8/atlaspy.egg-info/top_level.txt
--rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-23 21:15:03.227628 atlaspy-0.0.8/setup.cfg
--rw-r--r--   0 allucas    (501) staff       (20)     2197 2023-06-23 21:13:40.000000 atlaspy-0.0.8/setup.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:24:47.994446 atlaspy-0.0.9/
+-rw-r--r--   0 allucas    (501) staff       (20)       40 2023-06-23 20:00:41.000000 atlaspy-0.0.9/MANIFEST.in
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 21:24:47.994288 atlaspy-0.0.9/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)     1988 2023-06-23 02:28:30.000000 atlaspy-0.0.9/README.md
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:24:47.989581 atlaspy-0.0.9/atlaspy/
+-rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.9/atlaspy/__init__.py
+-rw-r--r--   0 allucas    (501) staff       (20)    30454 2023-06-23 20:11:36.000000 atlaspy-0.0.9/atlaspy/core.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:24:47.990431 atlaspy-0.0.9/atlaspy/source_data/
+-rwxrwxr-x   0 allucas    (501) staff       (20)     8196 2023-06-23 02:01:21.000000 atlaspy-0.0.9/atlaspy/source_data/.DS_Store
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:24:47.990773 atlaspy-0.0.9/atlaspy/source_data/atlases/
+-rwxrwxr-x   0 allucas    (501) staff       (20)    10244 2023-06-23 18:03:18.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/.DS_Store
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:24:47.991971 atlaspy-0.0.9/atlaspy/source_data/atlases/luts/
+-rw-r--r--   0 allucas    (501) staff       (20)     6148 2023-06-22 23:19:38.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/luts/.DS_Store
+-rw-r--r--   0 allucas    (501) staff       (20)     2382 2023-06-22 23:19:38.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/luts/aal.csv
+-rw-r--r--   0 allucas    (501) staff       (20)     3635 2023-06-23 18:01:47.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/luts/bna.csv
+-rw-r--r--   0 allucas    (501) staff       (20)     3132 2023-06-23 02:00:02.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/luts/dkt.csv
+-rw-r--r--   0 allucas    (501) staff       (20)     3497 2023-06-23 17:56:10.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/luts/ho.csv
+-rw-r--r--   0 allucas    (501) staff       (20)     8374 2023-06-23 17:58:25.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/luts/sch400.csv
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:24:47.993878 atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/
+-rw-r--r--   0 allucas    (501) staff       (20)     6148 2023-06-23 17:32:07.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/.DS_Store
+-rwxr-xr-x   0 allucas    (501) staff       (20)   197670 2023-06-23 17:46:28.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/aal.nii.gz
+-rwxrwxr-x   0 allucas    (501) staff       (20)   176321 2021-10-29 17:28:35.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/bna.nii.gz
+-rwxrwxr-x   0 allucas    (501) staff       (20)   359072 2023-06-23 17:32:12.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/dkt.nii.gz
+-rwxr-xr-x   0 allucas    (501) staff       (20)   183758 2023-06-23 17:34:18.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/ho.nii.gz
+-rw-rw-r--   0 allucas    (501) staff       (20)   213076 2023-06-23 17:35:27.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/sch400.nii.gz
+-rwxrwxr-x   0 allucas    (501) staff       (20)   373298 2023-06-23 17:32:54.000000 atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/vep.nii.gz
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-23 21:24:47.990288 atlaspy-0.0.9/atlaspy.egg-info/
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-23 21:24:47.000000 atlaspy-0.0.9/atlaspy.egg-info/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      861 2023-06-23 21:24:47.000000 atlaspy-0.0.9/atlaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-23 21:24:47.000000 atlaspy-0.0.9/atlaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       50 2023-06-23 21:24:47.000000 atlaspy-0.0.9/atlaspy.egg-info/requires.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-23 21:24:47.000000 atlaspy-0.0.9/atlaspy.egg-info/top_level.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-23 21:24:47.994512 atlaspy-0.0.9/setup.cfg
+-rw-r--r--   0 allucas    (501) staff       (20)     2197 2023-06-23 21:24:14.000000 atlaspy-0.0.9/setup.py
```

### Comparing `atlaspy-0.0.8/README.md` & `atlaspy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/core.py` & `atlaspy-0.0.9/atlaspy/core.py`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/.DS_Store` & `atlaspy-0.0.9/atlaspy/source_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/.DS_Store` & `atlaspy-0.0.9/atlaspy/source_data/atlases/.DS_Store`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/luts/.DS_Store` & `atlaspy-0.0.9/atlaspy/source_data/atlases/luts/.DS_Store`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/luts/aal.csv` & `atlaspy-0.0.9/atlaspy/source_data/atlases/luts/aal.csv`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/luts/bna.csv` & `atlaspy-0.0.9/atlaspy/source_data/atlases/luts/bna.csv`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/luts/dkt.csv` & `atlaspy-0.0.9/atlaspy/source_data/atlases/luts/dkt.csv`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/luts/ho.csv` & `atlaspy-0.0.9/atlaspy/source_data/atlases/luts/ho.csv`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/luts/sch400.csv` & `atlaspy-0.0.9/atlaspy/source_data/atlases/luts/sch400.csv`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/.DS_Store` & `atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/.DS_Store`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/aal.nii.gz` & `atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/aal.nii.gz`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/bna.nii.gz` & `atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/bna.nii.gz`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/dkt.nii.gz` & `atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/dkt.nii.gz`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/ho.nii.gz` & `atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/ho.nii.gz`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/sch400.nii.gz` & `atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/sch400.nii.gz`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy/source_data/atlases/niftis/vep.nii.gz` & `atlaspy-0.0.9/atlaspy/source_data/atlases/niftis/vep.nii.gz`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/atlaspy.egg-info/SOURCES.txt` & `atlaspy-0.0.9/atlaspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlaspy-0.0.8/setup.py` & `atlaspy-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # Modify the data install dir to match the source install dir
 for scheme in INSTALL_SCHEMES.values():
     scheme['data'] = scheme['purelib']
 
 
 setup(
     name='atlaspy',
-    version='0.0.8',
+    version='0.0.9',
     description='Python library for working with brain atlases',
     author='Alfredo Lucas',
     author_email='alfredo1238@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     package_data={'atlaspy.source_data': ["*"]},
```

