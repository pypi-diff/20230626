# Comparing `tmp/sem_desc-4.4.4.tar.gz` & `tmp/sem_desc-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sem_desc-4.4.4.tar", max compression
+gzip compressed data, was "sem_desc-4.5.0.tar", max compression
```

## Comparing `sem_desc-4.4.4.tar` & `sem_desc-4.5.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      167 2023-02-24 01:26:22.248119 sem_desc-4.4.4/README.md
--rw-r--r--   0        0        0     1007 2023-02-24 01:26:22.248119 sem_desc-4.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/__init__.py
--rw-r--r--   0        0        0     1854 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/data/namespaces.yml
--rw-r--r--   0        0        0     8347 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/dataset.py
--rw-r--r--   0        0        0        0 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/evaluation/__init__.py
--rw-r--r--   0        0        0     3077 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/evaluation/cpa_cta_metrics.py
--rw-r--r--   0        0        0     2979 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/evaluation/hierarchy_scoring_fn.py
--rw-r--r--   0        0        0      166 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/evaluation/prelude.py
--rw-r--r--   0        0        0    23593 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/evaluation/sm_metrics.py
--rw-r--r--   0        0        0     1844 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/evaluation/transformation.py
--rw-r--r--   0        0        0        0 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/inputs/__init__.py
--rw-r--r--   0        0        0     1056 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/inputs/column.py
--rw-r--r--   0        0        0     1789 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/inputs/context.py
--rw-r--r--   0        0        0     2589 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/inputs/link.py
--rw-r--r--   0        0        0      295 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/inputs/prelude.py
--rw-r--r--   0        0        0     3527 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/inputs/table.py
--rw-r--r--   0        0        0        0 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/misc/__init__.py
--rw-r--r--   0        0        0     1339 2023-02-24 01:26:22.248119 sem_desc-4.4.4/sm/misc/bijection.py
--rw-r--r--   0        0        0     8221 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/misc/deser.py
--rw-r--r--   0        0        0     6950 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/misc/exp_manager.py
--rw-r--r--   0        0        0     3764 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/misc/fn_cache.py
--rw-r--r--   0        0        0    12133 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/misc/funcs.py
--rw-r--r--   0        0        0     1832 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/misc/logger.py
--rw-r--r--   0        0        0     2670 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/misc/matrix.py
--rw-r--r--   0        0        0      179 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/misc/prelude.py
--rw-r--r--   0        0        0     4472 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/misc/ray_helper.py
--rw-r--r--   0        0        0     3773 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/misc/timer.py
--rw-r--r--   0        0        0        0 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/namespaces/__init__.py
--rw-r--r--   0        0        0     3456 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/namespaces/namespace.py
--rw-r--r--   0        0        0     2972 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/namespaces/prefix_index.py
--rw-r--r--   0        0        0      179 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/namespaces/prelude.py
--rw-r--r--   0        0        0     5795 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/namespaces/wikidata.py
--rw-r--r--   0        0        0        0 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/outputs/__init__.py
--rw-r--r--   0        0        0    29296 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/outputs/semantic_model.py
--rw-r--r--   0        0        0      134 2023-02-24 01:26:22.252119 sem_desc-4.4.4/sm/prelude.py
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 sem_desc-4.4.4/setup.py
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 sem_desc-4.4.4/PKG-INFO
+-rw-r--r--   0        0        0      167 2023-02-24 08:07:22.957311 sem_desc-4.5.0/README.md
+-rw-r--r--   0        0        0     1007 2023-02-24 08:07:22.957311 sem_desc-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-24 08:07:22.957311 sem_desc-4.5.0/sm/__init__.py
+-rw-r--r--   0        0        0     1854 2023-02-24 08:07:22.957311 sem_desc-4.5.0/sm/data/namespaces.yml
+-rw-r--r--   0        0        0     8347 2023-02-24 08:07:22.957311 sem_desc-4.5.0/sm/dataset.py
+-rw-r--r--   0        0        0        0 2023-02-24 08:07:22.957311 sem_desc-4.5.0/sm/evaluation/__init__.py
+-rw-r--r--   0        0        0     3094 2023-02-24 08:07:22.957311 sem_desc-4.5.0/sm/evaluation/cpa_cta_metrics.py
+-rw-r--r--   0        0        0     4069 2023-02-24 08:07:22.957311 sem_desc-4.5.0/sm/evaluation/hierarchy_scoring_fn.py
+-rw-r--r--   0        0        0      510 2023-02-24 08:07:22.957311 sem_desc-4.5.0/sm/evaluation/prelude.py
+-rw-r--r--   0        0        0    23670 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/evaluation/sm_metrics.py
+-rw-r--r--   0        0        0     1844 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/evaluation/transformation.py
+-rw-r--r--   0        0        0     1039 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/evaluation/utils.py
+-rw-r--r--   0        0        0        0 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/inputs/__init__.py
+-rw-r--r--   0        0        0     1056 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/inputs/column.py
+-rw-r--r--   0        0        0     1789 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/inputs/context.py
+-rw-r--r--   0        0        0     2589 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/inputs/link.py
+-rw-r--r--   0        0        0      295 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/inputs/prelude.py
+-rw-r--r--   0        0        0     3527 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/inputs/table.py
+-rw-r--r--   0        0        0        0 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/__init__.py
+-rw-r--r--   0        0        0     1339 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/bijection.py
+-rw-r--r--   0        0        0     8221 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/deser.py
+-rw-r--r--   0        0        0     6950 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/exp_manager.py
+-rw-r--r--   0        0        0     3764 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/fn_cache.py
+-rw-r--r--   0        0        0    12133 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/funcs.py
+-rw-r--r--   0        0        0     1832 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/logger.py
+-rw-r--r--   0        0        0     2670 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/matrix.py
+-rw-r--r--   0        0        0      179 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/prelude.py
+-rw-r--r--   0        0        0     4472 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/ray_helper.py
+-rw-r--r--   0        0        0     3773 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/misc/timer.py
+-rw-r--r--   0        0        0        0 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/namespaces/__init__.py
+-rw-r--r--   0        0        0     3456 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/namespaces/namespace.py
+-rw-r--r--   0        0        0     2972 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/namespaces/prefix_index.py
+-rw-r--r--   0        0        0      179 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/namespaces/prelude.py
+-rw-r--r--   0        0        0     5795 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/namespaces/wikidata.py
+-rw-r--r--   0        0        0        0 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/outputs/__init__.py
+-rw-r--r--   0        0        0    29296 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/outputs/semantic_model.py
+-rw-r--r--   0        0        0      134 2023-02-24 08:07:22.961311 sem_desc-4.5.0/sm/prelude.py
+-rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 sem_desc-4.5.0/setup.py
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 sem_desc-4.5.0/PKG-INFO
```

### Comparing `sem_desc-4.4.4/pyproject.toml` & `sem_desc-4.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sem-desc"
-version = "4.4.4"
+version = "4.5.0"
 description = "Package providing basic functionalities for the semantic modeling problem"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 packages = [
     { include = "sm" }
 ]
