# Comparing `tmp/nubopy-1.0.3.tar.gz` & `tmp/nubopy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nubopy-1.0.3.tar", last modified: Tue Apr 18 17:15:33 2023, max compression
+gzip compressed data, was "nubopy-1.0.4.tar", last modified: Mon Jun 26 10:34:54 2023, max compression
```

## Comparing `nubopy-1.0.3.tar` & `nubopy-1.0.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.674484 nubopy-1.0.3/
--rw-r--r--   0 mikediessner   (501) staff       (20)     1500 2023-03-16 09:32:23.000000 nubopy-1.0.3/LICENSE.md
--rw-r--r--   0 mikediessner   (501) staff       (20)     2096 2023-04-18 17:15:33.674281 nubopy-1.0.3/PKG-INFO
--rw-r--r--   0 mikediessner   (501) staff       (20)     1683 2023-04-05 15:30:35.000000 nubopy-1.0.3/README.md
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.644530 nubopy-1.0.3/nubo/
--rw-r--r--   0 mikediessner   (501) staff       (20)       94 2023-02-28 09:35:10.000000 nubopy-1.0.3/nubo/__init__.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.646615 nubopy-1.0.3/nubo/acquisition/
--rw-r--r--   0 mikediessner   (501) staff       (20)      136 2023-03-07 13:05:46.000000 nubopy-1.0.3/nubo/acquisition/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1014 2023-03-30 17:33:30.000000 nubopy-1.0.3/nubo/acquisition/acquisition_function.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     4436 2023-04-06 08:23:23.000000 nubopy-1.0.3/nubo/acquisition/analytical.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     9239 2023-04-04 09:43:08.000000 nubopy-1.0.3/nubo/acquisition/monte_carlo.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.648111 nubopy-1.0.3/nubo/models/
--rw-r--r--   0 mikediessner   (501) staff       (20)       70 2023-03-03 10:04:54.000000 nubopy-1.0.3/nubo/models/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1833 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/models/fit.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2764 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/models/gaussian_process.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.656055 nubopy-1.0.3/nubo/optimisation/
--rw-r--r--   0 mikediessner   (501) staff       (20)      232 2023-03-31 10:52:35.000000 nubopy-1.0.3/nubo/optimisation/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     8268 2023-04-03 12:42:29.000000 nubopy-1.0.3/nubo/optimisation/adam.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2285 2023-04-03 12:42:54.000000 nubopy-1.0.3/nubo/optimisation/lbfgsb.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     3475 2023-04-03 12:42:41.000000 nubopy-1.0.3/nubo/optimisation/mixed.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     6995 2023-04-03 12:47:24.000000 nubopy-1.0.3/nubo/optimisation/multipoint.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2717 2023-04-18 16:22:14.000000 nubopy-1.0.3/nubo/optimisation/singlepoint.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2432 2023-04-03 12:47:44.000000 nubopy-1.0.3/nubo/optimisation/slsqp.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1325 2023-04-03 12:49:09.000000 nubopy-1.0.3/nubo/optimisation/utils.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.667461 nubopy-1.0.3/nubo/test_functions/
--rw-r--r--   0 mikediessner   (501) staff       (20)      359 2023-02-28 09:35:10.000000 nubopy-1.0.3/nubo/test_functions/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2800 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/ackley.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2530 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/dixonprice.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2419 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/griewank.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     7953 2023-03-29 09:52:55.000000 nubopy-1.0.3/nubo/test_functions/hartmann.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2661 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/levy.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2319 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/rastrigin.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2345 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/schwefel.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2217 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/sphere.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2276 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/sumsquares.py
--rw-r--r--   0 mikediessner   (501) staff       (20)      291 2023-03-08 10:27:07.000000 nubopy-1.0.3/nubo/test_functions/test_functions.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2440 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/test_functions/zakharov.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.669450 nubopy-1.0.3/nubo/utils/
--rw-r--r--   0 mikediessner   (501) staff       (20)      151 2023-03-14 10:12:07.000000 nubopy-1.0.3/nubo/utils/__init__.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1164 2023-03-16 09:32:23.000000 nubopy-1.0.3/nubo/utils/generate_inputs.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     3359 2023-03-29 09:52:55.000000 nubopy-1.0.3/nubo/utils/latin_hypercube.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     1818 2023-03-23 09:40:34.000000 nubopy-1.0.3/nubo/utils/transform.py
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.671485 nubopy-1.0.3/nubopy.egg-info/
--rw-r--r--   0 mikediessner   (501) staff       (20)     2096 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/PKG-INFO
--rw-r--r--   0 mikediessner   (501) staff       (20)     1256 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/SOURCES.txt
--rw-r--r--   0 mikediessner   (501) staff       (20)        1 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/dependency_links.txt
--rw-r--r--   0 mikediessner   (501) staff       (20)       27 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/requires.txt
--rw-r--r--   0 mikediessner   (501) staff       (20)        5 2023-04-18 17:15:33.000000 nubopy-1.0.3/nubopy.egg-info/top_level.txt
--rw-r--r--   0 mikediessner   (501) staff       (20)      553 2023-04-18 17:15:26.000000 nubopy-1.0.3/pyproject.toml
--rw-r--r--   0 mikediessner   (501) staff       (20)       38 2023-04-18 17:15:33.674520 nubopy-1.0.3/setup.cfg
-drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-04-18 17:15:33.673868 nubopy-1.0.3/tests/
--rw-r--r--   0 mikediessner   (501) staff       (20)    16878 2023-03-29 11:44:07.000000 nubopy-1.0.3/tests/test_acquisition.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     2876 2023-03-29 09:52:55.000000 nubopy-1.0.3/tests/test_models.py
--rw-r--r--   0 mikediessner   (501) staff       (20)    22786 2023-03-31 10:16:55.000000 nubopy-1.0.3/tests/test_optimisation.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     9449 2023-03-29 09:52:55.000000 nubopy-1.0.3/tests/test_test_functions.py
--rw-r--r--   0 mikediessner   (501) staff       (20)     4123 2023-03-29 09:52:55.000000 nubopy-1.0.3/tests/test_utils.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-06-26 10:34:54.826060 nubopy-1.0.4/
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1500 2023-04-28 10:08:45.000000 nubopy-1.0.4/LICENSE.md
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2929 2023-06-26 10:34:54.825910 nubopy-1.0.4/PKG-INFO
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2516 2023-05-12 10:57:25.000000 nubopy-1.0.4/README.md
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-06-26 10:34:54.811310 nubopy-1.0.4/nubo/
+-rw-r--r--   0 mikediessner   (501) staff       (20)       94 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/__init__.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-06-26 10:34:54.812858 nubopy-1.0.4/nubo/acquisition/
+-rw-r--r--   0 mikediessner   (501) staff       (20)      136 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/acquisition/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1014 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/acquisition/acquisition_function.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     4436 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/acquisition/analytical.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     9235 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/acquisition/monte_carlo.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-06-26 10:34:54.813886 nubopy-1.0.4/nubo/models/
+-rw-r--r--   0 mikediessner   (501) staff       (20)       70 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/models/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1833 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/models/fit.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2764 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/models/gaussian_process.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-06-26 10:34:54.817431 nubopy-1.0.4/nubo/optimisation/
+-rw-r--r--   0 mikediessner   (501) staff       (20)      232 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/optimisation/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     8270 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/optimisation/adam.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2285 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/optimisation/lbfgsb.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     3475 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/optimisation/mixed.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     6996 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/optimisation/multipoint.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2717 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/optimisation/singlepoint.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2432 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/optimisation/slsqp.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1325 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/optimisation/utils.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-06-26 10:34:54.821555 nubopy-1.0.4/nubo/test_functions/
+-rw-r--r--   0 mikediessner   (501) staff       (20)      359 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2800 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/ackley.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2530 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/dixonprice.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2419 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/griewank.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     7953 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/hartmann.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2661 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/levy.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2319 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/rastrigin.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2345 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/schwefel.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2217 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/sphere.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2276 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/sumsquares.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)      291 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/test_functions.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2440 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/test_functions/zakharov.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-06-26 10:34:54.822754 nubopy-1.0.4/nubo/utils/
+-rw-r--r--   0 mikediessner   (501) staff       (20)      151 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/utils/__init__.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1164 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/utils/generate_inputs.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     3359 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/utils/latin_hypercube.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1818 2023-04-28 10:08:45.000000 nubopy-1.0.4/nubo/utils/transform.py
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-06-26 10:34:54.824421 nubopy-1.0.4/nubopy.egg-info/
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2929 2023-06-26 10:34:54.000000 nubopy-1.0.4/nubopy.egg-info/PKG-INFO
+-rw-r--r--   0 mikediessner   (501) staff       (20)     1256 2023-06-26 10:34:54.000000 nubopy-1.0.4/nubopy.egg-info/SOURCES.txt
+-rw-r--r--   0 mikediessner   (501) staff       (20)        1 2023-06-26 10:34:54.000000 nubopy-1.0.4/nubopy.egg-info/dependency_links.txt
+-rw-r--r--   0 mikediessner   (501) staff       (20)       27 2023-06-26 10:34:54.000000 nubopy-1.0.4/nubopy.egg-info/requires.txt
+-rw-r--r--   0 mikediessner   (501) staff       (20)        5 2023-06-26 10:34:54.000000 nubopy-1.0.4/nubopy.egg-info/top_level.txt
+-rw-r--r--   0 mikediessner   (501) staff       (20)      554 2023-06-26 10:23:53.000000 nubopy-1.0.4/pyproject.toml
+-rw-r--r--   0 mikediessner   (501) staff       (20)       38 2023-06-26 10:34:54.826090 nubopy-1.0.4/setup.cfg
+drwxr-xr-x   0 mikediessner   (501) staff       (20)        0 2023-06-26 10:34:54.825672 nubopy-1.0.4/tests/
+-rw-r--r--   0 mikediessner   (501) staff       (20)    16878 2023-04-28 10:08:45.000000 nubopy-1.0.4/tests/test_acquisition.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     2876 2023-04-28 10:08:45.000000 nubopy-1.0.4/tests/test_models.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)    22786 2023-04-28 10:08:45.000000 nubopy-1.0.4/tests/test_optimisation.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     9449 2023-04-28 10:08:45.000000 nubopy-1.0.4/tests/test_test_functions.py
+-rw-r--r--   0 mikediessner   (501) staff       (20)     4123 2023-04-28 10:08:45.000000 nubopy-1.0.4/tests/test_utils.py
```

### Comparing `nubopy-1.0.3/LICENSE.md` & `nubopy-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/PKG-INFO` & `nubopy-1.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: nubopy
-Version: 1.0.3
-Summary: A transparent Python package for Bayesian optimisation
-Author-email: Mike Diessner <m.diessner2@ncl.ac.uk>
-Project-URL: Homepage, https://mikediessner.github.io/nubo
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # NUBO
 
 NUBO, short for Newcastle University Bayesian optimisation, is a Bayesian
