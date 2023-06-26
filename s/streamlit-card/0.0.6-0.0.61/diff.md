# Comparing `tmp/streamlit-card-0.0.6.tar.gz` & `tmp/streamlit-card-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-card-0.0.6.tar", last modified: Mon Jun 26 20:01:46 2023, max compression
+gzip compressed data, was "streamlit-card-0.0.61.tar", last modified: Mon Jun 26 20:07:51 2023, max compression
```

## Comparing `streamlit-card-0.0.6.tar` & `streamlit-card-0.0.61.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:01:46.532910 streamlit-card-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 20:00:46.000000 streamlit-card-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 20:00:46.000000 streamlit-card-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-26 20:01:46.532910 streamlit-card-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-26 20:00:46.000000 streamlit-card-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:01:46.532910 streamlit-card-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-26 20:00:46.000000 streamlit-card-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:01:46.524910 streamlit-card-0.0.6/streamlit_card/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-26 20:00:46.000000 streamlit-card-0.0.6/streamlit_card/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:01:46.524910 streamlit-card-0.0.6/streamlit_card/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:01:46.528910 streamlit-card-0.0.6/streamlit_card/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-06-26 20:01:15.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   646432 2023-06-26 20:01:15.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/precache-manifest.6b8328ae49df780207c52d2ceeaeadd9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:01:46.524910 streamlit-card-0.0.6/streamlit_card/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:01:46.532910 streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   498410 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)  2066554 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/main.9d157205.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/main.9d157205.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-26 20:01:33.000000 streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:01:46.524910 streamlit-card-0.0.6/streamlit_card.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-26 20:01:46.000000 streamlit-card-0.0.6/streamlit_card.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-26 20:01:46.000000 streamlit-card-0.0.6/streamlit_card.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:01:46.000000 streamlit-card-0.0.6/streamlit_card.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 20:01:46.000000 streamlit-card-0.0.6/streamlit_card.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 20:01:46.000000 streamlit-card-0.0.6/streamlit_card.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:07:51.078249 streamlit-card-0.0.61/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 20:06:35.000000 streamlit-card-0.0.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 20:06:35.000000 streamlit-card-0.0.61/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-26 20:07:51.078249 streamlit-card-0.0.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-26 20:06:35.000000 streamlit-card-0.0.61/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:07:51.078249 streamlit-card-0.0.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-26 20:06:35.000000 streamlit-card-0.0.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:07:51.070248 streamlit-card-0.0.61/streamlit_card/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-26 20:06:35.000000 streamlit-card-0.0.61/streamlit_card/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:07:51.070248 streamlit-card-0.0.61/streamlit_card/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:07:51.074248 streamlit-card-0.0.61/streamlit_card/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-06-26 20:07:13.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   646432 2023-06-26 20:07:13.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/precache-manifest.6b8328ae49df780207c52d2ceeaeadd9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:07:51.070248 streamlit-card-0.0.61/streamlit_card/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:07:51.078249 streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   498410 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2066554 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/main.9d157205.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/main.9d157205.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-26 20:07:38.000000 streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:07:51.070248 streamlit-card-0.0.61/streamlit_card.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-26 20:07:51.000000 streamlit-card-0.0.61/streamlit_card.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-26 20:07:51.000000 streamlit-card-0.0.61/streamlit_card.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:07:51.000000 streamlit-card-0.0.61/streamlit_card.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 20:07:51.000000 streamlit-card-0.0.61/streamlit_card.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 20:07:51.000000 streamlit-card-0.0.61/streamlit_card.egg-info/top_level.txt
```

### Comparing `streamlit-card-0.0.6/LICENSE` & `streamlit-card-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/PKG-INFO` & `streamlit-card-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-card
-Version: 0.0.6
+Version: 0.0.61
 Summary: A streamlit component, to make UI cards
 Home-page: https://github.com/gamcoh/st-card
 Author: gamcoh
 Author-email: cohengamliel8@gmail.com
 Keywords: card streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-card-0.0.6/README.md` & `streamlit-card-0.0.61/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/setup.py` & `streamlit-card-0.0.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 
 setuptools.setup(
     name="streamlit-card",
-    version="0.0.6",
+    version="0.0.61",
     author="gamcoh",
     author_email="cohengamliel8@gmail.com",
     description="A streamlit component, to make UI cards",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/gamcoh/st-card",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-card-0.0.6/streamlit_card/__init__.py` & `streamlit-card-0.0.61/streamlit_card/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import streamlit.components.v1 as components
 
-_RELEASE = False
+_RELEASE = True
 COMPONENT_NAME = "streamlit_card"
 
 if _RELEASE:  # use the build instead of development if release is true
     root_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(root_dir, "frontend/build")
 
     _streamlit_card = components.declare_component(
```

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/asset-manifest.json` & `streamlit-card-0.0.61/streamlit_card/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/bootstrap.min.css` & `streamlit-card-0.0.61/streamlit_card/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/bootstrap.min.css.map` & `streamlit-card-0.0.61/streamlit_card/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/index.html` & `streamlit-card-0.0.61/streamlit_card/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/service-worker.js` & `streamlit-card-0.0.61/streamlit_card/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js` & `streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js.map` & `streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/main.9d157205.chunk.js` & `streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/main.9d157205.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/main.9d157205.chunk.js.map` & `streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/main.9d157205.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js` & `streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map` & `streamlit-card-0.0.61/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-0.0.6/streamlit_card.egg-info/PKG-INFO` & `streamlit-card-0.0.61/streamlit_card.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-card
-Version: 0.0.6
+Version: 0.0.61
 Summary: A streamlit component, to make UI cards
 Home-page: https://github.com/gamcoh/st-card
 Author: gamcoh
 Author-email: cohengamliel8@gmail.com
 Keywords: card streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-card-0.0.6/streamlit_card.egg-info/SOURCES.txt` & `streamlit-card-0.0.61/streamlit_card.egg-info/SOURCES.txt`

 * *Files identical despite different names*

