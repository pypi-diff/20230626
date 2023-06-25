# Comparing `tmp/cdxbasics-0.2.8.tar.gz` & `tmp/cdxbasics-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cdxbasics-0.2.8.tar", last modified: Sun Jan  8 00:20:27 2023, max compression
+gzip compressed data, was "dist\cdxbasics-0.2.9.tar", last modified: Sun Jan  8 01:33:00 2023, max compression
```

## Comparing `cdxbasics-0.2.8.tar` & `cdxbasics-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/
--rw-rw-rw-   0        0        0     1089 2020-04-03 15:27:00.000000 cdxbasics-0.2.8/LICENSE
--rw-rw-rw-   0        0        0    29059 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    28623 2023-01-07 22:43:10.000000 cdxbasics-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/cdxbasics/
--rw-rw-rw-   0        0        0      235 2023-01-08 00:20:26.000000 cdxbasics-0.2.8/cdxbasics/__init__.py
--rw-rw-rw-   0        0        0    38585 2023-01-07 21:39:08.000000 cdxbasics-0.2.8/cdxbasics/config.py
--rw-rw-rw-   0        0        0    17138 2023-01-07 20:02:18.000000 cdxbasics-0.2.8/cdxbasics/dynaplot.py
--rw-rw-rw-   0        0        0     4353 2022-07-02 07:27:54.000000 cdxbasics-0.2.8/cdxbasics/kwargs.py
--rw-rw-rw-   0        0        0    11272 2023-01-02 20:03:55.000000 cdxbasics-0.2.8/cdxbasics/logger.py
--rw-rw-rw-   0        0        0     6147 2023-01-02 23:00:09.000000 cdxbasics-0.2.8/cdxbasics/prettydict.py
--rw-rw-rw-   0        0        0    38228 2023-01-07 23:37:51.000000 cdxbasics-0.2.8/cdxbasics/subdir.py
--rw-rw-rw-   0        0        0    15726 2023-01-08 00:19:02.000000 cdxbasics-0.2.8/cdxbasics/util.py
--rw-rw-rw-   0        0        0     9524 2023-01-02 20:03:55.000000 cdxbasics-0.2.8/cdxbasics/verbose.py
-drwxrwxrwx   0        0        0        0 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/cdxbasics.egg-info/
--rw-rw-rw-   0        0        0    29059 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/cdxbasics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/cdxbasics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/cdxbasics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/cdxbasics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/cdxbasics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-08 00:20:27.000000 cdxbasics-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1800 2023-01-04 20:41:04.000000 cdxbasics-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-08 01:33:00.000000 cdxbasics-0.2.9/
+-rw-rw-rw-   0        0        0     1089 2020-04-03 15:27:00.000000 cdxbasics-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0    29059 2023-01-08 01:33:00.000000 cdxbasics-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    28623 2023-01-07 22:43:10.000000 cdxbasics-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-08 01:33:00.000000 cdxbasics-0.2.9/cdxbasics/
+-rw-rw-rw-   0        0        0      235 2023-01-08 01:32:58.000000 cdxbasics-0.2.9/cdxbasics/__init__.py
+-rw-rw-rw-   0        0        0    38585 2023-01-08 00:42:45.000000 cdxbasics-0.2.9/cdxbasics/config.py
+-rw-rw-rw-   0        0        0    17138 2023-01-07 20:02:18.000000 cdxbasics-0.2.9/cdxbasics/dynaplot.py
+-rw-rw-rw-   0        0        0     4353 2022-07-02 07:27:54.000000 cdxbasics-0.2.9/cdxbasics/kwargs.py
+-rw-rw-rw-   0        0        0    11272 2023-01-02 20:03:55.000000 cdxbasics-0.2.9/cdxbasics/logger.py
+-rw-rw-rw-   0        0        0     6147 2023-01-02 23:00:09.000000 cdxbasics-0.2.9/cdxbasics/prettydict.py
+-rw-rw-rw-   0        0        0    38228 2023-01-07 23:37:51.000000 cdxbasics-0.2.9/cdxbasics/subdir.py
+-rw-rw-rw-   0        0        0    15719 2023-01-08 01:26:24.000000 cdxbasics-0.2.9/cdxbasics/util.py
+-rw-rw-rw-   0        0        0     9524 2023-01-02 20:03:55.000000 cdxbasics-0.2.9/cdxbasics/verbose.py
+drwxrwxrwx   0        0        0        0 2023-01-08 01:33:00.000000 cdxbasics-0.2.9/cdxbasics.egg-info/
+-rw-rw-rw-   0        0        0    29059 2023-01-08 01:32:59.000000 cdxbasics-0.2.9/cdxbasics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-01-08 01:33:00.000000 cdxbasics-0.2.9/cdxbasics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-08 01:32:59.000000 cdxbasics-0.2.9/cdxbasics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-01-08 01:32:59.000000 cdxbasics-0.2.9/cdxbasics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-01-08 01:32:59.000000 cdxbasics-0.2.9/cdxbasics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-08 01:33:00.000000 cdxbasics-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1800 2023-01-04 20:41:04.000000 cdxbasics-0.2.9/setup.py
```

### Comparing `cdxbasics-0.2.8/LICENSE` & `cdxbasics-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.8/PKG-INFO` & `cdxbasics-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdxbasics
-Version: 0.2.8
+Version: 0.2.9
 Summary: Basic Python tools
 Home-page: https://github.com/hansbuehler/cdxbasics
 Author: Hans Buehler
 Author-email: github@buehler.london
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cdxbasics-0.2.8/README.md` & `cdxbasics-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.8/cdxbasics/config.py` & `cdxbasics-0.2.9/cdxbasics/config.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.8/cdxbasics/dynaplot.py` & `cdxbasics-0.2.9/cdxbasics/dynaplot.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.8/cdxbasics/kwargs.py` & `cdxbasics-0.2.9/cdxbasics/kwargs.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.8/cdxbasics/logger.py` & `cdxbasics-0.2.9/cdxbasics/logger.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.8/cdxbasics/prettydict.py` & `cdxbasics-0.2.9/cdxbasics/prettydict.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.8/cdxbasics/subdir.py` & `cdxbasics-0.2.9/cdxbasics/subdir.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.8/cdxbasics/util.py` & `cdxbasics-0.2.9/cdxbasics/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,23 +80,23 @@
     """ Checks whether 'f' is a function in an extended sense. Check 'types_functions' for what is tested against"""
     return isinstance(f,types_functions())
 
 def isAtomic( o ):
     """ Returns true if 'o' is a string, int, float, date or bool """
     if type(o) in [str,int,bool,float,datetime.date]:
         return True
-    if not np is None and isinstance(o,(np.float_,np.int_)):
+    if not np is None and isinstance(o,np.generic):
         return True
     return False
 
 def isFloat( o ):
     """ Checks whether a type is a float """
     if type(o) is float:
         return True
-    if not np is None and isinstance(o,np.float_):
+    if not np is None and isinstance(o,np.floating):
         return True
     return False
 
 # =============================================================================
 # string formatting
 # =============================================================================
```

### Comparing `cdxbasics-0.2.8/cdxbasics/verbose.py` & `cdxbasics-0.2.9/cdxbasics/verbose.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.8/cdxbasics.egg-info/PKG-INFO` & `cdxbasics-0.2.9/cdxbasics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdxbasics
-Version: 0.2.8
+Version: 0.2.9
 Summary: Basic Python tools
 Home-page: https://github.com/hansbuehler/cdxbasics
 Author: Hans Buehler
 Author-email: github@buehler.london
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cdxbasics-0.2.8/setup.py` & `cdxbasics-0.2.9/setup.py`

 * *Files identical despite different names*

