# Comparing `tmp/iambic-2.4.3.tar.gz` & `tmp/iambic-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic-2.4.3.tar", last modified: Tue Mar  9 04:03:28 2021, max compression
+gzip compressed data, was "iambic-3.0.0.tar", max compression
```

## Comparing `iambic-2.4.3.tar` & `iambic-3.0.0.tar`

### file list

```diff
@@ -1,62 +1,60 @@
--rw-r--r--   0        0        0     1080 2021-03-09 04:03:14.945774 iambic-2.4.3/LICENSE
--rw-r--r--   0        0        0     2755 2021-03-09 04:03:14.945774 iambic-2.4.3/README.md
--rw-r--r--   0        0        0     2755 2021-03-09 04:03:14.945774 iambic-2.4.3/README.md
--rw-r--r--   0        0        0      150 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/__init__.py
--rw-r--r--   0        0        0      337 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/ast/__init__.py
--rw-r--r--   0        0        0     2216 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/ast/base.py
--rw-r--r--   0        0        0    10639 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/ast/index.py
--rw-r--r--   0        0        0    18178 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/ast/node.py
--rw-r--r--   0        0        0       46 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/bin/__init__.py
--rw-r--r--   0        0        0       46 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/bin/cli.py
--rw-r--r--   0        0        0      127 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/parse/__init__.py
--rw-r--r--   0        0        0      216 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/parse/data.py
--rw-r--r--   0        0        0    10663 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/parse/text.py
--rw-r--r--   0        0        0     2167 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/plays/__init__.py
--rwxr-xr-x   0        0        0    99742 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/plays/comedies/a-midsummer-night-s-dream.md
--rwxr-xr-x   0        0        0   130985 2021-03-09 04:03:14.949775 iambic-2.4.3/iambic/plays/comedies/as-you-like-it.md
--rwxr-xr-x   0        0        0   136556 2021-03-09 04:03:14.953775 iambic-2.4.3/iambic/plays/comedies/love-s-labours-lost.md
--rwxr-xr-x   0        0        0   129463 2021-03-09 04:03:14.953775 iambic-2.4.3/iambic/plays/comedies/much-ado-about-nothing.md
--rwxr-xr-x   0        0        0    93245 2021-03-09 04:03:14.953775 iambic-2.4.3/iambic/plays/comedies/the-comedy-of-errors.md
--rwxr-xr-x   0        0        0   137390 2021-03-09 04:03:14.953775 iambic-2.4.3/iambic/plays/comedies/the-merry-wives-of-windsor.md
--rwxr-xr-x   0        0        0   122434 2021-03-09 04:03:14.953775 iambic-2.4.3/iambic/plays/comedies/twelfth-night.md
--rwxr-xr-x   0        0        0   106800 2021-03-09 04:03:14.953775 iambic-2.4.3/iambic/plays/comedies/two-gentlemen-of-verona.md
--rw-r--r--   0        0        0   123177 2021-03-09 04:03:14.957775 iambic-2.4.3/iambic/plays/histories/edward-iii.md
--rwxr-xr-x   0        0        0   149920 2021-03-09 04:03:14.957775 iambic-2.4.3/iambic/plays/histories/henry-iv-part-1.md
--rwxr-xr-x   0        0        0   162507 2021-03-09 04:03:14.957775 iambic-2.4.3/iambic/plays/histories/henry-iv-part-2.md
--rwxr-xr-x   0        0        0   159624 2021-03-09 04:03:14.961775 iambic-2.4.3/iambic/plays/histories/henry-v.md
--rwxr-xr-x   0        0        0   137028 2021-03-09 04:03:14.961775 iambic-2.4.3/iambic/plays/histories/henry-vi-part-1.md
--rwxr-xr-x   0        0        0   157170 2021-03-09 04:03:14.961775 iambic-2.4.3/iambic/plays/histories/henry-vi-part-2.md
--rwxr-xr-x   0        0        0   152470 2021-03-09 04:03:14.961775 iambic-2.4.3/iambic/plays/histories/henry-vi-part-3.md
--rwxr-xr-x   0        0        0   152202 2021-03-09 04:03:14.965775 iambic-2.4.3/iambic/plays/histories/henry-viii.md
--rwxr-xr-x   0        0        0   126037 2021-03-09 04:03:14.965775 iambic-2.4.3/iambic/plays/histories/king-john.md
--rwxr-xr-x   0        0        0   138408 2021-03-09 04:03:14.965775 iambic-2.4.3/iambic/plays/histories/richard-ii.md
--rwxr-xr-x   0        0        0   185826 2021-03-09 04:03:14.965775 iambic-2.4.3/iambic/plays/histories/richard-iii.md
--rwxr-xr-x   0        0        0   140867 2021-03-09 04:03:14.969775 iambic-2.4.3/iambic/plays/problems/all-s-well-that-ends-well.md
--rwxr-xr-x   0        0        0   135863 2021-03-09 04:03:14.969775 iambic-2.4.3/iambic/plays/problems/measure-for-measure.md
--rwxr-xr-x   0        0        0   126434 2021-03-09 04:03:14.969775 iambic-2.4.3/iambic/plays/problems/the-merchant-of-venice.md
--rwxr-xr-x   0        0        0   129487 2021-03-09 04:03:14.969775 iambic-2.4.3/iambic/plays/problems/the-taming-of-the-shrew.md
--rwxr-xr-x   0        0        0   165738 2021-03-09 04:03:14.969775 iambic-2.4.3/iambic/plays/problems/troilus-and-cressida.md
--rwxr-xr-x   0        0        0   163905 2021-03-09 04:03:14.973775 iambic-2.4.3/iambic/plays/roman/antony-and-cleopatra.md
--rwxr-xr-x   0        0        0   174446 2021-03-09 04:03:14.973775 iambic-2.4.3/iambic/plays/roman/coriolanus.md
--rwxr-xr-x   0        0        0   122085 2021-03-09 04:03:14.973775 iambic-2.4.3/iambic/plays/roman/julius-caesar.md
--rwxr-xr-x   0        0        0   127702 2021-03-09 04:03:14.973775 iambic-2.4.3/iambic/plays/roman/titus-andronicus.md
--rwxr-xr-x   0        0        0   150418 2021-03-09 04:03:14.977775 iambic-2.4.3/iambic/plays/romances/a-winter-s-tale.md
--rwxr-xr-x   0        0        0   170166 2021-03-09 04:03:14.977775 iambic-2.4.3/iambic/plays/romances/cymbeline.md
--rwxr-xr-x   0        0        0   114926 2021-03-09 04:03:14.977775 iambic-2.4.3/iambic/plays/romances/pericles.md
--rwxr-xr-x   0        0        0   103379 2021-03-09 04:03:14.977775 iambic-2.4.3/iambic/plays/romances/the-tempest.md
--rwxr-xr-x   0        0        0   189481 2021-03-09 04:03:14.981775 iambic-2.4.3/iambic/plays/tragedies/hamlet.md
--rwxr-xr-x   0        0        0   163976 2021-03-09 04:03:14.981775 iambic-2.4.3/iambic/plays/tragedies/king-lear.md
--rwxr-xr-x   0        0        0   108666 2021-03-09 04:03:14.981775 iambic-2.4.3/iambic/plays/tragedies/macbeth.md
--rwxr-xr-x   0        0        0   163726 2021-03-09 04:03:14.981775 iambic-2.4.3/iambic/plays/tragedies/othello.md
--rwxr-xr-x   0        0        0   149287 2021-03-09 04:03:14.985775 iambic-2.4.3/iambic/plays/tragedies/romeo-and-juliet.md
--rwxr-xr-x   0        0        0   117322 2021-03-09 04:03:14.985775 iambic-2.4.3/iambic/plays/tragedies/timon-of-athens.md
--rw-r--r--   0        0        0      388 2021-03-09 04:03:14.985775 iambic-2.4.3/iambic/render/__init__.py
--rw-r--r--   0        0        0     1108 2021-03-09 04:03:14.985775 iambic-2.4.3/iambic/render/html.py
--rw-r--r--   0        0        0      566 2021-03-09 04:03:14.985775 iambic-2.4.3/iambic/render/json.py
--rw-r--r--   0        0        0     7539 2021-03-09 04:03:14.985775 iambic-2.4.3/iambic/render/markdown.py
--rw-r--r--   0        0        0     6545 2021-03-09 04:03:14.985775 iambic-2.4.3/iambic/render/table.py
--rw-r--r--   0        0        0     2762 2021-03-09 04:03:14.985775 iambic-2.4.3/iambic/roman.py
--rw-r--r--   0        0        0     1686 2021-03-09 04:03:14.985775 iambic-2.4.3/pyproject.toml
--rw-r--r--   0        0        0    16736 2021-03-09 04:03:14.985775 iambic-2.4.3/schema.json
--rw-r--r--   0        0        0     3904 2021-03-09 04:03:29.717570 iambic-2.4.3/setup.py
--rw-r--r--   0        0        0     4331 2021-03-09 04:03:29.718100 iambic-2.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-25 23:05:20.486997 iambic-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2755 2023-06-25 23:05:20.486997 iambic-3.0.0/README.md
+-rw-r--r--   0        0        0      151 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/__init__.py
+-rw-r--r--   0        0        0      337 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/ast/__init__.py
+-rw-r--r--   0        0        0     2265 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/ast/base.py
+-rw-r--r--   0        0        0    10665 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/ast/index.py
+-rw-r--r--   0        0        0    19090 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/ast/node.py
+-rw-r--r--   0        0        0       46 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/bin/__init__.py
+-rw-r--r--   0        0        0       46 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/bin/cli.py
+-rw-r--r--   0        0        0      127 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/parse/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/parse/data.py
+-rw-r--r--   0        0        0    10662 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/parse/text.py
+-rw-r--r--   0        0        0     2154 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/plays/__init__.py
+-rwxr-xr-x   0        0        0    99742 2023-06-25 23:05:20.490998 iambic-3.0.0/iambic/plays/comedies/a-midsummer-night-s-dream.md
+-rwxr-xr-x   0        0        0   130985 2023-06-25 23:05:20.494998 iambic-3.0.0/iambic/plays/comedies/as-you-like-it.md
+-rwxr-xr-x   0        0        0   136556 2023-06-25 23:05:20.494998 iambic-3.0.0/iambic/plays/comedies/love-s-labours-lost.md
+-rwxr-xr-x   0        0        0   129463 2023-06-25 23:05:20.494998 iambic-3.0.0/iambic/plays/comedies/much-ado-about-nothing.md
+-rwxr-xr-x   0        0        0    93245 2023-06-25 23:05:20.494998 iambic-3.0.0/iambic/plays/comedies/the-comedy-of-errors.md
+-rwxr-xr-x   0        0        0   137390 2023-06-25 23:05:20.498998 iambic-3.0.0/iambic/plays/comedies/the-merry-wives-of-windsor.md
+-rwxr-xr-x   0        0        0   122434 2023-06-25 23:05:20.498998 iambic-3.0.0/iambic/plays/comedies/twelfth-night.md
+-rwxr-xr-x   0        0        0   106800 2023-06-25 23:05:20.498998 iambic-3.0.0/iambic/plays/comedies/two-gentlemen-of-verona.md
+-rw-r--r--   0        0        0   123177 2023-06-25 23:05:20.498998 iambic-3.0.0/iambic/plays/histories/edward-iii.md
+-rwxr-xr-x   0        0        0   149920 2023-06-25 23:05:20.502998 iambic-3.0.0/iambic/plays/histories/henry-iv-part-1.md
+-rwxr-xr-x   0        0        0   162507 2023-06-25 23:05:20.502998 iambic-3.0.0/iambic/plays/histories/henry-iv-part-2.md
+-rwxr-xr-x   0        0        0   159624 2023-06-25 23:05:20.502998 iambic-3.0.0/iambic/plays/histories/henry-v.md
+-rwxr-xr-x   0        0        0   137028 2023-06-25 23:05:20.502998 iambic-3.0.0/iambic/plays/histories/henry-vi-part-1.md
+-rwxr-xr-x   0        0        0   157170 2023-06-25 23:05:20.506998 iambic-3.0.0/iambic/plays/histories/henry-vi-part-2.md
+-rwxr-xr-x   0        0        0   152470 2023-06-25 23:05:20.506998 iambic-3.0.0/iambic/plays/histories/henry-vi-part-3.md
+-rwxr-xr-x   0        0        0   152202 2023-06-25 23:05:20.506998 iambic-3.0.0/iambic/plays/histories/henry-viii.md
+-rwxr-xr-x   0        0        0   126037 2023-06-25 23:05:20.506998 iambic-3.0.0/iambic/plays/histories/king-john.md
+-rwxr-xr-x   0        0        0   138408 2023-06-25 23:05:20.510998 iambic-3.0.0/iambic/plays/histories/richard-ii.md
+-rwxr-xr-x   0        0        0   185826 2023-06-25 23:05:20.510998 iambic-3.0.0/iambic/plays/histories/richard-iii.md
+-rwxr-xr-x   0        0        0   140867 2023-06-25 23:05:20.510998 iambic-3.0.0/iambic/plays/problems/all-s-well-that-ends-well.md
+-rwxr-xr-x   0        0        0   135863 2023-06-25 23:05:20.514998 iambic-3.0.0/iambic/plays/problems/measure-for-measure.md
+-rwxr-xr-x   0        0        0   126434 2023-06-25 23:05:20.514998 iambic-3.0.0/iambic/plays/problems/the-merchant-of-venice.md
+-rwxr-xr-x   0        0        0   129487 2023-06-25 23:05:20.514998 iambic-3.0.0/iambic/plays/problems/the-taming-of-the-shrew.md
+-rwxr-xr-x   0        0        0   165738 2023-06-25 23:05:20.514998 iambic-3.0.0/iambic/plays/problems/troilus-and-cressida.md
+-rwxr-xr-x   0        0        0   163905 2023-06-25 23:05:20.518998 iambic-3.0.0/iambic/plays/roman/antony-and-cleopatra.md
+-rwxr-xr-x   0        0        0   174446 2023-06-25 23:05:20.518998 iambic-3.0.0/iambic/plays/roman/coriolanus.md
+-rwxr-xr-x   0        0        0   122085 2023-06-25 23:05:20.518998 iambic-3.0.0/iambic/plays/roman/julius-caesar.md
+-rwxr-xr-x   0        0        0   127702 2023-06-25 23:05:20.522998 iambic-3.0.0/iambic/plays/roman/titus-andronicus.md
+-rwxr-xr-x   0        0        0   150418 2023-06-25 23:05:20.522998 iambic-3.0.0/iambic/plays/romances/a-winter-s-tale.md
+-rwxr-xr-x   0        0        0   170166 2023-06-25 23:05:20.522998 iambic-3.0.0/iambic/plays/romances/cymbeline.md
+-rwxr-xr-x   0        0        0   114926 2023-06-25 23:05:20.526998 iambic-3.0.0/iambic/plays/romances/pericles.md
+-rwxr-xr-x   0        0        0   103379 2023-06-25 23:05:20.526998 iambic-3.0.0/iambic/plays/romances/the-tempest.md
+-rwxr-xr-x   0        0        0   189481 2023-06-25 23:05:20.526998 iambic-3.0.0/iambic/plays/tragedies/hamlet.md
+-rwxr-xr-x   0        0        0   163976 2023-06-25 23:05:20.526998 iambic-3.0.0/iambic/plays/tragedies/king-lear.md
+-rwxr-xr-x   0        0        0   108666 2023-06-25 23:05:20.530998 iambic-3.0.0/iambic/plays/tragedies/macbeth.md
+-rwxr-xr-x   0        0        0   163726 2023-06-25 23:05:20.530998 iambic-3.0.0/iambic/plays/tragedies/othello.md
+-rwxr-xr-x   0        0        0   149287 2023-06-25 23:05:20.530998 iambic-3.0.0/iambic/plays/tragedies/romeo-and-juliet.md
+-rwxr-xr-x   0        0        0   117322 2023-06-25 23:05:20.534999 iambic-3.0.0/iambic/plays/tragedies/timon-of-athens.md
+-rw-r--r--   0        0        0      388 2023-06-25 23:05:20.534999 iambic-3.0.0/iambic/render/__init__.py
+-rw-r--r--   0        0        0     1108 2023-06-25 23:05:20.534999 iambic-3.0.0/iambic/render/html.py
+-rw-r--r--   0        0        0      566 2023-06-25 23:05:20.534999 iambic-3.0.0/iambic/render/json.py
+-rw-r--r--   0        0        0     7539 2023-06-25 23:05:20.534999 iambic-3.0.0/iambic/render/markdown.py
+-rw-r--r--   0        0        0     6719 2023-06-25 23:05:20.534999 iambic-3.0.0/iambic/render/table.py
+-rw-r--r--   0        0        0     2762 2023-06-25 23:05:20.534999 iambic-3.0.0/iambic/roman.py
+-rw-r--r--   0        0        0     1966 2023-06-25 23:05:20.534999 iambic-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    16736 2023-06-25 23:05:20.534999 iambic-3.0.0/schema.json
+-rw-r--r--   0        0        0     4365 1970-01-01 00:00:00.000000 iambic-3.0.0/PKG-INFO
```

### Comparing `iambic-2.4.3/LICENSE` & `iambic-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/README.md` & `iambic-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/ast/base.py` & `iambic-3.0.0/iambic/ast/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 import enum
 import re
 
