# Comparing `tmp/reixs-0.5.9.tar.gz` & `tmp/reixs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reixs-0.5.9.tar", last modified: Fri May 12 22:16:50 2023, max compression
+gzip compressed data, was "reixs-0.6.0.tar", last modified: Mon Jun 26 16:13:34 2023, max compression
```

## Comparing `reixs-0.5.9.tar` & `reixs-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:16:50.313173 reixs-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-12 22:16:39.000000 reixs-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-12 22:16:50.313173 reixs-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-12 22:16:39.000000 reixs-0.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 22:16:39.000000 reixs-0.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-12 22:16:50.313173 reixs-0.5.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:16:50.309173 reixs-0.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:16:50.313173 reixs-0.5.9/src/reixs/
--rw-r--r--   0 runner    (1001) docker     (123)    57479 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (123)    33022 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/ReadData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/add_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/beamline_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/mca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/rixs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/rsxs_mcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/rsxs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/sca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/simplemath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/spec_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-12 22:16:39.000000 reixs-0.5.9/src/reixs/xeol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:16:50.313173 reixs-0.5.9/src/reixs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-12 22:16:50.000000 reixs-0.5.9/src/reixs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-12 22:16:50.000000 reixs-0.5.9/src/reixs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:16:50.000000 reixs-0.5.9/src/reixs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-12 22:16:50.000000 reixs-0.5.9/src/reixs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 22:16:50.000000 reixs-0.5.9/src/reixs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:13:34.278690 reixs-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-26 16:13:22.000000 reixs-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-26 16:13:34.278690 reixs-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-26 16:13:22.000000 reixs-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 16:13:22.000000 reixs-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-26 16:13:34.278690 reixs-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:13:34.274690 reixs-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:13:34.278690 reixs-0.6.0/src/reixs/
+-rw-r--r--   0 runner    (1001) docker     (123)    58552 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32990 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/ReadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/add_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/beamline_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/rixs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/rsxs_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/rsxs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/sca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/simplemath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/spec_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-26 16:13:22.000000 reixs-0.6.0/src/reixs/xeol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:13:34.278690 reixs-0.6.0/src/reixs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-26 16:13:34.000000 reixs-0.6.0/src/reixs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-26 16:13:34.000000 reixs-0.6.0/src/reixs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:13:34.000000 reixs-0.6.0/src/reixs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 16:13:34.000000 reixs-0.6.0/src/reixs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 16:13:34.000000 reixs-0.6.0/src/reixs.egg-info/top_level.txt
```

### Comparing `reixs-0.5.9/LICENSE` & `reixs-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/PKG-INFO` & `reixs-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.9
+Version: 0.6.0
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.9/README.md` & `reixs-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/setup.cfg` & `reixs-0.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reixs
-version = 0.5.9
+version = 0.6.0
 author = Patrick Braun
 author_email = patrick.braun@usask.ca
 description = Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pmb399/REIXSAnalysis
 project_urls =
```

### Comparing `reixs-0.5.9/src/reixs/LoadData.py` & `reixs-0.6.0/src/reixs/LoadData.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import pandas as pd
 from scipy.interpolate import interp1d, interp2d
 
 # Plotting
 from bokeh.io import push_notebook
 from bokeh.plotting import show, figure
-from bokeh.models import ColumnDataSource, HoverTool, LinearColorMapper, ColorBar, Span, Label
+from bokeh.models import ColumnDataSource, HoverTool, LinearColorMapper, LogColorMapper, ColorBar, Span, Label
 
 # Utilities
 import os
 from collections import defaultdict
 import io
 import shutil
 
@@ -240,14 +240,16 @@
 
         Parameters
         ----------
         linewidth : int, optional
         title : string, optional
         xlabel : string, optional
         ylabel : string, optional
+        plot_height : int, optional
+        plot_width : int, optional
         """
 
         # Organize all data assosciated with object in sorted dictionary.
         plot_data = defaultdict(list)
         for i, val in enumerate(self.data):
             for k, v in val.items():
                 plot_data["x_stream"].append(v.x_stream)
@@ -738,32 +740,64 @@
         pos_y : float
         text : string
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
         self.plot_labels.append([pos_x, pos_y, text, kwargs])
 
-    def plot(self, title=None, kind='Image', xlabel=None, ylabel=None, plot_height=600, plot_width=600):
-        """Plot all data assosciated with class instance/object."""
+    def plot(self, title=None, kind='Image', xlabel=None, ylabel=None, plot_height=600, plot_width=600, 
+            vmin=None, vmax=None, colormap = "linear"):
+        """
+        Plot all data assosciated with class instance/object.
 
