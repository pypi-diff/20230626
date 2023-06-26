# Comparing `tmp/pyclamp-0.0.1.tar.gz` & `tmp/pyclamp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclamp-0.0.1.tar", last modified: Mon Jun 26 19:45:16 2023, max compression
+gzip compressed data, was "pyclamp-0.0.2.tar", last modified: Mon Jun 26 20:28:25 2023, max compression
```

## Comparing `pyclamp-0.0.1.tar` & `pyclamp-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-06-26 19:45:16.872779 pyclamp-0.0.1/
--rw-r--r--   0 marcel     (501) staff       (20)     3088 2023-06-26 14:49:16.000000 pyclamp-0.0.1/.gitignore
--rw-r--r--   0 marcel     (501) staff       (20)     1077 2023-06-25 18:53:47.000000 pyclamp-0.0.1/LICENSE
--rw-r--r--   0 marcel     (501) staff       (20)     8195 2023-06-26 19:45:16.872607 pyclamp-0.0.1/PKG-INFO
--rw-r--r--   0 marcel     (501) staff       (20)     7447 2023-06-26 19:15:06.000000 pyclamp-0.0.1/README.md
-drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-06-26 19:45:16.871583 pyclamp-0.0.1/pyclamp/
--rw-r--r--   0 marcel     (501) staff       (20)    24978 2023-06-26 18:01:11.000000 pyclamp-0.0.1/pyclamp/DataModel.py
--rw-r--r--   0 marcel     (501) staff       (20)     9998 2023-06-23 17:52:10.000000 pyclamp-0.0.1/pyclamp/PyQtTreeModel.py
--rw-r--r--   0 marcel     (501) staff       (20)        0 2023-06-26 18:27:58.000000 pyclamp-0.0.1/pyclamp/__init__.py
--rw-r--r--   0 marcel     (501) staff       (20)      324 2023-06-26 18:27:59.000000 pyclamp-0.0.1/pyclamp/__main__.py
--rw-r--r--   0 marcel     (501) staff       (20)    19340 2015-02-27 00:18:34.000000 pyclamp-0.0.1/pyclamp/heka_reader.py
--rw-r--r--   0 marcel     (501) staff       (20)    92278 2023-06-26 18:33:08.000000 pyclamp-0.0.1/pyclamp/pyCLAMP.py
-drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-06-26 19:45:16.872377 pyclamp-0.0.1/pyclamp.egg-info/
--rw-r--r--   0 marcel     (501) staff       (20)     8195 2023-06-26 19:45:16.000000 pyclamp-0.0.1/pyclamp.egg-info/PKG-INFO
--rw-r--r--   0 marcel     (501) staff       (20)      319 2023-06-26 19:45:16.000000 pyclamp-0.0.1/pyclamp.egg-info/SOURCES.txt
--rw-r--r--   0 marcel     (501) staff       (20)        1 2023-06-26 19:45:16.000000 pyclamp-0.0.1/pyclamp.egg-info/dependency_links.txt
--rw-r--r--   0 marcel     (501) staff       (20)       44 2023-06-26 19:45:16.000000 pyclamp-0.0.1/pyclamp.egg-info/requires.txt
--rw-r--r--   0 marcel     (501) staff       (20)        8 2023-06-26 19:45:16.000000 pyclamp-0.0.1/pyclamp.egg-info/top_level.txt
--rw-r--r--   0 marcel     (501) staff       (20)       38 2023-06-26 19:45:16.872833 pyclamp-0.0.1/setup.cfg
--rw-r--r--   0 marcel     (501) staff       (20)     1217 2023-06-26 19:45:02.000000 pyclamp-0.0.1/setup.py
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-06-26 20:28:25.581216 pyclamp-0.0.2/
+-rw-r--r--   0 marcel     (501) staff       (20)     3088 2023-06-26 14:49:16.000000 pyclamp-0.0.2/.gitignore
+-rw-r--r--   0 marcel     (501) staff       (20)     1077 2023-06-25 18:53:47.000000 pyclamp-0.0.2/LICENSE
+-rw-r--r--   0 marcel     (501) staff       (20)     8205 2023-06-26 20:28:25.581041 pyclamp-0.0.2/PKG-INFO
+-rw-r--r--   0 marcel     (501) staff       (20)     7457 2023-06-26 20:23:36.000000 pyclamp-0.0.2/README.md
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-06-26 20:28:25.580148 pyclamp-0.0.2/pyclamp/
+-rw-r--r--   0 marcel     (501) staff       (20)    24978 2023-06-26 18:01:11.000000 pyclamp-0.0.2/pyclamp/DataModel.py
+-rw-r--r--   0 marcel     (501) staff       (20)     9998 2023-06-23 17:52:10.000000 pyclamp-0.0.2/pyclamp/PyQtTreeModel.py
+-rw-r--r--   0 marcel     (501) staff       (20)        0 2023-06-26 18:27:58.000000 pyclamp-0.0.2/pyclamp/__init__.py
+-rw-r--r--   0 marcel     (501) staff       (20)      332 2023-06-26 20:17:06.000000 pyclamp-0.0.2/pyclamp/__main__.py
+-rw-r--r--   0 marcel     (501) staff       (20)    19340 2015-02-27 00:18:34.000000 pyclamp-0.0.2/pyclamp/heka_reader.py
+-rw-r--r--   0 marcel     (501) staff       (20)    92286 2023-06-26 20:23:09.000000 pyclamp-0.0.2/pyclamp/pyCLAMP.py
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-06-26 20:28:25.580824 pyclamp-0.0.2/pyclamp.egg-info/
+-rw-r--r--   0 marcel     (501) staff       (20)     8205 2023-06-26 20:28:25.000000 pyclamp-0.0.2/pyclamp.egg-info/PKG-INFO
+-rw-r--r--   0 marcel     (501) staff       (20)      319 2023-06-26 20:28:25.000000 pyclamp-0.0.2/pyclamp.egg-info/SOURCES.txt
+-rw-r--r--   0 marcel     (501) staff       (20)        1 2023-06-26 20:28:25.000000 pyclamp-0.0.2/pyclamp.egg-info/dependency_links.txt
+-rw-r--r--   0 marcel     (501) staff       (20)       44 2023-06-26 20:28:25.000000 pyclamp-0.0.2/pyclamp.egg-info/requires.txt
+-rw-r--r--   0 marcel     (501) staff       (20)        8 2023-06-26 20:28:25.000000 pyclamp-0.0.2/pyclamp.egg-info/top_level.txt
+-rw-r--r--   0 marcel     (501) staff       (20)       38 2023-06-26 20:28:25.581261 pyclamp-0.0.2/setup.cfg
+-rw-r--r--   0 marcel     (501) staff       (20)     1217 2023-06-26 20:28:07.000000 pyclamp-0.0.2/setup.py
```

### Comparing `pyclamp-0.0.1/.gitignore` & `pyclamp-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyclamp-0.0.1/LICENSE` & `pyclamp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclamp-0.0.1/PKG-INFO` & `pyclamp-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclamp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Time series recordings analysis in Python with UI similar to pCLAMP.
 Home-page: https://github.com/marcel-goldschen-ohm/pyCLAMP
 Download-URL: 
 Author: Marcel Goldschen-Ohm
 Author-email: goldschen-ohm@utexas.edu
 Maintainer: Marcel Goldschen-Ohm
 Maintainer-email: goldschen-ohm@utexas.edu
