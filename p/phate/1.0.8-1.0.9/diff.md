# Comparing `tmp/phate-1.0.8.tar.gz` & `tmp/phate-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PHATE/PHATE/dist/tmph0a89h1r/phate-1.0.8.tar", last modified: Tue Jun 21 19:46:56 2022, max compression
+gzip compressed data, was "/home/runner/work/PHATE/PHATE/dist/tmptq5vfd6e/phate-1.0.9.tar", last modified: Wed Nov  2 14:32:43 2022, max compression
```

## Comparing `phate-1.0.8.tar` & `phate-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 19:46:56.000000 phate-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     5444 2022-06-21 19:46:56.000000 phate-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4186 2022-06-21 19:46:38.000000 phate-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 19:46:56.000000 phate-1.0.8/phate/
--rw-r--r--   0 runner    (1001) docker     (116)      232 2022-06-21 19:46:38.000000 phate-1.0.8/phate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2645 2022-06-21 19:46:38.000000 phate-1.0.8/phate/cluster.py
--rw-r--r--   0 runner    (1001) docker     (116)      413 2022-06-21 19:46:38.000000 phate-1.0.8/phate/io.py
--rw-r--r--   0 runner    (1001) docker     (116)     7429 2022-06-21 19:46:38.000000 phate-1.0.8/phate/mds.py
--rw-r--r--   0 runner    (1001) docker     (116)    39651 2022-06-21 19:46:38.000000 phate-1.0.8/phate/phate.py
--rw-r--r--   0 runner    (1001) docker     (116)    23218 2022-06-21 19:46:38.000000 phate-1.0.8/phate/plot.py
--rw-r--r--   0 runner    (1001) docker     (116)      407 2022-06-21 19:46:38.000000 phate-1.0.8/phate/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (116)     1100 2022-06-21 19:46:38.000000 phate-1.0.8/phate/tree.py
--rw-r--r--   0 runner    (1001) docker     (116)     3067 2022-06-21 19:46:38.000000 phate-1.0.8/phate/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2022-06-21 19:46:38.000000 phate-1.0.8/phate/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     3967 2022-06-21 19:46:38.000000 phate-1.0.8/phate/vne.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 19:46:56.000000 phate-1.0.8/phate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5444 2022-06-21 19:46:55.000000 phate-1.0.8/phate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      356 2022-06-21 19:46:56.000000 phate-1.0.8/phate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-21 19:46:55.000000 phate-1.0.8/phate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      225 2022-06-21 19:46:56.000000 phate-1.0.8/phate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2022-06-21 19:46:56.000000 phate-1.0.8/phate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      135 2022-06-21 19:46:56.000000 phate-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2490 2022-06-21 19:46:38.000000 phate-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 19:46:56.000000 phate-1.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (116)     7057 2022-06-21 19:46:38.000000 phate-1.0.8/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-02 14:32:43.000000 phate-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     5444 2022-11-02 14:32:43.000000 phate-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4186 2022-11-02 14:32:24.000000 phate-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-02 14:32:43.000000 phate-1.0.9/phate/
+-rw-r--r--   0 runner    (1001) docker     (116)      232 2022-11-02 14:32:24.000000 phate-1.0.9/phate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2645 2022-11-02 14:32:24.000000 phate-1.0.9/phate/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (116)      413 2022-11-02 14:32:24.000000 phate-1.0.9/phate/io.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7429 2022-11-02 14:32:24.000000 phate-1.0.9/phate/mds.py
+-rw-r--r--   0 runner    (1001) docker     (116)    39651 2022-11-02 14:32:24.000000 phate-1.0.9/phate/phate.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23218 2022-11-02 14:32:24.000000 phate-1.0.9/phate/plot.py
+-rw-r--r--   0 runner    (1001) docker     (116)      407 2022-11-02 14:32:24.000000 phate-1.0.9/phate/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1100 2022-11-02 14:32:24.000000 phate-1.0.9/phate/tree.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3067 2022-11-02 14:32:24.000000 phate-1.0.9/phate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2022-11-02 14:32:24.000000 phate-1.0.9/phate/version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3967 2022-11-02 14:32:24.000000 phate-1.0.9/phate/vne.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-02 14:32:43.000000 phate-1.0.9/phate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5444 2022-11-02 14:32:43.000000 phate-1.0.9/phate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      356 2022-11-02 14:32:43.000000 phate-1.0.9/phate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-02 14:32:43.000000 phate-1.0.9/phate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      227 2022-11-02 14:32:43.000000 phate-1.0.9/phate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2022-11-02 14:32:43.000000 phate-1.0.9/phate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      135 2022-11-02 14:32:43.000000 phate-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2492 2022-11-02 14:32:24.000000 phate-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-02 14:32:43.000000 phate-1.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (116)     7057 2022-11-02 14:32:24.000000 phate-1.0.9/test/test.py
```

### Comparing `phate-1.0.8/PKG-INFO` & `phate-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: phate
-Version: 1.0.8
+Version: 1.0.9
 Summary: PHATE
 Home-page: https://github.com/KrishnaswamyLab/PHATE
