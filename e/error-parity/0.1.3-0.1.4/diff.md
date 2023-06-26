# Comparing `tmp/error-parity-0.1.3.tar.gz` & `tmp/error-parity-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-parity-0.1.3.tar", last modified: Fri Jun 16 14:07:05 2023, max compression
+gzip compressed data, was "error-parity-0.1.4.tar", last modified: Mon Jun 26 14:21:21 2023, max compression
```

## Comparing `error-parity-0.1.3.tar` & `error-parity-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 14:06:55.000000 error-parity-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 14:06:55.000000 error-parity-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-16 14:07:05.620197 error-parity-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-16 14:06:55.000000 error-parity-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/error_parity/
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/equal_odds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/roc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/error_parity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 14:06:55.000000 error-parity-0.1.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 14:06:55.000000 error-parity-0.1.3/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 14:06:55.000000 error-parity-0.1.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:07:05.620197 error-parity-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-16 14:06:55.000000 error-parity-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:55.000000 error-parity-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-16 14:06:55.000000 error-parity-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-16 14:06:55.000000 error-parity-0.1.3/tests/test_equal_odds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 14:21:08.000000 error-parity-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 14:21:08.000000 error-parity-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-26 14:21:21.744439 error-parity-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-26 14:21:08.000000 error-parity-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/error_parity/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/equal_odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-26 14:21:08.000000 error-parity-0.1.4/error_parity/roc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/error_parity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 14:21:21.000000 error-parity-0.1.4/error_parity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 14:21:08.000000 error-parity-0.1.4/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 14:21:08.000000 error-parity-0.1.4/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 14:21:08.000000 error-parity-0.1.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:21:21.744439 error-parity-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-26 14:21:08.000000 error-parity-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:21.744439 error-parity-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:21:08.000000 error-parity-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-26 14:21:08.000000 error-parity-0.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-26 14:21:08.000000 error-parity-0.1.4/tests/test_cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-26 14:21:08.000000 error-parity-0.1.4/tests/test_equal_odds.py
```

### Comparing `error-parity-0.1.3/LICENSE` & `error-parity-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.3/PKG-INFO` & `error-parity-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.3
+Version: 0.1.4
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/AndreFCruz/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -95,7 +95,14 @@
   - i.e., equal group-specific TPR and FPR;
 
 Road-map:
 - [ ] equal opportunity;
   - i.e., equal group-specific TPR;
 - [ ] demographic parity;
   - i.e., equal group-specific predicted prevalence;
