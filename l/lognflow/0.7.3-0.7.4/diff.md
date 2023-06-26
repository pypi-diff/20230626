# Comparing `tmp/lognflow-0.7.3.tar.gz` & `tmp/lognflow-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.7.3.tar", last modified: Fri Jun 23 13:30:36 2023, max compression
+gzip compressed data, was "lognflow-0.7.4.tar", last modified: Mon Jun 26 01:03:26 2023, max compression
```

## Comparing `lognflow-0.7.3.tar` & `lognflow-0.7.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:30:36.102231 lognflow-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-23 13:30:21.000000 lognflow-0.7.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-23 13:30:21.000000 lognflow-0.7.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-23 13:30:21.000000 lognflow-0.7.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-23 13:30:21.000000 lognflow-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-23 13:30:21.000000 lognflow-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-23 13:30:36.102231 lognflow-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-23 13:30:21.000000 lognflow-0.7.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:30:36.102231 lognflow-0.7.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 13:30:21.000000 lognflow-0.7.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:30:36.102231 lognflow-0.7.3/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-23 13:30:21.000000 lognflow-0.7.3/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65631 2023-06-23 13:30:21.000000 lognflow-0.7.3/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-06-23 13:30:21.000000 lognflow-0.7.3/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-23 13:30:21.000000 lognflow-0.7.3/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:30:36.102231 lognflow-0.7.3/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-23 13:30:36.000000 lognflow-0.7.3/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-23 13:30:36.000000 lognflow-0.7.3/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:30:36.000000 lognflow-0.7.3/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:30:35.000000 lognflow-0.7.3/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 13:30:36.000000 lognflow-0.7.3/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 13:30:36.000000 lognflow-0.7.3/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-23 13:30:36.102231 lognflow-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-23 13:30:21.000000 lognflow-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:30:36.102231 lognflow-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 13:30:21.000000 lognflow-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-06-23 13:30:21.000000 lognflow-0.7.3/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-23 13:30:21.000000 lognflow-0.7.3/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 13:30:21.000000 lognflow-0.7.3/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 01:03:16.000000 lognflow-0.7.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-26 01:03:16.000000 lognflow-0.7.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-26 01:03:16.000000 lognflow-0.7.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-26 01:03:16.000000 lognflow-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 01:03:16.000000 lognflow-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-26 01:03:26.865371 lognflow-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-26 01:03:16.000000 lognflow-0.7.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 01:03:16.000000 lognflow-0.7.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 01:03:16.000000 lognflow-0.7.4/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65639 2023-06-26 01:03:16.000000 lognflow-0.7.4/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-06-26 01:03:16.000000 lognflow-0.7.4/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-26 01:03:16.000000 lognflow-0.7.4/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 01:03:26.000000 lognflow-0.7.4/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-26 01:03:26.869371 lognflow-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-26 01:03:16.000000 lognflow-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:03:26.865371 lognflow-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 01:03:16.000000 lognflow-0.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-06-26 01:03:16.000000 lognflow-0.7.4/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-26 01:03:16.000000 lognflow-0.7.4/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 01:03:16.000000 lognflow-0.7.4/tests/test_printprogress.py
```

### Comparing `lognflow-0.7.3/CONTRIBUTING.rst` & `lognflow-0.7.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/HISTORY.rst` & `lognflow-0.7.4/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -96,8 +96,12 @@
 * text_to_object added to logviewer to read dict or list logged via log_single
 * test pass for logviewer including the test for text_to_object
 
 0.7.3 (2023-06-01)
 ------------------
 * bug fixed in logviewer in the use of suffix in get_stack_of_files
 * log_imshow takes colorbar and remove_axis_ticks flags.
-* every lognflow instance has a logviewer pointing to its log_dir called logged.
+* every lognflow instance has a logviewer pointing to its log_dir called logged.
+
+0.7.4 (2023-06-26)
+------------------
+* critical bug fixed in log_imshow
```

### Comparing `lognflow-0.7.3/LICENSE` & `lognflow-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/PKG-INFO` & `lognflow-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.3
+Version: 0.7.4
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -190,7 +190,11 @@
 * test pass for logviewer including the test for text_to_object
 
 0.7.3 (2023-06-01)
 ------------------
 * bug fixed in logviewer in the use of suffix in get_stack_of_files
 * log_imshow takes colorbar and remove_axis_ticks flags.
 * every lognflow instance has a logviewer pointing to its log_dir called logged.
+
+0.7.4 (2023-06-26)
+------------------
+* critical bug fixed in log_imshow
```

### Comparing `lognflow-0.7.3/README.rst` & `lognflow-0.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/docs/Makefile` & `lognflow-0.7.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/docs/conf.py` & `lognflow-0.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/docs/installation.rst` & `lognflow-0.7.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/docs/make.bat` & `lognflow-0.7.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/lognflow/lognflow.py` & `lognflow-0.7.4/lognflow/lognflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -988,17 +988,17 @@
                 use_multichannel_to_square = True
         
         if(use_multichannel_to_square):
             parameter_value = self. multichannel_to_square(
                 parameter_value, borders = borders)
         if(FLAG_img_ready):
             fig, ax = plt.subplots()
-            ax.imshow(parameter_value, cmap = cmap, **kwargs)
+            im = ax.imshow(parameter_value, cmap = cmap, **kwargs)
             if(colorbar):
-                ax.colorbar()
+                plt.colorbar(im)
             if(remove_axis_ticks):
                 plt.setp(ax, xticks=[], yticks=[])
             fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
             return fpath
```

### Comparing `lognflow-0.7.3/lognflow/logviewer.py` & `lognflow-0.7.4/lognflow/logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/lognflow/printprogress.py` & `lognflow-0.7.4/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/lognflow.egg-info/PKG-INFO` & `lognflow-0.7.4/lognflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.3
+Version: 0.7.4
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -190,7 +190,11 @@
 * test pass for logviewer including the test for text_to_object
 
 0.7.3 (2023-06-01)
 ------------------
 * bug fixed in logviewer in the use of suffix in get_stack_of_files
 * log_imshow takes colorbar and remove_axis_ticks flags.
 * every lognflow instance has a logviewer pointing to its log_dir called logged.
+
+0.7.4 (2023-06-26)
+------------------
+* critical bug fixed in log_imshow
```

### Comparing `lognflow-0.7.3/lognflow.egg-info/SOURCES.txt` & `lognflow-0.7.4/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/setup.py` & `lognflow-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.7.3'
+__version__ = '0.7.4'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.7.3/tests/test_lognflow.py` & `lognflow-0.7.4/tests/test_lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/tests/test_logviewer.py` & `lognflow-0.7.4/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.3/tests/test_printprogress.py` & `lognflow-0.7.4/tests/test_printprogress.py`

 * *Files identical despite different names*

