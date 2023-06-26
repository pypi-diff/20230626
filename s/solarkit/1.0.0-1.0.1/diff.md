# Comparing `tmp/solarkit-1.0.0.tar.gz` & `tmp/solarkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarkit-1.0.0.tar", last modified: Mon May 22 17:57:58 2023, max compression
+gzip compressed data, was "solarkit-1.0.1.tar", last modified: Mon Jun 26 10:29:29 2023, max compression
```

## Comparing `solarkit-1.0.0.tar` & `solarkit-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 17:57:58.170034 solarkit-1.0.0/
--rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2054 2023-05-22 17:57:58.169534 solarkit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1449 2023-05-22 17:56:15.000000 solarkit-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 17:57:58.170535 solarkit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1062 2023-05-22 17:57:31.000000 solarkit-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:57:58.163535 solarkit-1.0.0/solarkit/
--rw-rw-rw-   0        0        0      290 2023-05-08 17:26:35.000000 solarkit-1.0.0/solarkit/__init__.py
--rw-rw-rw-   0        0        0     3632 2023-05-22 17:14:51.000000 solarkit-1.0.0/solarkit/planet.py
--rw-rw-rw-   0        0        0     4657 2023-05-22 17:33:44.000000 solarkit-1.0.0/solarkit/solar_system.py
--rw-rw-rw-   0        0        0     2099 2023-05-08 17:26:57.000000 solarkit-1.0.0/solarkit/utils.py
--rw-rw-rw-   0        0        0    14098 2023-05-22 17:51:27.000000 solarkit-1.0.0/solarkit/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:57:58.168534 solarkit-1.0.0/solarkit.egg-info/
--rw-rw-rw-   0        0        0     2054 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 17:57:58.000000 solarkit-1.0.0/solarkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 10:29:29.176308 solarkit-1.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2054 2023-06-26 10:29:29.175808 solarkit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1449 2023-05-22 17:56:15.000000 solarkit-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 10:29:29.176807 solarkit-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2023-06-26 10:29:20.000000 solarkit-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 10:29:29.161306 solarkit-1.0.1/solarkit/
+-rw-rw-rw-   0        0        0      290 2023-05-08 17:26:35.000000 solarkit-1.0.1/solarkit/__init__.py
+-rw-rw-rw-   0        0        0     3632 2023-05-22 17:14:51.000000 solarkit-1.0.1/solarkit/planet.py
+-rw-rw-rw-   0        0        0     4657 2023-05-22 17:33:44.000000 solarkit-1.0.1/solarkit/solar_system.py
+-rw-rw-rw-   0        0        0     2099 2023-05-08 17:26:57.000000 solarkit-1.0.1/solarkit/utils.py
+-rw-rw-rw-   0        0        0    14775 2023-06-26 10:26:16.000000 solarkit-1.0.1/solarkit/viewer.py
+drwxrwxrwx   0        0        0        0 2023-06-26 10:29:29.174805 solarkit-1.0.1/solarkit.egg-info/
+-rw-rw-rw-   0        0        0     2054 2023-06-26 10:29:29.000000 solarkit-1.0.1/solarkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-26 10:29:29.000000 solarkit-1.0.1/solarkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 10:29:29.000000 solarkit-1.0.1/solarkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-26 10:29:29.000000 solarkit-1.0.1/solarkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 10:29:29.000000 solarkit-1.0.1/solarkit.egg-info/top_level.txt
```

### Comparing `solarkit-1.0.0/LICENSE` & `solarkit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solarkit-1.0.0/PKG-INFO` & `solarkit-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `solarkit-1.0.0/README.md` & `solarkit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `solarkit-1.0.0/setup.py` & `solarkit-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = "Visualise a solar system and do cool stuff with it"
 
 # Setting up
 setup(
     name="solarkit",
     version=VERSION,
     author="Carlos Lorenzo",
```

### Comparing `solarkit-1.0.0/solarkit/planet.py` & `solarkit-1.0.1/solarkit/planet.py`

 * *Files identical despite different names*

### Comparing `solarkit-1.0.0/solarkit/solar_system.py` & `solarkit-1.0.1/solarkit/solar_system.py`

 * *Files identical despite different names*

### Comparing `solarkit-1.0.0/solarkit/utils.py` & `solarkit-1.0.1/solarkit/utils.py`

 * *Files identical despite different names*

### Comparing `solarkit-1.0.0/solarkit/viewer.py` & `solarkit-1.0.1/solarkit/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ax: plt.Axes = field(init=False)
     
     tmax: float = field(init=False)
     dt: float = field(init=False)
     t: float = field(init=False, default=0)
     
     
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         
         if not self.planets_to_use:
             self.planets_to_use = list(self.system.planets.keys())
             
         
         self.system.planets = dict(sorted(self.system.planets.items(), key=lambda planet: planet[1].P))
         
@@ -58,21 +58,22 @@
         self.dt = self.tmax/2500
         
     def __str__(self) -> str:
         return f"Planets: {self.system.__str__()}\n3D: {self.compute_3D}\nAnimation FPS: {self.target_fps}"
     
     
     
-    def initialise_plotter(self, square_ratio: bool = True) -> None:
+    def initialise_plotter(self, square_ratio: bool = True, dpi: int = 1000, size: float = 8) -> None:
         """
-        Initalises the area where everythin will be drawn on. Call every time you want to draw a new model
+        Initalises the area where everything will be drawn on. Call every time you want to draw a new model
         
         Args:
-            square_ratio (bool): Set the ratio of the plot to 1:1
-        
+            square_ratio (bool): Set the ratio of the plot to 1:1. Defaults to True.
+            dpi (int): Resolution (higher dpi, more resolution). Defaults to 1000.
+            size (float): Default size (arbitrary units, higher size, larger default plot)
         """
         
         if self.compute_3D:
             self.fig: plt.figure = plt.figure()
             self.ax: plt.Axes = self.fig.add_subplot(projection='3d')
             self.ax.view_init(None, 225)
           
@@ -81,86 +82,97 @@
             
             if square_ratio:
                 #set aspect ratio to 1
                 RATIO = 1.0
                 x_left, x_right = self.ax.get_xlim()
                 y_low, y_high = self.ax.get_ylim()
                 self.ax.set_aspect(abs((x_right - x_left)/(y_low - y_high)) * RATIO)
-    
+
+        
+        self.fig.set_size_inches(size, size)
+        matplotlib.rcParams['figure.dpi'] = dpi
+        
     def server_mode(self) -> None:
         """
         Allow matplotlib to work when not in main thread (when running in server) 
         """
+        
         matplotlib.use("Agg")
     
     def close_graph(self) -> None:
         """
         Closes matplotlib tab
         """
         
         plt.close()
     
     def add_grid(self) -> None:
         """
         Adds a grid
         """
+        
         plt.grid()
     
     def add_legend(self) -> None:
         """
         Adds a legend
         """
+        
         plt.legend()
     
-    def lable_axes(self, x_lable: str = " x (AU)", y_lable: str = "y (AU)", z_lable: str = "z (AU)"):
+    def lable_axes(self, x_lable: str = " x (AU)", y_lable: str = "y (AU)", z_lable: str = "z (AU)") -> None:
         """
         Adds lables to axes. Call to override default axes' lables
 
         Args:
             x_lable (str, optional): x lable. Defaults to " x (AU)".
             y_lable (str, optional): y lable. Defaults to "y (AU)".
             z_lable (str, optional): z lable. Defaults to "z (AU)".
         """
         
         self.ax.set_xlabel(x_lable)
         self.ax.set_ylabel(y_lable)
         if self.compute_3D:
             self.ax.set_zlabel(z_lable)
     
-    def show_plot(self):
+    def show_plot(self) -> None:
         """
         Show drawn figure (calls plt.show())
         """
+        
         plt.show()
     
     def save_figure(self, path: str, filename: str) -> None:
         """
-        Save figure as image
+        Save figure as an image
 
         Args:
             path (str): directory where the image will be stored
             filename (str): name of image
         """
         
 
         if not os.path.exists(path):
             os.mkdir(path)
         
         plt.savefig(f"{path}/{filename}", dpi=250)
         
-    def get_figure_data(self) -> str:
+    def get_figure_data(self, dpi: int = 1000) -> str:
         """
         Get the figure data of Viewer object to embed into browser (for example)
+        
+        Args:
+            dpi (int): Resolution (higher dpi, more resolution). Defaults to 1000.
 
         Returns:
             str: Figure data to be embedded in html
         """
         
         imgdata = StringIO()
-        self.fig.savefig(imgdata, format='svg')
+        self.fig.savefig(imgdata, format='svg', dpi=dpi)
         imgdata.seek(0)
         
         return imgdata.getvalue()
     
            
     def plot_orbit(self, orbit_data: Dict[str, List[float]]) -> None:
         """
@@ -220,15 +232,15 @@
             self.ax.scatter(0, 0, 0, s=100, label=name, c=colour)
             
         else:
             self.ax.scatter(0, 0, s=100, label=name, c=colour)
       
 
     
-    def third_law(self):
+    def third_law(self) -> None:
         """
         Proves Kepler's third law
         """
         
         
         x = [planet.a**3 for planet in  self.system.planets.values()]
         y = [planet.P**2 for planet in  self.system.planets.values()]
@@ -273,18 +285,18 @@
         self.ax.set_xlabel('Time (years)')
         self.ax.set_ylabel('Polar Angle (radians)')
         
         plt.title('Variation of Polar Angle with Time')
         
         
     def system_orbits(self) -> None:
-        
         """
         Plot the orbits of the selected planets
         """
+        
         self.plot_centre(name="Sun", colour="y")
         
         for planet_orbit_data in self.orbit_data:
             self.plot_orbit(orbit_data=planet_orbit_data)  
         
         plt.title("Planet orbits")
         self.lable_axes()
@@ -313,21 +325,24 @@
             plt.legend()
             plt.grid()
             
             plt.pause(1/self.target_fps)
             plt.cla()
     
     
-    def spinograph(self) -> None:
+    def spinograph(self, lines_drawn: int = 1234) -> None:
         """
-        Draw a spinograph with the chosen planets        
+        Draw a spinograph with the chosen planets 
+        
+        Args:
+            lines_drawn (Optional[int]): Sets how many lines drawn will be drawn . Defaults to 1234
         """
         
         self.tmax *= 10
-        self.dt = self.tmax / 1234
+        self.dt = self.tmax / lines_drawn
         
         
         while self.t < self.tmax:
             planet_data = [planet.compute_position(compute_3D=self.compute_3D, t=self.t) for planet in self.chosen_planets]
             
             x = [data["x"] for data in planet_data]
             y = [data["y"] for data in planet_data]
```

### Comparing `solarkit-1.0.0/solarkit.egg-info/PKG-INFO` & `solarkit-1.0.1/solarkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