```

### Comparing `sem_desc-4.4.4/sm/data/namespaces.yml` & `sem_desc-4.5.0/sm/data/namespaces.yml`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/dataset.py` & `sem_desc-4.5.0/sm/dataset.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/evaluation/cpa_cta_metrics.py` & `sem_desc-4.5.0/sm/evaluation/cpa_cta_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 from dataclasses import dataclass
 from typing import Set, Optional, Dict
 
 from sm.evaluation import sm_metrics
+from sm.evaluation.utils import PrecisionRecallF1
 
 from sm.outputs.semantic_model import SemanticModel, DataNode
 from sm.evaluation.transformation import SemModelTransformation
 from sm.outputs.semantic_model import ClassNode
 
 
 @dataclass
-class CTAEvalOutput:
-    precision: float
-    recall: float
-    f1: float
-
+class CTAEvalOutput(PrecisionRecallF1):
     n_corrects: float  # float as we allow for partial correctness
     n_examples: int
     n_predictions: int
 
 
 def cpa(
     gold_sm: SemanticModel,
     pred_sm: SemanticModel,
     id_props: Set[str],
     scoring_fn: Optional[sm_metrics.ScoringFn] = None,
-) -> sm_metrics.PrecisionRecallF1Output:
+) -> sm_metrics.SmPrecisionRecallF1Output:
     gold_sm = gold_sm.deep_copy()
     pred_sm = pred_sm.deep_copy()
 
     _cpa_transformation(gold_sm, id_props)
     _cpa_transformation(pred_sm, id_props)
 
     return sm_metrics.precision_recall_f1(
```

### Comparing `sem_desc-4.4.4/sm/evaluation/hierarchy_scoring_fn.py` & `sem_desc-4.5.0/sm/evaluation/hierarchy_scoring_fn.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,68 @@
 import math
-from typing import Dict, Callable, List, Mapping, Set, Iterable, Tuple
+from typing import Dict, Callable, List, Mapping, Protocol, Set, Iterable, Tuple
 from dataclasses import dataclass
 from sm.evaluation.sm_metrics import ScoringFn
 from tqdm import tqdm
 
 
 ItemParents = Dict[str, Iterable[str]]
+
 MAX_ANCESTOR_DISTANCE = 5
 MAX_DESCENDANT_DISTANCE = 3
