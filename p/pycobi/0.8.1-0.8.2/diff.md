# Comparing `tmp/pycobi-0.8.1.tar.gz` & `tmp/pycobi-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycobi-0.8.1.tar", last modified: Mon Jun 26 20:27:44 2023, max compression
+gzip compressed data, was "pycobi-0.8.2.tar", last modified: Mon Jun 26 21:56:40 2023, max compression
```

## Comparing `pycobi-0.8.1.tar` & `pycobi-0.8.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:44.470144 pycobi-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 20:27:33.000000 pycobi-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 20:27:33.000000 pycobi-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-26 20:27:44.470144 pycobi-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-26 20:27:33.000000 pycobi-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:44.466144 pycobi-0.8.1/pycobi/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi/automated_continuation.py
--rw-r--r--   0 runner    (1001) docker     (123)    48975 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi/pycobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:44.470144 pycobi-0.8.1/pycobi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:44.470144 pycobi-0.8.1/pycobi_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi_tests/test_odesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:27:44.470144 pycobi-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 20:27:33.000000 pycobi-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:40.721067 pycobi-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 21:56:30.000000 pycobi-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 21:56:30.000000 pycobi-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-26 21:56:40.717067 pycobi-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-26 21:56:30.000000 pycobi-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:40.717067 pycobi-0.8.2/pycobi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 21:56:30.000000 pycobi-0.8.2/pycobi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-26 21:56:30.000000 pycobi-0.8.2/pycobi/automated_continuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49943 2023-06-26 21:56:30.000000 pycobi-0.8.2/pycobi/pycobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-06-26 21:56:30.000000 pycobi-0.8.2/pycobi/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:40.717067 pycobi-0.8.2/pycobi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-26 21:56:40.000000 pycobi-0.8.2/pycobi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-26 21:56:40.000000 pycobi-0.8.2/pycobi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:56:40.000000 pycobi-0.8.2/pycobi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:56:40.000000 pycobi-0.8.2/pycobi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 21:56:40.000000 pycobi-0.8.2/pycobi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 21:56:40.000000 pycobi-0.8.2/pycobi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:56:40.717067 pycobi-0.8.2/pycobi_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 21:56:30.000000 pycobi-0.8.2/pycobi_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 21:56:30.000000 pycobi-0.8.2/pycobi_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-26 21:56:30.000000 pycobi-0.8.2/pycobi_tests/test_odesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:56:40.721067 pycobi-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 21:56:30.000000 pycobi-0.8.2/setup.py
```

### Comparing `pycobi-0.8.1/LICENSE` & `pycobi-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycobi-0.8.1/PKG-INFO` & `pycobi-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobi
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python tool for parameter continuation and bifurcation analysis
 Home-page: UNKNOWN
 Author: Richard Gast
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycobi-0.8.1/README.md` & `pycobi-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pycobi-0.8.1/pycobi/__init__.py` & `pycobi-0.8.2/pycobi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 # Richard Gast et al., in preparation.
 
 """Python package for parameter continuations and bifurcation analysis via Auto-07p in Python.
 """
 
 __author__ = "Richard Gast"
 __status__ = "Development"
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 from .pycobi import ODESystem
 from .utility import get_lyapunov_exponents, get_solution_eigenvalues, fractal_dimension
 from .automated_continuation import continue_period_doubling_bf, codim2_search
```

### Comparing `pycobi-0.8.1/pycobi/automated_continuation.py` & `pycobi-0.8.2/pycobi/automated_continuation.py`

 * *Files identical despite different names*

### Comparing `pycobi-0.8.1/pycobi/pycobi.py` & `pycobi-0.8.2/pycobi/pycobi.py`

 * *Files 2% similar despite different names*

```diff
@@ -566,29 +566,32 @@
         columns = [k for k, _ in list(summary.keys())]
         keys = [key if key in columns else self._var_map_inv[key] for key in keys]
         if point:
             return summary.loc[point, keys]
         return summary.loc[:, keys]
 
     def plot_continuation(self, x: str, y: str, cont: Union[Any, str, int], ax: plt.Axes = None,
-                          force_axis_lim_update: bool = False, **kwargs) -> LineCollection:
+                          force_axis_lim_update: bool = False, bifurcation_legend: bool = True, **kwargs
+                          ) -> LineCollection:
         """Line plot of 1D/2D parameter continuations and the respective codimension 1/2 bifurcations.
 
         Parameters
         ----------
         x
             Key of the parameter/variable plotted on the x-axis.
         y
             Key of the variable/parameter plotted on the y-axis.
         cont
             Key of the solution branch to be plotted.
         ax
             Axis in which to plot the data. If not provided, a new figure will be created.
         force_axis_lim_update
             If true, the axis limits of x and y axis will be updated after creating the line plots.
+        bifurcation_legend
+            If true, a legend will be plotted that lists the type of all special solutions on a continuation curve.
         kwargs
             Additional keyword arguments that allow to control the appearance of the line plot.
 
         Returns
         -------
         LineCollection
             Line object that was created.
@@ -608,16 +611,16 @@
         else:
             results = self.extract([x, y, 'stability', 'bifurcation'], cont=cont)
 
         # plot bifurcation points
         bifurcation_point_kwargs = ['default_color', 'default_marker', 'default_size', 'custom_bf_styles',
                                     'ignore']
         kwargs_tmp = {key: kwargs.pop(key) for key in bifurcation_point_kwargs if key in kwargs}
-        ax = self.plot_bifurcation_points(solution_types=results['bifurcation'], x_vals=results[x],
-                                          y_vals=results[y], ax=ax, **kwargs_tmp)
+        bfs, labels = self.plot_bifurcation_points(solution_types=results['bifurcation'], x_vals=results[x],
+                                                   y_vals=results[y], ax=ax, **kwargs_tmp)
 
         # set title variable if passed
         tvar = kwargs.pop('title_var', None)
         if tvar:
             tvar_results = self.extract([tvar], cont=cont)
             tval = tvar_results[tvar][0]
             ax.set_title(f"{tvar} = {tval}")
@@ -629,14 +632,16 @@
         ax.autoscale()
 
         # cosmetics
         ax.tick_params(axis='both', which='major', pad=tick_pad)
         ax.set_xlabel(x, labelpad=label_pad)
         ax.set_ylabel(y, labelpad=label_pad)
         self._update_axis_lims(ax, ax_data=[x_data, y_data], padding=axislim_pad, force_update=force_axis_lim_update)
+        if bifurcation_legend:
+            ax.legend()
 
         return line_col
 
     def plot_trajectory(self, variables: Union[list, tuple], cont: Union[Any, str, int], point: Union[str, int] = None,
                         ax: plt.Axes = None, force_axis_lim_update: bool = False, cutoff: float = None, **kwargs
                         ) -> LineCollection:
         """Plot trajectory of state variables through phase space over time.