-Download-URL: https://github.com/KrishnaswamyLab/PHATE/archive/v1.0.8.tar.gz
+Download-URL: https://github.com/KrishnaswamyLab/PHATE/archive/v1.0.9.tar.gz
 Author: Daniel Burkhardt, Krishnaswamy Lab, Yale University
 Author-email: daniel.burkhardt@yale.edu
 License: GNU General Public License Version 2
 Keywords: visualization,big-data,dimensionality-reduction,embedding,manifold-learning,computational-biology
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
```

### Comparing `phate-1.0.8/README.md` & `phate-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `phate-1.0.8/phate/cluster.py` & `phate-1.0.9/phate/cluster.py`

 * *Files identical despite different names*

### Comparing `phate-1.0.8/phate/mds.py` & `phate-1.0.9/phate/mds.py`

 * *Files identical despite different names*

### Comparing `phate-1.0.8/phate/phate.py` & `phate-1.0.9/phate/phate.py`

 * *Files identical despite different names*

### Comparing `phate-1.0.8/phate/plot.py` & `phate-1.0.9/phate/plot.py`

 * *Files identical despite different names*

### Comparing `phate-1.0.8/phate/tree.py` & `phate-1.0.9/phate/tree.py`

 * *Files identical despite different names*

### Comparing `phate-1.0.8/phate/utils.py` & `phate-1.0.9/phate/utils.py`

 * *Files identical despite different names*

### Comparing `phate-1.0.8/phate/vne.py` & `phate-1.0.9/phate/vne.py`

 * *Files identical despite different names*

### Comparing `phate-1.0.8/phate.egg-info/PKG-INFO` & `phate-1.0.9/phate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: phate
-Version: 1.0.8
+Version: 1.0.9
 Summary: PHATE
 Home-page: https://github.com/KrishnaswamyLab/PHATE
-Download-URL: https://github.com/KrishnaswamyLab/PHATE/archive/v1.0.8.tar.gz
+Download-URL: https://github.com/KrishnaswamyLab/PHATE/archive/v1.0.9.tar.gz
 Author: Daniel Burkhardt, Krishnaswamy Lab, Yale University
 Author-email: daniel.burkhardt@yale.edu
 License: GNU General Public License Version 2
 Keywords: visualization,big-data,dimensionality-reduction,embedding,manifold-learning,computational-biology
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
```

### Comparing `phate-1.0.8/setup.py` & `phate-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "scipy>=1.1.0",
     "scikit-learn>=0.20.0",
     "future",
     "tasklogger>=1.0",
     "graphtools>=1.3.1",
     "scprep>=0.11.1",
     "Deprecated",
-    "s_gd2>=1.5",
+    "s_gd2>=1.8.1",
 ]
 
 test_requires = ["nose2", "anndata", "coverage", "coveralls", "nose"]
 
 doc_requires = ["sphinx", "sphinxcontrib-napoleon"]
 
 version_py = os.path.join(os.path.dirname(__file__), "phate", "version.py")
```

### Comparing `phate-1.0.8/test/test.py` & `phate-1.0.9/test/test.py`

 * *Files identical despite different names*

