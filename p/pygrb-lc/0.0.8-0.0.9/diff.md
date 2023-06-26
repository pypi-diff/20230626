# Comparing `tmp/pygrb_lc-0.0.8.tar.gz` & `tmp/pygrb_lc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrb_lc-0.0.8.tar", last modified: Sun Jun 18 21:45:47 2023, max compression
+gzip compressed data, was "pygrb_lc-0.0.9.tar", last modified: Thu Jun 22 21:24:55 2023, max compression
```

## Comparing `pygrb_lc-0.0.8.tar` & `pygrb_lc-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-18 21:45:47.950636 pygrb_lc-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-18 21:45:47.950636 pygrb_lc-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/src/pygrb_lc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/blind_search.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/crossmatching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/furie.py
--rw-r--r--   0 runner    (1001) docker     (123)    32959 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/src/pygrb_lc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-18 21:45:47.000000 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-18 21:45:47.000000 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:45:47.000000 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 21:45:47.000000 pygrb_lc-0.0.8/src/pygrb_lc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:47.946636 pygrb_lc-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/tests/test_light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-18 21:45:35.000000 pygrb_lc-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.527002 pygrb_lc-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/src/pygrb_lc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/blind_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/crossmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/furie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32983 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/src/pygrb_lc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-22 21:24:55.000000 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 21:24:55.000000 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:24:55.000000 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 21:24:55.000000 pygrb_lc-0.0.9/src/pygrb_lc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:55.531002 pygrb_lc-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/tests/test_light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-22 21:24:46.000000 pygrb_lc-0.0.9/tests/test_utils.py
```

### Comparing `pygrb_lc-0.0.8/LICENSE` & `pygrb_lc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.8/PKG-INFO` & `pygrb_lc-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pygrb_lc
-Version: 0.0.8
-Summary: Python package for GRB analysis
-Home-page: https://github.com/Jorezzz/pygrb_lc
-Author: Mozgunov Georgiy
-Author-email: georgiy99@bk.ru
-Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pygrb_lc
 Package to load and handle GRB (Gamma-ray bursts) light curves, their furie transformations and various other functions.
 
 To install run the following command
 
 ```bash
 pip install --upgrade pygrb_lc
@@ -31,15 +16,15 @@
 Main object in this package is LightCurve object and its children. Start by creating one
 ```python
 from pygrb_lc.light_curves import LightCurve # base class for ligth curve
 
 lc = LightCurve()
 print(lc)
 ```
-It is created but empty, semplest way to provide data is by data argument, that requires numpy.ndarray with 2 (time, signal) or 4 (time, time_err, signal, signal_err) columns
+It is created but empty, semplest way to provide data is by ```data``` argument, that requires ```numpy.ndarray``` with 2 (time, signal) or 4 (time, time_err, signal, signal_err) columns
 ```python
 import numpy as np
 
 data = np.loadtxt('test.txt')
 lc = LightCurve(data = data)
 print(lc)
 ```
@@ -51,15 +36,15 @@
 from pygrb_lc.light_curves import SPI_ACS_LightCurve, GBM_LightCurve
 
 lc1 = SPI_ACS_LightCurve('2020-01-01 00:00:00', 500, loading_method = 'web')
 lc2 = GBM_LightCurve('2020-01-01 00:00:00', ['na'], duration = 500, loading_method = 'web')
 ```
 ## Furie transformations
 
-Furie transformation is performed by FurieTransformation class. It requires LightCurve object as an argument
+Furie transformation is performed by FurieLightCurve class. It requires LightCurve object as an argument
 ```python
 from pygrb_lc.furie import FurieLightCurve
 
 lc = LightCurve(data = np.loadtxt('test.txt'))
 flc = FurieLightCurve(lc, interval_t90 = (0, 10))
 
 flc.plot()
@@ -67,7 +52,14 @@
 
 All classes have plot method, you can provide matplotlib.pyplot.Axes object as an argument to plot on existing plot
 ```python
 fig,(ax1,ax2) = plt.subplots(2,1)
 lc.plot(ax = ax1)
 flc.plot(ax = ax2)
 ```
+
+
+# Roadmap
+Add support of main GRB catalogues and their connection with light curves. 
+Create Catalogue class that can be compared and intersected to other. 
+Add support of spectra (based on current ```photon_data``` in GBM_LightCurve class)
+Add typical functions for approximation: Band function, power law, etc. and their interaction with ```LightCurve``` and ```FurieLightCurve``` classes.
```