@@ -787,16 +792,16 @@
             ax.add_collection(line_col)
         ax.autoscale()
         ax.legend(points)
 
         return ax
 
     def plot_bifurcation_points(self, solution_types: DataFrame, x_vals: DataFrame, y_vals: DataFrame, ax: plt.Axes,
-                                default_color: str = 'k', default_marker: str = '*', default_size: float = 50,
-                                ignore: list = None, custom_bf_styles: dict = None) -> plt.Axes:
+                                default_color: str = 'k', default_marker: str = '*', default_size: float = 10,
+                                ignore: list = None, custom_bf_styles: dict = None) -> tuple:
         """Plot markers for special solutions at coordinates in 2D space.
 
         Parameters
         ----------
         solution_types
             Type of each solution, entries of DataFrame should be strings.
         x_vals
@@ -814,43 +819,55 @@
         ignore
             List of solution types that should not be displayed.
         custom_bf_styles
             Dictionary containing adjustments to the default bifurcation markers and colors.
 
         Returns
         -------
-        plt.Axes
-            Axis object that contains the plotted special solutions.
+        tuple
+            A 2-entry tuple of (1) a list of PathCollections that correspond to bifurcation points, and (2) a list of
+            corresponding bifurcation types.
         """
 
         if not ignore:
             ignore = []
 
         # set bifurcation styles
         if custom_bf_styles:
             for key, args in custom_bf_styles.items():
                 self.update_bifurcation_style(key, **args)
         bf_styles = self._bifurcation_styles.copy()
         plt.sca(ax)
 
         # draw bifurcation points
+        points, labels = ax.get_legend_handles_labels()
         for bf, x, y in zip(solution_types.values, x_vals.values, y_vals.values):
             if bf not in "EPMXRG" and bf not in ignore:
                 if bf in bf_styles:
                     m = bf_styles[bf]['marker']
                     c = bf_styles[bf]['color']
                 else:
                     m = default_marker
                     c = default_color
                 if y.shape and np.sum(y.shape) > 1:
-                    plt.scatter(x, y.max(), s=default_size, marker=m, c=c)
-                    plt.scatter(x, y.min(), s=default_size, marker=m, c=c)
+                    if bf not in labels:
+                        line = plt.plot(x, y.max(), markersize=default_size, marker=m, c=c, label=bf)
+                        points.append(line[0])
+                        labels.append(bf)
+                    else:
+                        plt.plot(x, y.max(), markersize=default_size, marker=m, c=c)
+                    plt.plot(x, y.min(), markersize=default_size, marker=m, c=c)
                 else:
-                    plt.scatter(x, y, s=default_size, marker=m, c=c)
-        return ax
+                    if bf not in labels:
+                        line = plt.plot(x, y, markersize=default_size, marker=m, c=c, label=bf)
+                        points.append(line[0])
+                        labels.append(bf)
+                    else:
+                        plt.plot(x, y, markersize=default_size, marker=m, c=c)
+        return points, labels
 
     def update_bifurcation_style(self, bf_type: str, marker: str = None, color: str = None) -> None:
         """Update the default marker and color of a given special solution type.
 
         Parameters
         ----------
         bf_type
```

### Comparing `pycobi-0.8.1/pycobi/utility.py` & `pycobi-0.8.2/pycobi/utility.py`

 * *Files identical despite different names*

### Comparing `pycobi-0.8.1/pycobi.egg-info/PKG-INFO` & `pycobi-0.8.2/pycobi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobi
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python tool for parameter continuation and bifurcation analysis
 Home-page: UNKNOWN
 Author: Richard Gast
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycobi-0.8.1/pycobi_tests/__init__.py` & `pycobi-0.8.2/pycobi_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pycobi-0.8.1/pycobi_tests/test_odesystem.py` & `pycobi-0.8.2/pycobi_tests/test_odesystem.py`

 * *Files identical despite different names*

### Comparing `pycobi-0.8.1/setup.py` & `pycobi-0.8.2/setup.py`

 * *Files identical despite different names*

