# Comparing `tmp/dash_express_components-0.0.8.tar.gz` & `tmp/dash_express_components-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_express_components-0.0.8.tar", last modified: Mon Jan 24 13:01:15 2022, max compression
+gzip compressed data, was "dash_express_components-0.0.9.tar", last modified: Mon Jan 24 21:49:04 2022, max compression
```

## Comparing `dash_express_components-0.0.8.tar` & `dash_express_components-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 13:01:15.255008 dash_express_components-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-01-24 13:01:15.255008 dash_express_components-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3712 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 13:01:15.255008 dash_express_components-0.0.8/dash_express_components/
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/BarCount.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Box.py
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/CombinecatTransform.py
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/DashExpressComponents.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/EvalTransform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    14064 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/HistogramLine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Imshow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1572 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Localstore.py
--rw-r--r--   0 runner    (1001) docker     (121)     1768 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/MeltTransform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/MetaCheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Parametrize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/PlotterBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Probability.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/ScatterMatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/SubComponentBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Table.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/Violin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3512 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (121)  3687759 2022-01-24 13:01:11.000000 dash_express_components-0.0.8/dash_express_components/async-graph.js
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-24 13:01:11.000000 dash_express_components-0.0.8/dash_express_components/async-graph.js.map
--rw-r--r--   0 runner    (1001) docker     (121)   495006 2022-01-24 13:01:11.000000 dash_express_components-0.0.8/dash_express_components/dash_express_components.min.js
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-01-24 13:01:11.000000 dash_express_components-0.0.8/dash_express_components/dash_express_components.min.js.map
--rw-r--r--   0 runner    (1001) docker     (121)    74189 2022-01-24 13:01:13.000000 dash_express_components-0.0.8/dash_express_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-01-24 13:01:12.000000 dash_express_components-0.0.8/dash_express_components/package-info.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 13:01:15.255008 dash_express_components-0.0.8/dash_express_components/plottypes/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/plottypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/plottypes/_bar_count.py
--rw-r--r--   0 runner    (1001) docker     (121)     4104 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/plottypes/_histogram_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     4956 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/plottypes/_imshow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/plottypes/_probability.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/plottypes/_table.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 13:01:15.255008 dash_express_components-0.0.8/dash_express_components/transformationtypes/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/transformationtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/transformationtypes/_combinecat.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/transformationtypes/_eval.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/transformationtypes/_melt.py
--rw-r--r--   0 runner    (1001) docker     (121)    15596 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/dash_express_components/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 13:01:15.255008 dash_express_components-0.0.8/dash_express_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-01-24 13:01:15.000000 dash_express_components-0.0.8/dash_express_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-01-24 13:01:15.000000 dash_express_components-0.0.8/dash_express_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-24 13:01:15.000000 dash_express_components-0.0.8/dash_express_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-24 13:01:15.000000 dash_express_components-0.0.8/dash_express_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/package.json
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-24 13:01:15.255008 dash_express_components-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-01-24 12:58:38.000000 dash_express_components-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 21:49:04.287763 dash_express_components-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-01-24 21:49:04.287763 dash_express_components-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3712 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 21:49:04.283763 dash_express_components-0.0.9/dash_express_components/
+-rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/BarCount.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Box.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/CombinecatTransform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/DashExpressComponents.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56262 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/DataTable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/EvalTransform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13955 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/HistogramLine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Imshow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1572 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Localstore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1768 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/MeltTransform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/MetaCheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Parametrize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Plotter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/PlotterBase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Probability.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Scatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/ScatterMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/SubComponentBase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/Violin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3540 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (121)  3687759 2022-01-24 21:49:00.000000 dash_express_components-0.0.9/dash_express_components/async-graph.js
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-24 21:49:00.000000 dash_express_components-0.0.9/dash_express_components/async-graph.js.map
+-rw-r--r--   0 runner    (1001) docker     (121)  1675901 2022-01-24 21:49:00.000000 dash_express_components-0.0.9/dash_express_components/dash_express_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-01-24 21:49:00.000000 dash_express_components-0.0.9/dash_express_components/dash_express_components.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (121)   173958 2022-01-24 21:49:02.000000 dash_express_components-0.0.9/dash_express_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-01-24 21:49:01.000000 dash_express_components-0.0.9/dash_express_components/package-info.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 21:49:04.283763 dash_express_components-0.0.9/dash_express_components/plottypes/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/plottypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/plottypes/_bar_count.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4104 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/plottypes/_histogram_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4956 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/plottypes/_imshow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/plottypes/_probability.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/plottypes/_table.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 21:49:04.283763 dash_express_components-0.0.9/dash_express_components/transformationtypes/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/transformationtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/transformationtypes/_combinecat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/transformationtypes/_eval.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/transformationtypes/_melt.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15596 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/dash_express_components/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 21:49:04.283763 dash_express_components-0.0.9/dash_express_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-01-24 21:49:04.000000 dash_express_components-0.0.9/dash_express_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-01-24 21:49:04.000000 dash_express_components-0.0.9/dash_express_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-24 21:49:04.000000 dash_express_components-0.0.9/dash_express_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-24 21:49:04.000000 dash_express_components-0.0.9/dash_express_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/package.json
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-24 21:49:04.287763 dash_express_components-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2022-01-24 21:45:43.000000 dash_express_components-0.0.9/setup.py
```

### Comparing `dash_express_components-0.0.8/README.md` & `dash_express_components-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/BarCount.py` & `dash_express_components-0.0.9/dash_express_components/BarCount.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Base.py` & `dash_express_components-0.0.9/dash_express_components/Base.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Box.py` & `dash_express_components-0.0.9/dash_express_components/Box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/CombinecatTransform.py` & `dash_express_components-0.0.9/dash_express_components/CombinecatTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Configurator.py` & `dash_express_components-0.0.9/dash_express_components/Configurator.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/DashExpressComponents.py` & `dash_express_components-0.0.9/dash_express_components/DashExpressComponents.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/EvalTransform.py` & `dash_express_components-0.0.9/dash_express_components/EvalTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Filter.py` & `dash_express_components-0.0.9/dash_express_components/Filter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Graph.py` & `dash_express_components-0.0.9/dash_express_components/Graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,27 +234,19 @@
     object containing the data to extend, `traceIndices` (optional) is
     an array of trace indices that should be extended, and `maxPoints`
     (optional) is either an integer defining the maximum number of
     points allowed or an object with key:value pairs matching
     `updateData` Reference the Plotly.extendTraces API for full usage:
     https://plotly.com/javascript/plotlyjs-function-reference/#plotlyextendtraces.
 