+        Parameters
+        ----------
+        title : string, optional
+        kind : string, optional
+        xlabel : string, optional
+        ylabel : string, optional
+        plot_height : int, optional
+        plot_width : int, optional
+        vmin : float, optional
+        vmax : float, optional
+        colormap : string
+            Use: "linear" or "log"
+        """
         # Iterate over the one (1) scan in object - this is for legacy reason and shall be removed in the future.
         for i, val in enumerate(self.data):
             for k, v in val.items():
 
                 # Create the figure
                 p = figure(height=plot_height, width=plot_width, tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")],
                            tools="pan,wheel_zoom,box_zoom,reset,hover,crosshair,save")
                 p.x_range.range_padding = p.y_range.range_padding = 0
 
                 # Gridded scales now calculated directly during the MCA load and only need to be referenced here
 
                 # must give a vector of image data for image parameter
-                color_mapper = LinearColorMapper(palette="Viridis256",
-                                                 low=v.new_z.min(),
-                                                 high=v.new_z.max())
+                if vmin == None:
+                    mapper_low = v.new_z.min()
+                else:
+                    mapper_low = vmin
+
+                if vmax == None:
+                    mapper_high = v.new_z.max()
+                else:
+                    mapper_high = vmax
+
+                if colormap == "linear":
+                    myMapper = LinearColorMapper
+                elif colormap == "log":
+                    myMapper = LogColorMapper
+                else:
+                    raise UserWarning("Only 'linear' and 'log' implemented.")
+
+                color_mapper = myMapper(palette="Viridis256",
+                                                 low=mapper_low,
+                                                 high=mapper_high)
 
                 # Plot image and use limits as given by even grid.
                 p.image(image=[v.new_z], x=v.xmin, y=v.ymin, dw=v.xmax-v.xmin,
                         dh=v.ymax-v.ymin, color_mapper=color_mapper, level="image")
                 p.grid.grid_line_width = 0.5
 
                 # Defining properties of color mapper
```

### Comparing `reixs-0.5.9/src/reixs/ReadData.py` & `reixs-0.6.0/src/reixs/ReadData.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,19 +129,19 @@
                             f[f'{my.scan}/{self.REIXSconfig["HDF5_sdd_energy"]}'])
                     except:
                         warnings.warn(
                             "Could not load SDD data / SDD energy scale")
 
                     try:
                         my.xeol_data = np.array(
-                            f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_data"]}'], dtype=np.float)
+                            f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_data"]}'])
                         my.xeol_energy = np.array(
                             f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_energy"]}'])
                         my.xeol_background = np.array(
-                            f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_background"]}'], dtype=np.float)
+                            f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_background"]}'])
 
                     except:
                         warnings.warn(
                             "Could not load XEOL data / XEOL emission scale")
 
                     try:
                         my.mcp_data = np.transpose(
```

### Comparing `reixs-0.5.9/src/reixs/add_subtract.py` & `reixs-0.6.0/src/reixs/add_subtract.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/beamline_info.py` & `reixs-0.6.0/src/reixs/beamline_info.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/mca.py` & `reixs-0.6.0/src/reixs/mca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/mesh.py` & `reixs-0.6.0/src/reixs/mesh.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/parser.py` & `reixs-0.6.0/src/reixs/parser.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/rixs_readutil.py` & `reixs-0.6.0/src/reixs/rixs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/rsxs_mcp.py` & `reixs-0.6.0/src/reixs/rsxs_mcp.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/rsxs_readutil.py` & `reixs-0.6.0/src/reixs/rsxs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/sca.py` & `reixs-0.6.0/src/reixs/sca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/simplemath.py` & `reixs-0.6.0/src/reixs/simplemath.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,22 +160,37 @@
     xmin = x_data.min()
     xmax = x_data.max()
     ymin = y_data.min()
     ymax = y_data.max()
     zmin = z_data.min()
     zmax = z_data.max()
 
+    if xmin == x_data[0] and xmax == x_data[-1]:
+        pass
+    else:
+        print("You likely scanned backwards. Converting image axis...")
+        xmax = x_data.min()
+        xmin = x_data.max()
+
+    if ymin == y_data[0] and ymax == y_data[-1]:
+        pass
+    else:
+        print("You likely scanned backwards. Converting image axis...")
+        ymax = y_data.min()
+        ymin = y_data.max()
+
     xunique = np.unique(x_data)
     yunique = np.unique(y_data)
 
     xbin = len(xunique)
     ybin = len(yunique)
 
     new_z, xedge, yedge = np.histogram2d(x_data, y_data, bins=[xbin, ybin], range=[
                                             [xmin, xmax], [ymin, ymax]], weights=z_data)
+    new_z = np.transpose(new_z)
 
     return xmin, xmax, ymin, ymax, xedge, yedge, new_z, zmin, zmax
 
 def bin_data(x_data,y_data,binsize):
     """Reduce noise by averaging data points via binning mechanisms
     
         Parameters
```

### Comparing `reixs-0.5.9/src/reixs/spec_config.py` & `reixs-0.6.0/src/reixs/spec_config.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/util.py` & `reixs-0.6.0/src/reixs/util.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs/xeol.py` & `reixs-0.6.0/src/reixs/xeol.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.9/src/reixs.egg-info/PKG-INFO` & `reixs-0.6.0/src/reixs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.9
+Version: 0.6.0
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.9/src/reixs.egg-info/SOURCES.txt` & `reixs-0.6.0/src/reixs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