-
 __all__ = (
     "NodeType",
     "NodeToken",
     "NODE_PATTERN",
     "JOIN_TOKENS",
 )
 
@@ -37,14 +36,17 @@
 
     JOIN1 = "…"
     JOIN2 = "..."
     JOIN = "/"
     META1 = "---"
     META2 = "..."
 
+    def __str__(self):
+        return self.value
+
 
 JOIN_TOKENS = (NodeToken.JOIN, NodeToken.JOIN1, NodeToken.JOIN2)
 
 
 NODE_PATTERN = re.compile(
     r"""
     (
```

### Comparing `iambic-2.4.3/iambic/ast/index.py` & `iambic-3.0.0/iambic/ast/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,33 @@
 # -*- coding: UTF-8 -*-
 import functools
 from collections import defaultdict
 from itertools import chain
 from typing import (
     DefaultDict,
     Dict,
-    Optional,
+    Iterable,
     List,
-    Set,
-    Union,
+    Mapping,
+    Optional,
+    Self,
     ValuesView,
     cast,
-    Mapping,
-    Iterable,
-    Tuple,
 )
 
 import iambic.ast.node as ast
 
 __all__ = ("Index",)
 
 
-IndexKeyT = Union[ast.NodeType, str]
-IndexInputT = Union[
-    Mapping[str, ast.GenericNode], Iterable[Tuple[str, ast.GenericNode]]
-]
+IndexKeyT = ast.NodeType | str
+IndexInputT = Mapping[str, ast.GenericNode] | Iterable[tuple[str, ast.GenericNode]]
 
 
-class Index(Dict[str, Union[ast.ResolvedNodeT, ast.GenericNode]]):
+class Index(Dict[str, ast.ResolvedNodeT | ast.GenericNode]):
     """An ordered collection of nodes in a script.
 
     ``Parser.parse`` builds a list of :class:`GenericNode`, which can be resolved into the specific
     data-type for the :class:`NodeType` assigned.
     """
 
     def __init__(self, iterable: IndexInputT = None, **kwargs: ast.GenericNode):
@@ -109,52 +105,50 @@
         return cast(ValuesView[ast.Exit], self.get_values(ast.NodeType.EXIT))
 
     @property
     def intermission(self) -> Optional[ast.Intermission]:
         inter = {*self.get_values(ast.NodeType.INTER)}
         return cast(Optional[ast.Intermission], inter.pop() if inter else None)
 
-    def resolve_presence(self):
-        members: Iterable[Union[ast.Entrance, ast.Exit]] = chain(
-            self.entrances, self.exits
-        )
+    def resolve_presence(self: Self):
+        members: Iterable[ast.Entrance | ast.Exit] = chain(self.entrances, self.exits)
         personae = {x.text: x for x in self.personae}
         for member in members:
             present = (*(p.id for t, p in personae.items() if t in member.text),)
             member.personae = present
 
     _NP = {ast.NodeType.DIR, ast.NodeType.ENTER, ast.NodeType.EXIT}
 
     def _resolve_events(
         self,
         speech: List[ast.SpeechNodeT],
-        associates: Set[Union[ast.Direction, ast.Entrance, ast.Exit]],
+        associates: set[ast.Direction | ast.Entrance | ast.Exit],
     ):
         start, end = speech[0].index, speech[-1].index
         events = {e for e in associates if start < e.index < end}
         associates -= events
         speech.extend(events)
 
     def get_speeches(self) -> List[ast.Speech]:
         # Candidates for members of speeches.
-        members: List[Union[ast.Dialogue, ast.Action]] = sorted(
+        members: List[ast.Dialogue | ast.Action] = sorted(
             chain(self.dialogue, self.actions),
             key=ast.indexgetter,
         )
-        associates: Set[Union[ast.Direction, ast.Entrance, ast.Exit]] = {
+        associates: set[ast.Direction | ast.Entrance | ast.Exit] = {
             *self.directions,
             *self.entrances,
             *self.exits,
         }
         persona: Optional[ast.Persona] = None
         scene: ast.Scene = self[members[0].scene]
         speech: List[ast.SpeechNodeT] = []
         speeches: List[ast.Speech] = []
 
-        for i, node in enumerate(members):
+        for node in members:
             # If we're in a new scene, we're definitely in a new speech.
             if node.scene != scene.id:
                 if persona and scene and speech:
                     self._resolve_events(speech, associates)
                     spch = ast.Speech(
                         persona.id, scene.id, ast.sort_body(speech), speech[0].index
                     )
@@ -194,53 +188,55 @@
                 persona.id, scene.id, ast.sort_body(speech), speech[0].index
             )
             speeches.append(spch)
 
         return speeches
 
     def claimed_events(
-        self, speeches: Set[ast.Speech]
-    ) -> Set[Union[ast.Direction, ast.Exit, ast.Entrance]]:
+        self, speeches: set[ast.Speech]
+    ) -> set[ast.Direction | ast.Exit | ast.Entrance]:
         return {
             y
             for x in speeches
             for y in x.body
             if isinstance(y, (ast.Direction, ast.Entrance, ast.Exit))
         }
 
     def finalize_scenes(self) -> Iterable[ast.ActNodeT]:
         speeches = {*self.get_speeches()}
         claimed = self.claimed_events(speeches)
-        directions = {*self.directions} - claimed
-        entrances = {*self.entrances} - claimed
-        exits = {*self.exits} - claimed
-        children = speeches | directions | entrances | exits
+        directions = {*self.directions, *self.entrances, *self.exits} - claimed
+        children: set[ast.Direction | ast.Entrance | ast.Exit | ast.Speech] = (
+            speeches | directions  # type: ignore[assignment]
+        )
         scenes = []
-        scene: Union[ast.Scene, ast.Epilogue, ast.Prologue]
-        for scene in chain(self.scenes, self.epilogues, self.prologues):  # type: ignore
-            child_nodes = {c for c in children if c.scene == scene.id}
-            s: ast.Speech
-            personae: Set[ast.NodeID] = {
-                s.persona  # type: ignore
-                for s in child_nodes
-                if s.type == ast.NodeType.SPCH
-            }
-            if child_nodes:
-                scene.body = ast.sort_body(child_nodes)
-                scene.personae = (*personae,)
-                scenes.append(scene)
-                children -= child_nodes
+        scene: ast.Scene | ast.Epilogue | ast.Prologue
+        scene_groups = cast(
+            Iterable[Iterable[ast.Scene | ast.Epilogue | ast.Prologue]],
+            (self.scenes, self.epilogues, self.prologues),
+        )
+        for scene_group in scene_groups:
+            for scene in scene_group:
+                child_nodes = {c for c in children if c.scene == scene.id}
+                personae: set[ast.NodeID] = {
+                    s.persona for s in child_nodes if isinstance(s, ast.Speech)
+                }
+                if child_nodes:
+                    scene.body = ast.sort_body(child_nodes)
+                    scene.personae = (*personae,)
+                    scenes.append(scene)
+                    children -= child_nodes
 
         return scenes
 
     def finalize_acts(
         self, scenes: Iterable[ast.ActNodeT]
-    ) -> List[Union[ast.Act, ast.Epilogue, ast.Prologue]]:
+    ) -> List[ast.Act | ast.Epilogue | ast.Prologue]:
         scenes = {*scenes}
-        logues: Set[Union[ast.Prologue, ast.Epilogue]] = {
+        logues: set[ast.Prologue | ast.Epilogue] = {
             s
             for s in scenes
             if isinstance(s, (ast.Epilogue, ast.Prologue)) and not s.act
         }
         scenes -= logues
         intermission = self.intermission
         # Add the act-level logues which have a Scene-like structure
@@ -249,16 +245,16 @@
         # Get the act-level logues which have an Act-like structure
         _logues = (
             log
             for log in chain(self.prologues, self.epilogues)
             if not log.body and not log.act
         )
         for act in chain(_logues, self.acts):  # type: ignore
-            children: Set[
-                Union[ast.Scene, ast.Intermission, ast.Prologue, ast.Epilogue]
+            children: set[
+                ast.Scene | ast.Intermission | ast.Prologue | ast.Epilogue
             ] = {s for s in scenes if s.act == act.id}
             if children:
                 scenes -= children
                 # Add the intermission if there is one.
                 if intermission and intermission.act == act.id:
                     children.add(intermission)
                 act.body = ast.sort_body(children)
@@ -278,9 +274,9 @@
         play = ast.Play(
             ast.sort_body(acts), (*self.personae,), meta=(meta or ast.Metadata())
         )
         return play
 
     @staticmethod
     @functools.lru_cache(maxsize=2000)
-    def node_sort(node: Union[ast.ResolvedNodeT, ast.GenericNode]):
+    def node_sort(node: ast.ResolvedNodeT | ast.GenericNode):
         return node.index
```

### Comparing `iambic-2.4.3/iambic/ast/node.py` & `iambic-3.0.0/iambic/ast/node.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-#!/usr/bin/env python
-# -*- coding: UTF-8 -*-
 from __future__ import annotations
 
 import dataclasses
-import functools
 from operator import attrgetter
-from typing import (
-    ClassVar,
-    Optional,
-    Union,
-    Tuple,
-    Mapping,
-    Type,
-    List,
-    TypeVar,
-    NewType,
-    Iterable,
-    Set,
-)
+from typing import ClassVar, Iterable, Mapping, NewType, Self, Type, TypeVar
 
 import typic
 from inflection import parameterize, titleize
 
 from iambic import roman
-from .base import NodeType
 
+from .base import NodeType
 
 __all__ = (
     "Act",
     "ActBodyT",
     "ActNodeT",
     "Scene",
     "SceneBodyT",
@@ -61,78 +46,84 @@
 NodeID = NewType("NodeID", str)
 indexgetter = attrgetter("index")
 
 
 _T = TypeVar("_T")
 
 
-def sort_body(body: Iterable[_T]) -> Tuple[_T, ...]:
+def sort_body(body: Iterable[_T]) -> tuple[_T, ...]:
     return tuple(sorted(body, key=indexgetter))
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Act:
     """A representation of a single Act in a Play."""
 
     type: ClassVar[NodeType] = NodeType.ACT
     index: int
     text: str
     num: int
-    body: "ActBodyT" = typic.field(compare=False, hash=False, default=())  # type: ignore
+    body: ActBodyT = dataclasses.field(compare=False, hash=False, default=())
+    id: NodeID = dataclasses.field(init=False)
+    col: str = dataclasses.field(init=False)
+
+    def __post_init__(self):
+        self.col = self._getcol()
+        self.id = self._getid()
 
-    @typic.cached_property
-    def id(self) -> NodeID:
+    def _getid(self) -> NodeID:
         return NodeID(parameterize(f"{self.type.lower()}-{self.col}"))
 
-    @typic.cached_property
-    def col(self):
+    def _getcol(self):
         return roman.numeral(self.num)
 
     @classmethod
-    def from_node(cls, node: "GenericNode") -> "Act":
+    def from_node(cls, node: GenericNode) -> Self:
         numeral = node.pieces[1]
         num = int(numeral) if numeral.isdigit() else roman.integer(numeral)
         return cls(index=node.index, text=node.match_text, num=num)
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Scene:
     """A representation of a single Scene in a play."""
 
     type: ClassVar[NodeType] = NodeType.SCENE
     index: int
     text: str
     num: int
-    setting: Optional[str] = None
-    act: Optional[NodeID] = None
-    body: SceneBodyT = typic.field(compare=False, hash=False, default=())  # type: ignore
-    personae: PersonaeIDT = typic.field(compare=False, hash=False, default=())  # type: ignore
+    setting: str | None = None
+    act: NodeID | None = None
+    body: SceneBodyT = dataclasses.field(compare=False, hash=False, default=())
+    personae: PersonaeIDT = dataclasses.field(compare=False, hash=False, default=())
+    id: NodeID = dataclasses.field(init=False)
+    col: str = dataclasses.field(init=False)
+
+    def __post_init__(self):
+        self.col = self._getcol()
+        self.id = self._getid()
 
-    @typic.cached_property
-    def id(self) -> NodeID:
+    def _getid(self) -> NodeID:
         return NodeID(
             f"{self.act}-{self.type.lower()}-{roman.numeral(self.num).lower()}"
         )
 
-    @typic.cached_property
-    def col(self) -> str:
+    def _getcol(self) -> str:
         pre = self.act or ""
         if pre:
             pieces = pre.split("-")
             if len(pieces) == 2:
                 pre = pieces[1] if pre.startswith("act") else pieces[0][0]
                 pre = f"{pre.upper()}: "
             else:
                 pre = f"{pieces[0].title()}: "
         return f"{pre}{roman.numeral(self.num).lower()}"
 
     @classmethod
-    def from_node(cls, node: "GenericNode") -> "Scene":
+    def from_node(cls, node: GenericNode) -> Self:
         numeral = node.pieces[1]
         num = int(numeral) if numeral.isdigit() else roman.integer(numeral)
         setting = node.match.get("setting") or None
         parent = node.parent or node.act or node.scene
         if parent is None:
             raise ValueError(f"Can't build {cls.__name__!r} from node: {node}")
         return cls(
@@ -140,305 +131,295 @@
             text=node.match_text,
             num=num,
             act=parent,
             setting=setting,
         )
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Prologue:
     """A representation of a single Prologue in a play.
 
     Notes:
         Prologues (and Epilogues) may have the body structure of either an Act or Scene.
     """
 
     type: ClassVar[NodeType] = NodeType.PROL
     index: int
     text: str
-    setting: Optional[str] = None
-    act: Optional[NodeID] = None
-    body: "LogueBodyT" = typic.field(compare=False, hash=False, default=())  # type: ignore
-    personae: PersonaeIDT = typic.field(compare=False, hash=False, default=())  # type: ignore
-    as_act: bool = typic.field(init=False)  # type: ignore
+    setting: str | None = None
+    act: NodeID | None = None
+    body: LogueBodyT = dataclasses.field(compare=False, hash=False, default=())
+    personae: PersonaeIDT = dataclasses.field(compare=False, hash=False, default=())
+    as_act: bool = dataclasses.field(init=False)
+    id: NodeID = dataclasses.field(init=False)
+    col: str = dataclasses.field(init=False)
 
     def __post_init__(self):
         # If the body conforms to the `ActBodyT` type, it should be treated as such.
         self.as_act = bool(
             self.body
             and isinstance(self.body[0], (Scene, Intermission, Epilogue, Prologue))
         )
+        self.col = self._getcol()
+        self.id = self._getid()
 
-    @typic.cached_property
-    def id(self) -> NodeID:
+    def _getid(self) -> NodeID:
         pre = f"{self.act}-" if self.act else ""
         return NodeID(f"{pre}{self.type.lower()}-{self.index}")
 
-    @typic.cached_property
-    def col(self):
+    def _getcol(self):
         pre = self.act or ""
         if pre:
             pieces = self.act.split("-")
             if len(pieces) == 2:
                 pre = f"{pieces[1].upper()}: "
             else:
                 pre = f"{pieces[0].title()}: "
         return f"{pre}{self.type.title()}"
 
     @classmethod
-    def from_node(cls, node: "GenericNode") -> "Prologue":
+    def from_node(cls, node: GenericNode) -> Prologue:
         setting = node.match.get("setting") or None
         return cls(
             index=node.index, text=node.match_text, setting=setting, act=node.parent
         )
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Epilogue(Prologue):
     """A representation of a single Epilogue in a play.
 
     Notes:
         Epilogues (and Prologues) may have the body structure of either an Act or Scene.
     """
 
     type: ClassVar[NodeType] = NodeType.EPIL
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Intermission:
     """A representation of an Intermission in a play."""
 
     type: ClassVar[NodeType] = NodeType.INTER
     index: int
     text: str
     act: NodeID
+    id: NodeID = dataclasses.field(init=False)
+    col: str = dataclasses.field(init=False)
 
-    @typic.cached_property
-    def id(self) -> NodeID:
-        return NodeID("intermission")
+    def __post_init__(self):
+        self.col = titleize(self.text)
+        self.id = NodeID("intermission")
 
     @classmethod
-    def from_node(cls, node: "GenericNode") -> "Intermission":
+    def from_node(cls, node: GenericNode) -> Self:
         if not node.parent:
             raise ValueError(f"Can't build {cls.__name__!r} from node: {node}")
         return cls(index=node.index, text=node.match_text, act=node.parent)
 
-    @typic.cached_property
-    def col(self):
-        return titleize(self.text)
 
-
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Persona:
     """A representation of a single character in a Play."""
 
     type: ClassVar[NodeType] = NodeType.PERS
     index: int
     text: str
     name: str
-    short: Optional[str] = None
+    short: str | None = None
+    id: NodeID = dataclasses.field(init=False)
+    ids: set[NodeID] = dataclasses.field(init=False)
+
+    def __post_init__(self):
+        self.id = NodeID(parameterize(self.name))
+        self.ids = {NodeID(parameterize(n.strip())) for n in self.name.split("&")}
 
     def __eq__(self, other) -> bool:
         return other.name == self.name if hasattr(other, "name") else False
 
-    @typic.cached_property
-    def id(self) -> NodeID:
-        return NodeID(parameterize(self.name))
-
-    @typic.cached_property
-    def ids(self) -> Set[NodeID]:
-        return {NodeID(parameterize(n.strip())) for n in self.name.split("&")}
-
     @property
     def is_multi(self) -> bool:
         return "&" in self.name
 
     @classmethod
-    def from_node(cls, node: "GenericNode") -> "Persona":
+    def from_node(cls, node: GenericNode) -> Self:
         return cls(
             index=node.index,
             text=node.match_text,
             name=titleize(node.match_text),
         )
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Entrance:
     """A representation of an entrance for character(s) in a Scene."""
 
     type: ClassVar[NodeType] = NodeType.ENTER
     index: int
     text: str
     scene: NodeID
     personae: PersonaeIDT = ()
+    id: NodeID = dataclasses.field(init=False)
 
-    @typic.cached_property
-    def id(self) -> NodeID:
-        return NodeID(f"{self.scene}-{self.type.lower()}-{self.index}")
+    def __post_init__(self):
+        self.id = NodeID(f"{self.scene}-{self.type.lower()}-{self.index}")
 
     @classmethod
-    def from_node(cls, node: "GenericNode") -> "Entrance":
+    def from_node(cls, node: GenericNode) -> Self:
         if not node.parent:
             raise ValueError(f"Can't build {cls.__name__!r} from node: {node}")
         return cls(index=node.index, text=node.match_text, scene=node.parent)
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Exit(Entrance):
     """A representation of an exit for character(s) in a Scene."""
 
     type: ClassVar[NodeType] = NodeType.EXIT
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Action:
     """A representation of a stage direction related to a specific character."""
 
     type: ClassVar[NodeType] = NodeType.ACTION
     action: str
     persona: NodeID
     scene: NodeID
     index: int
+    id: NodeID = dataclasses.field(init=False)
 
-    @typic.cached_property
-    def id(self) -> NodeID:
-        return NodeID(f"{self.scene}-{self.persona}-{self.type.lower()}-{self.index}")
+    def __post_init__(self):
+        self.id = NodeID(
+            f"{self.scene}-{self.persona}-{self.type.lower()}-{self.index}"
+        )
 
     @classmethod
-    def from_node(cls, node: "GenericNode") -> "Action":
+    def from_node(cls, node: GenericNode) -> Self:
         if not node.parent or not node.scene:
             raise ValueError(f"Can't build {cls.__name__!r} from node: {node}")
         return cls(
             action=node.match_text,
             persona=node.parent,
             scene=node.scene,
             index=node.index,
         )
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Direction:
     """A representation of a stage direction."""
 
     type: ClassVar[NodeType] = NodeType.DIR
     action: str
     scene: NodeID
     index: int
     stop: bool = True
+    id: NodeID = dataclasses.field(init=False)
 
-    @typic.cached_property
-    def id(self) -> NodeID:
-        return NodeID(f"{self.scene}-{self.type.lower()}-{self.index}")
+    def __post_init__(self):
+        self.id = NodeID(f"{self.scene}-{self.type.lower()}-{self.index}")
 
     @classmethod
-    def from_node(cls, node: "GenericNode") -> "Direction":
+    def from_node(cls, node: GenericNode) -> Self:
         if not node.parent:
             raise ValueError(f"Can't build {cls.__name__!r} from node: {node}")
         return cls(action=node.match_text, scene=node.parent, index=node.index)
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Dialogue:
     """A representation of a line of dialogue for a character in a scene."""
 
     type: ClassVar[NodeType] = NodeType.DIAL
     line: str
     persona: NodeID
     scene: NodeID
     index: int
     lineno: int
     linepart: int = 0
+    id: NodeID = dataclasses.field(init=False)
 
-    @typic.cached_property
-    def id(self) -> NodeID:
-        return NodeID(
+    def __post_init__(self):
+        self.id = NodeID(
             f"{self.persona}-{self.type.lower()}-{self.lineno}-{self.linepart}"
         )
 
     @classmethod
-    def from_node(cls, node: "GenericNode") -> "Dialogue":
+    def from_node(cls, node: GenericNode) -> Self:
         if None in {node.parent, node.scene, node.lineno, node.linepart}:
             raise ValueError(f"Can't build {cls.__name__!r} from node: {node}")
         return cls(
             line=node.match_text,
-            persona=node.parent,  # type: ignore
-            scene=node.scene,  # type: ignore
-            index=node.index,  # type: ignore
-            lineno=node.lineno,  # type: ignore
-            linepart=node.linepart,  # type: ignore
+            persona=node.parent,
+            scene=node.scene,
+            index=node.index,
+            lineno=node.lineno,
+            linepart=node.linepart,
         )
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Speech:
     """A representation of an unbroken piece of dialogue related to a single character."""
 
     type: ClassVar[NodeType] = NodeType.SPCH
     persona: NodeID
     scene: NodeID
     body: SpeechBodyT
     index: int
+    linerange: tuple[int, int] = dataclasses.field(init=False)
+    linepart: int = dataclasses.field(init=False)
+    num_lines: int = dataclasses.field(init=False)
+    id: NodeID = dataclasses.field(init=False)
 
     def __post_init__(self):
         self.body = sort_body(self.body)
+        self.linerange = self._getlinerange()
+        self.linepart = self._getlinepart()
+        self.num_lines = self._getnum_lines()
+        self.id = self._getid()
 
-    @typic.cached_property
-    def linerange(self) -> Tuple[int, int]:
+    def _getlinerange(self) -> tuple[int, int]:
         linenos = sorted((x.lineno for x in self.body if isinstance(x, Dialogue)))
         return linenos[0], linenos[-1]
 
-    @typic.cached_property
-    def linepart(self) -> int:
+    def _getlinepart(self) -> int:
         return next((x.linepart for x in self.body if isinstance(x, Dialogue)), 0)
 
-    @typic.cached_property
-    def num_lines(self) -> int:
+    def _getnum_lines(self) -> int:
         x, y = self.linerange
-        # line count starts at 1
-        # a range of 1 - 1 is 1 line
         return y - (x - 1)
 
-    @typic.cached_property
-    def id(self) -> NodeID:
+    def _getid(self) -> NodeID:
         uri = (
             f"{self.scene}-{self.persona}-{self.type.lower()}-"
             f"{'-'.join(map(str, self.linerange))}"
         )
         if self.linepart:
             uri += f"-{roman.numeral(self.linepart).lower()}"
         return NodeID(uri)
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Metadata:
     """General information about a given play."""
 
     type: ClassVar[NodeType] = NodeType.META
     rights: str = "Creative Commons Non-Commercial Share Alike 3.0"
     language: str = "en-GB-emodeng"
     publisher: str = "Published w/ ❤️ using iambic - https://pypi.org/project/iambic"
-    title: Optional[str] = None
-    subtitle: Optional[str] = None
+    title: str | None = None
+    subtitle: str | None = None
     edition: int = 1
     author: str = "William Shakespeare"
-    editors: Tuple[str, ...] = ()
-    tags: Tuple[str, ...] = ()
+    editors: tuple[str, ...] = ()
+    tags: tuple[str, ...] = ()
 
-    @functools.lru_cache(1)
     def asmeta(self):  # pragma: nocover
         dikt = {
             "creator": [{"type": "author", "text": self.author}],
             "contributor": [{"type": "editor", "text": "MIT"}],
             "rights": self.rights,
             "language": self.language,
             "publisher": self.publisher,
@@ -455,45 +436,46 @@
             ({"type": "editor", "text": x} for x in self.editors or [])
         )
         dikt["subject"].extend(self.tags or [])
 
         return dikt
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class Play:
     """A representation of a play in its entirety."""
 
     type: ClassVar[NodeType] = NodeType.PLAY
     body: PlayBodyT = ()
-    personae: Tuple[Persona, ...] = ()
-    meta: Metadata = typic.field(default_factory=Metadata)  # type: ignore
+    personae: tuple[Persona, ...] = ()
+    meta: Metadata = dataclasses.field(default_factory=Metadata)
+    id: NodeID = dataclasses.field(init=False)
+    linecount: int | None = dataclasses.field(init=False)
 
     def __post_init__(self):
         self.body = sort_body(self.body)
+        self.id = self._getid()
+        self.linecount = self._getlinecount()
 
-    @typic.cached_property
-    def id(self) -> NodeID:
+    def _getid(self) -> NodeID:
         return NodeID(parameterize(f"{self.meta.title}-{self.type.lower()}"))
 
-    @typic.cached_property
-    def linecount(self) -> int:
+    def _getlinecount(self) -> int:
         count = 0
         final = self.body[-1]
         scene = final.body[-1] if isinstance(final, Act) else final
         if isinstance(scene, Intermission):
             raise ValueError(f"A Play may not end with an Intermission: {scene}")
         for entry in reversed(scene.body):
             if isinstance(entry, Speech):
                 count = entry.linerange[-1]
                 break
+
         return count
 
-    @functools.lru_cache(maxsize=1)
     def asjsonld(self):
         fn, ln = self.meta.author.split()
         data = {
             "@context": "https://schema.org",
             "@type": "Play",
             "name": self.meta.title,
             "author": {
@@ -526,25 +508,22 @@
             "keywords": [*self.meta.tags],
             "character": [{"@type": "Person", "name": c.name} for c in self.personae],
         }
 
         return data
 
 
-@typic.slotted
-@dataclasses.dataclass(unsafe_hash=True, order=True)
+@dataclasses.dataclass(slots=True, weakref_slot=True, unsafe_hash=True, order=True)
 class GenericNode:
     """The root-object of a script.
 
     A script ``Node`` represents a single line of text in a script.
     """
 
-    __resolver_map__: ClassVar[
-        Mapping[NodeType, Type[ResolvedNodeT]]
-    ] = typic.FrozenDict(
+    __resolver_map__: ClassVar[Mapping[NodeType, Type[_FromNodeT]]] = typic.FrozenDict(
         {
             NodeType.ACT: Act,
             NodeType.ACTION: Action,
             NodeType.DIAL: Dialogue,
             NodeType.DIR: Direction,
             NodeType.ENTER: Entrance,
             NodeType.EPIL: Epilogue,
@@ -559,68 +538,74 @@
         }
     )
     # Minimum data for a Node
     type: NodeType
     text: str
     index: int
     # Additional fields which may be present
-    lineno: Optional[int] = None
-    linepart: Optional[int] = None
+    lineno: int | None = None
+    linepart: int | None = None
     # Given by text parser
     # If reading from JSON, we don't have/need this,
     # it will be provided inherently by the data-structure
     # on resolution-time.
     match: typic.FrozenDict = dataclasses.field(default_factory=typic.FrozenDict)
-    parent: Optional[NodeID] = None
-    act: Optional[NodeID] = None
-    scene: Optional[NodeID] = None
+    parent: NodeID | None = None
+    act: NodeID | None = None
+    scene: NodeID | None = None
+    pieces: list[str] = dataclasses.field(init=False)
+    match_text: str = dataclasses.field(init=False)
+    _resolved: _FromNodeT | None = dataclasses.field(
+        init=False, default=None, compare=False
+    )
 
-    @typic.cached_property
-    def resolved(self) -> "ResolvedNodeT":
+    def __post_init__(self):
+        self.match_text = self.match[self.type] if self.match else self.text
+        self.pieces = self.match_text.split()
+
+    @property
+    def resolved(self: Self) -> ResolvedNodeT:
         """Resolve a GenericNode into a typed, "resolved" Node.
 
         Raises
         ------
         TypeError
             If the NodeType provided has no resolved Node mapping.
         """
+        if self._resolved is not None:
+            return self._resolved
+
         if self.type in self.__resolver_map__:
-            model: Type[ResolvedNodeT] = self.__resolver_map__[self.type]
-            return model.from_node(self)  # type: ignore
+            model: type[_FromNodeT] = self.__resolver_map__[self.type]
+            self._resolved = model.from_node(self)
+            return self._resolved
+
         raise ValueError(
             f"Unrecognized node-type <{self.type}> for text <{self.text}>. "
             f"Valid types are: {tuple(self.__resolver_map__)}"
         )
 
-    @typic.cached_property
-    def pieces(self) -> List[str]:
-        return self.match_text.split()
-
-    @typic.cached_property
-    def match_text(self) -> str:
-        return self.match[self.type] if self.match else self.text
-
-
-ResolvedNodeT = Union[
-    Act,
-    Scene,
-    Prologue,
-    Epilogue,
-    Persona,
-    Entrance,
-    Exit,
-    Action,
-    Direction,
-    Dialogue,
-    Speech,
-    Intermission,
-]
-SpeechNodeT = Union[Dialogue, Action, Direction, Entrance, Exit]
-SpeechBodyT = Tuple[SpeechNodeT, ...]
-ActNodeT = Union[Scene, Intermission, Epilogue, Prologue]
-ActBodyT = Tuple[ActNodeT, ...]
-SceneNodeT = Union[Direction, Entrance, Exit, Speech]
-SceneBodyT = Tuple[SceneNodeT, ...]
-LogueBodyT = Union[ActBodyT, SceneBodyT]
-PlayNodeT = Union[Act, Epilogue, Prologue]
-PlayBodyT = Tuple[PlayNodeT, ...]
-PersonaeIDT = Tuple[NodeID, ...]
+
+_FromNodeT = (
+    Act
+    | Scene
+    | Prologue
+    | Epilogue
+    | Persona
+    | Entrance
+    | Exit
+    | Action
+    | Direction
+    | Dialogue
+    | Intermission
+)
+ResolvedNodeT = _FromNodeT | Speech
+SpeechNodeT = Dialogue | Action | Direction | Entrance | Exit
+SpeechBodyT = tuple[SpeechNodeT, ...]
+ActNodeT = Scene | Intermission | Epilogue | Prologue
+ActBodyT = tuple[ActNodeT, ...]
+SceneNodeT = Direction | Entrance | Exit | Speech
+SceneBodyT = tuple[SceneNodeT, ...]
+LogueBodyT = ActBodyT | SceneBodyT
+PlayNodeT = Act | Epilogue | Prologue
+PlayBodyT = tuple[PlayNodeT, ...]
+PersonaeIDT = tuple[NodeID, ...]
```

### Comparing `iambic-2.4.3/iambic/parse/text.py` & `iambic-3.0.0/iambic/parse/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from collections import defaultdict
 
 import typic
 import yaml
 from html2text import html2text
 
 from iambic.ast import (
+    JOIN_TOKENS,
+    NODE_PATTERN,
     GenericNode,
+    Index,
+    InputType,
+    Metadata,
+    NodeToken,
     NodeType,
     Play,
-    InputType,
-    JOIN_TOKENS,
     ResolvedNodeT,
-    Index,
-    NodeToken,
-    NODE_PATTERN,
-    Metadata,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def _safe_resolve(
     node: typing.Optional[GenericNode], *, attr: str = None
@@ -251,15 +251,14 @@
         text = text.replace(f"# {title}", "") if title else text
         return title, text
 
     @classmethod
     def extract_metadata(
         cls, text: str
     ) -> typing.Tuple[typing.Optional[Metadata], str]:
-
         meta = None
         if text.startswith(NodeToken.META1):
             text = text[len(NodeToken.META1) + 1 :]
             token = None
             for t in {NodeToken.META1, NodeToken.META2}:
                 _token = f"\n{t}"
                 if _token in text:
```

### Comparing `iambic-2.4.3/iambic/plays/__init__.py` & `iambic-3.0.0/iambic/plays/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 import pathlib
-from typing import Set, Iterator, Optional, Union, Mapping
+from typing import Iterator, Mapping, Self
 
 import inflection
 import typic
 
-from iambic import parse, ast
+from iambic import ast, parse
 
 
 class Corpus:
-
     PATH: pathlib.Path = pathlib.Path(__file__).parent
     CACHE_SIZE: int = 1000
 
-    def __init__(self):
+    def __init__(self: Self):
         self._corpus: Mapping[str, pathlib.Path] = {x.name: x for x in self}
         self.__hits: int = 0
 
-    def _maybe_reset(self):
+    def _maybe_reset(self: Self):
         if self.__hits > self.CACHE_SIZE:
             self.__getitem__.cache_clear()
             self.__hits = 0
 
     @staticmethod
-    def _get_names(path: pathlib.Path) -> Set[str]:
+    def _get_names(path: pathlib.Path) -> set[str]:
         names = {path.name}
         for child in path.iterdir():
             if child.suffix == ".md":
                 names.add(inflection.parameterize(child.stem))
         return names
 
     def __iter__(self) -> Iterator[pathlib.Path]:
@@ -60,15 +59,15 @@
                 return v.read_text()
         raise KeyError(
             f"Couldn't locate a play with key {item!r}. Available keys are: {(*seen,)}"
         )
 
     def get(
         self, item: str, default: str = None, *, parsed: bool = False
-    ) -> Optional[Union[str, ast.Play, ast.Index]]:
+    ) -> str | ast.Play | ast.Index | None:
         try:
             text = self[item]
             return parse.text(text) if parsed else text
         except KeyError:
             return default
```

### Comparing `iambic-2.4.3/iambic/plays/comedies/a-midsummer-night-s-dream.md` & `iambic-3.0.0/iambic/plays/comedies/a-midsummer-night-s-dream.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/comedies/as-you-like-it.md` & `iambic-3.0.0/iambic/plays/comedies/as-you-like-it.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/comedies/love-s-labours-lost.md` & `iambic-3.0.0/iambic/plays/comedies/love-s-labours-lost.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/comedies/much-ado-about-nothing.md` & `iambic-3.0.0/iambic/plays/comedies/much-ado-about-nothing.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/comedies/the-comedy-of-errors.md` & `iambic-3.0.0/iambic/plays/comedies/the-comedy-of-errors.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/comedies/the-merry-wives-of-windsor.md` & `iambic-3.0.0/iambic/plays/comedies/the-merry-wives-of-windsor.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/comedies/twelfth-night.md` & `iambic-3.0.0/iambic/plays/comedies/twelfth-night.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/comedies/two-gentlemen-of-verona.md` & `iambic-3.0.0/iambic/plays/comedies/two-gentlemen-of-verona.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/edward-iii.md` & `iambic-3.0.0/iambic/plays/histories/edward-iii.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/henry-iv-part-1.md` & `iambic-3.0.0/iambic/plays/histories/henry-iv-part-1.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/henry-iv-part-2.md` & `iambic-3.0.0/iambic/plays/histories/henry-iv-part-2.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/henry-v.md` & `iambic-3.0.0/iambic/plays/histories/henry-v.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/henry-vi-part-1.md` & `iambic-3.0.0/iambic/plays/histories/henry-vi-part-1.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/henry-vi-part-2.md` & `iambic-3.0.0/iambic/plays/histories/henry-vi-part-2.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/henry-vi-part-3.md` & `iambic-3.0.0/iambic/plays/histories/henry-vi-part-3.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/henry-viii.md` & `iambic-3.0.0/iambic/plays/histories/henry-viii.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/king-john.md` & `iambic-3.0.0/iambic/plays/histories/king-john.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/richard-ii.md` & `iambic-3.0.0/iambic/plays/histories/richard-ii.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/histories/richard-iii.md` & `iambic-3.0.0/iambic/plays/histories/richard-iii.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/problems/all-s-well-that-ends-well.md` & `iambic-3.0.0/iambic/plays/problems/all-s-well-that-ends-well.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/problems/measure-for-measure.md` & `iambic-3.0.0/iambic/plays/problems/measure-for-measure.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/problems/the-merchant-of-venice.md` & `iambic-3.0.0/iambic/plays/problems/the-merchant-of-venice.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/problems/the-taming-of-the-shrew.md` & `iambic-3.0.0/iambic/plays/problems/the-taming-of-the-shrew.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/problems/troilus-and-cressida.md` & `iambic-3.0.0/iambic/plays/problems/troilus-and-cressida.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/roman/antony-and-cleopatra.md` & `iambic-3.0.0/iambic/plays/roman/antony-and-cleopatra.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/roman/coriolanus.md` & `iambic-3.0.0/iambic/plays/roman/coriolanus.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/roman/julius-caesar.md` & `iambic-3.0.0/iambic/plays/roman/julius-caesar.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/roman/titus-andronicus.md` & `iambic-3.0.0/iambic/plays/roman/titus-andronicus.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/romances/a-winter-s-tale.md` & `iambic-3.0.0/iambic/plays/romances/a-winter-s-tale.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/romances/cymbeline.md` & `iambic-3.0.0/iambic/plays/romances/cymbeline.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/romances/pericles.md` & `iambic-3.0.0/iambic/plays/romances/pericles.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/romances/the-tempest.md` & `iambic-3.0.0/iambic/plays/romances/the-tempest.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/tragedies/hamlet.md` & `iambic-3.0.0/iambic/plays/tragedies/hamlet.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/tragedies/king-lear.md` & `iambic-3.0.0/iambic/plays/tragedies/king-lear.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/tragedies/macbeth.md` & `iambic-3.0.0/iambic/plays/tragedies/macbeth.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/tragedies/othello.md` & `iambic-3.0.0/iambic/plays/tragedies/othello.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/tragedies/romeo-and-juliet.md` & `iambic-3.0.0/iambic/plays/tragedies/romeo-and-juliet.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/plays/tragedies/timon-of-athens.md` & `iambic-3.0.0/iambic/plays/tragedies/timon-of-athens.md`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/render/html.py` & `iambic-3.0.0/iambic/render/html.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 import functools
 
 from markdown import Markdown
 
 from iambic import ast
-from .markdown import render_markdown
 
+from .markdown import render_markdown
 
 EXTENSIONS = ("meta", "attr_list", "pymdownx.details", "tables", "pymdownx.tabbed")
 
 
 @functools.lru_cache(maxsize=1)
 def renderer(*extensions) -> Markdown:
     extensions = tuple(set(EXTENSIONS).union(set(extensions)))
```

### Comparing `iambic-2.4.3/iambic/render/json.py` & `iambic-3.0.0/iambic/render/json.py`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/iambic/render/markdown.py` & `iambic-3.0.0/iambic/render/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 import dataclasses
 import functools
 from textwrap import indent
-from typing import Iterable, Mapping, Union, cast, Dict, Tuple
+from typing import Dict, Iterable, Mapping, Tuple, Union, cast
 
 from inflection import titleize
 
 from iambic import ast
-from .table import RichMarker, tabulate, iter_tabs, export_grid, Column
+
+from .table import Column, RichMarker, export_grid, iter_tabs, tabulate
 
 TITLE = "# {0}"
 ACT = "## {0}"
 SCENE = "### {0}"
 DIR = "*{0}*"
 ACTION = r"*\[{0}]*"
 CHAR = "**{0}**"
@@ -192,15 +193,14 @@
         zip(tbl[Column.CHAR], tbl[Column.CLINE]), key=lambda cl: cl[-1], reverse=True
     ):
         yield f"        - {character} ({line_count} lines)"
     yield ""
 
 
 def iter_overview(play: ast.Play) -> Iterable[str]:
-
     yield ACT.format("Overview")
     yield ""
     yield from iter_stats(play)
     yield from iter_publication(play.meta)
     yield ACT.format("Index")
     yield ""
     yield from iter_character_index(play)
```

### Comparing `iambic-2.4.3/iambic/render/table.py` & `iambic-3.0.0/iambic/render/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 import enum
 import textwrap
-from typing import List, Dict, Tuple, Union, Type, Any, Iterable, cast
+from typing import Any, Dict, Iterable, List, Tuple, Type, Union, cast
 
 import tabulate as _tabulate
 
 from iambic import ast
 
-
 Row = List[str]
 Table = Dict[str, Row]
 Matrix = List[Tuple[str, ...]]
 
 
 class Column(str, enum.Enum):
     """Predefined column names"""
@@ -21,30 +20,39 @@
     APPR = "First Appearance"
     CLINE = "Lines"
     PLINE = "Player Lines"
     PLAYR = "Player"
     SORT = "Sort"
     GSWAP = " [SW]"
 
+    def __str__(self) -> str:
+        return self.value
+
 
 class Marker(str, enum.Enum):
     """The character to use when marking a persona as present in a scene."""
 
     SPEAK = "X"
     PRES = "O"
     NONE = ""
 
+    def __str__(self) -> str:
+        return self.value
+
 
 class RichMarker(str, enum.Enum):
     """The rich text character to use when marking a persona as present in a scene."""
 
     SPEAK = "💬"
     PRES = "👁️‍🗨️"
     NONE = ""
 
+    def __str__(self) -> str:
+        return self.value
+
 
 class Tabulator:
     """Generate a tabular representation of :py:class:`~iambic.ast.Play`
 
     Also known as a 'character map', this utility will generate a table
     which shows the number of lines for a given character and where they
     appear in the play.
@@ -113,24 +121,23 @@
             Column.CHAR.value: [x.name for x in _personae],
             Column.APPR.value: [x.index for x in _personae],
             Column.CLINE.value: [0 for _ in _personae],
         }
         char_column: List[str] = table[Column.CHAR.value]
         cline_column: List[int] = table[Column.CLINE.value]
         char_index: Dict[str, int] = {y: x for x, y in enumerate(char_column)}