@@ -49,15 +49,15 @@
 * [scipy](https://scipy.org)
 * [lmfit](https://lmfit.github.io/lmfit-py/)
 * [PyQt6](https://pypi.org/project/PyQt6/)
 * [pyqtgraph](https://www.pyqtgraph.org)
 * [qtawesome](https://github.com/spyder-ide/qtawesome)
 
 # Run the pyCLAMP UI
-Just run the command `pyclamp` to bring up the UI.
+Just run the command `python -m pyclamp` to bring up the UI.
 
 # pyCLAMP Data Structure
 - Data is stored as nested dictionaries or lists of dictionaries for maximum flexiblity and extensibility.
     - Need new functionality? Just add a new key at whichever level of the heirarchy is appropriate.
     - The data is entirely composed only of `dict`, `list`, `str`, `int`, `float`, and numpy `ndarray` values and thus can be easily serialized to JSON, .MAT, etc.
     - The data is entirely self-describing and can be easily explored and manipulated independent of the UI or any other code in this package.
 - Data series traces are organized heirarchically by episode, channel, trace which should cover most experimental recording paradigms.
```

### Comparing `pyclamp-0.0.1/README.md` & `pyclamp-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 * [scipy](https://scipy.org)
 * [lmfit](https://lmfit.github.io/lmfit-py/)
 * [PyQt6](https://pypi.org/project/PyQt6/)
 * [pyqtgraph](https://www.pyqtgraph.org)
 * [qtawesome](https://github.com/spyder-ide/qtawesome)
 
 # Run the pyCLAMP UI
-Just run the command `pyclamp` to bring up the UI.
+Just run the command `python -m pyclamp` to bring up the UI.
 
 # pyCLAMP Data Structure
 - Data is stored as nested dictionaries or lists of dictionaries for maximum flexiblity and extensibility.
     - Need new functionality? Just add a new key at whichever level of the heirarchy is appropriate.
     - The data is entirely composed only of `dict`, `list`, `str`, `int`, `float`, and numpy `ndarray` values and thus can be easily serialized to JSON, .MAT, etc.
     - The data is entirely self-describing and can be easily explored and manipulated independent of the UI or any other code in this package.
 - Data series traces are organized heirarchically by episode, channel, trace which should cover most experimental recording paradigms.
```

### Comparing `pyclamp-0.0.1/pyclamp/DataModel.py` & `pyclamp-0.0.2/pyclamp/DataModel.py`

 * *Files identical despite different names*

### Comparing `pyclamp-0.0.1/pyclamp/PyQtTreeModel.py` & `pyclamp-0.0.2/pyclamp/PyQtTreeModel.py`

 * *Files identical despite different names*

### Comparing `pyclamp-0.0.1/pyclamp/heka_reader.py` & `pyclamp-0.0.2/pyclamp/heka_reader.py`

 * *Files identical despite different names*

### Comparing `pyclamp-0.0.1/pyclamp/pyCLAMP.py` & `pyclamp-0.0.2/pyclamp/pyCLAMP.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 import lmfit  # for curve fitting
 import PyQt6  # for the UI
 from PyQt6.QtCore import *
 from PyQt6.QtGui import *
 from PyQt6.QtWidgets import *
 import pyqtgraph as pg  # for plots: https://www.pyqtgraph.org
 import qtawesome as qta  # for some nice icons: https://github.com/spyder-ide/qtawesome
-from DataModel import *  # !!! defines the data model for pyCLAMP
+from .DataModel import *  # !!! defines the data model for pyCLAMP
 
 try:
     # OPTIONAL: For importing HEKA data files.
     # https://github.com/campagnola/heka_reader
     # e.g., Just put heka_reader.py in the same directory as this file.
-    import heka_reader
+    from . import heka_reader
 except ImportError:
     heka_reader = None
 
 
 pg.setConfigOption('background', (200, 200, 200))  # Default background for plots.
 pg.setConfigOption('foreground', (0, 0, 0))   # Default foreground color for text, lines, axes, etc.
```

### Comparing `pyclamp-0.0.1/pyclamp.egg-info/PKG-INFO` & `pyclamp-0.0.2/pyclamp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclamp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Time series recordings analysis in Python with UI similar to pCLAMP.
 Home-page: https://github.com/marcel-goldschen-ohm/pyCLAMP
 Download-URL: 
 Author: Marcel Goldschen-Ohm
 Author-email: goldschen-ohm@utexas.edu
 Maintainer: Marcel Goldschen-Ohm
 Maintainer-email: goldschen-ohm@utexas.edu
@@ -49,15 +49,15 @@
 * [scipy](https://scipy.org)
 * [lmfit](https://lmfit.github.io/lmfit-py/)
 * [PyQt6](https://pypi.org/project/PyQt6/)
 * [pyqtgraph](https://www.pyqtgraph.org)
 * [qtawesome](https://github.com/spyder-ide/qtawesome)
 
 # Run the pyCLAMP UI
-Just run the command `pyclamp` to bring up the UI.
+Just run the command `python -m pyclamp` to bring up the UI.
 
 # pyCLAMP Data Structure
 - Data is stored as nested dictionaries or lists of dictionaries for maximum flexiblity and extensibility.
     - Need new functionality? Just add a new key at whichever level of the heirarchy is appropriate.
     - The data is entirely composed only of `dict`, `list`, `str`, `int`, `float`, and numpy `ndarray` values and thus can be easily serialized to JSON, .MAT, etc.
     - The data is entirely self-describing and can be easily explored and manipulated independent of the UI or any other code in this package.
 - Data series traces are organized heirarchically by episode, channel, trace which should cover most experimental recording paradigms.
```

### Comparing `pyclamp-0.0.1/setup.py` & `pyclamp-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
 
     ### Metadata
 
     name='pyclamp',
 
-    version='0.0.1',
+    version='0.0.2',
 
     description='Time series recordings analysis in Python with UI similar to pCLAMP.',
 
     long_description=(HERE / "README.md").read_text(),
     long_description_content_type = "text/markdown",
 
     url='https://github.com/marcel-goldschen-ohm/pyCLAMP',
```