+
+
+## Citing
+
+This repository contains code and supplementary materials for the following preprint:
+
+> André F. Cruz and Moritz Hardt. "Unprocessing Seven Years of Algorithmic Fairness." [arXiv preprint, 2023](https://arxiv.org/pdf/2306.07261.pdf).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `error-parity-0.1.3/README.md` & `error-parity-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,7 +70,14 @@
   - i.e., equal group-specific TPR and FPR;
 
 Road-map:
 - [ ] equal opportunity;
   - i.e., equal group-specific TPR;
 - [ ] demographic parity;
   - i.e., equal group-specific predicted prevalence;
+
+
+## Citing
+
+This repository contains code and supplementary materials for the following preprint:
+
+> André F. Cruz and Moritz Hardt. "Unprocessing Seven Years of Algorithmic Fairness." [arXiv preprint, 2023](https://arxiv.org/pdf/2306.07261.pdf).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `error-parity-0.1.3/error_parity/classifiers.py` & `error-parity-0.1.4/error_parity/classifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Helper functions to construct and use randomized classifiers.
 """
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
-from typing import Dict, List, Callable
+from typing import Callable
 
 import numpy as np
 from scipy.spatial import ConvexHull
 
 
 class Classifier(ABC):
     @abstractmethod
@@ -92,15 +92,15 @@
         return (self.rng.random(size=len(X)) >= (1 - self.target_fpr)).astype(int)
 
 
 class EnsembleGroupwiseClassifiers(Classifier):
     """Constructs a classifier from a set of group-specific classifiers.
     """
 
-    def __init__(self, group_to_clf: Dict[int | str, Callable]):
+    def __init__(self, group_to_clf: dict[int | str, Callable]):
         """Constructs a classifier from a set of group-specific classifiers.
 
         Must be provided exactly one classifier per unique group value.
 
         Parameters
         ----------
         group_to_clf : dict[int | str, callable]
@@ -122,45 +122,46 @@
 
         Returns
         -------
         y_pred : np.ndarray
             The predictions, where the prediction for each sample is handed off
             to a group-specific classifier for that sample.
         """
-        assert len(X) == len(group)
-        num_samples = len(X)
+        if len(X) != len(group):
+            raise ValueError(f"Invalid input sizes len(X) != len(group)")
 
         # Array to store predictions
+        num_samples = len(X)
         y_pred = np.zeros(num_samples)
 
         # Filter to keep track of all samples that received a prediction
         cumulative_filter = np.zeros(num_samples).astype(bool)
 
         for group_value, group_clf in self.group_to_clf.items():
             group_filter = (group == group_value)
             y_pred[group_filter] = group_clf(X[group_filter])
             cumulative_filter |= group_filter
 
-        assert np.sum(cumulative_filter) == num_samples, (
-            f"Computed group-wise predictions for {np.sum(cumulative_filter)} "
-            f"samples, but got {num_samples} input samples."
-        )
+        if np.sum(cumulative_filter) != num_samples:
+            raise RuntimeError(
+                f"Computed group-wise predictions for {np.sum(cumulative_filter)} "
+                f"samples, but got {num_samples} input samples.")
 
         return y_pred
 
 
 class RandomizedClassifier(Classifier):
     """Constructs a randomized classifier from the given  classifiers and 
     their probabilities.
     """
 
     def __init__(
             self,
-            classifiers: List[Classifier],
-            probabilities: List[float],
+            classifiers: list[Classifier],
+            probabilities: list[float],
             seed: int = 42,
         ):
         """Constructs a randomized classifier from the given  classifiers and 
         their probabilities.
         
         This classifier will compute predictions for the whole input dataset at 
         once, which will in general be faster for larger inputs (when compared 
@@ -178,15 +179,19 @@
             A random seed, by default 42.
 
         Returns
         -------
         callable
             The corresponding randomized classifier.
         """
-        assert len(classifiers) == len(probabilities)
+        if len(classifiers) != len(probabilities):
+            raise ValueError(
+                f"Invalid arguments: len(classifiers) != len(probabilities); "
+                f"({len(classifiers)} != {len(probabilities)});")
+
         self.classifiers = classifiers
         self.probabilities = probabilities
         self.rng = np.random.default_rng(seed)
     
     def __call__(self, X: np.ndarray, group: np.ndarray = None) -> int:
         # Assign each sample to a classifier
         clf_idx = self.rng.choice(
@@ -230,43 +235,54 @@
         if all(np.isclose(point_B, target_point)):
             return np.array([1]), np.expand_dims(point_B, axis=0)
         
         # If not, we'll have to triangulate the target using A and B
         point_A_fpr, point_A_tpr = point_A
         point_B_fpr, point_B_tpr = point_B
         target_fpr, target_tpr = target_point
-        assert point_A_fpr <= target_fpr <= point_B_fpr, (
-            f"FALSE: {point_A_fpr} <= {target_fpr} <= {point_B_fpr}"
-        )
+        if not (point_A_fpr <= target_fpr <= point_B_fpr):
+            raise ValueError(
+                f"Invalid input. FPR should fulfill: "
+                f"({point_A_fpr} point_A_FPR) <= ({target_fpr} target_fpr) <= "
+                f"({point_B_fpr} point_B_fpr)")
 
         # Calculate weights for points A and B
         weight_A = (target_fpr - point_B_fpr) / (point_A_fpr - point_B_fpr)
 
         # Result of projecting target point P directly UPWARDS towards the AB line
         weights_AB = np.array([weight_A, 1 - weight_A])
         point_P_upwards = weights_AB @ np.vstack((point_A, point_B))
-        assert np.isclose(point_P_upwards[0], target_fpr)
+        if not np.isclose(point_P_upwards[0], target_fpr):
+            raise RuntimeError(
+                "Failed projecting target_fpr to ROC hull frontier. "
+                f"Got proj. FPR={point_P_upwards[0]}; target FPR={target_fpr};")
         
         # Check if the target point lies in the AB line (and return if so)
         if all(np.isclose(point_P_upwards, target_point)):
             return weights_AB, np.vstack((point_A, point_B))
 
         # Result of projecting target point P directly DOWNWARDS towards the diagonal tpr==fpr
         point_P_downwards = np.array([target_fpr, target_fpr])
 
         # Calculate weights for P upwards and P downwards
         weight_P_upwards = (target_tpr - point_P_downwards[1]) / (point_P_upwards[1] - point_P_downwards[1])
 
-        # Sanity check...
+        # Sanity checks...
         all_points = np.vstack((point_A, point_B, point_P_downwards))
         all_weights = np.hstack((weight_P_upwards * weights_AB, 1 - weight_P_upwards))
 
-        assert np.isclose(all_weights.sum(), 1)
-        # assert all(all_weights <= 1) and all(all_weights >= 0)
-        assert all(np.isclose(target_point, all_weights @ all_points))
+        if not np.isclose(all_weights.sum(), 1):
+            raise RuntimeError(
+                f"Sum of linear interpolation weights was {all_weights.sum()}, "
+                f"should be 1!")
+
+        if not all(np.isclose(target_point, all_weights @ all_points)):
+            raise RuntimeError(
+                f"Triangulation of target point failed. "
+                f"Target was {target_point}; got {all_weights @ all_points}.")
 
         return all_weights, all_points
 
     @staticmethod
     def construct_at_target_ROC(
             predictor: callable,
             roc_curve_data: tuple,
@@ -296,19 +312,25 @@
         # Unpack useful constants
         target_fpr, target_tpr = target_roc_point
         fpr, tpr, thrs = roc_curve_data
 
         # Check if we have more than two ROC points
         # (3 minimum to compute convex hull)
         if len(fpr) <= 1:
-            raise ValueError(f"Invalid ROC curve data for classifier: fpr:{fpr}; tpr:{tpr};")
+            raise ValueError(
+                f"Invalid ROC curve data (only has one point): "
+                f"fpr:{fpr}; tpr:{tpr}.")
 
         if len(fpr) == 2:
             logging.warning(f"Got ROC data with only 2 points: producing a random classifier...")
-            assert np.isclose(target_roc_point[0], target_roc_point[1])
+            if not np.isclose(target_roc_point[0], target_roc_point[1]):
+                logging.error(
+                    f"Invalid target ROC point ({target_roc_point}) is not in "
+                    "diagonal ROC line, but a random-classifier ROC was provided.")
+
             return BinaryClassifierAtROCDiagonal(target_fpr=target_roc_point[0])
 
         # Compute hull of ROC curve
         roc_curve_points = np.stack((fpr, tpr), axis=1)
         hull = ConvexHull(roc_curve_points)
 
         # Filter out ROC points in the interior of the convex hull and other suboptimal points
@@ -333,53 +355,59 @@
         weights, points = RandomizedClassifier.find_weights_given_two_points(
             point_A=point_A_roc,
             point_B=point_B_roc,
             target_point=target_roc_point,
         )
 
         if max(weights) > 1:
-            logging.error(f"This should never happen; got weights over 100%: w={weights}")
-            import ipdb; ipdb.set_trace()
+            logging.error(f"Got triangulation weights over 100%: w={weights};")
 
         # Instantiate classifiers for points A and B
         clf_a = BinaryClassifier(predictor, threshold=thrs[point_A_idx])
         clf_b = BinaryClassifier(predictor, threshold=thrs[point_B_idx])
 
-        # If all weight is on a single deterministic point, return that deterministic classifier
-        if len(weights) == 1:
-            assert np.isclose(max(weights), 1.0)
+        # Check if most of the probability mass is on a single classifier
+        if np.isclose(max(weights), 1.0):
             if all(np.isclose(target_roc_point, point_A_roc)):
                 return clf_a
 
             elif all(np.isclose(target_roc_point, point_B_roc)):
                 return clf_b
             
             else:
-                raise RuntimeError("Invalid triangulation.")
+                # differences from target point to A or B are significant enough
+                # to warrant triangulating between multiple points
+                pass
+
+        # If only one point returned, then that point should have weight==1.0
+        # (hence, should've been caught by the previous if statement)
+        if len(weights) == 1:
+            raise RuntimeError("Invalid triangulation.")
         
         # If there are two points, return a randomized classifier between the two
         elif len(weights) == 2:
-            if np.isclose(max(weights), 1.0):
-                logging.warning(f"TODO: could use a single deterministic classifier")   # TODO
-
             return RandomizedClassifier(
                 classifiers=[clf_a, clf_b],
                 probabilities=weights,
                 seed=seed,
             )
 
         # If it's in the interior of the ROC curve, requires instantiating a randomized classifier at the diagonal
         elif len(weights) == 3:
             fpr_rand, tpr_rand = points[2]
-            assert fpr_rand == tpr_rand
+            if not np.isclose(fpr_rand, tpr_rand):
+                raise RuntimeError(
+                    f"Triangulation point at ROC diagonal has FPR != TPR "
+                    f"({fpr_rand} != {tpr_rand}); ")
+
             # >>> BUG this would be better but for some reason it doesn't work!
             # rng = np.random.default_rng(42)
             # clf_rand = lambda X: (rng.random(size=len(X)) >= (1 - fpr_rand)).astype(int)
             # # or...
-            # clf_rand = BinaryClassifierAtROCDiagonal(target_fpr=fpr_rand)   # BUG
+            # clf_rand = BinaryClassifierAtROCDiagonal(target_fpr=fpr_rand)
             # <<<
             clf_rand = lambda X: (np.random.random(size=len(X)) >= (1 - fpr_rand)).astype(int)
 
             return RandomizedClassifier(
                 classifiers=[clf_a, clf_b, clf_rand],
                 probabilities=weights,
                 seed=seed)
```

### Comparing `error-parity-0.1.3/error_parity/cvxpy_utils.py` & `error-parity-0.1.4/error_parity/cvxpy_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 """A set of helper functions for using cvxpy.
 """
+from __future__ import annotations
 import logging
-import operator
 from itertools import product
-from typing import Dict, Tuple, List
 
 import numpy as np
 import cvxpy as cp
 from cvxpy.expressions.variable import Variable
 from cvxpy.expressions.expression import Expression
 
 from .roc_utils import calc_cost_of_point, compute_global_roc_from_groupwise
 
 
 # Maximum distance from solution to feasibility or optimality
 SOLUTION_TOLERANCE = 1e-9
 
 
-def compute_line(p1, p2):
+def compute_line(p1: np.ndarray, p2: np.ndarray) -> tuple[float, float]:
     """Computes the slope and intercept of the line that passes
     through the two given points.
     
     The intercept is the value at x=0!
     (or NaN for vertical lines)
     
     For vertical lines just use the x-value of one of the points
     to find the intercept at y=0.
+
+    Parameters
+    ----------
+    p1 : np.ndarray
+        A 2-D point.
+    p2 : np.ndarray
+        A 2-D point.
+
+    Returns
+    -------
+    tuple[float, float]
+        A tuple pair with (slope, intercept) of the line that goes from p1 to p2.
+
+    Raises
+    ------
+    ValueError
+        Raised when input is invalid, e.g., when p1 == p2.
     """
+
     p1x, p1y = p1
     p2x, p2y = p2
     if all(p1 == p2):
         raise ValueError("Invalid points: p1==p2;")
 
     # Vertical line
     if np.isclose(p2x, p1x):
@@ -41,54 +58,79 @@
     else:
         slope = (p2y - p1y) / (p2x - p1x)
         intercept = p1y - slope * p1x
 
     return slope, intercept
 
 
-def compute_halfspace_inequality(p1, p2):
-    """Computes the halfspace inequality defined by the vector p1->p2;
-    -> input points must be in COUNTER CLOCK-WISE order (right-hand rule);
-    -> as such, the inequality enforces that points must lie on the right
-    of the line defined by the p1->p2 vector;
-    -> where "right" depends on the direction of the vector;
-    
-    Return
+def compute_halfspace_inequality(
+        p1: np.ndarray,
+        p2: np.ndarray,
+    ) -> tuple[float, float, float]:
+    """Computes the halfspace inequality defined by the vector p1->p2, such that
+        Ax + b <= 0,
+        where A and b are extracted from the line that goes through p1->p2.
+
+    As such, the inequality enforces that points must lie on the LEFT of the 
+    line defined by the p1->p2 vector.
+
+    In other words, input points are assumed to be in COUNTER CLOCK-WISE order 
+    (right-hand rule).
+
+    Parameters
+    ----------
+    p1 : np.ndarray
+        A point in the halfspace.
+    p2 : np.ndarray
+        Another point in the halfspace.
+
+    Returns
+    -------
+    tuple[float, float, float]
+        Returns an array of size=(n_dims + 1), with format [A; b],
+        representing the inequality Ax + b <= 0.
+
+    Raises
     ------
-    Returns an array of size=(n_dims + 1), with format [A; b],
-    representing the inequality Ax + b <= 0.
+    RuntimeError
+        Thrown in case if inconsistent internal state variables.
     """
     slope, intercept = compute_line(p1, p2)
 
     # Unpack the points for ease of use
     p1x, p1y = p1
     p2x, p2y = p2
 
-    # if slope is infinity, the constraint only applies to the values of x
-    # - the b intercept value will correspond to this value of x;
-    # - the sign of the constraint will depend on the vector p1->p2 pointing
-    # downards (x <= b) or upwards (x >= b);
+    # if slope is infinity, the constraint only applies to the values of x;
+    # > the halfspace's b intercept value will correspond to this value of x;
     if np.isinf(slope):
-        assert np.isclose(p1x, p2x)
+
+        # Sanity check for vertical line
+        if not np.isclose(p1x, p2x):
+            raise RuntimeError(
+                "Got infinite slope for line containing two points with "
+                "different x-axis coordinates.")
         
-        # Vector pointing downards? then, x >= b
+        # Vector pointing downwards? then, x >= b
         if p2y < p1y:
             return [-1, 0, p1x]
         
         # Vector pointing upwards? then, x <= b
         elif p2y > p1y:
             return [1, 0, -p1x]
         
-    # elif slope is zero, the constraint only applies to the values of y
-    # - we still need to figure out the sign of y in the inequality;
-    # - may be y <= b or y >= b, depending on whether p1->p2 points
-    # rightwards (y <= b) or leftwards (y >= b);
+    # elif slope is zero, the constraint only applies to the values of y;
+    # > the halfspace's b intercept value will correspond to this value of y;
     elif np.isclose(slope, 0.0):
-        assert np.isclose(p1y, p2y)
-        assert np.isclose(p1y, intercept)
+
+        # Sanity checks for horizontal line
+        if not np.isclose(p1y, p2y) or not np.isclose(p1y, intercept):
+            raise RuntimeError(
+                f"Invalid horizontal line; points p1 and p2 should have same "
+                f"y-axis value as intercept ({p1y}, {p2y}, {intercept}).")
 
         # Vector pointing leftwards? then, y <= b
         if p2x < p1x:
             return [0, 1, -p1y]
         
         # Vector pointing rightwards? then, y >= b
         elif p2x > p1x:
@@ -107,68 +149,81 @@
         elif p2x > p1x:
             return [slope, -1, intercept]
         
     logging.error(f"No constraint can be concluded from points p1={p1} and p2={p2};")
     return [0, 0, 0]
 
 
-def polygon_halfspace_inequalities(points: np.ndarray) -> np.ndarray:
-    """Parses the given points of a polygon, in COUNTER CLOCK-WISE order,
-    and constructs halfspaces from each consecutive pair of points.
-    
-    Output is in scipy.spatial.HalfspaceIntersection format;
-    i.e., an ndarray of format [A; b], for Ax + b <= 0.
-    """
-    # Array of shape (num_inequalities, num_dims + 1)
-    halfspaces = np.ndarray(shape=(len(points), points.shape[-1] + 1), dtype=float)
-
-    for i in range(len(points)):
-        p1 = np.ravel(points[i])
-        p2 = np.ravel(points[(i+1) % len(points)])
+def make_cvxpy_halfspace_inequality(
+        p1: np.ndarray,
+        p2: np.ndarray,
+        cvxpy_point: Variable,
+    ) -> Expression:
+    """Creates a single cvxpy inequality constraint that enforces the given 
+    point, `cvxpy_point`, to lie on the left of the vector p1->p2.
 
-        halfspaces[i] = compute_halfspace_inequality(p1, p2)
-    
-    return halfspaces
+    Points must be sorted in counter clock-wise order!
 
+    Parameters
+    ----------
+    p1 : np.ndarray
+        A point p1.
+    p2 : np.ndarray
+        Another point p2.
+    cvxpy_point : Variable
+        The cvxpy variable over which the constraint will be applied.
 
-def make_cvxpy_halfspace_inequality(p1, p2, cvxpy_point: Variable):
-    """Points sorted in counter clock-wise order!
+    Returns
+    -------
+    Expression
+        A linear inequality constraint of type Ax + b <= 0.
     """
     x_coeff, y_coeff, b = compute_halfspace_inequality(p1, p2)
     return np.array([x_coeff, y_coeff]) @ cvxpy_point + b <= 0
 
 
 def make_cvxpy_point_in_polygon_constraints(
         polygon_vertices: np.ndarray,
-        cvxpy_point: Variable
-    ) -> Expression:
-    """Creates the set of cvxpy constraints that force the given cvxpy variables
-    to lie within the polygon defined by the given vertices.
-    
-    Polygon points sorted in COUNTER CLOCK-WISE order!
+        cvxpy_point: Variable,
+    ) -> list[Expression]:
+    """Creates the set of cvxpy constraints that force the given cvxpy variable
+    point to lie within the polygon defined by the given vertices.
+
+    Parameters
+    ----------
+    polygon_vertices : np.ndarray
+        A sequence of points that make up a polygon.
+        Points must be sorted in COUNTER CLOCK-WISE order! (right-hand rule)
+    cvxpy_point : cvxpy.Variable
+        A cvxpy variable representing a point, over which the constraints will
+        be applied.
+
+    Returns
+    -------
+    list[Expression]
+        A list of cvxpy constraints.
     """
     return [
         make_cvxpy_halfspace_inequality(
             polygon_vertices[i], polygon_vertices[(i+1) % len(polygon_vertices)],
             cvxpy_point,
         )
         for i in range(len(polygon_vertices))
     ]
 
 
-
 def compute_equal_odds_optimum(
-        groupwise_roc_hulls: Dict[int, np.ndarray],
+        groupwise_roc_hulls: dict[int, np.ndarray],
         fairness_tolerance: float,
         group_sizes_label_pos: np.ndarray,
         group_sizes_label_neg: np.ndarray,
         global_prevalence: float,
         false_positive_cost: float = 1.,
         false_negative_cost: float = 1.,
-    ) -> Tuple[np.ndarray, np.ndarray]:
+    ) -> tuple[np.ndarray, np.ndarray]:
     """Computes the solution to finding the optimal fair (equal odds) classifier.
 
     Can relax the equal odds constraint by some given tolerance.
 
     Parameters
     ----------
     groupwise_roc_hulls : dict[int, np.ndarray]
@@ -189,20 +244,23 @@
         The cost of a FALSE POSITIVE error, by default 1.
     false_negative_cost : float, optional
         The cost of a FALSE NEGATIVE error, by default 1.
 
     Returns
     -------
     (groupwise_roc_points, global_roc_point) : tuple[np.ndarray, np.ndarray]
-        A pair tuple, (<1>, <2>), containing:
+        A tuple pair, (<1>, <2>), containing:
         1: an array with the group-wise ROC points for the solution.
         2: an array with the single global ROC point for the solution.
     """
     n_groups = len(groupwise_roc_hulls)
-    assert n_groups == len(group_sizes_label_neg) == len(group_sizes_label_pos)
+    if n_groups != len(group_sizes_label_neg) or n_groups != len(group_sizes_label_pos):
+        raise ValueError(
+            f"Invalid arguments; all of the following should have the same "
+            f"length: groupwise_roc_hulls, group_sizes_label_neg, group_sizes_label_pos;")
 
     # Group-wise ROC points
     groupwise_roc_points_vars = [
         cp.Variable(shape=2, name=f"ROC point for group {i}", nonneg=True)
         for i in range(n_groups)
     ]
 
@@ -239,59 +297,66 @@
         false_pos_cost=false_positive_cost,
         false_neg_cost=false_negative_cost,
     ))
 
     # Define cvxpy problem
     prob = cp.Problem(obj, constraints)
 