-        personae = {x.id: x for x in play.personae}
+        personae = {str(x.id): x for x in play.personae}
         for act in play.body:
             # Epilogues and Prologues can be shaped like Scenes or Acts.
             # And can be top-level, like Acts.
             children: ast.ActBodyT = cast(
                 ast.ActBodyT,
                 (act.body if (isinstance(act, ast.Act) or act.as_act) else (act,)),
             )
             for scene in children:
-
                 table[scene.col] = [marker_type.NONE.value for _ in char_column]
                 if isinstance(scene, ast.Intermission):
                     continue
                 self._tabulate_scene(
                     scene=scene,
                     node_column=table[scene.col],
                     cline_column=cline_column,
```

### Comparing `iambic-2.4.3/iambic/roman.py` & `iambic-3.0.0/iambic/roman.py`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/pyproject.toml` & `iambic-3.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iambic"
-version = "2.4.3"
+version = "3.0.0"
 description = "Data extraction and rendering library for Shakespearean text."
 authors = ["Sean Stewart <sean_stewart@me.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/seandstewart/iambic"
 keywords = ["text", "render", "shakespeare", "text-processing"]
 classifiers = [
@@ -26,30 +26,45 @@
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
     "Typing :: Typed",
 ]
 include = ["*.md", "*.json"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-typical = "^2.1"
-ujson = "^2.0"
-markdown = "^3.2.2"
-pymdown-extensions = "^7.1"
+python = "^3.11"
+typical = "^2"
+ujson = "^5"
+markdown = "^3"
+pymdown-extensions = "^10"
 html2text = "^2020.1.16"
 tabulate = "^0.8.9"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.3"
-pytest-cov = "^2.8"
-pre-commit = "^1.20"
-flake8 = "^3.7.9"
-mkdocs-awesome-pages-plugin = "^2.2.0"
-mkdocs = "^1.1"
-mypy = "^0.761"
-mkdocs-material = "^7.0"
+[tool.poetry.group.docs.dependencies]
+mkdocs-awesome-pages-plugin = "^2"
+mkdocs = "^1"
+mkdocs-material = "^9"
 fontawesome-markdown = "^0.2.6"
-black = { version = "^20.8b1", allow-prereleases = true}
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7"
+pytest-cov = "^4"
+pre-commit = "^3"
+flake8 = "^6"
+flake8-bugbear = "^23"
+mypy = "^1"
+black = "^23"
+isort = "^5"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.5.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.mypy]
+mypy_path = "$MYPY_CONFIG_FILE_DIR/"
+no_namespace_packages = true
+python_version = "3.11"
+install_types = true
+non_interactive = true
+ignore_missing_imports = true
+no_strict_optional = true
+follow_imports = "silent"
+exclude = ".*tests/.*|.*docs/.*"
```

### Comparing `iambic-2.4.3/schema.json` & `iambic-3.0.0/schema.json`

 * *Files identical despite different names*

### Comparing `iambic-2.4.3/PKG-INFO` & `iambic-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: iambic
-Version: 2.4.3
+Version: 3.0.0
 Summary: Data extraction and rendering library for Shakespearean text.
 Home-page: https://github.com/seandstewart/iambic
 License: MIT
 Keywords: text,render,shakespeare,text-processing
 Author: Sean Stewart
 Author-email: sean_stewart@me.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
-Requires-Dist: markdown (>=3.2.2,<4.0.0)
-Requires-Dist: pymdown-extensions (>=7.1,<8.0)
+Requires-Dist: markdown (>=3,<4)
+Requires-Dist: pymdown-extensions (>=10,<11)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
-Requires-Dist: typical (>=2.1,<3.0)
-Requires-Dist: ujson (>=2.0,<3.0)
+Requires-Dist: typical (>=2,<3)
+Requires-Dist: ujson (>=5,<6)
 Project-URL: Repository, https://github.com/seandstewart/iambic
 Description-Content-Type: text/markdown
 
 iambic: Data extraction and rendering library for Shakespearean text. :scroll: 
 ==============================================================================
 [![image](https://img.shields.io/pypi/v/iambic.svg)](https://pypi.org/project/iambic/)
 [![image](https://img.shields.io/pypi/l/iambic.svg)](https://pypi.org/project/iambic/)
```