### Comparing `pygrb_lc-0.0.8/README.md` & `pygrb_lc-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pygrb_lc
+Version: 0.0.9
+Summary: Python package for GRB analysis
+Home-page: https://github.com/Jorezzz/pygrb_lc
+Author: Mozgunov Georgiy
+Author-email: georgiy99@bk.ru
+Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pygrb_lc
 Package to load and handle GRB (Gamma-ray bursts) light curves, their furie transformations and various other functions.
 
 To install run the following command
 
 ```bash
 pip install --upgrade pygrb_lc
@@ -16,15 +31,15 @@
 Main object in this package is LightCurve object and its children. Start by creating one
 ```python
 from pygrb_lc.light_curves import LightCurve # base class for ligth curve
 
 lc = LightCurve()
 print(lc)
 ```
-It is created but empty, semplest way to provide data is by data argument, that requires numpy.ndarray with 2 (time, signal) or 4 (time, time_err, signal, signal_err) columns
+It is created but empty, semplest way to provide data is by ```data``` argument, that requires ```numpy.ndarray``` with 2 (time, signal) or 4 (time, time_err, signal, signal_err) columns
 ```python
 import numpy as np
 
 data = np.loadtxt('test.txt')
 lc = LightCurve(data = data)
 print(lc)
 ```
@@ -36,23 +51,30 @@
 from pygrb_lc.light_curves import SPI_ACS_LightCurve, GBM_LightCurve
 
 lc1 = SPI_ACS_LightCurve('2020-01-01 00:00:00', 500, loading_method = 'web')
 lc2 = GBM_LightCurve('2020-01-01 00:00:00', ['na'], duration = 500, loading_method = 'web')
 ```
 ## Furie transformations
 
-Furie transformation is performed by FurieTransformation class. It requires LightCurve object as an argument
+Furie transformation is performed by FurieLightCurve class. It requires LightCurve object as an argument
 ```python
 from pygrb_lc.furie import FurieLightCurve
 
 lc = LightCurve(data = np.loadtxt('test.txt'))
 flc = FurieLightCurve(lc, interval_t90 = (0, 10))
 
 flc.plot()
 ```
 
 All classes have plot method, you can provide matplotlib.pyplot.Axes object as an argument to plot on existing plot
 ```python
 fig,(ax1,ax2) = plt.subplots(2,1)
 lc.plot(ax = ax1)
 flc.plot(ax = ax2)
-```
+```
+
+
+# Roadmap
+Add support of main GRB catalogues and their connection with light curves. 
+Create Catalogue class that can be compared and intersected to other. 
+Add support of spectra (based on current ```photon_data``` in GBM_LightCurve class)
+Add typical functions for approximation: Band function, power law, etc. and their interaction with ```LightCurve``` and ```FurieLightCurve``` classes.
```

### Comparing `pygrb_lc-0.0.8/setup.cfg` & `pygrb_lc-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygrb_lc
-version = 0.0.8
+version = 0.0.9
 author = Mozgunov Georgiy
 author_email = georgiy99@bk.ru
 description = Python package for GRB analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Jorezzz/pygrb_lc
 project_urls =
```

### Comparing `pygrb_lc-0.0.8/src/pygrb_lc/blind_search.py` & `pygrb_lc-0.0.9/src/pygrb_lc/blind_search.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.8/src/pygrb_lc/config.py` & `pygrb_lc-0.0.9/src/pygrb_lc/config.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.8/src/pygrb_lc/crossmatching.py` & `pygrb_lc-0.0.9/src/pygrb_lc/crossmatching.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.8/src/pygrb_lc/furie.py` & `pygrb_lc-0.0.9/src/pygrb_lc/furie.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.8/src/pygrb_lc/light_curves.py` & `pygrb_lc-0.0.9/src/pygrb_lc/light_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,23 +705,23 @@
         plt.axvline(t_5_low)
         plt.axvline(t_5_high)
         plt.axvline(t_95_low)
         plt.axvline(t_95_high)
 
     return t_90, (-negative_err, positive_err)
 