-    # _plot_polygons([groupwise_roc_hulls[i] for i in range(n_groups)]) # NOTE: just for debugging
-
     # Run solver
     prob.solve(solver=cp.ECOS, abstol=SOLUTION_TOLERANCE, feastol=SOLUTION_TOLERANCE)
     # NOTE: these tolerances are supposed to be smaller than the default np.isclose tolerances
     # (useful when comparing if two points are the same, within the cvxpy accuracy tolerance)
 
     # Log solution
     logging.info(f"cvxpy solver took {prob.solver_stats.solve_time}s; status is {prob.status}.")
 
     if prob.status not in ["infeasible", "unbounded"]:
         # Otherwise, problem.value is inf or -inf, respectively.
         logging.info(f"Optimal solution value: {prob.value}")
         for variable in prob.variables():
             logging.info(f"Variable {variable.name()}: value {variable.value}")
     else:
-        import ipdb; ipdb.set_trace()   # TODO
+        # This line should never be reached (there are always trivial fair
+        # solutions in the ROC diagonal)
         raise ValueError(f"cvxpy problem has no solution; status={prob.status}")
 
     groupwise_roc_points = np.vstack([p.value for p in groupwise_roc_points_vars])
     global_roc_point = global_roc_point_var.value
 
     # Sanity check solution cost
