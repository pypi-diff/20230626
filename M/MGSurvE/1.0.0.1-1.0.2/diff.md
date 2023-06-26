# Comparing `tmp/MGSurvE-1.0.0.1.tar.gz` & `tmp/MGSurvE-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-1.0.0.1.tar", last modified: Mon Jun 26 18:36:57 2023, max compression
+gzip compressed data, was "MGSurvE-1.0.2.tar", last modified: Mon Jun 26 20:07:56 2023, max compression
```

## Comparing `MGSurvE-1.0.0.1.tar` & `MGSurvE-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-26 18:36:57.604495 MGSurvE-1.0.0.1/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/LICENSE
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-26 18:36:57.603510 MGSurvE-1.0.0.1/MGSurvE/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       23 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.0.1/MGSurvE/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.0.1/MGSurvE/kernels.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21376 2023-06-08 23:51:28.000000 MGSurvE-1.0.0.1/MGSurvE/landscape.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/matrices.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/network.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/optimization.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.0.1/MGSurvE/optimizationPSO.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18240 2023-06-26 18:31:03.000000 MGSurvE-1.0.0.1/MGSurvE/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/pointProcess.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-26 18:36:57.604180 MGSurvE-1.0.0.1/MGSurvE.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4619 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      221 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4619 2023-06-26 18:36:57.604371 MGSurvE-1.0.0.1/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4185 2023-06-22 17:37:58.000000 MGSurvE-1.0.0.1/README.md
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-06-26 18:36:57.604561 MGSurvE-1.0.0.1/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-06-08 23:51:28.000000 MGSurvE-1.0.0.1/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-26 20:07:56.144384 MGSurvE-1.0.2/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.2/LICENSE
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-26 20:07:56.142984 MGSurvE-1.0.2/MGSurvE/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.2/MGSurvE/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-06-26 20:07:55.000000 MGSurvE-1.0.2/MGSurvE/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.2/MGSurvE/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.2/MGSurvE/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-05-11 16:34:41.000000 MGSurvE-1.0.2/MGSurvE/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.2/MGSurvE/kernels.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21376 2023-06-08 23:51:28.000000 MGSurvE-1.0.2/MGSurvE/landscape.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.2/MGSurvE/matrices.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.2/MGSurvE/network.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-1.0.2/MGSurvE/optimization.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.2/MGSurvE/optimizationPSO.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18240 2023-06-26 18:31:03.000000 MGSurvE-1.0.2/MGSurvE/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.2/MGSurvE/pointProcess.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-26 20:07:56.143984 MGSurvE-1.0.2/MGSurvE.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4617 2023-06-26 20:07:56.000000 MGSurvE-1.0.2/MGSurvE.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-06-26 20:07:56.000000 MGSurvE-1.0.2/MGSurvE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-06-26 20:07:56.000000 MGSurvE-1.0.2/MGSurvE.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      221 2023-06-26 20:07:56.000000 MGSurvE-1.0.2/MGSurvE.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-06-26 20:07:56.000000 MGSurvE-1.0.2/MGSurvE.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4617 2023-06-26 20:07:56.144235 MGSurvE-1.0.2/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4185 2023-06-22 17:37:58.000000 MGSurvE-1.0.2/README.md
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-06-26 20:07:56.144444 MGSurvE-1.0.2/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-06-08 23:51:28.000000 MGSurvE-1.0.2/setup.py
```

### Comparing `MGSurvE-1.0.0.1/LICENSE` & `MGSurvE-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/auxiliary.py` & `MGSurvE-1.0.2/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/colors.py` & `MGSurvE-1.0.2/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/constants.py` & `MGSurvE-1.0.2/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/kernels.py` & `MGSurvE-1.0.2/MGSurvE/kernels.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/landscape.py` & `MGSurvE-1.0.2/MGSurvE/landscape.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/matrices.py` & `MGSurvE-1.0.2/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/network.py` & `MGSurvE-1.0.2/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/optimization.py` & `MGSurvE-1.0.2/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/optimizationPSO.py` & `MGSurvE-1.0.2/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/plots.py` & `MGSurvE-1.0.2/MGSurvE/plots.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE/pointProcess.py` & `MGSurvE-1.0.2/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-1.0.2/MGSurvE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.0.1
+Version: 1.0.2
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-1.0.0.1/PKG-INFO` & `MGSurvE-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.0.1
+Version: 1.0.2
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-1.0.0.1/README.md` & `MGSurvE-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.1/setup.py` & `MGSurvE-1.0.2/setup.py`

 * *Files identical despite different names*

