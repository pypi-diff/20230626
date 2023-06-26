# Comparing `tmp/histcmp-0.5.2.tar.gz` & `tmp/histcmp-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcmp-0.5.2.tar", max compression
+gzip compressed data, was "histcmp-0.5.3.tar", max compression
```

## Comparing `histcmp-0.5.2.tar` & `histcmp-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0      771 2022-10-24 09:38:26.302652 histcmp-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-02 08:41:54.599617 histcmp-0.5.2/src/histcmp/__init__.py
--rw-r--r--   0        0        0    13656 2022-09-02 08:41:54.599804 histcmp-0.5.2/src/histcmp/checks.py
--rw-r--r--   0        0        0     6167 2022-10-24 09:26:13.465697 histcmp-0.5.2/src/histcmp/cli.py
--rw-r--r--   0        0        0    10682 2022-10-24 09:23:18.590626 histcmp-0.5.2/src/histcmp/compare.py
--rw-r--r--   0        0        0      500 2022-09-02 08:41:54.600186 histcmp-0.5.2/src/histcmp/config.py
--rw-r--r--   0        0        0      726 2022-09-02 08:41:54.600267 histcmp-0.5.2/src/histcmp/console.py
--rw-r--r--   0        0        0      186 2022-09-02 08:41:54.600358 histcmp-0.5.2/src/histcmp/github.py
--rw-r--r--   0        0        0      117 2022-09-02 08:41:54.600450 histcmp-0.5.2/src/histcmp/icons.py
--rw-r--r--   0        0        0     4949 2022-09-21 11:44:12.287776 histcmp-0.5.2/src/histcmp/plot.py
--rw-r--r--   0        0        0     3773 2022-10-06 13:39:04.629172 histcmp-0.5.2/src/histcmp/report.py
--rw-r--r--   0        0        0     5791 2022-10-24 09:31:41.424054 histcmp-0.5.2/src/histcmp/root_helpers.py
--rw-r--r--   0        0        0      878 1985-10-26 08:15:00.000000 histcmp-0.5.2/src/histcmp/static/alpinejs.intersect.min.js
--rw-r--r--   0        0        0    37696 2022-09-02 08:41:54.601106 histcmp-0.5.2/src/histcmp/static/alpinejs.min.js
--rw-r--r--   0        0        0   244777 2022-09-02 08:41:54.601888 histcmp-0.5.2/src/histcmp/static/css/bulma/bulma-rtl.css
--rw-r--r--   0        0        0    98265 2022-09-02 08:41:54.602432 histcmp-0.5.2/src/histcmp/static/css/bulma/bulma-rtl.css.map
--rw-r--r--   0        0        0   206763 2022-09-02 08:41:54.603072 histcmp-0.5.2/src/histcmp/static/css/bulma/bulma-rtl.min.css
--rw-r--r--   0        0        0   244630 2022-09-02 08:41:54.603862 histcmp-0.5.2/src/histcmp/static/css/bulma/bulma.css
--rw-r--r--   0        0        0    98250 2022-09-02 08:41:54.604451 histcmp-0.5.2/src/histcmp/static/css/bulma/bulma.css.map
--rw-r--r--   0        0        0   206620 2022-09-02 08:41:54.605152 histcmp-0.5.2/src/histcmp/static/css/bulma/bulma.min.css
--rw-r--r--   0        0        0      315 2022-09-02 08:41:54.605264 histcmp-0.5.2/src/histcmp/static/css/main.css
--rw-r--r--   0        0        0     2088 2022-09-21 11:33:42.486639 histcmp-0.5.2/src/histcmp/templates/base.html.j2
--rw-r--r--   0        0        0     2399 2022-09-20 12:18:10.041720 histcmp-0.5.2/src/histcmp/templates/main.html.j2
--rw-r--r--   0        0        0     1134 2022-10-24 09:39:00.384156 histcmp-0.5.2/setup.py
--rw-r--r--   0        0        0      922 2022-10-24 09:39:00.384338 histcmp-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      771 2023-06-26 07:32:57.363218 histcmp-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-02 08:41:54.599617 histcmp-0.5.3/src/histcmp/__init__.py
+-rw-r--r--   0        0        0    13656 2022-09-02 08:41:54.599804 histcmp-0.5.3/src/histcmp/checks.py
+-rw-r--r--   0        0        0     6167 2022-10-24 09:26:13.465697 histcmp-0.5.3/src/histcmp/cli.py
+-rw-r--r--   0        0        0    10682 2022-10-24 09:23:18.590626 histcmp-0.5.3/src/histcmp/compare.py
+-rw-r--r--   0        0        0      500 2022-09-02 08:41:54.600186 histcmp-0.5.3/src/histcmp/config.py
+-rw-r--r--   0        0        0      726 2022-09-02 08:41:54.600267 histcmp-0.5.3/src/histcmp/console.py
+-rw-r--r--   0        0        0      186 2022-09-02 08:41:54.600358 histcmp-0.5.3/src/histcmp/github.py
+-rw-r--r--   0        0        0      117 2022-09-02 08:41:54.600450 histcmp-0.5.3/src/histcmp/icons.py
+-rw-r--r--   0        0        0     4949 2022-09-21 11:44:12.287776 histcmp-0.5.3/src/histcmp/plot.py
+-rw-r--r--   0        0        0     3773 2022-10-06 13:39:04.629172 histcmp-0.5.3/src/histcmp/report.py
+-rw-r--r--   0        0        0     5791 2022-10-24 09:31:41.424054 histcmp-0.5.3/src/histcmp/root_helpers.py
+-rw-r--r--   0        0        0      878 1985-10-26 08:15:00.000000 histcmp-0.5.3/src/histcmp/static/alpinejs.intersect.min.js
+-rw-r--r--   0        0        0    37696 2022-09-02 08:41:54.601106 histcmp-0.5.3/src/histcmp/static/alpinejs.min.js
+-rw-r--r--   0        0        0   244777 2022-09-02 08:41:54.601888 histcmp-0.5.3/src/histcmp/static/css/bulma/bulma-rtl.css
+-rw-r--r--   0        0        0    98265 2022-09-02 08:41:54.602432 histcmp-0.5.3/src/histcmp/static/css/bulma/bulma-rtl.css.map
+-rw-r--r--   0        0        0   206763 2022-09-02 08:41:54.603072 histcmp-0.5.3/src/histcmp/static/css/bulma/bulma-rtl.min.css
+-rw-r--r--   0        0        0   244630 2022-09-02 08:41:54.603862 histcmp-0.5.3/src/histcmp/static/css/bulma/bulma.css
+-rw-r--r--   0        0        0    98250 2022-09-02 08:41:54.604451 histcmp-0.5.3/src/histcmp/static/css/bulma/bulma.css.map
+-rw-r--r--   0        0        0   206620 2022-09-02 08:41:54.605152 histcmp-0.5.3/src/histcmp/static/css/bulma/bulma.min.css
+-rw-r--r--   0        0        0      315 2022-09-02 08:41:54.605264 histcmp-0.5.3/src/histcmp/static/css/main.css
+-rw-r--r--   0        0        0     2088 2022-09-21 11:33:42.486639 histcmp-0.5.3/src/histcmp/templates/base.html.j2
+-rw-r--r--   0        0        0     2399 2022-09-20 12:18:10.041720 histcmp-0.5.3/src/histcmp/templates/main.html.j2
+-rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 histcmp-0.5.3/PKG-INFO
```

### Comparing `histcmp-0.5.2/pyproject.toml` & `histcmp-0.5.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "histcmp"
-version = "0.5.2"
+version = "0.5.3"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 license = "MIT"
 packages = [
   { include = "histcmp", from = "src" },
 ]