+INF_DISTANCE = 100
+
+
+class ItemDistanceProtocol(Protocol):
+    def get_distance(self, pred_item: str, target_item: str) -> int:
+        """Get the distance between the predicted and target items. The distance is positive
+        if the predicted item is an ancestor of the target item, and negative if the predicted
+        item is a descendant of the target item.
+        If the predicted item is not related to the target item, the distance can be choosed to be any number larger than MAX_ANCESTOR_DISTANCE or less than MAX_DESCENDANT_DISTANCE."""
+        ...
+
+
+@dataclass
+class DictItemDistance:
+    __slots__ = ["item2parents"]
+
+    # mapping from the item to its parents and their distances
+    # 1 is direct parent, 2 is grandparent, etc.
+    item2parents: Mapping[str, Mapping[str, int]]
+
+    def get_distance(self, pred_item: str, target_item: str) -> int:
+        if pred_item == target_item:
+            return 0
+        if pred_item in self.item2parents[target_item]:
+            return self.item2parents[target_item][pred_item]
+        if target_item in self.item2parents[pred_item]:
+            return -self.item2parents[pred_item][target_item]
+        return INF_DISTANCE
 
 
 class HierarchyScoringFn(ScoringFn):
     def __init__(
         self,
-        item2parents: Mapping[str, Mapping[str, int]],
+        item_distance: ItemDistanceProtocol,
     ):
-        """ """
-        # mapping from the item to its parents and their distances
-        # 1 is direct parent, 2 is grandparent, etc.
-        self.item2parents: Mapping[str, Mapping[str, int]] = item2parents
+        self.item_distance = item_distance
 
     def get_match_score(self, pred_item: str, target_item: str):
         if pred_item == target_item:
             return 1.0
-        if pred_item in self.item2parents[target_item]:
-            # pred_predicate is the parent of the target
-            distance = self.item2parents[target_item][pred_item]
+        distance = self.item_distance.get_distance(pred_item, target_item)
+        assert distance != 0.0
+        if distance > 0:
+            # pred_predicate is the ancestor of the target
             if distance > MAX_ANCESTOR_DISTANCE:
                 return 0.0
             return math.pow(0.8, distance)
-        if target_item in self.item2parents[pred_item]:
-            distance = self.item2parents[pred_item][target_item]
+        if distance < 0:
+            # pred_predicate is the descendant of the target
+            distance = -distance
             if distance > MAX_DESCENDANT_DISTANCE:
                 return 0.0
             return math.pow(0.7, distance)
         return 0.0
 
     @staticmethod
     def construct(
@@ -70,12 +98,14 @@
                     distance, item2parents[item].get(node, float("inf"))
                 )
 
                 for parent in get_item_parents(node):
                     stack.append((parent, distance + 1))
 
         return HierarchyScoringFn(
-            {
-                get_item_uri(k): {get_item_uri(k2): v2 for k2, v2 in v.items()}
-                for k, v in item2parents.items()
-            }
+            DictItemDistance(
+                {
+                    get_item_uri(k): {get_item_uri(k2): v2 for k2, v2 in v.items()}
+                    for k, v in item2parents.items()
+                }
+            )
         )
```

### Comparing `sem_desc-4.4.4/sm/evaluation/sm_metrics.py` & `sem_desc-4.5.0/sm/evaluation/sm_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 import math
 import os
 from dataclasses import dataclass
 from itertools import permutations, chain
-from typing import Dict, Tuple, List, Set, Optional, Callable, Generator, TYPE_CHECKING
+from typing import (
+    Dict,
+    Sequence,
+    Tuple,
+    List,
+    Set,
+    Optional,
+    Callable,
+    Generator,
+    TYPE_CHECKING,
+)
 
 from loguru import logger
 from pyrsistent import pvector, PVector
+from sm.evaluation.utils import PrecisionRecallF1
 
 from sm.outputs.semantic_model import (
     SemanticModel,
     ClassNode,
     DataNode,
     LiteralNode,
 )
@@ -172,15 +183,15 @@
         # a map from x' => x (pred_sm to gold_sm)
         self.prime2x: Dict[int, Optional[int]] = {}
         # map from x => x'
         self.x2prime: Dict[int, Optional[int]] = {}
 
     @staticmethod
     def construct_from_mapping(
-        mapping: List[Tuple[Optional[int], Optional[int]]]
+        mapping: Sequence[Tuple[Optional[int], Optional[int]]]
     ) -> "PartialBijection":
         """
         :param mapping: a list of map from x' => x
         """
         self = PartialBijection()
         self.prime2x = {x_prime: x for x_prime, x in mapping if x_prime is not None}
         self.x2prime = {x: x_prime for x_prime, x in mapping if x is not None}