-- figure (dict; default {    data: [],    layout: {},    frames: [],}):
+- figure (boolean | number | string | dict | list; default {    data: [],    layout: {},    frames: [],}):
     Plotly `figure` object. See schema:
     https://plotly.com/javascript/reference  `config` is set
     separately by the `config` property.
 
-    `figure` is a dict with keys:
-
-    - data (list of dicts; optional)
-
-    - frames (list of dicts; optional)
-
-    - layout (dict; optional)
-
 - hoverData (dict; optional):
     Data from latest hover event. Read-only.
 
 - loading_state (dict; optional):
     Object that holds the loading state object coming from
     dash-renderer.
```

### Comparing `dash_express_components-0.0.8/dash_express_components/HistogramLine.py` & `dash_express_components-0.0.9/dash_express_components/HistogramLine.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Imshow.py` & `dash_express_components-0.0.9/dash_express_components/Imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Localstore.py` & `dash_express_components-0.0.9/dash_express_components/Localstore.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/MeltTransform.py` & `dash_express_components-0.0.9/dash_express_components/MeltTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/MetaCheck.py` & `dash_express_components-0.0.9/dash_express_components/MetaCheck.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Parametrize.py` & `dash_express_components-0.0.9/dash_express_components/Parametrize.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Plotter.py` & `dash_express_components-0.0.9/dash_express_components/Plotter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/PlotterBase.py` & `dash_express_components-0.0.9/dash_express_components/PlotterBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Probability.py` & `dash_express_components-0.0.9/dash_express_components/Probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Scatter.py` & `dash_express_components-0.0.9/dash_express_components/Scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/ScatterMatrix.py` & `dash_express_components-0.0.9/dash_express_components/ScatterMatrix.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/SubComponentBase.py` & `dash_express_components-0.0.9/dash_express_components/SubComponentBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Table.py` & `dash_express_components-0.0.9/dash_express_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Transform.py` & `dash_express_components-0.0.9/dash_express_components/Transform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/Violin.py` & `dash_express_components-0.0.9/dash_express_components/Violin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/__init__.py` & `dash_express_components-0.0.9/dash_express_components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .utils import *
 
 import os as _os
 import sys as _sys
 import json
 
 import dash as _dash
