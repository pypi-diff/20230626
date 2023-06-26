# Comparing `tmp/CONEstrip-0.1.tar.gz` & `tmp/CONEstrip-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CONEstrip-0.1.tar", last modified: Mon Jun 26 08:18:43 2023, max compression
+gzip compressed data, was "CONEstrip-0.1.1.tar", last modified: Mon Jun 26 09:46:31 2023, max compression
```

## Comparing `CONEstrip-0.1.tar` & `CONEstrip-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 08:18:43.328601 CONEstrip-0.1/
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     1338 2021-11-22 09:24:12.000000 CONEstrip-0.1/LICENSE
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     3525 2023-06-26 08:18:43.328601 CONEstrip-0.1/PKG-INFO
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     2963 2023-06-26 08:15:02.000000 CONEstrip-0.1/README.md
--rw-rw-r--   0 wieger    (1000) wieger    (1000)      104 2021-09-24 10:21:27.000000 CONEstrip-0.1/pyproject.toml
--rw-rw-r--   0 wieger    (1000) wieger    (1000)      687 2023-06-26 08:18:43.328601 CONEstrip-0.1/setup.cfg
-drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 08:18:43.320601 CONEstrip-0.1/src/
-drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 08:18:43.324601 CONEstrip-0.1/src/CONEstrip.egg-info/
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     3525 2023-06-26 08:18:43.000000 CONEstrip-0.1/src/CONEstrip.egg-info/PKG-INFO
--rw-rw-r--   0 wieger    (1000) wieger    (1000)      936 2023-06-26 08:18:43.000000 CONEstrip-0.1/src/CONEstrip.egg-info/SOURCES.txt
--rw-rw-r--   0 wieger    (1000) wieger    (1000)        1 2023-06-26 08:18:43.000000 CONEstrip-0.1/src/CONEstrip.egg-info/dependency_links.txt
--rw-rw-r--   0 wieger    (1000) wieger    (1000)       10 2023-06-26 08:18:43.000000 CONEstrip-0.1/src/CONEstrip.egg-info/top_level.txt
-drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 08:18:43.324601 CONEstrip-0.1/src/conestrip/
--rw-r--r--   0 wieger    (1000) wieger    (1000)        0 2022-01-31 16:22:11.000000 CONEstrip-0.1/src/conestrip/__init__.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     2673 2022-09-23 09:35:58.000000 CONEstrip-0.1/src/conestrip/cones.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     6501 2022-08-12 10:00:43.000000 CONEstrip-0.1/src/conestrip/conestrip_cdd.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)    15815 2022-08-12 09:59:03.000000 CONEstrip-0.1/src/conestrip/conestrip_z3.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     3284 2022-08-12 10:01:18.000000 CONEstrip-0.1/src/conestrip/extended_cones.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     2384 2022-08-12 09:59:03.000000 CONEstrip-0.1/src/conestrip/gamble_algorithms.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)      280 2022-09-29 12:48:29.000000 CONEstrip-0.1/src/conestrip/global_settings.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)    14782 2023-03-24 17:13:10.000000 CONEstrip-0.1/src/conestrip/optimization.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     3205 2022-02-04 08:23:03.000000 CONEstrip-0.1/src/conestrip/polyhedron.py
--rw-r--r--   0 wieger    (1000) wieger    (1000)     3065 2022-08-12 09:48:00.000000 CONEstrip-0.1/src/conestrip/prevision.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     4040 2022-08-12 09:59:32.000000 CONEstrip-0.1/src/conestrip/propositional_algorithms.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     1145 2022-06-24 10:52:38.000000 CONEstrip-0.1/src/conestrip/propositional_cones.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     9953 2022-08-12 09:51:55.000000 CONEstrip-0.1/src/conestrip/propositional_conestrip.py
--rwxrwxr-x   0 wieger    (1000) wieger    (1000)     2053 2022-06-10 07:27:02.000000 CONEstrip-0.1/src/conestrip/propositional_sentence_parser.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     3049 2022-10-27 12:36:23.000000 CONEstrip-0.1/src/conestrip/random_cones.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     6675 2022-08-12 10:01:30.000000 CONEstrip-0.1/src/conestrip/random_extended_cones.py
--rw-r--r--   0 wieger    (1000) wieger    (1000)     2656 2022-08-12 09:48:00.000000 CONEstrip-0.1/src/conestrip/sure_loss.py
--rw-rw-r--   0 wieger    (1000) wieger    (1000)     2299 2022-10-27 12:36:23.000000 CONEstrip-0.1/src/conestrip/utility.py
-drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 08:18:43.328601 CONEstrip-0.1/tests/
--rwxr-xr-x   0 wieger    (1000) wieger    (1000)     2207 2022-08-12 09:59:02.000000 CONEstrip-0.1/tests/test_algorithms.py
--rwxr-xr-x   0 wieger    (1000) wieger    (1000)    16433 2022-08-11 11:22:36.000000 CONEstrip-0.1/tests/test_cddlib.py
--rwxr-xr-x   0 wieger    (1000) wieger    (1000)     8310 2022-08-12 10:00:58.000000 CONEstrip-0.1/tests/test_conestrip.py
--rwxrwxr-x   0 wieger    (1000) wieger    (1000)     2222 2022-08-12 10:01:50.000000 CONEstrip-0.1/tests/test_conestrip_cdd.py
--rwxrwxr-x   0 wieger    (1000) wieger    (1000)     1723 2022-09-01 16:37:10.000000 CONEstrip-0.1/tests/test_optimization.py
--rwxr-xr-x   0 wieger    (1000) wieger    (1000)     2055 2022-08-12 10:02:03.000000 CONEstrip-0.1/tests/test_propositional_conestrip.py
+drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 09:46:31.271160 CONEstrip-0.1.1/
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     1338 2021-11-22 09:24:12.000000 CONEstrip-0.1.1/LICENSE
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     4296 2023-06-26 09:46:31.271160 CONEstrip-0.1.1/PKG-INFO
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     3732 2023-06-26 09:32:46.000000 CONEstrip-0.1.1/README.md
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)      104 2021-09-24 10:21:27.000000 CONEstrip-0.1.1/pyproject.toml
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)      689 2023-06-26 09:46:31.271160 CONEstrip-0.1.1/setup.cfg
+drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 09:46:31.267161 CONEstrip-0.1.1/src/
+drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 09:46:31.267161 CONEstrip-0.1.1/src/CONEstrip.egg-info/
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     4296 2023-06-26 09:46:31.000000 CONEstrip-0.1.1/src/CONEstrip.egg-info/PKG-INFO
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)      936 2023-06-26 09:46:31.000000 CONEstrip-0.1.1/src/CONEstrip.egg-info/SOURCES.txt
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)        1 2023-06-26 09:46:31.000000 CONEstrip-0.1.1/src/CONEstrip.egg-info/dependency_links.txt
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)       10 2023-06-26 09:46:31.000000 CONEstrip-0.1.1/src/CONEstrip.egg-info/top_level.txt
+drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 09:46:31.271160 CONEstrip-0.1.1/src/conestrip/
+-rw-r--r--   0 wieger    (1000) wieger    (1000)        0 2022-01-31 16:22:11.000000 CONEstrip-0.1.1/src/conestrip/__init__.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     2673 2022-09-23 09:35:58.000000 CONEstrip-0.1.1/src/conestrip/cones.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     6501 2022-08-12 10:00:43.000000 CONEstrip-0.1.1/src/conestrip/conestrip_cdd.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)    15815 2022-08-12 09:59:03.000000 CONEstrip-0.1.1/src/conestrip/conestrip_z3.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     3284 2022-08-12 10:01:18.000000 CONEstrip-0.1.1/src/conestrip/extended_cones.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     2384 2022-08-12 09:59:03.000000 CONEstrip-0.1.1/src/conestrip/gamble_algorithms.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)      280 2022-09-29 12:48:29.000000 CONEstrip-0.1.1/src/conestrip/global_settings.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)    14782 2023-03-24 17:13:10.000000 CONEstrip-0.1.1/src/conestrip/optimization.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     3205 2022-02-04 08:23:03.000000 CONEstrip-0.1.1/src/conestrip/polyhedron.py
+-rw-r--r--   0 wieger    (1000) wieger    (1000)     3065 2022-08-12 09:48:00.000000 CONEstrip-0.1.1/src/conestrip/prevision.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     4040 2022-08-12 09:59:32.000000 CONEstrip-0.1.1/src/conestrip/propositional_algorithms.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     1145 2022-06-24 10:52:38.000000 CONEstrip-0.1.1/src/conestrip/propositional_cones.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     9953 2022-08-12 09:51:55.000000 CONEstrip-0.1.1/src/conestrip/propositional_conestrip.py
+-rwxrwxr-x   0 wieger    (1000) wieger    (1000)     2053 2022-06-10 07:27:02.000000 CONEstrip-0.1.1/src/conestrip/propositional_sentence_parser.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     3049 2022-10-27 12:36:23.000000 CONEstrip-0.1.1/src/conestrip/random_cones.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     6675 2022-08-12 10:01:30.000000 CONEstrip-0.1.1/src/conestrip/random_extended_cones.py
+-rw-r--r--   0 wieger    (1000) wieger    (1000)     2656 2022-08-12 09:48:00.000000 CONEstrip-0.1.1/src/conestrip/sure_loss.py
+-rw-rw-r--   0 wieger    (1000) wieger    (1000)     2299 2022-10-27 12:36:23.000000 CONEstrip-0.1.1/src/conestrip/utility.py
+drwxrwxr-x   0 wieger    (1000) wieger    (1000)        0 2023-06-26 09:46:31.271160 CONEstrip-0.1.1/tests/
+-rwxr-xr-x   0 wieger    (1000) wieger    (1000)     2207 2022-08-12 09:59:02.000000 CONEstrip-0.1.1/tests/test_algorithms.py
+-rwxr-xr-x   0 wieger    (1000) wieger    (1000)    16433 2022-08-11 11:22:36.000000 CONEstrip-0.1.1/tests/test_cddlib.py
+-rwxr-xr-x   0 wieger    (1000) wieger    (1000)     8310 2022-08-12 10:00:58.000000 CONEstrip-0.1.1/tests/test_conestrip.py
+-rwxrwxr-x   0 wieger    (1000) wieger    (1000)     2222 2022-08-12 10:01:50.000000 CONEstrip-0.1.1/tests/test_conestrip_cdd.py
+-rwxrwxr-x   0 wieger    (1000) wieger    (1000)     1723 2022-09-01 16:37:10.000000 CONEstrip-0.1.1/tests/test_optimization.py
+-rwxr-xr-x   0 wieger    (1000) wieger    (1000)     2055 2022-08-12 10:02:03.000000 CONEstrip-0.1.1/tests/test_propositional_conestrip.py
```

### Comparing `CONEstrip-0.1/LICENSE` & `CONEstrip-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/PKG-INFO` & `CONEstrip-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: CONEstrip
-Version: 0.1
-Summary: An implementation of the CONEstrip algorithms using python and z3.
-Home-page: https://github.com/wiegerw/CONEstrip
-Author: Wieger Wesselink
-Author-email: j.w.wesselink@tue.nl
-Project-URL: Bug Tracker, https://github.com/wiegerw/CONEstrip/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # The CONEstrip library
 This repository contains a Python framework for reasoning with uncertainty.
 This is joint work with Erik Quaeghebeur. N.B. This is ongoing work, so not
 everything is finished yet.
 
 ## The CONEstrip algorithm
 In the paper [The CONEstrip algorithm](https://doi.org/10.1007/978-3-642-33042-1_6)
@@ -56,10 +41,29 @@
 The propositional CONEstrip algorithm is defined in terms of WPMaxSAT problems. We
 note that WPMaxSAT problems can be conveniently expressed using the propositional
 logic of Z3. Hence, also this algorithm has been implemented using
 [Z3](https://github.com/Z3Prover/z3).
 
 ## Documentation
 
-A detailed specification of the implementation can be found in [CONEstrip.pdf](doc/CONEstrip.pdf).
+A detailed specification of the implementation can be found in [CONEstrip.pdf](https://github.com/wiegerw/CONEstrip/blob/main/doc/CONEstrip.pdf).
 Note that this is not a tutorial, but rather a precise description of the algorithms
 that were implemented.
+
+## Installation
+
+The code is available as the PyPI package [CONEstrip](https://pypi.org/project/CONEstrip/).
+It can be installed using
+
+```
+pip install CONEstrip
+```
+
+## Licensing
+
+The code is available under the [Boost Software License 1.0](http://www.boost.org/LICENSE_1_0.txt).
+A [local copy](https://github.com/wiegerw/CONEstrip/blob/main/LICENSE) is included in the repository.
+
+For testing the [Toy Parser Generator](https://github.com/CDSoft/tpg) package is used.
+This package is available under the
+[GNU Lesser General Public License v2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) license.
+A [local copy](https://github.com/wiegerw/CONEstrip/blob/main/LGPL-2.1.txt) is included in the repository.
```

### Comparing `CONEstrip-0.1/setup.cfg` & `CONEstrip-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CONEstrip
-version = 0.1
+version = 0.1.1
 author = Wieger Wesselink
 author_email = j.w.wesselink@tue.nl
 description = An implementation of the CONEstrip algorithms using python and z3.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/wiegerw/CONEstrip
 project_urls =
```

### Comparing `CONEstrip-0.1/src/CONEstrip.egg-info/PKG-INFO` & `CONEstrip-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CONEstrip
-Version: 0.1
+Version: 0.1.1
 Summary: An implementation of the CONEstrip algorithms using python and z3.
 Home-page: https://github.com/wiegerw/CONEstrip
 Author: Wieger Wesselink
 Author-email: j.w.wesselink@tue.nl
 Project-URL: Bug Tracker, https://github.com/wiegerw/CONEstrip/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
@@ -56,10 +56,29 @@
 The propositional CONEstrip algorithm is defined in terms of WPMaxSAT problems. We
 note that WPMaxSAT problems can be conveniently expressed using the propositional
 logic of Z3. Hence, also this algorithm has been implemented using
 [Z3](https://github.com/Z3Prover/z3).
 
 ## Documentation
 
-A detailed specification of the implementation can be found in [CONEstrip.pdf](doc/CONEstrip.pdf).
+A detailed specification of the implementation can be found in [CONEstrip.pdf](https://github.com/wiegerw/CONEstrip/blob/main/doc/CONEstrip.pdf).
 Note that this is not a tutorial, but rather a precise description of the algorithms
 that were implemented.
+
+## Installation
+
+The code is available as the PyPI package [CONEstrip](https://pypi.org/project/CONEstrip/).
+It can be installed using
+
+```
+pip install CONEstrip
+```
+
+## Licensing
+
+The code is available under the [Boost Software License 1.0](http://www.boost.org/LICENSE_1_0.txt).
+A [local copy](https://github.com/wiegerw/CONEstrip/blob/main/LICENSE) is included in the repository.
+
+For testing the [Toy Parser Generator](https://github.com/CDSoft/tpg) package is used.
+This package is available under the
+[GNU Lesser General Public License v2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) license.
+A [local copy](https://github.com/wiegerw/CONEstrip/blob/main/LGPL-2.1.txt) is included in the repository.
```

### Comparing `CONEstrip-0.1/src/CONEstrip.egg-info/SOURCES.txt` & `CONEstrip-0.1.1/src/CONEstrip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/cones.py` & `CONEstrip-0.1.1/src/conestrip/cones.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/conestrip_cdd.py` & `CONEstrip-0.1.1/src/conestrip/conestrip_cdd.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/conestrip_z3.py` & `CONEstrip-0.1.1/src/conestrip/conestrip_z3.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/extended_cones.py` & `CONEstrip-0.1.1/src/conestrip/extended_cones.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/gamble_algorithms.py` & `CONEstrip-0.1.1/src/conestrip/gamble_algorithms.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/optimization.py` & `CONEstrip-0.1.1/src/conestrip/optimization.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/polyhedron.py` & `CONEstrip-0.1.1/src/conestrip/polyhedron.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/prevision.py` & `CONEstrip-0.1.1/src/conestrip/prevision.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/propositional_algorithms.py` & `CONEstrip-0.1.1/src/conestrip/propositional_algorithms.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/propositional_cones.py` & `CONEstrip-0.1.1/src/conestrip/propositional_cones.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/propositional_conestrip.py` & `CONEstrip-0.1.1/src/conestrip/propositional_conestrip.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/propositional_sentence_parser.py` & `CONEstrip-0.1.1/src/conestrip/propositional_sentence_parser.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/random_cones.py` & `CONEstrip-0.1.1/src/conestrip/random_cones.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/random_extended_cones.py` & `CONEstrip-0.1.1/src/conestrip/random_extended_cones.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/sure_loss.py` & `CONEstrip-0.1.1/src/conestrip/sure_loss.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/src/conestrip/utility.py` & `CONEstrip-0.1.1/src/conestrip/utility.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/tests/test_algorithms.py` & `CONEstrip-0.1.1/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/tests/test_cddlib.py` & `CONEstrip-0.1.1/tests/test_cddlib.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/tests/test_conestrip.py` & `CONEstrip-0.1.1/tests/test_conestrip.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/tests/test_conestrip_cdd.py` & `CONEstrip-0.1.1/tests/test_conestrip_cdd.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/tests/test_optimization.py` & `CONEstrip-0.1.1/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `CONEstrip-0.1/tests/test_propositional_conestrip.py` & `CONEstrip-0.1.1/tests/test_propositional_conestrip.py`

 * *Files identical despite different names*

