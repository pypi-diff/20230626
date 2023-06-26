# Comparing `tmp/plottah-0.1.2.tar.gz` & `tmp/plottah-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plottah-0.1.2.tar", max compression
+gzip compressed data, was "plottah-0.1.3.tar", max compression
```

## Comparing `plottah-0.1.2.tar` & `plottah-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      835 2023-06-22 12:52:22.561511 plottah-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-06-22 11:30:53.499061 plottah-0.1.2/plottah/__init__.py
--rw-r--r--   0        0        0     1012 2023-06-22 12:44:11.607614 plottah-0.1.2/plottah/__main__.py
--rw-r--r--   0        0        0     1339 2023-06-19 19:34:19.357898 plottah-0.1.2/plottah/colors.py
--rw-r--r--   0        0        0     3056 2023-06-22 09:19:12.089888 plottah-0.1.2/plottah/config.py
--rw-r--r--   0        0        0      988 2023-06-22 09:55:14.056657 plottah-0.1.2/plottah/main.py
--rw-r--r--   0        0        0       24 2023-06-20 17:12:04.651705 plottah-0.1.2/plottah/plot_builder/__init__.py
--rw-r--r--   0        0        0     2684 2023-06-22 12:58:33.986776 plottah-0.1.2/plottah/plot_builder/builders.py
--rw-r--r--   0        0        0     7488 2023-06-22 12:44:18.976051 plottah-0.1.2/plottah/plot_handler/PlotHandler.py
--rw-r--r--   0        0        0       37 2023-06-20 17:27:02.673177 plottah-0.1.2/plottah/plot_handler/__init__.py
--rw-r--r--   0        0        0     7530 2023-06-22 12:44:22.633547 plottah-0.1.2/plottah/plots/BinEventRatePlot.py
--rw-r--r--   0        0        0     3987 2023-06-22 12:44:23.133501 plottah-0.1.2/plottah/plots/DistPlot.py
--rw-r--r--   0        0        0     1927 2023-06-22 07:41:05.603043 plottah-0.1.2/plottah/plots/PlotProtocol.py
--rw-r--r--   0        0        0     3578 2023-06-22 12:44:24.105798 plottah-0.1.2/plottah/plots/RocCurvePlot.py
--rw-r--r--   0        0        0      117 2023-06-16 12:50:48.680563 plottah-0.1.2/plottah/plots/__init__.py
--rw-r--r--   0        0        0     4050 2023-06-16 12:25:45.788578 plottah-0.1.2/plottah/utils.py
--rw-r--r--   0        0        0      506 2023-06-22 12:58:49.386772 plottah-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 plottah-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      835 2023-06-22 12:52:22.561511 plottah-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-22 11:30:53.499061 plottah-0.1.3/plottah/__init__.py
+-rw-r--r--   0        0        0     1012 2023-06-22 12:44:11.607614 plottah-0.1.3/plottah/__main__.py
+-rw-r--r--   0        0        0     1339 2023-06-19 19:34:19.357898 plottah-0.1.3/plottah/colors.py
+-rw-r--r--   0        0        0     3056 2023-06-22 09:19:12.089888 plottah-0.1.3/plottah/config.py
+-rw-r--r--   0        0        0      988 2023-06-22 09:55:14.056657 plottah-0.1.3/plottah/main.py
+-rw-r--r--   0        0        0       24 2023-06-20 17:12:04.651705 plottah-0.1.3/plottah/plot_builder/__init__.py
+-rw-r--r--   0        0        0     2684 2023-06-22 12:58:33.986776 plottah-0.1.3/plottah/plot_builder/builders.py
+-rw-r--r--   0        0        0     7488 2023-06-22 12:44:18.976051 plottah-0.1.3/plottah/plot_handler/PlotHandler.py
+-rw-r--r--   0        0        0       37 2023-06-20 17:27:02.673177 plottah-0.1.3/plottah/plot_handler/__init__.py
+-rw-r--r--   0        0        0     7530 2023-06-22 12:44:22.633547 plottah-0.1.3/plottah/plots/BinEventRatePlot.py
+-rw-r--r--   0        0        0     3987 2023-06-22 12:44:23.133501 plottah-0.1.3/plottah/plots/DistPlot.py
+-rw-r--r--   0        0        0     1927 2023-06-22 07:41:05.603043 plottah-0.1.3/plottah/plots/PlotProtocol.py
+-rw-r--r--   0        0        0     3578 2023-06-22 12:44:24.105798 plottah-0.1.3/plottah/plots/RocCurvePlot.py
+-rw-r--r--   0        0        0      117 2023-06-16 12:50:48.680563 plottah-0.1.3/plottah/plots/__init__.py
+-rw-r--r--   0        0        0     4050 2023-06-16 12:25:45.788578 plottah-0.1.3/plottah/utils.py
+-rw-r--r--   0        0        0      505 2023-06-26 11:25:35.065446 plottah-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 plottah-0.1.3/PKG-INFO
```

### Comparing `plottah-0.1.2/README.md` & `plottah-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/__main__.py` & `plottah-0.1.3/plottah/__main__.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/colors.py` & `plottah-0.1.3/plottah/colors.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/config.py` & `plottah-0.1.3/plottah/config.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/main.py` & `plottah-0.1.3/plottah/main.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/plot_builder/builders.py` & `plottah-0.1.3/plottah/plot_builder/builders.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/plot_handler/PlotHandler.py` & `plottah-0.1.3/plottah/plot_handler/PlotHandler.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/plots/BinEventRatePlot.py` & `plottah-0.1.3/plottah/plots/BinEventRatePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/plots/DistPlot.py` & `plottah-0.1.3/plottah/plots/DistPlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/plots/PlotProtocol.py` & `plottah-0.1.3/plottah/plots/PlotProtocol.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/plots/RocCurvePlot.py` & `plottah-0.1.3/plottah/plots/RocCurvePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.2/plottah/utils.py` & `plottah-0.1.3/plottah/utils.py`

 * *Files identical despite different names*