-optimisation framework for the optimisation of expensive-to-evaluate black box
+optimisation framework for the optimisation of expensive-to-evaluate black-box
 functions, such as physical experiments and computer simulations. It is
 developed and maintained by the
 [Fluid Dynamics Lab](https://www.experimental-fluid-dynamics.com) at
 [Newcastle University](https://www.ncl.ac.uk). NUBO focuses primarily on
 transparency and user experience to make Bayesian optimisation easily
 accessible to researchers from all disciplines. Transparency is ensured by
 clean and comprehensible code, precise references, and thorough documentation.
@@ -32,7 +20,33 @@
 knowledge of Python to optimise your simulations and experiments. NUBO is
 distributed as an open-source software under the
 [BSD 3-Clause licence](https://joinup.ec.europa.eu/licence/bsd-3-clause-new-or-revised-license).
 
  > Thanks for considering NUBO. If you have any questions, comments, or issues
  > feel free to email us at m.diessner2@newcastle.ac.uk. Any feedback is highly
  > appreciated and will help make NUBO better in the future.
+
+## Install NUBO
+
+Install NUBO and all its dependencies directly from the
+[Python Package Index](https://pypi.org) *PyPI* using the
+[Python package manager](https://pip.pypa.io/en/latest/) *pip* with the
+following code. We recommend the use of a virtual environment.S
+
+    pip install nubopy
+
+## Cite NUBO
+
+If you are using NUBO for your research, please cite as:
+
+    Mike Diessner, Kevin Wilson, and Richard D. Whalley. "NUBO: A Transparent Python Package for Bayesian Optimisation," arXiv preprint arXiv:2305.06709, 2023.
+
+If you are using Bibtex, please cite as:
+
+```
+@article{diessner2023nubo,
+         title={NUBO: A Transparent Python Package for Bayesian Optimisation},
+         author={Diessner, Mike and Wilson, Kevin and Whalley, Richard D},
+         journal={arXiv preprint arXiv:2305.06709},
+         year={2023}
+}
+```
```

### Comparing `nubopy-1.0.3/nubo/acquisition/acquisition_function.py` & `nubopy-1.0.4/nubo/acquisition/acquisition_function.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/acquisition/analytical.py` & `nubopy-1.0.4/nubo/acquisition/analytical.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/acquisition/monte_carlo.py` & `nubopy-1.0.4/nubo/acquisition/monte_carlo.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     x_pending : ``torch.Tensor``
         (size n x d) Training inputs of currently pending points.
     samples : ``int``
          Number of Monte Carlo samples, default is 512.
     fix_base_samples : ``bool``
         Whether base samples used to compute Monte Carlo samples of
         acquisition function should be fixed for the optimisation step.
-        If false (default) stochastic optimizer (Adam) have to be used. If
+        If false (default) stochastic optimizer (Adam) has to be used. If
         true deterministic optimizer (L-BFGS-B, SLSQP) can be used.
     base_samples : ``NoneType`` or ``torch.Tensor``
         Base samples used to compute Monte Carlo samples drawn if
         `fix_base_samples` is true.
     dims : ``int``
         Number of input dimensions.
     """
@@ -61,15 +61,15 @@
         x_pending : ``torch.Tensor``, optional
             (size n x d) Training inputs of currently pending points.
         samples : ``int``, optional
              Number of Monte Carlo samples, default is 512.
         fix_base_samples : ``bool``, optional
             Whether base samples used to compute Monte Carlo samples of
             acquisition function should be fixed for the optimisation step.
-            If false (default) stochastic optimizer (Adam) have to be used. If
+            If false (default) stochastic optimizer (Adam) has to be used. If
             true deterministic optimizer (L-BFGS-B, SLSQP) can be used.
         """
         
         self.gp = gp
         self.y_best = y_best
         self.x_pending = x_pending
         self.samples = samples
@@ -143,15 +143,15 @@
     x_pending : ``torch.Tensor``
         (size n x d) Training inputs of currently pending points.
     samples : ``int``
          Number of Monte Carlo samples, default is 512.
     fix_base_samples : ``bool``
         Whether base samples used to compute Monte Carlo samples of
         acquisition function should be fixed for the optimisation step.
-        If false (default) stochastic optimizer (Adam) have to be used. If
+        If false (default) stochastic optimizer (Adam) has to be used. If
         true deterministic optimizer (L-BFGS-B, SLSQP) can be used.
     base_samples : ``NoneType`` or ``torch.Tensor``
         Base samples used to compute Monte Carlo samples drawn if
         `fix_base_samples` is true.
     dims : ``int``
         Number of input dimensions.
     """
@@ -172,15 +172,15 @@
         x_pending : ``torch.Tensor`
             (size n x d) Training inputs of currently pending points.
         samples : ``int``
             Number of Monte Carlo samples, default is 512.
         fix_base_samples : ``bool``
             Whether base samples used to compute Monte Carlo samples of
             acquisition function should be fixed for the optimisation step.
-            If false (default) stochastic optimizer (Adam) have to be used. If
+            If false (default) stochastic optimizer (Adam) has to be used. If
             true deterministic optimizer (L-BFGS-B, SLSQP) can be used.
         base_samples : ``NoneType`` or ``torch.Tensor``
             Base samples used to compute Monte Carlo samples drawn if
             `fix_base_samples` is true.
         dims : ``int``
             Number of input dimensions.
         """
```

### Comparing `nubopy-1.0.3/nubo/models/fit.py` & `nubopy-1.0.4/nubo/models/fit.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/models/gaussian_process.py` & `nubopy-1.0.4/nubo/models/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/optimisation/adam.py` & `nubopy-1.0.4/nubo/optimisation/adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     """
     Multi-start Adam optimiser using the ``torch.optim.Adam`` implementation
     from ``PyTorch``.
     
     Used for optimising Monte Carlo acquisition function when base samples are
     not fixed. Bounds are enforced by transforming `func` with the sigmoid
     function and scaling results. Picks the best `num_starts` points from a
-    total `num_samples` Latin hypercube samples to initialise the optimser.
+    total `num_samples` Latin hypercube samples to initialise the optimiser.
     Returns the best result. Minimises `func`.
 
     Parameters
     ----------
     func : ``Callable``
         Function to optimise.
     bounds : ``torch.Tensor``
@@ -201,15 +201,15 @@
     """
     Multi-start Adam optimiser using the ``torch.optim.Adam`` implementation
     from ``PyTorch``.
     
     Used for optimising Monte Carlo acquisition function when base samples are
     not fixed. Bounds are enforced by clamping where values exceed them. Picks
     the best `num_starts` points from a total `num_samples` Latin hypercube
-    samples to initialise the optimser. Returns the best result. Minimises
+    samples to initialise the optimiser. Returns the best result. Minimises
     `func`.
 
     Parameters
     ----------
     func : ``Callable``
         Function to optimise.
     bounds : ``torch.Tensor``
```

### Comparing `nubopy-1.0.3/nubo/optimisation/lbfgsb.py` & `nubopy-1.0.4/nubo/optimisation/lbfgsb.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/optimisation/mixed.py` & `nubopy-1.0.4/nubo/optimisation/mixed.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/optimisation/multipoint.py` & `nubopy-1.0.4/nubo/optimisation/multipoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                      **kwargs: Any) -> Tuple[Tensor, Tensor]:
     """
     Sequential greedy optimisation loop for Monte Carlo acquisition functions.
 
     Optimises Monte Carlo acquisition functions to return multi-point batches
     for parallel evaluation. Computes one point after the other for a batch
     always keeping previous points fixed, i.e. compute point 1, compute point 2
-    holding point 1 fixed, compute point 3 holding point 1 and 2 fixed and so
+    holding point 1 fixed, compute point 3 holding points 1 and 2 fixed and so
     on until the batch is full. Minimises `func`.
 
     Parameters
     ----------
     func : ``Callable``
         Function to optimise.
     method : ``str``
```

### Comparing `nubopy-1.0.3/nubo/optimisation/singlepoint.py` & `nubopy-1.0.4/nubo/optimisation/singlepoint.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/optimisation/slsqp.py` & `nubopy-1.0.4/nubo/optimisation/slsqp.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/optimisation/utils.py` & `nubopy-1.0.4/nubo/optimisation/utils.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/ackley.py` & `nubopy-1.0.4/nubo/test_functions/ackley.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/dixonprice.py` & `nubopy-1.0.4/nubo/test_functions/dixonprice.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/griewank.py` & `nubopy-1.0.4/nubo/test_functions/griewank.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/hartmann.py` & `nubopy-1.0.4/nubo/test_functions/hartmann.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/levy.py` & `nubopy-1.0.4/nubo/test_functions/levy.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/rastrigin.py` & `nubopy-1.0.4/nubo/test_functions/rastrigin.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/schwefel.py` & `nubopy-1.0.4/nubo/test_functions/schwefel.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/sphere.py` & `nubopy-1.0.4/nubo/test_functions/sphere.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/sumsquares.py` & `nubopy-1.0.4/nubo/test_functions/sumsquares.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/test_functions/zakharov.py` & `nubopy-1.0.4/nubo/test_functions/zakharov.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/utils/generate_inputs.py` & `nubopy-1.0.4/nubo/utils/generate_inputs.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/utils/latin_hypercube.py` & `nubopy-1.0.4/nubo/utils/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubo/utils/transform.py` & `nubopy-1.0.4/nubo/utils/transform.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/nubopy.egg-info/PKG-INFO` & `nubopy-1.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nubopy
-Version: 1.0.3
+Version: 1.0.4
 Summary: A transparent Python package for Bayesian optimisation
 Author-email: Mike Diessner <m.diessner2@ncl.ac.uk>
 Project-URL: Homepage, https://mikediessner.github.io/nubo
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # NUBO
 
 NUBO, short for Newcastle University Bayesian optimisation, is a Bayesian
-optimisation framework for the optimisation of expensive-to-evaluate black box
+optimisation framework for the optimisation of expensive-to-evaluate black-box
 functions, such as physical experiments and computer simulations. It is
 developed and maintained by the
 [Fluid Dynamics Lab](https://www.experimental-fluid-dynamics.com) at
 [Newcastle University](https://www.ncl.ac.uk). NUBO focuses primarily on
 transparency and user experience to make Bayesian optimisation easily
 accessible to researchers from all disciplines. Transparency is ensured by
 clean and comprehensible code, precise references, and thorough documentation.
@@ -32,7 +32,33 @@
 knowledge of Python to optimise your simulations and experiments. NUBO is
 distributed as an open-source software under the
 [BSD 3-Clause licence](https://joinup.ec.europa.eu/licence/bsd-3-clause-new-or-revised-license).
 
  > Thanks for considering NUBO. If you have any questions, comments, or issues
  > feel free to email us at m.diessner2@newcastle.ac.uk. Any feedback is highly
  > appreciated and will help make NUBO better in the future.
+
+## Install NUBO
+
+Install NUBO and all its dependencies directly from the
+[Python Package Index](https://pypi.org) *PyPI* using the
+[Python package manager](https://pip.pypa.io/en/latest/) *pip* with the
+following code. We recommend the use of a virtual environment.S
+
+    pip install nubopy
+
+## Cite NUBO
+
+If you are using NUBO for your research, please cite as:
+
+    Mike Diessner, Kevin Wilson, and Richard D. Whalley. "NUBO: A Transparent Python Package for Bayesian Optimisation," arXiv preprint arXiv:2305.06709, 2023.
+
+If you are using Bibtex, please cite as:
+
+```
+@article{diessner2023nubo,
+         title={NUBO: A Transparent Python Package for Bayesian Optimisation},
+         author={Diessner, Mike and Wilson, Kevin and Whalley, Richard D},
+         journal={arXiv preprint arXiv:2305.06709},
+         year={2023}
+}
+```
```

### Comparing `nubopy-1.0.3/nubopy.egg-info/SOURCES.txt` & `nubopy-1.0.4/nubopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/pyproject.toml` & `nubopy-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nubopy"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Mike Diessner", email="m.diessner2@ncl.ac.uk" },
 ]
 description = "A transparent Python package for Bayesian optimisation"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 dependencies = ["torch", "gpytorch", "scipy", "numpy"]
 classifiers = [
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
 ]
 
 [project.urls]
```

### Comparing `nubopy-1.0.3/tests/test_acquisition.py` & `nubopy-1.0.4/tests/test_acquisition.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/tests/test_models.py` & `nubopy-1.0.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/tests/test_optimisation.py` & `nubopy-1.0.4/tests/test_optimisation.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/tests/test_test_functions.py` & `nubopy-1.0.4/tests/test_test_functions.py`

 * *Files identical despite different names*

### Comparing `nubopy-1.0.3/tests/test_utils.py` & `nubopy-1.0.4/tests/test_utils.py`

 * *Files identical despite different names*

