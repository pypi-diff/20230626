# Comparing `tmp/feffery_antd_charts-0.0.1rc8.tar.gz` & `tmp/feffery_antd_charts-0.0.1rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_antd_charts-0.0.1rc8.tar", last modified: Mon Oct 10 14:20:40 2022, max compression
+gzip compressed data, was "feffery_antd_charts-0.0.1rc9.tar", last modified: Mon Oct 10 14:24:11 2022, max compression
```

## Comparing `feffery_antd_charts-0.0.1rc8.tar` & `feffery_antd_charts-0.0.1rc9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-10-10 14:20:40.893993 feffery_antd_charts-0.0.1rc8/
--rw-rw-rw-   0        0        0     1087 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc8/LICENSE
--rw-rw-rw-   0        0        0      434 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc8/MANIFEST.in
--rw-rw-rw-   0        0        0      298 2022-10-10 14:20:40.892996 feffery_antd_charts-0.0.1rc8/PKG-INFO
--rw-rw-rw-   0        0        0       49 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-10 14:20:40.879033 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/
--rw-rw-rw-   0        0        0     5125 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdArea.py
--rw-rw-rw-   0        0        0     5997 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdBar.py
--rw-rw-rw-   0        0        0     4142 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdBox.py
--rw-rw-rw-   0        0        0     3565 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdChord.py
--rw-rw-rw-   0        0        0     6146 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdColumn.py
--rw-rw-rw-   0        0        0     6716 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdDecompositionTree.py
--rw-rw-rw-   0        0        0     6389 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdFundFlow.py
--rw-rw-rw-   0        0        0     4784 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdFunnel.py
--rw-rw-rw-   0        0        0     3983 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdHistogram.py
--rw-rw-rw-   0        0        0     5399 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdLine.py
--rw-rw-rw-   0        0        0     4944 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdPie.py
--rw-rw-rw-   0        0        0     5079 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdRadar.py
--rw-rw-rw-   0        0        0     4377 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdRose.py
--rw-rw-rw-   0        0        0     4085 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdSankey.py
--rw-rw-rw-   0        0        0     5476 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdScatter.py
--rw-rw-rw-   0        0        0     4037 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdStock.py
--rw-rw-rw-   0        0        0     4655 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdSunburst.py
--rw-rw-rw-   0        0        0     4058 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdTreemap.py
--rw-rw-rw-   0        0        0     4643 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdWordCloud.py
--rw-rw-rw-   0        0        0     1543 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/FefferyAntdCharts.py
--rw-rw-rw-   0        0        0     2600 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/__init__.py
--rw-rw-rw-   0        0        0     1075 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/_imports_.py
--rw-rw-rw-   0        0        0  2695491 2022-10-10 14:09:58.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/feffery_antd_charts.min.js
--rw-rw-rw-   0        0        0 11078291 2022-09-23 14:31:21.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/feffery_antd_charts.min.js.map
--rw-rw-rw-   0        0        0   201167 2022-10-10 14:10:01.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/metadata.json
--rw-rw-rw-   0        0        0     2493 2022-10-10 14:10:00.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts/package-info.json
-drwxrwxrwx   0        0        0        0 2022-10-10 14:20:40.891003 feffery_antd_charts-0.0.1rc8/feffery_antd_charts.egg-info/
--rw-rw-rw-   0        0        0      298 2022-10-10 14:20:40.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2022-10-10 14:20:40.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-10 14:20:40.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-10-10 14:20:40.000000 feffery_antd_charts-0.0.1rc8/feffery_antd_charts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2493 2022-10-10 14:20:20.000000 feffery_antd_charts-0.0.1rc8/package.json
--rw-rw-rw-   0        0        0       42 2022-10-10 14:20:40.893993 feffery_antd_charts-0.0.1rc8/setup.cfg
--rw-rw-rw-   0        0        0      533 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-10 14:24:11.881949 feffery_antd_charts-0.0.1rc9/
+-rw-rw-rw-   0        0        0     1087 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc9/LICENSE
+-rw-rw-rw-   0        0        0      434 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc9/MANIFEST.in
+-rw-rw-rw-   0        0        0      298 2022-10-10 14:24:11.881949 feffery_antd_charts-0.0.1rc9/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-10 14:24:11.871976 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/
+-rw-rw-rw-   0        0        0     5125 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdArea.py
+-rw-rw-rw-   0        0        0     5997 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdBar.py
+-rw-rw-rw-   0        0        0     4142 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdBox.py
+-rw-rw-rw-   0        0        0     3565 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdChord.py
+-rw-rw-rw-   0        0        0     6146 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdColumn.py
+-rw-rw-rw-   0        0        0     6716 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdDecompositionTree.py
+-rw-rw-rw-   0        0        0     6389 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdFundFlow.py
+-rw-rw-rw-   0        0        0     4784 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdFunnel.py
+-rw-rw-rw-   0        0        0     3983 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdHistogram.py
+-rw-rw-rw-   0        0        0     5399 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdLine.py
+-rw-rw-rw-   0        0        0     4944 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdPie.py
+-rw-rw-rw-   0        0        0     5079 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdRadar.py
+-rw-rw-rw-   0        0        0     4377 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdRose.py
+-rw-rw-rw-   0        0        0     4085 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdSankey.py
+-rw-rw-rw-   0        0        0     5476 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdScatter.py
+-rw-rw-rw-   0        0        0     4037 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdStock.py
+-rw-rw-rw-   0        0        0     4655 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdSunburst.py
+-rw-rw-rw-   0        0        0     4058 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdTreemap.py
+-rw-rw-rw-   0        0        0     4643 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdWordCloud.py
+-rw-rw-rw-   0        0        0     1543 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/FefferyAntdCharts.py
+-rw-rw-rw-   0        0        0     2600 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/__init__.py
+-rw-rw-rw-   0        0        0     1075 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/_imports_.py
+-rw-rw-rw-   0        0        0  2695491 2022-10-10 14:22:03.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/feffery_antd_charts.min.js
+-rw-rw-rw-   0        0        0 11078291 2022-09-23 14:31:21.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/feffery_antd_charts.min.js.map
+-rw-rw-rw-   0        0        0   201167 2022-10-10 14:22:06.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/metadata.json
+-rw-rw-rw-   0        0        0     2493 2022-10-10 14:22:04.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts/package-info.json
+drwxrwxrwx   0        0        0        0 2022-10-10 14:24:11.879954 feffery_antd_charts-0.0.1rc9/feffery_antd_charts.egg-info/
+-rw-rw-rw-   0        0        0      298 2022-10-10 14:24:11.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2022-10-10 14:24:11.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-10 14:24:11.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2022-10-10 14:24:11.000000 feffery_antd_charts-0.0.1rc9/feffery_antd_charts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2493 2022-10-10 14:21:10.000000 feffery_antd_charts-0.0.1rc9/package.json
+-rw-rw-rw-   0        0        0       42 2022-10-10 14:24:11.882946 feffery_antd_charts-0.0.1rc9/setup.cfg
+-rw-rw-rw-   0        0        0      533 2022-09-23 01:52:48.000000 feffery_antd_charts-0.0.1rc9/setup.py
```

### Comparing `feffery_antd_charts-0.0.1rc8/LICENSE` & `feffery_antd_charts-0.0.1rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdArea.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdArea.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdBar.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdBar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdBox.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdBox.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdChord.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdChord.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdColumn.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdColumn.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdDecompositionTree.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdDecompositionTree.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdFundFlow.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdFundFlow.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdFunnel.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdFunnel.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdHistogram.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdHistogram.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdLine.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdLine.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdPie.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdPie.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdRadar.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdRadar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdRose.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdRose.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdSankey.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdSankey.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdScatter.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdScatter.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdStock.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdStock.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdSunburst.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdSunburst.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdTreemap.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdTreemap.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/AntdWordCloud.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/AntdWordCloud.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/FefferyAntdCharts.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/FefferyAntdCharts.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/__init__.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/_imports_.py` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/feffery_antd_charts.min.js` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/feffery_antd_charts.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -60,15 +60,15 @@
             return t
         })
     }), "undefined" != typeof jsonpScriptSrc && (a = jsonpScriptSrc, jsonpScriptSrc = function(t) {
         var e = /\/_dash-component-suites\//.test(o().src),
             t = a(t);
         if (!e) return t;
         e = t.split("/"), t = e.slice(-1)[0].split(".");
-        return t.splice(1, 0, "v0_0_1-rc8m1665410962"), e.splice(-1, 1, t.join(".")), e.join("/")
+        return t.splice(1, 0, "v0_0_1-rc9m1665411683"), e.splice(-1, 1, t.join(".")), e.join("/")
     }), i(i.s = 410)
 }([function(i, t, e) {
     "use strict";
     e.r(t), e.d(t, "contains", function() {
         return f
     }), e.d(t, "includes", function() {
         return f
```

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/feffery_antd_charts.min.js.map` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/feffery_antd_charts.min.js.map`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/metadata.json` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/metadata.json`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts/package-info.json` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.0.1-rc9'"}*

```diff
@@ -59,9 +59,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_charts -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.0.1-rc8"
+    "version": "0.0.1-rc9"
 }
```

### Comparing `feffery_antd_charts-0.0.1rc8/feffery_antd_charts.egg-info/SOURCES.txt` & `feffery_antd_charts-0.0.1rc9/feffery_antd_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.0.1rc8/package.json` & `feffery_antd_charts-0.0.1rc9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.0.1-rc9'"}*

```diff
@@ -59,9 +59,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_charts -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.0.1-rc8"
+    "version": "0.0.1-rc9"
 }
```

### Comparing `feffery_antd_charts-0.0.1rc8/setup.py` & `feffery_antd_charts-0.0.1rc9/setup.py`

 * *Files identical despite different names*

