# Comparing `tmp/reasoner-pydantic-4.0.8.tar.gz` & `tmp/reasoner-pydantic-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.0.8.tar", last modified: Sun Jun  4 23:50:13 2023, max compression
+gzip compressed data, was "reasoner-pydantic-4.0.9.tar", last modified: Mon Jun 26 20:28:03 2023, max compression
```

## Comparing `reasoner-pydantic-4.0.8.tar` & `reasoner-pydantic-4.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-04 23:50:13.000000 reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 23:50:13.374250 reasoner-pydantic-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-04 23:50:02.000000 reasoner-pydantic-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:28:03.586345 reasoner-pydantic-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-26 20:28:03.586345 reasoner-pydantic-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:28:03.582345 reasoner-pydantic-4.0.9/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:28:03.582345 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:28:03.586345 reasoner-pydantic-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/setup.py
```

### Comparing `reasoner-pydantic-4.0.8/PKG-INFO` & `reasoner-pydantic-4.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.8
+Version: 4.0.9
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
-Author: Kenneth Morton
-Author-email: kenny@covar.com
+Author: Abrar Mesbah
+Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Reasoner-Pydantic
 
 [![Test status via GitHub Actions](https://github.com/TranslatorSRI/reasoner-pydantic/workflows/test/badge.svg)](https://github.com/TranslatorSRI/reasoner-pydantic/actions?query=workflow%3Atest) [ℹ️](tests/README.md)
```

### Comparing `reasoner-pydantic-4.0.8/README.md` & `reasoner-pydantic-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """Reasoner-pydantic module."""
 
-from .kgraph import KnowledgeGraph, Node, Edge
+from .kgraph import (
+    KnowledgeGraph,
+    Node,
+    Edge,
+    RetrievalSource,
+)
 from .qgraph import (
     QueryGraph,
     QNode,
     QEdge,
     AttributeConstraint,
 )
 from .results import Result, NodeBinding, EdgeBinding, Results, Analysis
@@ -32,24 +37,28 @@
 )
 from .metakg import (
     MetaEdge,
     MetaNode,
     MetaKnowledgeGraph,
     MetaAttribute,
 )
+from .utils import (
+    HashableSequence,
+)
 
 components = [
     Attribute,
     BiolinkEntity,
     BiolinkPredicate,
     BiolinkQualifier,
     CURIE,
     Edge,
     EdgeBinding,
     KnowledgeGraph,
+    RetrievalSource,
     LogEntry,
     Message,
     Node,
     NodeBinding,
     QEdge,
     QNode,
     Query,
@@ -67,8 +76,9 @@
     MetaAttribute,
     Results,
     AuxiliaryGraph,
     AuxiliaryGraphs,
     Operation,
     Workflow,
     Analysis,
+    HashableSequence,
 ]
```

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/auxgraphs.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 
     def items(self):
         return self.__root__.items()
 
     def keys(self):
         return self.__root__.keys()
 
+    def __getitem__(self, k):
+        return self.__root__[k]
+
+    def __iter__(self):
+        return iter(self.__root__)
+
     def parse_obj(obj):
         auxiliary_graphs = parse_obj_as(AuxiliaryGraphs, obj)
         graphs = AuxiliaryGraphs()
         graphs.__root__ = HashableMapping[str, AuxiliaryGraph]()
         for id, graph in obj.items():
             graphs.__root__[id] = AuxiliaryGraph.parse_obj(graph)
         graphs.update(auxiliary_graphs)
```

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/message.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,52 +37,53 @@
         None, title="dict of auxiliary graphs", nullable=True
     )
 
     class Config:
         title = "message"
         extra = "forbid"
 
-    def parse_obj(obj):
+    def parse_obj(obj, normalize=True):
         message = parse_obj_as(Message, obj)
         qgraph = None
         kgraph = None
         results = None
         auxgraphs = None
         if "query_graph" in obj.keys() and obj["query_graph"] is not None:
             qgraph = QueryGraph.parse_obj(obj["query_graph"])
         if "knowledge_graph" in obj.keys() and obj["knowledge_graph"] is not None:
             kgraph = KnowledgeGraph.parse_obj(obj["knowledge_graph"])
         if "results" in obj.keys() and obj["results"] is not None:
             results = Results.parse_obj(obj["results"])
         if "auxiliary_graphs" in obj.keys() and obj["auxiliary_graphs"] is not None:
             auxgraphs = AuxiliaryGraphs.parse_obj(obj["auxiliary_graphs"])
