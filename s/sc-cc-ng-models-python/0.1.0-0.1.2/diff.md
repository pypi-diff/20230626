# Comparing `tmp/sc_cc_ng_models_python-0.1.0.tar.gz` & `tmp/sc_cc_ng_models_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_cc_ng_models_python-0.1.0.tar", max compression
+gzip compressed data, was "sc_cc_ng_models_python-0.1.2.tar", max compression
```

## Comparing `sc_cc_ng_models_python-0.1.0.tar` & `sc_cc_ng_models_python-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      576 2023-06-26 14:02:21.217632 sc_cc_ng_models_python-0.1.0/README.md
--rw-r--r--   0        0        0      351 2023-06-26 13:57:07.567333 sc_cc_ng_models_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8120 2023-06-26 14:00:27.035572 sc_cc_ng_models_python-0.1.0/sc_cc_ng_models_python/__init__.py
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 sc_cc_ng_models_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      576 2023-06-26 14:02:21.217632 sc_cc_ng_models_python-0.1.2/README.md
+-rw-r--r--   0        0        0      425 2023-06-26 15:24:31.142183 sc_cc_ng_models_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10285 2023-06-26 15:26:33.437183 sc_cc_ng_models_python-0.1.2/sc_cc_ng_models_python/__init__.py
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 sc_cc_ng_models_python-0.1.2/PKG-INFO
```

### Comparing `sc_cc_ng_models_python-0.1.0/README.md` & `sc_cc_ng_models_python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sc_cc_ng_models_python-0.1.0/sc_cc_ng_models_python/__init__.py` & `sc_cc_ng_models_python-0.1.2/sc_cc_ng_models_python/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from hashlib import sha256
 from typing import List, Union, Optional
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from itertools import chain, starmap
 from enum import Enum
 
-import numpy as np
-
 class ContextType(Enum):
 	ACCELERATION = "ACCELERATION"
 	ACCELERATION_ELECTRIC = "ACCELERATION_ELECTRIC"
 	ACCESSORIES = "ACCESSORIES"
 	BATTERY_NOMINAL_ENERGY = "BATTERY_NOMINAL_ENERGY"
 	BATTERY_USABLE_ENERGY = "BATTERY_USABLE_ENERGY"
 	BRAKING_DISTANCE = "BRAKING_DISTANCE"
@@ -179,7 +177,92 @@
 
     @staticmethod
     def from_dict(d: dict) -> "BitVal":
         return BitVal(
             context=d["context"],
             value=d["value"],
         )
+
+    def to_dict(self) -> dict:
+        return {
+            "context": self.context,
+            "value": self.value,
+        }
+
+class ContextRelation(Enum):
+    ALL = "ALL"
+    ANY = "ANY"
+
+@dataclass
+class SubContextFilter:
+
+    contexts: List[ContextType]
+    relation: ContextRelation
+    _not: bool = field(default=False)
+
+    def validate(self, values: List[str]) -> bool:
+        if self.relation == ContextRelation.ALL:
+            res = all(
+                map(
+                    lambda context: context.value in values,
+                    self.contexts,
+                )
+            )
+        else:
+            res = any(
+                map(
+                    lambda context: context.value in values,
+                    self.contexts,
+                )
+            )
+
+        return bool((self._not * 1) - (res * 1))
+
+    def to_dict(self) -> dict:
+        return {
+            "contexts": [context.value for context in self.contexts],
+            "relation": self.relation.value,
+            "Not": self._not,
+        }
+
+@dataclass
+class ContextFilter:
+
+    relation: ContextRelation
+    subContextFilters: List[SubContextFilter]
+    _not: bool = field(default=False)
+
+    @staticmethod
+    def empty() -> "ContextFilter":
+        return ContextFilter(
+            _not=False,
+            relation=ContextRelation.ALL,
+            subContextFilters=[],
+        )
+
+    def validate(self, values: List[str]) -> bool:
+        if not self.subContextFilters:
+            return True
+
+        if self.relation == ContextRelation.ALL:
+            res = all(
+                map(
+                    lambda sub: sub.validate(values),
+                    self.subContextFilters,
+                )
+            )
+        else:
+            res = any(
+                map(
+                    lambda sub: sub.validate(values),
+                    self.subContextFilters,
+                )
+            )
+
+        return bool((self._not * 1) - (res * 1))
+
+    def to_dict(self) -> dict:
+        return {
+            "relation": self.relation.value,
+            "subContextFilters": [sub.to_dict() for sub in self.subContextFilters],
+            "Not": self._not,
+        }
```

