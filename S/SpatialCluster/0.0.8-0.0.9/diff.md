# Comparing `tmp/SpatialCluster-0.0.8.tar.gz` & `tmp/SpatialCluster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpatialCluster-0.0.8.tar", last modified: Wed Nov 24 20:36:01 2021, max compression
+gzip compressed data, was "SpatialCluster-0.0.9.tar", last modified: Wed Nov 24 21:12:00 2021, max compression
```

## Comparing `SpatialCluster-0.0.8.tar` & `SpatialCluster-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2021-11-24 20:36:01.424029 SpatialCluster-0.0.8/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1103 2021-11-23 22:55:25.000000 SpatialCluster-0.0.8/LICENSE
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      605 2021-11-24 20:36:01.422506 SpatialCluster-0.0.8/PKG-INFO
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      220 2021-11-23 23:51:12.000000 SpatialCluster-0.0.8/README.md
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2021-11-24 20:36:01.409507 SpatialCluster-0.0.8/SpatialCluster/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)    17728 2021-11-24 20:17:22.000000 SpatialCluster-0.0.8/SpatialCluster/DMoN.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      208 2021-11-24 20:35:33.000000 SpatialCluster-0.0.8/SpatialCluster/__init__.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      198 2021-11-24 19:45:31.000000 SpatialCluster-0.0.8/SpatialCluster/constants.py
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)     5462 2021-11-24 20:35:20.000000 SpatialCluster-0.0.8/SpatialCluster/core.py
-drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2021-11-24 20:36:01.419519 SpatialCluster-0.0.8/SpatialCluster.egg-info/
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      605 2021-11-24 20:36:01.000000 SpatialCluster-0.0.8/SpatialCluster.egg-info/PKG-INFO
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      331 2021-11-24 20:36:01.000000 SpatialCluster-0.0.8/SpatialCluster.egg-info/SOURCES.txt
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)        1 2021-11-24 20:36:01.000000 SpatialCluster-0.0.8/SpatialCluster.egg-info/dependency_links.txt
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)       41 2021-11-24 20:36:01.000000 SpatialCluster-0.0.8/SpatialCluster.egg-info/requires.txt
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)       15 2021-11-24 20:36:01.000000 SpatialCluster-0.0.8/SpatialCluster.egg-info/top_level.txt
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      108 2021-11-23 23:33:31.000000 SpatialCluster-0.0.8/pyproject.toml
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)       38 2021-11-24 20:36:01.424029 SpatialCluster-0.0.8/setup.cfg
--rwxrwxrwx   0 aksel     (1000) aksel     (1000)      840 2021-11-24 20:35:37.000000 SpatialCluster-0.0.8/setup.py
+drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2021-11-24 21:12:00.113873 SpatialCluster-0.0.9/
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1103 2021-11-23 22:55:25.000000 SpatialCluster-0.0.9/LICENSE
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      836 2021-11-24 21:12:00.111904 SpatialCluster-0.0.9/PKG-INFO
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      220 2021-11-23 23:51:12.000000 SpatialCluster-0.0.9/README.md
+drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2021-11-24 21:12:00.093952 SpatialCluster-0.0.9/SpatialCluster/
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)    17728 2021-11-24 20:17:22.000000 SpatialCluster-0.0.9/SpatialCluster/DMoN.py
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      208 2021-11-24 21:02:09.000000 SpatialCluster-0.0.9/SpatialCluster/__init__.py
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      198 2021-11-24 19:45:31.000000 SpatialCluster-0.0.9/SpatialCluster/constants.py
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)     5462 2021-11-24 20:35:20.000000 SpatialCluster-0.0.9/SpatialCluster/core.py
+drwxrwxrwx   0 aksel     (1000) aksel     (1000)        0 2021-11-24 21:12:00.109874 SpatialCluster-0.0.9/SpatialCluster.egg-info/
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      836 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/PKG-INFO
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      331 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)        1 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)       41 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/requires.txt
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)       15 2021-11-24 21:12:00.000000 SpatialCluster-0.0.9/SpatialCluster.egg-info/top_level.txt
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)      108 2021-11-23 23:33:31.000000 SpatialCluster-0.0.9/pyproject.toml
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)       38 2021-11-24 21:12:00.113873 SpatialCluster-0.0.9/setup.cfg
+-rwxrwxrwx   0 aksel     (1000) aksel     (1000)     1124 2021-11-24 21:02:53.000000 SpatialCluster-0.0.9/setup.py
```

### Comparing `SpatialCluster-0.0.8/LICENSE` & `SpatialCluster-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SpatialCluster-0.0.8/PKG-INFO` & `SpatialCluster-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,39 @@
 Metadata-Version: 2.1
 Name: SpatialCluster
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spatial cluster package
 Home-page: https://github.com/AxlKings/SpatialCluster
 Author: AxelReyesO (Axel Reyes O)
 Author-email: <axel.reyes@sansano.usm.cl>
-License: UNKNOWN
+License: MIT
 Keywords: python spatial urban cluster
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-UNKNOWN
+<h1 align="center">SpatialCluster</h1>
+
+<p align="center">
+    <em>
+        Create Urban Maps
+    </em>
+</p>
+
+
+
+## Installation
+
+Install using `pip`!
+
+```sh
+$ pip install SpatialCluster
+```
+
+## To do...
```

### Comparing `SpatialCluster-0.0.8/SpatialCluster/DMoN.py` & `SpatialCluster-0.0.9/SpatialCluster/DMoN.py`

 * *Files identical despite different names*

### Comparing `SpatialCluster-0.0.8/SpatialCluster/core.py` & `SpatialCluster-0.0.9/SpatialCluster/core.py`

 * *Files identical despite different names*

### Comparing `SpatialCluster-0.0.8/SpatialCluster.egg-info/PKG-INFO` & `SpatialCluster-0.0.9/SpatialCluster.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,39 @@
 Metadata-Version: 2.1
 Name: SpatialCluster
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spatial cluster package
 Home-page: https://github.com/AxlKings/SpatialCluster
 Author: AxelReyesO (Axel Reyes O)
 Author-email: <axel.reyes@sansano.usm.cl>
-License: UNKNOWN
+License: MIT
 Keywords: python spatial urban cluster
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-UNKNOWN
+<h1 align="center">SpatialCluster</h1>
+
+<p align="center">
+    <em>
+        Create Urban Maps
+    </em>
+</p>
+
+
+
+## Installation
+
+Install using `pip`!
+
+```sh
+$ pip install SpatialCluster
+```
+
+## To do...
```

### Comparing `SpatialCluster-0.0.8/setup.py` & `SpatialCluster-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+# read the contents of your README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
+VERSION = '0.0.9'
 DESCRIPTION = 'Spatial cluster package'
 
 # Setting up
 setup(
     name="SpatialCluster",
     version=VERSION,
     author="AxelReyesO (Axel Reyes O)",
     author_email="<axel.reyes@sansano.usm.cl>",
     description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['tensorflow','scipy','numpy','matplotlib','folium'],
     url="https://github.com/AxlKings/SpatialCluster",
     keywords='python spatial urban cluster',
+    license='MIT',
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