+from dash import dash_table
 
 # noinspection PyUnresolvedReferences
 from ._imports_ import *
 from ._imports_ import __all__
 
 if not hasattr(_dash, '__plotly_dash') and not hasattr(_dash, 'development'):
     print('Dash was not successfully imported. '
```

### Comparing `dash_express_components-0.0.8/dash_express_components/_imports_.py` & `dash_express_components-0.0.9/dash_express_components/_imports_.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .Configurator import Configurator
+from .DataTable import DataTable
 from .Filter import Filter
 from .Graph import Graph
 from .Localstore import Localstore
 from .MetaCheck import MetaCheck
 from .Parametrize import Parametrize
 from .Plotter import Plotter
 from .Transform import Transform
@@ -20,14 +21,15 @@
 from .CombinecatTransform import CombinecatTransform
 from .EvalTransform import EvalTransform
 from .MeltTransform import MeltTransform
 from .SubComponentBase import SubComponentBase
 
 __all__ = [
     "Configurator",
+    "DataTable",
     "Filter",
     "Graph",
     "Localstore",
     "MetaCheck",
     "Parametrize",
     "Plotter",
     "Transform",
```

### Comparing `dash_express_components-0.0.8/dash_express_components/async-graph.js` & `dash_express_components-0.0.9/dash_express_components/async-graph.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /*! For license information please see async-graph.js.LICENSE.txt */
 (window.webpackJsonpdash_express_components = window.webpackJsonpdash_express_components || []).push([
 [0], {
-    141: function(t, e) {
+    143: function(t, e) {
         ! function(r) {
             if ("object" == typeof e && void 0 !== t) t.exports = r();
             else if ("function" == typeof define && define.amd) define([], r);
             else {
                 ("undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : this).Plotly = r()
             }
         }((function() {
@@ -143531,15 +143531,15 @@
                                             }, {}, [6])(6)
                                         }))
                                 }).call(this)
                         }).call(this, "undefined" != typeof global ? global : "undefined" != typeof self ? self : "undefined" != typeof window ? window : {})
                 }, {}]
         }, {}, [27])(27)
     }))
-}, 142: function(t, e, r) {
+}, 144: function(t, e, r) {
 (function(e) {
 var r = /^\s+|\s+$/g,
     n = /^[-+]0x[0-9a-f]+$/i,
     i = /^0b[01]+$/i,
     a = /^0o[0-7]+$/i,
     o = parseInt,
     s = "object" == typeof e && e && e.Object === Object && e,
@@ -143619,16 +143619,16 @@
     }
     return e = g(e) || 0, d(r) && (u = !!r.leading, a = (m = "maxWait" in r) ? f(g(r.maxWait) || 0, e) : a, v = "trailing" in r ? !!r.trailing : v), T.cancel = function() {
         void 0 !== s && clearTimeout(s), c = 0, n = l = i = s = void 0
     }, T.flush = function() {
         return void 0 === s ? o : w(p())
     }, T
 }
-}).call(this, r(77))
-}, 143: function(t, e, r) {
+}).call(this, r(70))
+}, 145: function(t, e, r) {
 (function(e) {
 var r = /^\s+|\s+$/g,
     n = /^[-+]0x[0-9a-f]+$/i,
     i = /^0b[01]+$/i,
     a = /^0o[0-7]+$/i,
     o = parseInt,
     s = "object" == typeof e && e && e.Object === Object && e,
@@ -143719,24 +143719,24 @@
     if ("function" != typeof t) throw new TypeError("Expected a function");
     return g(r) && (n = "leading" in r ? !!r.leading : n, i = "trailing" in r ? !!r.trailing : i), d(t, e, {
         leading: n,
         maxWait: e,
         trailing: i
     })
 }
-}).call(this, r(77))
-}, 144: function(t, e, r) {
+}).call(this, r(70))
+}, 146: function(t, e, r) {
 "use strict";
 r.r(e);
-var n = r(0),
+var n = r(1),
 i = r.n(n),
 a = r(20),
-o = r(142),
+o = r(144),
 s = r.n(o),
-l = r(143),
+l = r(145),
 c = r.n(l),
 u = function(t, e) {
     return (u = Object.setPrototypeOf || {
             __proto__: []
         }
         instanceof Array && function(t, e) {
             t.__proto__ = e
@@ -144334,18 +144334,18 @@
     }), t, e)
 })),
 st = _((function(t, e) {
     for (var r = {}, n = {}, i = 0, a = t.length; i < a;) n[t[i]] = 1, i += 1;
     for (var o in e) n.hasOwnProperty(o) || (r[o] = e[o]);
     return r
 })),
