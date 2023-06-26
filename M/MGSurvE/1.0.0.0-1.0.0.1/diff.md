# Comparing `tmp/MGSurvE-1.0.0.0.tar.gz` & `tmp/MGSurvE-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-1.0.0.0.tar", last modified: Wed Jun 21 23:42:09 2023, max compression
+gzip compressed data, was "MGSurvE-1.0.0.1.tar", last modified: Mon Jun 26 18:36:57 2023, max compression
```

## Comparing `MGSurvE-1.0.0.0.tar` & `MGSurvE-1.0.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 hector    (1002) hector    (1006)        0 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/
--rw-rw-r--   0 hector    (1002) hector    (1006)    35149 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/LICENSE
-drwxrwxr-x   0 hector    (1002) hector    (1006)        0 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/MGSurvE/
--rw-rw-r--   0 hector    (1002) hector    (1006)      275 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/MGSurvE/__init__.py
--rw-rw-r--   0 hector    (1002) hector    (1006)       23 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE/_version.py
--rw-rw-r--   0 hector    (1002) hector    (1006)     6881 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/MGSurvE/auxiliary.py
--rw-rw-r--   0 hector    (1002) hector    (1006)      605 2023-06-02 17:57:12.000000 MGSurvE-1.0.0.0/MGSurvE/colors.py
--rw-rw-r--   0 hector    (1002) hector    (1006)     1665 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/MGSurvE/constants.py
--rw-rw-r--   0 hector    (1002) hector    (1006)     7191 2023-06-08 23:47:04.000000 MGSurvE-1.0.0.0/MGSurvE/kernels.py
--rw-rw-r--   0 hector    (1002) hector    (1006)    21376 2023-06-05 16:05:28.000000 MGSurvE-1.0.0.0/MGSurvE/landscape.py
--rw-rw-r--   0 hector    (1002) hector    (1006)     4924 2022-03-15 21:24:52.000000 MGSurvE-1.0.0.0/MGSurvE/matrices.py
--rw-rw-r--   0 hector    (1002) hector    (1006)     1358 2022-03-15 21:24:52.000000 MGSurvE-1.0.0.0/MGSurvE/network.py
--rw-rw-r--   0 hector    (1002) hector    (1006)    45037 2023-04-05 15:58:13.000000 MGSurvE-1.0.0.0/MGSurvE/optimization.py
--rw-rw-r--   0 hector    (1002) hector    (1006)     9200 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/MGSurvE/optimizationPSO.py
--rw-rw-r--   0 hector    (1002) hector    (1006)    18219 2023-06-02 19:31:52.000000 MGSurvE-1.0.0.0/MGSurvE/plots.py
--rw-rw-r--   0 hector    (1002) hector    (1006)     6849 2023-03-04 15:56:03.000000 MGSurvE-1.0.0.0/MGSurvE/pointProcess.py
-drwxrwxr-x   0 hector    (1002) hector    (1006)        0 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/MGSurvE.egg-info/
--rw-rw-r--   0 hector    (1002) hector    (1006)     4611 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/PKG-INFO
--rw-rw-r--   0 hector    (1002) hector    (1006)      451 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/SOURCES.txt
--rw-rw-r--   0 hector    (1002) hector    (1006)        1 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/dependency_links.txt
--rw-rw-r--   0 hector    (1002) hector    (1006)      221 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/requires.txt
--rw-rw-r--   0 hector    (1002) hector    (1006)        8 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/top_level.txt
--rw-rw-r--   0 hector    (1002) hector    (1006)     4611 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/PKG-INFO
--rw-rw-r--   0 hector    (1002) hector    (1006)     4177 2023-06-12 15:17:24.000000 MGSurvE-1.0.0.0/README.md
--rw-rw-r--   0 hector    (1002) hector    (1006)       38 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/setup.cfg
--rw-rw-r--   0 hector    (1002) hector    (1006)     1428 2023-06-08 23:48:37.000000 MGSurvE-1.0.0.0/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-26 18:36:57.604495 MGSurvE-1.0.0.1/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/LICENSE
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-26 18:36:57.603510 MGSurvE-1.0.0.1/MGSurvE/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       23 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.0.1/MGSurvE/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.0.1/MGSurvE/kernels.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21376 2023-06-08 23:51:28.000000 MGSurvE-1.0.0.1/MGSurvE/landscape.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/matrices.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/network.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/optimization.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.0.1/MGSurvE/optimizationPSO.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18240 2023-06-26 18:31:03.000000 MGSurvE-1.0.0.1/MGSurvE/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.0.1/MGSurvE/pointProcess.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-26 18:36:57.604180 MGSurvE-1.0.0.1/MGSurvE.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4619 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      221 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-06-26 18:36:57.000000 MGSurvE-1.0.0.1/MGSurvE.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4619 2023-06-26 18:36:57.604371 MGSurvE-1.0.0.1/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4185 2023-06-22 17:37:58.000000 MGSurvE-1.0.0.1/README.md
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-06-26 18:36:57.604561 MGSurvE-1.0.0.1/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-06-08 23:51:28.000000 MGSurvE-1.0.0.1/setup.py
```

### Comparing `MGSurvE-1.0.0.0/LICENSE` & `MGSurvE-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/auxiliary.py` & `MGSurvE-1.0.0.1/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/colors.py` & `MGSurvE-1.0.0.1/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/constants.py` & `MGSurvE-1.0.0.1/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/kernels.py` & `MGSurvE-1.0.0.1/MGSurvE/kernels.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/landscape.py` & `MGSurvE-1.0.0.1/MGSurvE/landscape.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/matrices.py` & `MGSurvE-1.0.0.1/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/network.py` & `MGSurvE-1.0.0.1/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/optimization.py` & `MGSurvE-1.0.0.1/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/optimizationPSO.py` & `MGSurvE-1.0.0.1/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE/plots.py` & `MGSurvE-1.0.0.1/MGSurvE/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,17 +154,18 @@
                 zorder=zorders[1]
             )
         if latlon and not CARTOPY:
             warnings.warn("Please install cartopy to plot the traps' radii of attractiveness!")
         if not latlon:
             for r in trapsKernels[tType]['radii']:
                 circle = plt.Circle(
-                    (trap[0], trap[1]), r, 
-                    color=col, fill=fill, ls=ls, 
-                    lw=lws[1], zorder=zorders[1]
+                    (trap[0], trap[1]), r,
+                    color=col, fill=fill, ls=ls,
+                    zorder=zorders[1]
+                    # lw=lws[1], 
                 )
                 ax.add_patch(circle)
     return (fig, ax)
 
 
 def plotTrapsNetwork(
         fig, ax,
```

### Comparing `MGSurvE-1.0.0.0/MGSurvE/pointProcess.py` & `MGSurvE-1.0.0.1/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.0.0/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-1.0.0.1/MGSurvE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,21 +16,22 @@
 # MGSurvE: Mosquito Gene SurveillancE
 
 MGSurvE is a project that optimizes mosquito traps' placement in complex heterogeneous landscapes in an effort to minimize the time to detection of genetic variants of interest.
 
 Please have a look at the [documentation](https://chipdelmal.github.io/MGSurvE/) for more info and our [pypi](https://pypi.org/project/MGSurvE/) package for detailed [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html), and [tutorials](https://chipdelmal.github.io/MGSurvE/build/html/demos.html).
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MGSurvE)](https://pypi.org/project/MGSurvE/)
-[![PyPI version](https://badge.fury.io/py/MGSurvE.svg)](https://badge.fury.io/py/MGSurvE) 
-[![Docker](https://img.shields.io/docker/v/chipdelmal/mgsurve?color=success&label=docker%20img)](https://hub.docker.com/repository/docker/chipdelmal/mgsurve)
+[![PyPI version](https://badge.fury.io/py/MGSurvE.svg)](https://badge.fury.io/py/MGSurvE)
 [![Unit Tests](https://github.com/chipdelmal/MGSurvE/actions/workflows/PyTests.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/tree/main/MGSurvE/test)
 [![Flake8](https://github.com/chipdelmal/MGSurvE/actions/workflows/Flake8.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Flake8.yml)
 [![Conda](https://github.com/chipdelmal/MGSurvE/actions/workflows/Anaconda.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Anaconda.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Chipdelmal/MGSurvE)
+<!-- [![Docker](https://img.shields.io/docker/v/chipdelmal/mgsurve?color=success&label=docker%20img)](https://hub.docker.com/repository/docker/chipdelmal/mgsurve)-->
+
 
 
 To install the package's latest stable version run (usage of [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html) for environment management is strongly recommended):
 
 ```
 pip install MGSurvE
 ```
```

### Comparing `MGSurvE-1.0.0.0/PKG-INFO` & `MGSurvE-1.0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,21 +16,22 @@
 # MGSurvE: Mosquito Gene SurveillancE
 
 MGSurvE is a project that optimizes mosquito traps' placement in complex heterogeneous landscapes in an effort to minimize the time to detection of genetic variants of interest.
 
 Please have a look at the [documentation](https://chipdelmal.github.io/MGSurvE/) for more info and our [pypi](https://pypi.org/project/MGSurvE/) package for detailed [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html), and [tutorials](https://chipdelmal.github.io/MGSurvE/build/html/demos.html).
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MGSurvE)](https://pypi.org/project/MGSurvE/)
-[![PyPI version](https://badge.fury.io/py/MGSurvE.svg)](https://badge.fury.io/py/MGSurvE) 
-[![Docker](https://img.shields.io/docker/v/chipdelmal/mgsurve?color=success&label=docker%20img)](https://hub.docker.com/repository/docker/chipdelmal/mgsurve)
+[![PyPI version](https://badge.fury.io/py/MGSurvE.svg)](https://badge.fury.io/py/MGSurvE)
 [![Unit Tests](https://github.com/chipdelmal/MGSurvE/actions/workflows/PyTests.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/tree/main/MGSurvE/test)
 [![Flake8](https://github.com/chipdelmal/MGSurvE/actions/workflows/Flake8.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Flake8.yml)
 [![Conda](https://github.com/chipdelmal/MGSurvE/actions/workflows/Anaconda.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Anaconda.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Chipdelmal/MGSurvE)
+<!-- [![Docker](https://img.shields.io/docker/v/chipdelmal/mgsurve?color=success&label=docker%20img)](https://hub.docker.com/repository/docker/chipdelmal/mgsurve)-->
+
 
 
 To install the package's latest stable version run (usage of [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html) for environment management is strongly recommended):
 
 ```
 pip install MGSurvE
 ```
```

### Comparing `MGSurvE-1.0.0.0/README.md` & `MGSurvE-1.0.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # MGSurvE: Mosquito Gene SurveillancE
 
 MGSurvE is a project that optimizes mosquito traps' placement in complex heterogeneous landscapes in an effort to minimize the time to detection of genetic variants of interest.
 
 Please have a look at the [documentation](https://chipdelmal.github.io/MGSurvE/) for more info and our [pypi](https://pypi.org/project/MGSurvE/) package for detailed [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html), and [tutorials](https://chipdelmal.github.io/MGSurvE/build/html/demos.html).
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MGSurvE)](https://pypi.org/project/MGSurvE/)
-[![PyPI version](https://badge.fury.io/py/MGSurvE.svg)](https://badge.fury.io/py/MGSurvE) 
-[![Docker](https://img.shields.io/docker/v/chipdelmal/mgsurve?color=success&label=docker%20img)](https://hub.docker.com/repository/docker/chipdelmal/mgsurve)
+[![PyPI version](https://badge.fury.io/py/MGSurvE.svg)](https://badge.fury.io/py/MGSurvE)
 [![Unit Tests](https://github.com/chipdelmal/MGSurvE/actions/workflows/PyTests.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/tree/main/MGSurvE/test)
 [![Flake8](https://github.com/chipdelmal/MGSurvE/actions/workflows/Flake8.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Flake8.yml)
 [![Conda](https://github.com/chipdelmal/MGSurvE/actions/workflows/Anaconda.yml/badge.svg)](https://github.com/Chipdelmal/MGSurvE/blob/main/.github/workflows/Anaconda.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Chipdelmal/MGSurvE)
+<!-- [![Docker](https://img.shields.io/docker/v/chipdelmal/mgsurve?color=success&label=docker%20img)](https://hub.docker.com/repository/docker/chipdelmal/mgsurve)-->
+
 
 
 To install the package's latest stable version run (usage of [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html) for environment management is strongly recommended):
 
 ```
 pip install MGSurvE
 ```
```

### Comparing `MGSurvE-1.0.0.0/setup.py` & `MGSurvE-1.0.0.1/setup.py`

 * *Files identical despite different names*