@@ -233,18 +244,15 @@
 class ScoringFn:
     # noinspection PyMethodMayBeStatic
     def get_match_score(self, pred_predicate: str, target_predicate: str) -> float:
         return int(pred_predicate == target_predicate)
 
 
 @dataclass
-class PrecisionRecallF1Output:
-    precision: float
-    recall: float
-    f1: float
+class SmPrecisionRecallF1Output(PrecisionRecallF1):
     bijection: PartialBijection
     n_corrects: float  # float as we allow for partial correctness
     n_examples: int
     n_predictions: int
     gold_triples: Set[NodeTriple]
     pred_triples: Set[NodeTriple]
 
@@ -587,15 +595,15 @@
 
 
 def precision_recall_f1(
     gold_sm: "SemanticModel",
     pred_sm: "SemanticModel",
     scoring_fn: Optional[ScoringFn] = None,
     debug_dir: Optional[str] = None,
-) -> PrecisionRecallF1Output:
+) -> SmPrecisionRecallF1Output:
     if scoring_fn is None:
         scoring_fn = ScoringFn()
     pair_groups: List[PairLabelGroup] = prepare_args(gold_sm, pred_sm)
 
     mapping = []
     map_groups: List[PairLabelGroup] = []
     for pair in pair_groups:
@@ -663,15 +671,15 @@
         precision = TP / len(all_groups.X_prime_triples)
 
     if precision == 0 and recall == 0:
         f1 = 0.0
     else:
         f1 = 2 * precision * recall / (precision + recall)
 
-    return PrecisionRecallF1Output(
+    return SmPrecisionRecallF1Output(
         f1=f1,
         precision=precision,
         recall=recall,
         bijection=bijection,
         n_corrects=TP,
         n_examples=len(all_groups.X_triples),
         n_predictions=len(all_groups.X_prime_triples),
```

### Comparing `sem_desc-4.4.4/sm/evaluation/transformation.py` & `sem_desc-4.5.0/sm/evaluation/transformation.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/inputs/column.py` & `sem_desc-4.5.0/sm/inputs/column.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/inputs/context.py` & `sem_desc-4.5.0/sm/inputs/context.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/inputs/link.py` & `sem_desc-4.5.0/sm/inputs/link.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/inputs/table.py` & `sem_desc-4.5.0/sm/inputs/table.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/misc/bijection.py` & `sem_desc-4.5.0/sm/misc/bijection.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/misc/deser.py` & `sem_desc-4.5.0/sm/misc/deser.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/misc/exp_manager.py` & `sem_desc-4.5.0/sm/misc/exp_manager.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/misc/fn_cache.py` & `sem_desc-4.5.0/sm/misc/fn_cache.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/misc/funcs.py` & `sem_desc-4.5.0/sm/misc/funcs.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/misc/logger.py` & `sem_desc-4.5.0/sm/misc/logger.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/misc/matrix.py` & `sem_desc-4.5.0/sm/misc/matrix.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/misc/ray_helper.py` & `sem_desc-4.5.0/sm/misc/ray_helper.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/misc/timer.py` & `sem_desc-4.5.0/sm/misc/timer.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/namespaces/namespace.py` & `sem_desc-4.5.0/sm/namespaces/namespace.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/namespaces/prefix_index.py` & `sem_desc-4.5.0/sm/namespaces/prefix_index.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/namespaces/wikidata.py` & `sem_desc-4.5.0/sm/namespaces/wikidata.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/sm/outputs/semantic_model.py` & `sem_desc-4.5.0/sm/outputs/semantic_model.py`

 * *Files identical despite different names*

### Comparing `sem_desc-4.4.4/setup.py` & `sem_desc-4.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'serde2[all]>=1.6.0,<2.0.0',
  'timer4>=1.0.4,<2.0.0',
  'tqdm>=4.64.0,<5.0.0',
  'ujson>=5.5.0,<6.0.0']
 
 setup_kwargs = {
     'name': 'sem-desc',
-    'version': '4.4.4',
+    'version': '4.5.0',
     'description': 'Package providing basic functionalities for the semantic modeling problem',
     'long_description': '# SEM-DESC ![PyPI](https://img.shields.io/pypi/v/sem-desc)\n\nContaining basic functions (input, output, dataset, evaluation metrics) for the semantic modeling problem.\n',
     'author': 'Binh Vu',
     'author_email': 'binh@toan2.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/binh-vu/sm',
```

### Comparing `sem_desc-4.4.4/PKG-INFO` & `sem_desc-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sem-desc
-Version: 4.4.4
+Version: 4.5.0
 Summary: Package providing basic functionalities for the semantic modeling problem
 Home-page: https://github.com/binh-vu/sm
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

