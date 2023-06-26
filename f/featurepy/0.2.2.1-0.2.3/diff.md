# Comparing `tmp/featurepy-0.2.2.1.tar.gz` & `tmp/featurepy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurepy-0.2.2.1.tar", max compression
+gzip compressed data, was "featurepy-0.2.3.tar", max compression
```

## Comparing `featurepy-0.2.2.1.tar` & `featurepy-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,12 @@
--rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.2.2.1/LICENSE
--rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.2.2.1/README.md
--rw-r--r--   0        0        0      790 2023-06-14 13:43:09.864286 featurepy-0.2.2.1/pyproject.toml
--rw-r--r--   0        0        0      287 2023-06-11 09:55:40.361310 featurepy-0.2.2.1/src/featurepy/__init__.py
--rw-r--r--   0        0        0     1529 2023-06-14 00:06:33.902940 featurepy-0.2.2.1/src/featurepy/feature_class.py
--rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.2.2.1/src/featurepy/flask/__init__.py
--rw-r--r--   0        0        0      230 2023-05-18 14:59:44.476705 featurepy-0.2.2.1/src/featurepy/flask/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1901 2023-05-18 14:59:44.477827 featurepy-0.2.2.1/src/featurepy/flask/__pycache__/views.cpython-311.pyc
--rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.2.2.1/src/featurepy/flask/views.py
--rw-r--r--   0        0        0     3412 2023-06-13 23:31:59.687317 featurepy-0.2.2.1/src/featurepy/model_constraints.py
--rw-r--r--   0        0        0     1730 2023-06-11 15:46:14.698789 featurepy-0.2.2.1/src/featurepy/parametric_features.py
--rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.2.2.1/src/featurepy/scripts/__init__.py
--rw-r--r--   0        0        0      202 2023-06-03 17:07:40.240249 featurepy-0.2.2.1/src/featurepy/scripts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1328 2023-06-03 17:07:40.240691 featurepy-0.2.2.1/src/featurepy/scripts/__pycache__/features.cpython-311.pyc
--rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.2.2.1/src/featurepy/scripts/features.py
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 featurepy-0.2.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.2.3/LICENSE
+-rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.2.3/README.md
+-rw-r--r--   0        0        0      823 2023-06-26 21:47:34.127486 featurepy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-11 09:55:40.361310 featurepy-0.2.3/src/featurepy/__init__.py
+-rw-r--r--   0        0        0     1529 2023-06-14 00:06:33.902940 featurepy-0.2.3/src/featurepy/feature_class.py
+-rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.2.3/src/featurepy/flask/__init__.py
+-rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.2.3/src/featurepy/flask/views.py
+-rw-r--r--   0        0        0     3467 2023-06-21 09:40:58.948087 featurepy-0.2.3/src/featurepy/model_constraints.py
+-rw-r--r--   0        0        0     1773 2023-06-18 14:41:26.107466 featurepy-0.2.3/src/featurepy/parametric_features.py
+-rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.2.3/src/featurepy/scripts/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.2.3/src/featurepy/scripts/features.py
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 featurepy-0.2.3/PKG-INFO
```

### Comparing `featurepy-0.2.2.1/LICENSE` & `featurepy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.2.1/pyproject.toml` & `featurepy-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "featurepy"
-version = "0.2.2.1"
+version = "0.2.3"
 description = "Framework for building software product lines using feature-oriented programming (FOP) and aspect-oriented programming (AOP) in Python."
 authors = ["Adrian Wong <adrianwong227@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 featuremonkey3 = "^0.1.1"
@@ -20,11 +20,13 @@
 wtforms = "^3.0.1"
 beautifulsoup4 = "^4.12.2"
 flask-sqlalchemy = "^3.0.3"
 factory-boy = "^3.2.1"
 bootstrap-flask = "^2.2.0"
 flask-migrate = "^4.0.4"
 pytest = "^7.3.1"
+radon = "^6.0.1"
+numpy = "^1.25.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `featurepy-0.2.2.1/src/featurepy/feature_class.py` & `featurepy-0.2.3/src/featurepy/feature_class.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.2.1/src/featurepy/flask/views.py` & `featurepy-0.2.3/src/featurepy/flask/views.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.2.2.1/src/featurepy/model_constraints.py` & `featurepy-0.2.3/src/featurepy/model_constraints.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from aspectlib import Aspect, Proceed
 from yaml import safe_load
 
+# TODO: Re-order features
+
 
 class FeatureSelectionError(Exception):
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
 
@@ -38,15 +40,15 @@
 
 def _is_operator(token: str) -> bool:
     return token in ["or", "and", "not"]
 
 
 def parse_reqs(reqs, selections):
     tokens = reqs.split()
-    expr = " ".join([f"{token} in selections" if not _is_operator(
+    expr = " ".join([f"'{token}' in selections" if not _is_operator(
         token) else token for token in tokens])
     return eval(expr)
 
 
 def validate_selections(fm, selections: list[str], remaining_selections: list[str]):
     if not is_optional(fm) and not is_abstract(fm) and fm['name'] not in selections:
         raise FeatureSelectionError(
@@ -62,15 +64,15 @@
     if (is_abstract(fm) or fm['name'] in selections) and has_children(fm):
 
         if is_branch(fm, 'xor') and len(set([child['name'] for child in fm['children']]).intersection(set(selections))) != 1:
             raise FeatureSelectionError(
                 f"Incorrect number of xor features selected for branch {fm['name']}")
 
         for child in fm['children']:
-            if child['name'] in selections and selections.index(child['name']) > selections.index(fm['name']):
+            if not is_abstract(fm) and (child['name'] in selections and selections.index(child['name']) > selections.index(fm['name'])):
                 raise FeatureSelectionError(
                     f"Child feature {child['name']} is selected before parent {fm['name']}.")
             if is_branch(fm, 'or'):
                 child['optional'] = True
             remaining_selections = validate_selections(
                 child, selections, remaining_selections)
```

### Comparing `featurepy-0.2.2.1/src/featurepy/parametric_features.py` & `featurepy-0.2.3/src/featurepy/parametric_features.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from featuremonkey3 import CompositionError
 from aspectlib import Aspect, Return
 import inspect
 import importlib
 import re
 
+# TODO: Pass parameters to child features
+
 
 def parse_feature_args(feature: str) -> list[str]:
     # CANNOT PARSE LISTS, DICTS OR ANY DATA TYPE WITH COMMAS AND BRACKETS
     tokens = re.split("[(,)]", feature)
     featurename = tokens[0]
     args = []
     kwargs = {}
```

### Comparing `featurepy-0.2.2.1/PKG-INFO` & `featurepy-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurepy
-Version: 0.2.2.1
+Version: 0.2.3
 Summary: Framework for building software product lines using feature-oriented programming (FOP) and aspect-oriented programming (AOP) in Python.
 Author: Adrian Wong
 Author-email: adrianwong227@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aspectlib (>=2.0.0,<3.0.0)
```