-def plot_gbm_all_detectors(center_time: str, duration: float, binning: float = 0.5):
+def plot_gbm_all_detectors(center_time: str, duration: float, binning: float = 0.5, **kwargs):
     detector_list = [x for x in GBM_DETECTORS if x[0] == 'n']
     data = {}
 
     fig, ax = plt.subplots(4,3,figsize=(30,30))
     ax = ax.reshape(-1,)
     for i, detector in enumerate(detector_list[:-2]):
-        lc = GBM_LightCurve(center_time, [detector], duration = duration)
-        lc.rebin(0.5).plot(ax=ax[i], label = detector)
+        lc = GBM_LightCurve(center_time, [detector], duration = duration, **kwargs)
+        lc.rebin(binning).plot(ax=ax[i], label = detector)
         signal = lc.signal
         ax[i].axhline(np.mean(signal),color = 'blue')
         ax[i].axhline(np.mean(signal)+3*np.std(signal),color = 'green')
         ax[i].axhline(np.mean(signal)-3*np.std(signal),color = 'green')
         ax[i].legend()
         data[detector] = lc
     fig.suptitle(center_time)
```

### Comparing `pygrb_lc-0.0.8/src/pygrb_lc/time.py` & `pygrb_lc-0.0.9/src/pygrb_lc/time.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.8/src/pygrb_lc/utils.py` & `pygrb_lc-0.0.9/src/pygrb_lc/utils.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.8/src/pygrb_lc.egg-info/PKG-INFO` & `pygrb_lc-0.0.9/src/pygrb_lc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb-lc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,15 @@
 Main object in this package is LightCurve object and its children. Start by creating one
 ```python
 from pygrb_lc.light_curves import LightCurve # base class for ligth curve
 
 lc = LightCurve()
 print(lc)
 ```
-It is created but empty, semplest way to provide data is by data argument, that requires numpy.ndarray with 2 (time, signal) or 4 (time, time_err, signal, signal_err) columns
+It is created but empty, semplest way to provide data is by ```data``` argument, that requires ```numpy.ndarray``` with 2 (time, signal) or 4 (time, time_err, signal, signal_err) columns
 ```python
 import numpy as np
 
 data = np.loadtxt('test.txt')
 lc = LightCurve(data = data)
 print(lc)
 ```
@@ -51,15 +51,15 @@
 from pygrb_lc.light_curves import SPI_ACS_LightCurve, GBM_LightCurve
 
 lc1 = SPI_ACS_LightCurve('2020-01-01 00:00:00', 500, loading_method = 'web')
 lc2 = GBM_LightCurve('2020-01-01 00:00:00', ['na'], duration = 500, loading_method = 'web')
 ```
 ## Furie transformations
 
-Furie transformation is performed by FurieTransformation class. It requires LightCurve object as an argument
+Furie transformation is performed by FurieLightCurve class. It requires LightCurve object as an argument
 ```python
 from pygrb_lc.furie import FurieLightCurve
 
 lc = LightCurve(data = np.loadtxt('test.txt'))
 flc = FurieLightCurve(lc, interval_t90 = (0, 10))
 
 flc.plot()
@@ -67,7 +67,14 @@
 
 All classes have plot method, you can provide matplotlib.pyplot.Axes object as an argument to plot on existing plot
 ```python
 fig,(ax1,ax2) = plt.subplots(2,1)
 lc.plot(ax = ax1)
 flc.plot(ax = ax2)
 ```
+
+
+# Roadmap
+Add support of main GRB catalogues and their connection with light curves. 
+Create Catalogue class that can be compared and intersected to other. 
+Add support of spectra (based on current ```photon_data``` in GBM_LightCurve class)
+Add typical functions for approximation: Band function, power law, etc. and their interaction with ```LightCurve``` and ```FurieLightCurve``` classes.
```

### Comparing `pygrb_lc-0.0.8/tests/test_utils.py` & `pygrb_lc-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