-    assert np.isclose(
-        prob.value,
-        calc_cost_of_point(
-            fpr=global_roc_point[0],
-            fnr=1-global_roc_point[1],
-            prevalence=global_prevalence,
-            false_pos_cost=false_positive_cost,
-            false_neg_cost=false_negative_cost,
-        ))
+    solution_cost = calc_cost_of_point(
+        fpr=global_roc_point[0],
+        fnr=1-global_roc_point[1],
+        prevalence=global_prevalence,
+        false_pos_cost=false_positive_cost,
+        false_neg_cost=false_negative_cost,
+    )
+
+    if not np.isclose(solution_cost, prob.value):
+        logging.error(
+            f"Solution was found but cost did not pass sanity check! "
+            f"Found solution ROC point {global_roc_point} with theoretical cost "
+            f"{prob.value}, but actual cost is {solution_cost};")
 
     # Sanity check congruency between group-wise ROC points and global ROC point
     global_roc_from_groupwise = compute_global_roc_from_groupwise(
         groupwise_roc_points=groupwise_roc_points,
         groupwise_label_pos_weight=group_sizes_label_pos,
         groupwise_label_neg_weight=group_sizes_label_neg,
     )
-    assert all(np.isclose(global_roc_from_groupwise, global_roc_point))
+    if not all(np.isclose(global_roc_from_groupwise, global_roc_point)):
+        logging.error(
+            f"Solution: global ROC point ({global_roc_point}) does not seem to "
+            f"match group-wise ROC points; global should be "
+            f"({global_roc_from_groupwise}) to be consistent with group-wise;")
 
     return groupwise_roc_points, global_roc_point
 
 