-        m = Message(
-            query_graph=qgraph,
-            knowledge_graph=kgraph,
-            results=results,
-            auxiliary_graphs=auxgraphs,
+        m = parse_obj_as(Message, {})
+        m.query_graph, m.knowledge_graph, m.results, m.auxiliary_graphs = (
+            qgraph,
+            kgraph,
+            results,
+            auxgraphs,
         )
-        if m.knowledge_graph:
+        if m.knowledge_graph and normalize:
             m._normalize_kg_edge_ids()
-        m.update(message)
         return m
 
-    def update(self, other: "Message"):
+    def update(self, other: "Message", normalize=True):
         if hash(self.query_graph) != hash(other.query_graph):
             raise NotImplementedError("Query graph merging not supported yet")
         # Make a copy because normalization will modify results
         other = other.copy(deep=True)
 
         if other.knowledge_graph:
             if not self.knowledge_graph:
                 self.knowledge_graph = KnowledgeGraph(nodes=[], edges=[])
             # Normalize edges of incoming KG
             # This will place KG edge keys into the same hashing system
             # So that equivalence is determined by hash collision
-            other._normalize_kg_edge_ids()
+            if normalize:
+                other._normalize_kg_edge_ids()
             # The knowledge graph can now be udated because edge keys will be
             # hashed using the same method. The knowledge graph update method
             # will handle concatenating properties when necessary.
             self.knowledge_graph.update(other.knowledge_graph)
         if other.results:
             if self.results:
                 self.results.update(other.results)
@@ -197,14 +198,19 @@
 
     workflow: Optional[Workflow]
 
     class Config:
         title = "response"
         extra = "allow"
 
+    def parse_obj(obj, normalize=True):
+        response = parse_obj_as(Response, obj)
+        response.message = Message.parse_obj(obj["message"], normalize)
+        return response
+
 
 class AsyncQueryResponse(BaseModel):
     """ "Async Query Response."""
 
     status: Optional[str] = Field(None, nullable=True)
 
     description: Optional[str] = Field(None, nullable=True)
```

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/results.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Results models."""
+import copy
 from typing import Optional
 
 from pydantic import Field, parse_obj_as
 
 from .base_model import BaseModel
 from .utils import HashableMapping, HashableSet, HashableSequence
 from .shared import Attribute, CURIE
@@ -66,17 +67,17 @@
                 self.scoring_method,
             )
         )
 
     def update(self, other):
         for k in other.edge_bindings:
             if k in self.edge_bindings:
-                self.edge_bindings[k].update(other.edge_bindings[k])
+                self.edge_bindings[k].update(copy.deepcopy(other.edge_bindings[k]))
             else:
-                self.edge_bindings[k] = other.edge_bindings[k]
+                self.edge_bindings[k] = copy.deepcopy(other.edge_bindings[k])
         if other.attributes:
             if self.attributes:
                 self.attributes.update(other.attributes)
             else:
                 self.attributes = other.attributes
         if other.support_graphs:
             if self.support_graphs:
@@ -170,39 +171,57 @@
 
         self.analyses = combined_analyses
 
 
 class Results(BaseModel):
     """Results."""
 
-    __root__: Optional[HashableSet[Result]]
+    __root__: Optional[HashableSequence[Result]]
 
     class Config:
         title = "results"
         extra = "allow"
 
+    def append(self, result):
+        self.__root__.append(result)
+
     def add(self, result):
         results = self.__root__
-        if result in results:
+        try:
             # this is slow for larger results
-            for original_result in results:
-                if result == original_result:
-                    original_result.update(result)
-                    return
-        else:
-            results.add(result)
+            results[results.index(result)].update(result)
+        except ValueError:
+            results.append(result)
 
     def __len__(self):
         return len(self.__root__)
 
     def __iter__(self):
         return self.__root__.__iter__()
 
+    def __contains__(self, v):
+        return self.__root__.__contains__(v)
+
+    def __getitem__(self, i):
+        return self.__root__.__getitem__(i)
+
     def update(self, other):
-        for result in other.__root__:
-            self.add(result)
+        results = parse_obj_as(HashableMapping, {})
+        for result in other:
+            result = Result.parse_obj(result)
+            result_hash = hash(result)
+            if result_hash in results:
+                results[result_hash].update(result)
+            else:
+                results[hash(result)] = result
 
     def parse_obj(obj):
-        results = parse_obj_as(Results, obj)
+        parse_obj_as(Results, obj)
+        results = parse_obj_as(HashableMapping, {})
         for result in obj:
-            results.add(Result.parse_obj(result))
-        return results
+            result = Result.parse_obj(result)
+            result_hash = hash(result)
+            if result_hash in results:
+                results[result_hash].update(result)
+            else:
+                results[hash(result)] = result
+        return parse_obj_as(Results, list(results.values()))
```

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 ):
     """
     Custom class that implements MutableSequence and is hashable
     """
 
     __root__: List[ValueType] = list()
 
+    def __contains__(self, v):
+        return v in self.__root__
+
     def __getitem__(self, i):
         return self.__root__[i]
 
     def __iter__(self):
         return iter(self.__root__)
 
     def __len__(self):
```

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.0.9/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.8
+Version: 4.0.9
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
-Author: Kenneth Morton
-Author-email: kenny@covar.com
+Author: Abrar Mesbah
+Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Reasoner-Pydantic
 
 [![Test status via GitHub Actions](https://github.com/TranslatorSRI/reasoner-pydantic/workflows/test/badge.svg)](https://github.com/TranslatorSRI/reasoner-pydantic/actions?query=workflow%3Atest) [ℹ️](tests/README.md)
```

### Comparing `reasoner-pydantic-4.0.8/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.8/setup.py` & `reasoner-pydantic-4.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.0.8",
-    author="Kenneth Morton",
-    author_email="kenny@covar.com",
+    version="4.0.9",
+    author="Abrar Mesbah",
+    author_email="amesbah@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
     include_package_data=True,
     install_requires=["pydantic>=1.8"],
```