```

### Comparing `histcmp-0.5.2/src/histcmp/checks.py` & `histcmp-0.5.3/src/histcmp/checks.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/cli.py` & `histcmp-0.5.3/src/histcmp/cli.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/compare.py` & `histcmp-0.5.3/src/histcmp/compare.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/console.py` & `histcmp-0.5.3/src/histcmp/console.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/plot.py` & `histcmp-0.5.3/src/histcmp/plot.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/report.py` & `histcmp-0.5.3/src/histcmp/report.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/root_helpers.py` & `histcmp-0.5.3/src/histcmp/root_helpers.py`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/static/alpinejs.intersect.min.js` & `histcmp-0.5.3/src/histcmp/static/alpinejs.intersect.min.js`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/static/alpinejs.min.js` & `histcmp-0.5.3/src/histcmp/static/alpinejs.min.js`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/static/css/bulma/bulma-rtl.css` & `histcmp-0.5.3/src/histcmp/static/css/bulma/bulma-rtl.css`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/static/css/bulma/bulma-rtl.css.map` & `histcmp-0.5.3/src/histcmp/static/css/bulma/bulma-rtl.css.map`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/static/css/bulma/bulma-rtl.min.css` & `histcmp-0.5.3/src/histcmp/static/css/bulma/bulma-rtl.min.css`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/static/css/bulma/bulma.css` & `histcmp-0.5.3/src/histcmp/static/css/bulma/bulma.css`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/static/css/bulma/bulma.css.map` & `histcmp-0.5.3/src/histcmp/static/css/bulma/bulma.css.map`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/static/css/bulma/bulma.min.css` & `histcmp-0.5.3/src/histcmp/static/css/bulma/bulma.min.css`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/templates/base.html.j2` & `histcmp-0.5.3/src/histcmp/templates/base.html.j2`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/src/histcmp/templates/main.html.j2` & `histcmp-0.5.3/src/histcmp/templates/main.html.j2`

 * *Files identical despite different names*

### Comparing `histcmp-0.5.2/PKG-INFO` & `histcmp-0.5.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: histcmp
-Version: 0.5.2
+Version: 0.5.3
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (==8.0.4)
 Requires-Dist: hist[plot] (>=2.6.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: mplhep (>=0.3.26,<0.4.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
```

