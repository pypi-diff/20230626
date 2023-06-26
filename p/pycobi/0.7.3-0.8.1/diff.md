# Comparing `tmp/pycobi-0.7.3.tar.gz` & `tmp/pycobi-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycobi-0.7.3.tar", last modified: Mon Oct 17 21:40:31 2022, max compression
+gzip compressed data, was "pycobi-0.8.1.tar", last modified: Mon Jun 26 20:27:44 2023, max compression
```

## Comparing `pycobi-0.7.3.tar` & `pycobi-0.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 21:40:31.202363 pycobi-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-17 21:40:06.000000 pycobi-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-17 21:40:06.000000 pycobi-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4421 2022-10-17 21:40:31.202363 pycobi-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-10-17 21:40:06.000000 pycobi-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 21:40:31.202363 pycobi-0.7.3/pycobi/
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-10-17 21:40:06.000000 pycobi-0.7.3/pycobi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7664 2022-10-17 21:40:06.000000 pycobi-0.7.3/pycobi/automated_continuation.py
--rw-r--r--   0 runner    (1001) docker     (121)    45493 2022-10-17 21:40:06.000000 pycobi-0.7.3/pycobi/pycobi.py
--rw-r--r--   0 runner    (1001) docker     (121)     8829 2022-10-17 21:40:06.000000 pycobi-0.7.3/pycobi/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 21:40:31.202363 pycobi-0.7.3/pycobi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4421 2022-10-17 21:40:31.000000 pycobi-0.7.3/pycobi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-10-17 21:40:31.000000 pycobi-0.7.3/pycobi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 21:40:31.000000 pycobi-0.7.3/pycobi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 21:40:31.000000 pycobi-0.7.3/pycobi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-17 21:40:31.000000 pycobi-0.7.3/pycobi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-17 21:40:31.000000 pycobi-0.7.3/pycobi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 21:40:31.202363 pycobi-0.7.3/pycobi_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-17 21:40:06.000000 pycobi-0.7.3/pycobi_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-10-17 21:40:06.000000 pycobi-0.7.3/pycobi_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-10-17 21:40:06.000000 pycobi-0.7.3/pycobi_tests/test_odesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-17 21:40:31.202363 pycobi-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-10-17 21:40:06.000000 pycobi-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:44.470144 pycobi-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 20:27:33.000000 pycobi-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 20:27:33.000000 pycobi-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-26 20:27:44.470144 pycobi-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-26 20:27:33.000000 pycobi-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:44.466144 pycobi-0.8.1/pycobi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi/automated_continuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48975 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi/pycobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:44.470144 pycobi-0.8.1/pycobi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 20:27:44.000000 pycobi-0.8.1/pycobi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:44.470144 pycobi-0.8.1/pycobi_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-26 20:27:33.000000 pycobi-0.8.1/pycobi_tests/test_odesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:27:44.470144 pycobi-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 20:27:33.000000 pycobi-0.8.1/setup.py
```

### Comparing `pycobi-0.7.3/LICENSE` & `pycobi-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycobi-0.7.3/PKG-INFO` & `pycobi-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobi
-Version: 0.7.3
+Version: 0.8.1
 Summary: Python tool for parameter continuation and bifurcation analysis
 Home-page: UNKNOWN
 Author: Richard Gast
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -26,29 +26,26 @@
 # PyCoBi
 
 [![License](https://img.shields.io/github/license/pyrates-neuroscience/PyCoBi.svg)](https://github.com/pyrates-neuroscience/PyCoBi)
 [![Python](https://img.shields.io/pypi/pyversions/pycobi.svg?style=plastic)](https://badge.fury.io/py/pycobi)
 [![PyPI version](https://badge.fury.io/py/pycobi.svg)](https://badge.fury.io/py/pycobi)
 [![CircleCI](https://circleci.com/gh/pyrates-neuroscience/PyCoBi.svg?style=svg)](https://circleci.com/gh/pyrates-neuroscience/PyCoBi)
 [![Documentation Status](https://readthedocs.org/projects/pycobi/badge/?version=latest)](https://pycobi.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/448007450.svg)](https://zenodo.org/badge/latestdoi/448007450)
 
 <img src="PyCoBi_logo_color.png" width="20%" heigth="20%" align="right">
 
 *PyCoBi* is a **Py**thon tool for parameter **co**ntinuations and automated **bi**furcation analysis.
 It provides a Python interface to *Auto-07p* [1], allowing for a more intuitive usage of *Auto-07p* commands within Python scripts. 
 It provides direct access to solutions, branches, and their properties (i.e. special solutions, eigenvalues, etc.) as well as a range of plotting 
 functions to visualize bifurcation diagrams and solutions.
 Finally, it allows to automatically generate the user-supplied Fortran routines via [PyRates](https://github.com/pyrates-neuroscience/PyRates),
 such that *Auto-07p* can be fully used/controlled from within a single Python script, 
 without the need to supply additional non-Python files.
 
-**Use Example:** Use examples will be provided here soon. For now, have a look at the [this example](https://pyrates.readthedocs.io/en/latest/auto_analysis/continuation.html#sphx-glr-auto-analysis-continuation-py)
-which demonstrates how to create the required Fortran files for *Auto-07p* via [PyRates](https://github.com/pyrates-neuroscience/PyRates)
-and use them to run a 1D parameter continuation and bifurcation detection via *PyCoBi*.
-
 Installation
 ============
 
 To use *PyCoBi*, it is required to install [Auto-07p](https://github.com/auto-07p/auto-07p).
 You can follow these [installation instructions](https://github.com/auto-07p/auto-07p/tree/master/doc) for detailed 
 information on how to install *Auto-07p* in your specific setup.
 Note that it is not required to manually set any path variables, since *PyAuto* will take care of that for you.  
@@ -91,14 +88,19 @@
 ```shell
 pip install pycobi
 ```
 
 Alternatively, the development version of *PyCoBi* can be installed by cloning the github 
 repository and using the `setup.py` for installation (see steps 1 and 4). 
 
+Documentation
+=============
+
+A full API, documentation, and use examples can be found at [readthedocs](https://pycobi.readthedocs.io/en/latest/).
+
 References
 ==========
  
 [1] E.J. Doedel, T.F. Fairgrieve, B. Sandstede, A.R. Champneys, Y.A. Kuznetsov and W. Xianjun (2007) *Auto-07p:
        Continuation and bifurcation software for ordinary differential equations.* Technical report,
        Department of Computer Science, Concordia University, Montreal, Quebec.
```

### Comparing `pycobi-0.7.3/README.md` & `pycobi-0.8.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # PyCoBi
 
 [![License](https://img.shields.io/github/license/pyrates-neuroscience/PyCoBi.svg)](https://github.com/pyrates-neuroscience/PyCoBi)
 [![Python](https://img.shields.io/pypi/pyversions/pycobi.svg?style=plastic)](https://badge.fury.io/py/pycobi)
 [![PyPI version](https://badge.fury.io/py/pycobi.svg)](https://badge.fury.io/py/pycobi)
 [![CircleCI](https://circleci.com/gh/pyrates-neuroscience/PyCoBi.svg?style=svg)](https://circleci.com/gh/pyrates-neuroscience/PyCoBi)
 [![Documentation Status](https://readthedocs.org/projects/pycobi/badge/?version=latest)](https://pycobi.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/448007450.svg)](https://zenodo.org/badge/latestdoi/448007450)
 
 <img src="PyCoBi_logo_color.png" width="20%" heigth="20%" align="right">
 
 *PyCoBi* is a **Py**thon tool for parameter **co**ntinuations and automated **bi**furcation analysis.
 It provides a Python interface to *Auto-07p* [1], allowing for a more intuitive usage of *Auto-07p* commands within Python scripts. 
 It provides direct access to solutions, branches, and their properties (i.e. special solutions, eigenvalues, etc.) as well as a range of plotting 
 functions to visualize bifurcation diagrams and solutions.
 Finally, it allows to automatically generate the user-supplied Fortran routines via [PyRates](https://github.com/pyrates-neuroscience/PyRates),
 such that *Auto-07p* can be fully used/controlled from within a single Python script, 
 without the need to supply additional non-Python files.
 
-**Use Example:** Use examples will be provided here soon. For now, have a look at the [this example](https://pyrates.readthedocs.io/en/latest/auto_analysis/continuation.html#sphx-glr-auto-analysis-continuation-py)
-which demonstrates how to create the required Fortran files for *Auto-07p* via [PyRates](https://github.com/pyrates-neuroscience/PyRates)
-and use them to run a 1D parameter continuation and bifurcation detection via *PyCoBi*.
-
 Installation
 ============
 
 To use *PyCoBi*, it is required to install [Auto-07p](https://github.com/auto-07p/auto-07p).
 You can follow these [installation instructions](https://github.com/auto-07p/auto-07p/tree/master/doc) for detailed 
 information on how to install *Auto-07p* in your specific setup.
 Note that it is not required to manually set any path variables, since *PyAuto* will take care of that for you.  
@@ -66,13 +63,18 @@
 ```shell
 pip install pycobi
 ```
 
 Alternatively, the development version of *PyCoBi* can be installed by cloning the github 
 repository and using the `setup.py` for installation (see steps 1 and 4). 
 
+Documentation
+=============
+
+A full API, documentation, and use examples can be found at [readthedocs](https://pycobi.readthedocs.io/en/latest/).
+
 References
 ==========
  
 [1] E.J. Doedel, T.F. Fairgrieve, B. Sandstede, A.R. Champneys, Y.A. Kuznetsov and W. Xianjun (2007) *Auto-07p:
        Continuation and bifurcation software for ordinary differential equations.* Technical report,
        Department of Computer Science, Concordia University, Montreal, Quebec.
```

### Comparing `pycobi-0.7.3/pycobi/__init__.py` & `pycobi-0.8.1/pycobi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 # Richard Gast et al., in preparation.
 
 """Python package for parameter continuations and bifurcation analysis via Auto-07p in Python.
 """
 
 __author__ = "Richard Gast"
 __status__ = "Development"
-__version__ = "0.7.3"
+__version__ = "0.8.1"
 
 from .pycobi import ODESystem
 from .utility import get_lyapunov_exponents, get_solution_eigenvalues, fractal_dimension
 from .automated_continuation import continue_period_doubling_bf, codim2_search
```

### Comparing `pycobi-0.7.3/pycobi/automated_continuation.py` & `pycobi-0.8.1/pycobi/automated_continuation.py`

 * *Files identical despite different names*

### Comparing `pycobi-0.7.3/pycobi/pycobi.py` & `pycobi-0.8.1/pycobi/pycobi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 import os
 import matplotlib.pyplot as plt
 import numpy as np
-from pandas import DataFrame, MultiIndex
+from pandas import DataFrame, MultiIndex, Series
 from mpl_toolkits.mplot3d import Axes3D
 from pyrates import CircuitTemplate, clear
 from matplotlib.collections import LineCollection
 from mpl_toolkits.mplot3d.art3d import Line3DCollection
 from typing import Union, Any, Optional
 import pickle
 
 from .utility import get_solution_stability, get_solution_keys, get_branch_info, get_solution_variables, \
     get_solution_params, get_solution_eigenvalues, get_lyapunov_exponents
 
 
 class ODESystem:
 
     __slots__ = ["auto_solutions", "results", "_orig_dir", "dir", "_auto", "_last_cont", "_cont_num", "_results_map",
-                 "_branches", "_bifurcation_styles", "_temp"]
+                 "_branches", "_bifurcation_styles", "_temp", "additional_attributes", "_eq", "_var_map",
+                 "_var_map_inv"]
 
-    def __init__(self, working_dir: str = None, auto_dir: str = None, init_cont: bool = True, **kwargs) -> None:
+    def __init__(self, eq_file: str, working_dir: str = None, auto_dir: str = None, init_cont: bool = True,
+                 params: list = None, state_vars: list = None, **kwargs) -> None:
         """
 
         Parameters
         ----------
+        eq_file
+            Equation file that this instance of PyCoBi will use for all calls to `PyCoBi.run`
         working_dir
             Directory in which all the fortran equation and auto-07p constant files are saved.
         auto_dir
             Installation directory of auto-07p.
         init_cont
             If true, an integration with respect to time will be performed, using the equation file provided via the
             keyword argument `e=<fname>` (a file named `<fname>.f90` should exist in `working_dir`)
             and the auto constants provided via the keyword argument `c=<fname>`
             (a file named `c.<fname>` should exist in `working_dir`).
+        params
+            Optional ordered list with names of all parameters in the model equations. Can be used to refer to model
+            parameters.
+        state_vars
+            Optional ordered list that provides a name for each entry in the state vector of the model equations.
         kwargs
             Additional keyword arguments that will be provided to the `ODESystem.run` method for performing the time
             integration.
         """
         
         # make sure that auto-07p environment variables are set
         if 'AUTO_DIR' not in os.environ:
@@ -57,30 +66,45 @@
         self._orig_dir = os.getcwd()
         if working_dir:
             try:
                 os.chdir(working_dir)
             except FileNotFoundError:
                 os.chdir(f"{os.getcwd()}/{working_dir}")
         self.dir = os.getcwd()
+        self.additional_attributes = {}
 
         # private attributes
         self._auto = a
+        self._eq = eq_file
         self._last_cont = 0
         self._cont_num = 0
         self._results_map = {}
         self._branches = {}
         self._bifurcation_styles = {'LP': {'marker': 'v', 'color' : '#5D6D7E'},
                                     'HB': {'marker': 'o', 'color': '#148F77'},
                                     'CP': {'marker': 'd', 'color': '#5D6D7E'},
                                     'PD': {'marker': 'h', 'color': '#5D6D7E'},
                                     'BT': {'marker': 's', 'color': 'k'},
                                     'GH': {'marker': 'o', 'color': '#148F77'}
                                     }
         self._temp = kwargs.pop("template", None)
 
+        # create a map that links variable/parameter indices to string-based keys
+        self._var_map = {"t": {"cont": 14, "plot": "PAR(14)"}}
+        self._var_map_inv = {}
+        if params:
+            for i, key in enumerate(params):
+                self._var_map[key] = {"cont": i+1, "plot": f"PAR({i+1})"}
+        if state_vars:
+            for i, key in enumerate(state_vars):
+                self._var_map[key] = {"cont": i+1, "plot": f"U({i+1})"}
+        for key, val in self._var_map.items():
+            self._var_map_inv[val["cont"]] = key
+            self._var_map_inv[val["plot"]] = key
+
         # perform initial continuation in time to ensure convergence to steady-state solution
         if init_cont:
             _ = self.run(ICP=[14], **kwargs)
 
     def __getitem__(self, item):
         try:
             return self.results[item]
@@ -142,20 +166,22 @@
         # update circuit template variables
         if "node_vars" in kwargs:
             template.update_var(node_vars=kwargs.pop("node_vars"))
         if "edge_vars" in kwargs:
             template.update_var(edge_vars=kwargs.pop("edge_vars"))
 
         # generate fortran files
-        _ = template.get_run_func(func_name, dt, file_name=file_name_full, backend="fortran", float_precision="float64",
-                                  auto=True, vectorize=False, solver=solver, **kwargs)
+        _, _, params, state_vars = template.get_run_func(func_name, dt, file_name=file_name_full, backend="fortran",
+                                                         float_precision="float64", auto=True, vectorize=False,
+                                                         solver=solver, **kwargs)
 
         # initialize ODESystem
         return cls(working_dir=working_dir, auto_dir=auto_dir, init_cont=init_cont, e=file_name, c="ivp",
-                   template=template, **init_kwargs)
+                   template=template, params=params[3:], state_vars=list(state_vars), eq_file=file_name_full,
+                   **init_kwargs)
 
     @classmethod
     def from_file(cls, filename: str, auto_dir: str = None):
         """Load `ODESystem` from file using pickle.
 
         Parameters
         ----------
@@ -168,23 +194,19 @@
         -------
         ODESystem
             ODESystem instance containing all the attributes that are available as dictionary entries in `filename`.
         """
         pyauto_instance = cls('', auto_dir=auto_dir, init_cont=False)
         data = pickle.load(open(filename, 'rb'))
         for key, val in data.items():
-            if hasattr(pyauto_instance, key):
-                attr = getattr(pyauto_instance, key)
-                if type(attr) is dict:
-                    attr.update(val)
-                else:
-                    raise AttributeError(f'Attribute {key} is already contained on this PyCoBi instance and cannot be '
-                                         f'set.')
+            attr = getattr(pyauto_instance, key)
+            if type(attr) is dict:
+                attr.update(val)
             else:
-                setattr(pyauto_instance, key, val)
+                raise AttributeError(f'Attribute {key} already exists on this `ODESystem` instance.')
         return pyauto_instance
 
     def to_file(self, filename: str, results_only: bool = True, **kwargs) -> None:
         """Save continuation results on disc via pickle.
 
         Parameters
         ----------
@@ -255,14 +277,16 @@
             DataFrame with the results, auto solution branch object.
         """
 
         # auto call
         ###########
 
         # extract starting point of continuation
+        if self._last_cont == 0:
+            auto_kwargs["e"] = self._eq
         if 'IRS' in auto_kwargs or 's' in auto_kwargs:
             raise ValueError('Usage of keyword arguments `IRS` and `s` is disabled in pycobi. To start from a previous'
                              'solution, use the `starting_point` keyword argument and provide a tuple of branch '
                              'number and point number as returned by the `run` method.')
         if not starting_point and self._last_cont > 0:
             raise ValueError('A starting point is required for further continuation. Either provide a solution to start'
                              ' from via the `starting_point` keyword argument or create a fresh `ODESystem` instance.')
@@ -270,18 +294,19 @@
             origin = self._last_cont
         elif type(origin) is str:
             origin = self._results_map[origin]
         elif type(origin) is not int:
             origin = origin.pycobi_key
 
         # call to auto
-        constants = auto_kwargs.pop('c', None)
-        if constants:
-            solution = self._call_auto(starting_point, origin, c=constants, **auto_kwargs)
-            auto_kwargs['c'] = constants
+        constant_file = auto_kwargs.pop('c', None)
+        auto_kwargs = self._map_auto_kwargs(auto_kwargs)
+        if constant_file:
+            solution = self._call_auto(starting_point, origin, c=constant_file, **auto_kwargs)
+            auto_kwargs['c'] = constant_file
         else:
             solution = self._call_auto(starting_point, origin, **auto_kwargs)
 
         # extract information from auto solution
         ########################################
 
         # extract branch and solution info
@@ -392,32 +417,35 @@
         summary_old = self.results[key]
 
         # extract end points
         points_old, points_new = summary_old.index, summary.index
         start_old, start_new, end_old, end_new = points_old[0], points_new[0], points_old[-1], points_new[-1]
 
         # extract ICP values
-        icp_old = summary_old.loc[end_old, f"PAR({icp[0]})"][0]
-        icp_new = summary.loc[end_new, f"PAR({icp[0]})"][0]
+        key = f"PAR({icp[0]})"
+        if key in self._var_map_inv:
+            key = self._var_map_inv[key]
+        icp_old = summary_old.loc[end_old, key].values[0]
+        icp_new = summary.loc[end_new, key].values[0]
 
         # connect starting points of both continuations and re-label points accordingly
         if icp_new < icp_old:
             conts_sorted = [summary, summary_old]
             keys_sorted = [points_new, points_old]
         else:
             conts_sorted = [summary_old, summary]
             keys_sorted = [points_old, points_new]
         end_point = keys_sorted[0][-1]
 
         # move points into combined summary
         summary_final = {}
         for p1, p2 in zip(keys_sorted[0], keys_sorted[0][::-1]):
-            summary_final[p1] = conts_sorted[0].loc[p2, :]
+            summary_final[p1] = _extract_merge_point(p2, conts_sorted[0])
         for p in keys_sorted[1]:
-            summary_final[p+end_point] = conts_sorted[1].loc[p, :]
+            summary_final[p+end_point] = _extract_merge_point(p, conts_sorted[1])
 
         # store updated summary
         self.results[key] = DataFrame(summary_final).T
 
         return solution, self.results[key]
 
     def get_summary(self, cont: Optional[Union[Any, str, int]] = None, point=None) -> DataFrame:
@@ -531,14 +559,16 @@
 
         Returns
         -------
         DataFrame
             Contains the requested properties of the solution.
         """
         summary = self.get_summary(cont, point=point)
+        columns = [k for k, _ in list(summary.keys())]
+        keys = [key if key in columns else self._var_map_inv[key] for key in keys]
         if point:
             return summary.loc[point, keys]
         return summary.loc[:, keys]
 
     def plot_continuation(self, x: str, y: str, cont: Union[Any, str, int], ax: plt.Axes = None,
                           force_axis_lim_update: bool = False, **kwargs) -> LineCollection:
         """Line plot of 1D/2D parameter continuations and the respective codimension 1/2 bifurcations.
@@ -567,18 +597,18 @@
         if ax is None:
             fig, ax = plt.subplots()
         label_pad = kwargs.pop('labelpad', 5)
         tick_pad = kwargs.pop('tickpad', 5)
         axislim_pad = kwargs.pop('axislimpad', 0)
 
         # extract information from branch solutions
-        if x == 'PAR(14)':
+        if x in ["PAR(14)", "t"]:
             results = self.extract([x, y], cont=cont)
-            results['stability'] = np.asarray([True] * len(results['PAR(14)']))
-            results['bifurcation'] = np.asarray(['RG'] * len(results['PAR(14)']))
+            results['stability'] = np.asarray([True] * len(results[x]))
+            results['bifurcation'] = np.asarray(['RG'] * len(results[x]))
         else:
             results = self.extract([x, y, 'stability', 'bifurcation'], cont=cont)
 
         # plot bifurcation points
         bifurcation_point_kwargs = ['default_color', 'default_marker', 'default_size', 'custom_bf_styles',
                                     'ignore']
         kwargs_tmp = {key: kwargs.pop(key) for key in bifurcation_point_kwargs if key in kwargs}
@@ -940,17 +970,17 @@
                                 columns_2d.append(('lyapunov_exponents', i))
 
             data_2d.append(data_2d_tmp)
             data_1d.append(data_1d_tmp)
             add_columns = False
 
         # arrange data into DataFrame
-        df = DataFrame(data=data_2d, columns=MultiIndex.from_tuples(columns_2d), index=indices)
-        df2 = DataFrame(data=data_1d, columns=columns_1d, index=indices)
-        for i, key in enumerate(columns_1d):
+        df = self._to_dataframe(data_2d, columns=columns_2d, index=indices)
+        df2 = self._to_dataframe(data_1d, columns=columns_1d, index=indices)
+        for i, key in enumerate(df2.columns.values):
             df[key] = df2.loc[:, key]
         return df
 
     def _call_auto(self, starting_point: Union[str, int], origin: Union[Any, dict], **auto_kwargs) -> Any:
         if starting_point:
             _, s = self.get_solution(point=starting_point, cont=origin)
             solution = self._auto.run(s, **auto_kwargs)
@@ -966,14 +996,59 @@
             if force_update:
                 min_val, max_val = axis_limits
             else:
                 min_val, max_val = eval(f"ax.get_{ax_names[i]}lim()")
                 min_val, max_val = np.min([min_val, axis_limits[0]]), np.max([max_val, axis_limits[1]])
             eval(f"ax.set_{ax_names[i]}lim(min_val, max_val)")
 
+    def _map_auto_kwargs(self, kwargs: dict) -> dict:
+
+        # handle the continuation parameter
+        if "ICP" in kwargs:
+            val = kwargs.pop("ICP")
+            if type(val) is str:
+                kwargs["ICP"] = self._var_map[val]["cont"]
+            elif type(val) in [list, tuple]:
+                kwargs["ICP"] = [self._var_map[v]["cont"] if type(v) is str else v for v in val]
+            else:
+                kwargs["ICP"] = val
+
+        # handle the user-point parameter
+        if "UZR" in kwargs:
+            uzr_dict = kwargs.pop("UZR")
+            kwargs["UZR"] = {self._var_map[key]["cont"] if type(key) is str else key: val for key, val in uzr_dict.items()}
+
+        return kwargs
+
+    def _to_dataframe(self, data: list, columns: Union[list, tuple], index: list) -> DataFrame:
+
+        # map variable/parameter keys to string-based keys
+        columns_new = []
+        multi_idx = False
+        for c in columns:
+            if type(c) is tuple:
+                col = (self._var_map_inv[c[0]] if c[0] in self._var_map_inv else c[0], c[1])
+                multi_idx = True
+            else:
+                col = self._var_map_inv[c] if c in self._var_map_inv else c
+            columns_new.append(col)
+        if multi_idx:
+            columns = MultiIndex.from_tuples(tuple(columns_new))
+        else:
+            columns = columns_new
+
+        # create dataframe
+        try:
+            return DataFrame(data=data, columns=columns, index=index)
+        except ValueError as e:
+            if len(data) > len(index):
+                return DataFrame(data=data[:-1], columns=columns, index=index)
+            else:
+                raise e
+
     @staticmethod
     def _get_all_var_keys(solution):
         return [f'U({i+1})' for i in range(solution['NDIM'])]
 
     @staticmethod
     def _get_all_param_keys(solution):
         return solution.PAR.coordnames
@@ -1009,15 +1084,15 @@
         """
 
         # combine y and param vals
         try:
             x = np.reshape(x, (x.squeeze().shape[0], 1))
         except IndexError:
             pass
-        if hasattr(y[0], "shape") and y[0].shape[0] > 1:
+        if hasattr(y[0], "shape") and sum(y[0].shape) > 1:
             y = np.asarray([y[i] for i in range(y.shape[0])])
             y_max = np.reshape(y.max(axis=1), (y.shape[0], 1))
             y_min = np.reshape(y.min(axis=1), (y.shape[0], 1))
             y_min = np.append(x, y_min, axis=1)
             y = y_max
             add_min = True
         else:
@@ -1125,7 +1200,14 @@
         return line_col
 
     @staticmethod
     def _get_axis_lims(x: np.array, padding: float = 0.) -> tuple:
         x_min, x_max = x.min(), x.max()
         x_pad = (x_max - x_min) * padding
         return x_min - x_pad, x_max + x_pad
+
+
+def _extract_merge_point(p: int, df: DataFrame) -> Series:
+    p_tmp = df.loc[p, :]
+    if len(p_tmp.shape) > 1 and p_tmp.shape[0] > 1:
+        return p_tmp.iloc[0, :]
+    return p_tmp
```

### Comparing `pycobi-0.7.3/pycobi/utility.py` & `pycobi-0.8.1/pycobi/utility.py`

 * *Files identical despite different names*

### Comparing `pycobi-0.7.3/pycobi.egg-info/PKG-INFO` & `pycobi-0.8.1/pycobi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobi
-Version: 0.7.3
+Version: 0.8.1
 Summary: Python tool for parameter continuation and bifurcation analysis
 Home-page: UNKNOWN
 Author: Richard Gast
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -26,29 +26,26 @@
 # PyCoBi
 
 [![License](https://img.shields.io/github/license/pyrates-neuroscience/PyCoBi.svg)](https://github.com/pyrates-neuroscience/PyCoBi)
 [![Python](https://img.shields.io/pypi/pyversions/pycobi.svg?style=plastic)](https://badge.fury.io/py/pycobi)
 [![PyPI version](https://badge.fury.io/py/pycobi.svg)](https://badge.fury.io/py/pycobi)
 [![CircleCI](https://circleci.com/gh/pyrates-neuroscience/PyCoBi.svg?style=svg)](https://circleci.com/gh/pyrates-neuroscience/PyCoBi)
 [![Documentation Status](https://readthedocs.org/projects/pycobi/badge/?version=latest)](https://pycobi.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/448007450.svg)](https://zenodo.org/badge/latestdoi/448007450)
 
 <img src="PyCoBi_logo_color.png" width="20%" heigth="20%" align="right">
 
 *PyCoBi* is a **Py**thon tool for parameter **co**ntinuations and automated **bi**furcation analysis.
 It provides a Python interface to *Auto-07p* [1], allowing for a more intuitive usage of *Auto-07p* commands within Python scripts. 
 It provides direct access to solutions, branches, and their properties (i.e. special solutions, eigenvalues, etc.) as well as a range of plotting 
 functions to visualize bifurcation diagrams and solutions.
 Finally, it allows to automatically generate the user-supplied Fortran routines via [PyRates](https://github.com/pyrates-neuroscience/PyRates),
 such that *Auto-07p* can be fully used/controlled from within a single Python script, 
 without the need to supply additional non-Python files.
 
-**Use Example:** Use examples will be provided here soon. For now, have a look at the [this example](https://pyrates.readthedocs.io/en/latest/auto_analysis/continuation.html#sphx-glr-auto-analysis-continuation-py)
-which demonstrates how to create the required Fortran files for *Auto-07p* via [PyRates](https://github.com/pyrates-neuroscience/PyRates)
-and use them to run a 1D parameter continuation and bifurcation detection via *PyCoBi*.
-
 Installation
 ============
 
 To use *PyCoBi*, it is required to install [Auto-07p](https://github.com/auto-07p/auto-07p).
 You can follow these [installation instructions](https://github.com/auto-07p/auto-07p/tree/master/doc) for detailed 
 information on how to install *Auto-07p* in your specific setup.
 Note that it is not required to manually set any path variables, since *PyAuto* will take care of that for you.  
@@ -91,14 +88,19 @@
 ```shell
 pip install pycobi
 ```
 
 Alternatively, the development version of *PyCoBi* can be installed by cloning the github 
 repository and using the `setup.py` for installation (see steps 1 and 4). 
 
+Documentation
+=============
+
+A full API, documentation, and use examples can be found at [readthedocs](https://pycobi.readthedocs.io/en/latest/).
+
 References
 ==========
  
 [1] E.J. Doedel, T.F. Fairgrieve, B. Sandstede, A.R. Champneys, Y.A. Kuznetsov and W. Xianjun (2007) *Auto-07p:
        Continuation and bifurcation software for ordinary differential equations.* Technical report,
        Department of Computer Science, Concordia University, Montreal, Quebec.
```

### Comparing `pycobi-0.7.3/pycobi_tests/__init__.py` & `pycobi-0.8.1/pycobi_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pycobi-0.7.3/pycobi_tests/test_odesystem.py` & `pycobi-0.8.1/pycobi_tests/test_odesystem.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 # Utility
 #########
 
 
 def setup_module():
     print("\n")
-    print("============================")
-    print("| Test Suite : Input layer |")
-    print("============================")
+    print("==========================")
+    print("| Test Suite : ODESystem |")
+    print("==========================")
 
 
 @fixture(scope="session")  # type: str
 def auto_dir(pytestconfig) -> str:
     return pytestconfig.getoption("auto_dir")
 
 
@@ -35,15 +35,15 @@
 
 
 def test_1_1_init(auto_dir):
     """Testing the different instantiation options of the `ODESystem` class.
     """
 
     # initialize ODESystem the default way
-    ode1 = ODESystem(working_dir="resources", auto_dir=auto_dir, init_cont=False)
+    ode1 = ODESystem(eq_file='qif_eq', working_dir="resources", auto_dir=auto_dir, init_cont=False)
     ode1.close_session()
 
     # initialize ODESystem from YAML file
     model = "model_templates.neural_mass_models.qif.qif"
     ode2 = ODESystem.from_yaml(model, init_cont=False, file_name='qif_eq2', func_name="qif2", auto_dir=auto_dir)
     ode2.close_session(clear_files=True)
 
@@ -61,24 +61,26 @@
 
 
 def test_1_2_run(auto_dir):
     """Testing the run method for running auto commands via `ODESystem`.
     """
 
     # initialize ODESystem the default way
-    ode1 = ODESystem(working_dir="resources", auto_dir=auto_dir, init_cont=True, e="qif_eq", c="ivp", NPR=100)
+    ode1 = ODESystem(eq_file="qif_eq", working_dir="resources", auto_dir=auto_dir, init_cont=True, c="ivp", NPR=100)
     ode1.close_session()
 
     # initialize ODESystem from YAML file
     model = "model_templates.neural_mass_models.qif.qif"
     ode2 = ODESystem.from_yaml(model, init_cont=True, file_name='qif_eq2', func_name="qif2", auto_dir=auto_dir,
                                NPR=100, NMX=5000)
     ode2.close_session(clear_files=True)
 
     # initialize ODESystem from YAML file with different parameters
     ode3 = ODESystem.from_yaml(model, init_cont=True, file_name='qif_eq3', func_name="qif3", auto_dir=auto_dir,
                                node_vars={'p/qif_op/eta': 2.0}, NPR=100, NMX=5000)
     ode3.close_session(clear_files=True)
 
+    print(ode2[0].columns.values)
+
     # these tests should pass
-    assert (ode1[0].loc[:, "U(1)"] - ode2[0].loc[:, "U(1)"]).sum()[0] == approx(0.0, rel=accuracy, abs=accuracy)
-    assert abs((ode2[0].loc[:, "U(1)"] - ode3[0].loc[:, "U(1)"]).sum()[0]) > 0
+    assert (ode1[0]["U(1)"] - ode2[0]["p/qif_op/r"]).sum()[0] == approx(0.0, rel=accuracy, abs=accuracy)
+    assert abs((ode2[0]["p/qif_op/r"] - ode3[0]["p/qif_op/r"]).sum()[0]) > 0
```

### Comparing `pycobi-0.7.3/setup.py` & `pycobi-0.8.1/setup.py`

 * *Files identical despite different names*

