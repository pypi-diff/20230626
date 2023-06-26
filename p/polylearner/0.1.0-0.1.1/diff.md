# Comparing `tmp/polylearner-0.1.0.tar.gz` & `tmp/polylearner-0.1.1.tar.gz`

## Comparing `polylearner-0.1.0.tar` & `polylearner-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/__init__.py
--rw-r--r--   0        0        0    16273 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/lps.pl
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/hyperplanes/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/hyperplanes/__init__.py
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/hyperplanes/planes.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/hyperplanes/systems.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/learner/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/learner/__init__.py
--rw-r--r--   0        0        0    15704 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/learner/expressions.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/learner/polylearner.py
--rw-r--r--   0        0        0     9095 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/learner/symbolicsystems.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/learner/prolog/__init__.py
--rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 polylearner-0.1.0/src/learner/prolog/polylearner.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 polylearner-0.1.0/LICENSE
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 polylearner-0.1.0/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 polylearner-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 polylearner-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    18562 2020-02-02 00:00:00.000000 polylearner-0.1.1/learning.png
+-rw-r--r--   0        0        0    23379 2020-02-02 00:00:00.000000 polylearner-0.1.1/learning_parametrized.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0    16273 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/lps.pl
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/hyperplanes/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/hyperplanes/__init__.py
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/hyperplanes/planes.py
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/hyperplanes/systems.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/learner/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/learner/__init__.py
+-rw-r--r--   0        0        0    15704 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/learner/expressions.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/learner/polylearner.py
+-rw-r--r--   0        0        0     9095 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/learner/symbolicsystems.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/learner/prolog/__init__.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 polylearner-0.1.1/src/learner/prolog/polylearner.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 polylearner-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 polylearner-0.1.1/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 polylearner-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 polylearner-0.1.1/PKG-INFO
```

### Comparing `polylearner-0.1.0/src/lps.pl` & `polylearner-0.1.1/src/lps.pl`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/src/hyperplanes/README.md` & `polylearner-0.1.1/src/hyperplanes/README.md`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/src/hyperplanes/planes.py` & `polylearner-0.1.1/src/hyperplanes/planes.py`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/src/hyperplanes/systems.py` & `polylearner-0.1.1/src/hyperplanes/systems.py`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/src/learner/README.md` & `polylearner-0.1.1/src/learner/README.md`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/src/learner/expressions.py` & `polylearner-0.1.1/src/learner/expressions.py`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/src/learner/polylearner.py` & `polylearner-0.1.1/src/learner/polylearner.py`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/src/learner/symbolicsystems.py` & `polylearner-0.1.1/src/learner/symbolicsystems.py`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/src/learner/prolog/polylearner.py` & `polylearner-0.1.1/src/learner/prolog/polylearner.py`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/LICENSE` & `polylearner-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polylearner-0.1.0/README.md` & `polylearner-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 In simple terms, `P` generalizes `P1, .., Pn` by learning a *higher-level* polyhedron and its groundings to
 the *lower-level* polyhedra.
 
 We represent polyhedra as linear systems of the form `Ax <= b`, where `A` is a coefficient matrix, and `b` is vector
 of coefficients. 
 Take the following parametrized system
 
-<img height="237" src="./notebooks/learning_parametrized.png" width="357"/>
+<img height="237" src="./learning_parametrized.png" width="357"/>
 
 defined by a system `P`:
 ```
 x + y <= c
     y <= b
     x <= a
 ```
 
 by setting `a, b, c` to `1` we obtain the triangle on the left, while by setting `a, b` to `1` and `c` to `2`, we 
 obtain the square on the left; that is, `P` generalized both the triangle and rectangle.
 
-<img height="237" src="./notebooks/learning.png" width="460"/>
+<img height="237" src="./learning.png" width="460"/>
 
 # Quickstart
 ## Installation
 ```shell
 mkvirtualenv -p python3.11 polylearner
 pip install -r requirements.txt
 ```
```

### Comparing `polylearner-0.1.0/pyproject.toml` & `polylearner-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "polylearner"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Mattia Setzu", email="mattia.setzu@unipi.it" },
 ]
 description = "Learning from polyhedra: generalize multiple polyhedra into a parametric polyhedron."
 readme = "README.md"
 requires-python = ">3.10, <=3.11"
 classifiers = [
```

### Comparing `polylearner-0.1.0/PKG-INFO` & `polylearner-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylearner
-Version: 0.1.0
+Version: 0.1.1
 Summary: Learning from polyhedra: generalize multiple polyhedra into a parametric polyhedron.
 Project-URL: Homepage, https://github.com/msetzu/polylearner
 Project-URL: Bug Tracker, https://github.com/msetzu/polylearner/issues
 Author-email: Mattia Setzu <mattia.setzu@unipi.it>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -23,27 +23,27 @@
 In simple terms, `P` generalizes `P1, .., Pn` by learning a *higher-level* polyhedron and its groundings to
 the *lower-level* polyhedra.
 
 We represent polyhedra as linear systems of the form `Ax <= b`, where `A` is a coefficient matrix, and `b` is vector
 of coefficients. 
 Take the following parametrized system
 
-<img height="237" src="./notebooks/learning_parametrized.png" width="357"/>
+<img height="237" src="./learning_parametrized.png" width="357"/>
 
 defined by a system `P`:
 ```
 x + y <= c
     y <= b
     x <= a
 ```
 
 by setting `a, b, c` to `1` we obtain the triangle on the left, while by setting `a, b` to `1` and `c` to `2`, we 
 obtain the square on the left; that is, `P` generalized both the triangle and rectangle.
 
-<img height="237" src="./notebooks/learning.png" width="460"/>
+<img height="237" src="./learning.png" width="460"/>
 
 # Quickstart
 ## Installation
 ```shell
 mkvirtualenv -p python3.11 polylearner
 pip install -r requirements.txt
 ```
```