-def _plot_polygons(polygons: List[np.ndarray]):
+def _plot_polygons(polygons: list[np.ndarray]):
     from matplotlib import pyplot as plt
     fig = plt.figure(dpi=200, figsize=(5, 5))
 
     for i, poly in enumerate(polygons):
 
         # Plot ROC curve
         plt.fill(
```

### Comparing `error-parity-0.1.3/error_parity/equal_odds.py` & `error-parity-0.1.4/error_parity/equal_odds.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,17 @@
         # Relative group sizes for LN and LP samples
         group_sizes_label_neg = np.array([
             np.sum(1 - y[group == g]) for g in unique_groups
         ])
         group_sizes_label_pos = np.array([
             np.sum(y[group == g]) for g in unique_groups
         ])
-        assert np.sum(group_sizes_label_neg) + np.sum(group_sizes_label_pos) == len(y)
+
+        if np.sum(group_sizes_label_neg) + np.sum(group_sizes_label_pos) != len(y):
+            raise RuntimeError(f"Failed sanity check. Are you using non-binary labels?")
 
         # Convert to relative sizes
         group_sizes_label_neg = group_sizes_label_neg.astype(float) / np.sum(group_sizes_label_neg)
         group_sizes_label_pos = group_sizes_label_pos.astype(float) / np.sum(group_sizes_label_pos)
 
         # Compute group-wise ROC curves
         if y_scores is None:
@@ -427,14 +429,12 @@
         # Set axis settings
         plt.title(f"Solution to {self.tolerance}-relaxed equal odds optimum")
         plt.xlabel("False Positive Rate")
         plt.ylabel("True Positive Rate")
 
         plt.legend(loc="lower right", borderaxespad=2)
 
-        # plt.show()
-
     def __call__(self, X: np.ndarray, group: np.ndarray) -> int:
         return self._realized_classifier(X, group)
 
     def predict(self, X: np.ndarray, group: np.ndarray) -> int:
         return self(X, group)
```

### Comparing `error-parity-0.1.3/error_parity/roc_utils.py` & `error-parity-0.1.4/error_parity/roc_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,15 +94,21 @@
     global_roc_point : np.ndarray
         A single point that corresponds to the global outcome of the given
         group-wise ROC points.
     """
     n_groups, _ = groupwise_roc_points.shape
 
     # Some initial sanity checks
-    assert len(groupwise_label_pos_weight) == len(groupwise_label_neg_weight) == n_groups
+    if (len(groupwise_label_pos_weight) != len(groupwise_label_neg_weight) or
+        len(groupwise_label_pos_weight) != n_groups):
+       raise ValueError(
+           "Invalid input shapes: length of all arguments must be equal (the "
+           "number of different sensitive groups).")
+
+    # Normalize group LP (/LN) weights by their size
     if not np.isclose(groupwise_label_pos_weight.sum(), 1.0):
         groupwise_label_pos_weight /= groupwise_label_pos_weight.sum()
     if not np.isclose(groupwise_label_neg_weight.sum(), 1.0):
         groupwise_label_neg_weight /= groupwise_label_neg_weight.sum()
 
     # Compute global FPR (weighted by relative number of LNs in each group)
     global_fpr = groupwise_label_neg_weight @ groupwise_roc_points[:, 0]
```

### Comparing `error-parity-0.1.3/error_parity.egg-info/PKG-INFO` & `error-parity-0.1.4/error_parity.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.3
+Version: 0.1.4
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/AndreFCruz/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -95,7 +95,14 @@
   - i.e., equal group-specific TPR and FPR;
 
 Road-map:
 - [ ] equal opportunity;
   - i.e., equal group-specific TPR;
 - [ ] demographic parity;
   - i.e., equal group-specific predicted prevalence;
+
+
+## Citing
+
+This repository contains code and supplementary materials for the following preprint:
+
+> André F. Cruz and Moritz Hardt. "Unprocessing Seven Years of Algorithmic Fairness." [arXiv preprint, 2023](https://arxiv.org/pdf/2306.07261.pdf).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `error-parity-0.1.3/setup.py` & `error-parity-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.3/tests/conftest.py` & `error-parity-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.3/tests/test_equal_odds.py` & `error-parity-0.1.4/tests/test_equal_odds.py`

 * *Files identical despite different names*

