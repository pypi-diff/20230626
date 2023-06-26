# Comparing `tmp/waffle_utils-0.3.0.tar.gz` & `tmp/waffle_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_utils-0.3.0.tar", last modified: Mon Apr 17 10:32:15 2023, max compression
+gzip compressed data, was "waffle_utils-0.3.1.tar", last modified: Mon Jun 26 08:44:01 2023, max compression
```

## Comparing `waffle_utils-0.3.0.tar` & `waffle_utils-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      140 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1398 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      323 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       90 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2667 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2466 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/tests/test_cli.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       22 2023-04-17 10:30:16.000000 waffle_utils-0.3.0/waffle_utils/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/file/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/file/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4706 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/file/io.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      475 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/file/network.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3242 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/file/search.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/image/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      130 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/image/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      332 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/image/io.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/log/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      120 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/log/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1701 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/log/template.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      238 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/log/time.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3295 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       69 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      435 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/utils/validators.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/video/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1089 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/video/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1991 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/video/io.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4682 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/video/tools.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/visualize/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      105 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/visualize/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10198 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/visualize/plot.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1398 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      792 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       97 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       13 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      140 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1398 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      323 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       90 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2667 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2466 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/tests/test_cli.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/waffle_utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       22 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/waffle_utils/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/waffle_utils/file/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/waffle_utils/file/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4706 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/waffle_utils/file/io.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      475 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/waffle_utils/file/network.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3242 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/waffle_utils/file/search.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/waffle_utils/image/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      130 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/waffle_utils/image/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      332 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/waffle_utils/image/io.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/waffle_utils/log/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      120 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/waffle_utils/log/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1701 2023-03-28 04:12:00.000000 waffle_utils-0.3.1/waffle_utils/log/template.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      238 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/waffle_utils/log/time.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3295 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/waffle_utils/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/waffle_utils/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       69 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/waffle_utils/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      435 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/waffle_utils/utils/validators.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/waffle_utils/video/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1089 2023-03-20 23:39:58.000000 waffle_utils-0.3.1/waffle_utils/video/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1991 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/waffle_utils/video/io.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4682 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/waffle_utils/video/tools.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/waffle_utils/visualize/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      105 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/waffle_utils/visualize/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10346 2023-06-26 08:43:41.000000 waffle_utils-0.3.1/waffle_utils/visualize/plot.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-26 08:44:01.624640 waffle_utils-0.3.1/waffle_utils.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1398 2023-06-26 08:44:01.000000 waffle_utils-0.3.1/waffle_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      792 2023-06-26 08:44:01.000000 waffle_utils-0.3.1/waffle_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-06-26 08:44:01.000000 waffle_utils-0.3.1/waffle_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-06-26 08:44:01.000000 waffle_utils-0.3.1/waffle_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       97 2023-06-26 08:44:01.000000 waffle_utils-0.3.1/waffle_utils.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       13 2023-06-26 08:44:01.000000 waffle_utils-0.3.1/waffle_utils.egg-info/top_level.txt
```

### Comparing `waffle_utils-0.3.0/PKG-INFO` & `waffle_utils-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Waffle Utils 🥛
 Home-page: https://github.com/snuailab/waffle_utils
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_utils/issues
 Project-URL: Source, https://github.com/snuailab/waffle_utils
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_utils Version: 0.3.0 Summary: Waffle Utils
+Metadata-Version: 2.1 Name: waffle_utils Version: 0.3.1 Summary: Waffle Utils
 ð¥ Home-page: https://github.com/snuailab/waffle_utils Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports,
 https://github.com/snuailab/waffle_utils/issues Project-URL: Source, https://
 github.com/snuailab/waffle_utils Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_utils-0.3.0/setup.py` & `waffle_utils-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.3.0/tests/test_cli.py` & `waffle_utils-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.3.0/waffle_utils/file/io.py` & `waffle_utils-0.3.1/waffle_utils/file/io.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.3.0/waffle_utils/file/search.py` & `waffle_utils-0.3.1/waffle_utils/file/search.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.3.0/waffle_utils/log/template.py` & `waffle_utils-0.3.1/waffle_utils/log/template.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.3.0/waffle_utils/run.py` & `waffle_utils-0.3.1/waffle_utils/run.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.3.0/waffle_utils/video/__init__.py` & `waffle_utils-0.3.1/waffle_utils/video/__init__.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.3.0/waffle_utils/video/io.py` & `waffle_utils-0.3.1/waffle_utils/video/io.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.3.0/waffle_utils/video/tools.py` & `waffle_utils-0.3.1/waffle_utils/video/tools.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.3.0/waffle_utils/visualize/plot.py` & `waffle_utils-0.3.1/waffle_utils/visualize/plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,48 +4,51 @@
 from matplotlib import pyplot as plt
 
 # random 1000 colors with large variance to distinguish between continuous categories
 colors = np.random.rand(1000, 3)
 
 
 def _plot_scatter_1d(
-    datas: np.ndarray, categories: np.ndarray, ax: plt.Axes
+    datas: np.ndarray, categories: np.ndarray, num_category: int, ax: plt.Axes
 ) -> plt.Axes:
-    for i in range(len(np.unique(categories))):
+    for i in range(num_category):
+        idx = categories == i
         ax.scatter(
-            datas[categories == i],
-            np.zeros_like(datas[categories == i]),
+            datas[idx],
+            np.zeros_like(datas[idx]),
             color=colors[i],
         )
     return ax
 
 
 def _plot_scatter_2d(
-    datas: np.ndarray, categories: np.ndarray, ax: plt.Axes
+    datas: np.ndarray, categories: np.ndarray, num_category: int, ax: plt.Axes
 ) -> plt.Axes:
-    for i in range(len(np.unique(categories))):
+    for i in range(num_category):
+        idx = categories == i
         ax.scatter(
-            datas[categories == i, 0],
-            datas[categories == i, 1],
+            datas[idx, 0],
+            datas[idx, 1],
             color=colors[i],
         )
     return ax
 
 
 def _plot_scatter_3d(
-    datas: np.ndarray, categories: np.ndarray, ax: plt.Axes
+    datas: np.ndarray, categories: np.ndarray, num_category: int, ax: plt.Axes
 ) -> plt.Axes:
     x = datas[:, 0]
     y = datas[:, 1]
     z = datas[:, 2]
-    for i in range(len(np.unique(categories))):
+    for i in range(num_category):
+        idx = categories == i
         ax.scatter(
-            x[categories == i],
-            y[categories == i],
-            z[categories == i],
+            x[idx],
+            y[idx],
+            z[idx],
             color=colors[i],
         )
     return ax
 
 
 def _plot_bar(datas: np.ndarray, ax: plt.Axes) -> plt.Axes:
     # plot datas
@@ -125,14 +128,16 @@
         num_samples = datas.shape[0]
         num_categories = datas.shape[1]
         if xticks is None:
             xticks = [str(i) for i in range(num_samples)]
     elif plot_type == "scatter":
         num_samples = datas.shape[0]
         num_dimensions = datas.shape[1]
+        if names is None:
+            names = [str(i) for i in range(max(categories) + 1)]
 
     if categories is None:
         categories = np.zeros(num_samples, dtype=int)
     else:
         categories = np.array(categories)
 
     # handle errors
@@ -167,19 +172,19 @@
         if ax is None:
             ax = plt.axes()
         ax = _plot_line(datas, ax)
     elif plot_type == "scatter":
         if ax is None:
             ax = plt.axes(projection="3d" if num_dimensions == 3 else None)
         if datas.shape[1] == 1:
-            ax = _plot_scatter_1d(datas, categories, ax)
+            ax = _plot_scatter_1d(datas, categories, len(names), ax)
         elif datas.shape[1] == 2:
-            ax = _plot_scatter_2d(datas, categories, ax)
+            ax = _plot_scatter_2d(datas, categories, len(names), ax)
         elif datas.shape[1] == 3:
-            ax = _plot_scatter_3d(datas, categories, ax)
+            ax = _plot_scatter_3d(datas, categories, len(names), ax)
         else:
             raise NotImplementedError(
                 f"datas shape {datas.shape} is not supported"
             )
     else:
         raise ValueError(
             f"plot_type must be bar or line. plot_type: {plot_type}"
```

### Comparing `waffle_utils-0.3.0/waffle_utils.egg-info/PKG-INFO` & `waffle_utils-0.3.1/waffle_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Waffle Utils 🥛
 Home-page: https://github.com/snuailab/waffle_utils
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_utils/issues
 Project-URL: Source, https://github.com/snuailab/waffle_utils
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-utils Version: 0.3.0 Summary: Waffle Utils
+Metadata-Version: 2.1 Name: waffle-utils Version: 0.3.1 Summary: Waffle Utils
 ð¥ Home-page: https://github.com/snuailab/waffle_utils Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports,
 https://github.com/snuailab/waffle_utils/issues Project-URL: Source, https://
 github.com/snuailab/waffle_utils Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_utils-0.3.0/waffle_utils.egg-info/SOURCES.txt` & `waffle_utils-0.3.1/waffle_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