-lt = r(1),
+lt = r(0),
 ct = r.n(lt),
-ut = r(78),
-ft = r(141);
+ut = r(79),
+ft = r(143);
 
 function ht(t, e) {
 var r = Object.keys(t);
 if (Object.getOwnPropertySymbols) {
     var n = Object.getOwnPropertySymbols(t);
     e && (n = n.filter((function(e) {
         return Object.getOwnPropertyDescriptor(t, e).enumerable
```

### Comparing `dash_express_components-0.0.8/dash_express_components/package-info.json` & `dash_express_components-0.0.9/dash_express_components/package-info.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9454545454545455%*

 * *Differences: {"'dependencies'": "{'exceljs': '^4.3.0'}", "'version'": "'0.0.9'"}*

```diff
@@ -1,12 +1,13 @@
 {
     "author": "Viktor Kr\u00fcckl <viktor@krueckl.de>",
     "dependencies": {
         "@nx-js/compiler-util": "^2.0.0",
         "chroma-js": "^2.1.2",
+        "exceljs": "^4.3.0",
         "plotly.js": "^1.58.4",
         "plotly.js-dist": "^2.8.3",
         "ramda": "^0.26.1",
         "react-bootstrap": "^2.0.4",
         "react-datetime-picker": "^3.4.3",
         "react-list-editable": "^0.1.0",
         "react-resize-detector": "^6.7.7",
@@ -52,9 +53,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_express_components -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.8"
+    "version": "0.0.9"
 }
```

### Comparing `dash_express_components-0.0.8/dash_express_components/plottypes/_bar_count.py` & `dash_express_components-0.0.9/dash_express_components/plottypes/_bar_count.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/plottypes/_histogram_line.py` & `dash_express_components-0.0.9/dash_express_components/plottypes/_histogram_line.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/plottypes/_imshow.py` & `dash_express_components-0.0.9/dash_express_components/plottypes/_imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/plottypes/_probability.py` & `dash_express_components-0.0.9/dash_express_components/plottypes/_probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components/utils.py` & `dash_express_components-0.0.9/dash_express_components/utils.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.8/dash_express_components.egg-info/SOURCES.txt` & `dash_express_components-0.0.9/dash_express_components.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 dash_express_components/BarCount.py
 dash_express_components/Base.py
 dash_express_components/Box.py
 dash_express_components/CombinecatTransform.py
 dash_express_components/Configurator.py
 dash_express_components/DashExpressComponents.py
+dash_express_components/DataTable.py
 dash_express_components/EvalTransform.py
 dash_express_components/Filter.py
 dash_express_components/Graph.py
 dash_express_components/HistogramLine.py
 dash_express_components/Imshow.py
 dash_express_components/Localstore.py
 dash_express_components/MeltTransform.py
```

### Comparing `dash_express_components-0.0.8/package.json` & `dash_express_components-0.0.9/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9454545454545455%*

 * *Differences: {"'dependencies'": "{'exceljs': '^4.3.0'}", "'version'": "'0.0.9'"}*

```diff
@@ -1,12 +1,13 @@
 {
     "author": "Viktor Kr\u00fcckl <viktor@krueckl.de>",
     "dependencies": {
         "@nx-js/compiler-util": "^2.0.0",
         "chroma-js": "^2.1.2",
+        "exceljs": "^4.3.0",
         "plotly.js": "^1.58.4",
         "plotly.js-dist": "^2.8.3",
         "ramda": "^0.26.1",
         "react-bootstrap": "^2.0.4",
         "react-datetime-picker": "^3.4.3",
         "react-list-editable": "^0.1.0",
         "react-resize-detector": "^6.7.7",
@@ -52,9 +53,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_express_components -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.8"
+    "version": "0.0.9"
 }
```

### Comparing `dash_express_components-0.0.8/setup.py` & `dash_express_components-0.0.9/setup.py`

 * *Files identical despite different names*

