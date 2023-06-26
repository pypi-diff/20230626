# Comparing `tmp/dbt-graph-builder-0.0.1.tar.gz` & `tmp/dbt-graph-builder-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-graph-builder-0.0.1.tar", last modified: Thu Jun 22 10:26:22 2023, max compression
+gzip compressed data, was "dbt-graph-builder-0.1.0.tar", last modified: Mon Jun 26 12:58:27 2023, max compression
```

## Comparing `dbt-graph-builder-0.0.1.tar` & `dbt-graph-builder-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:26:22.678059 dbt-graph-builder-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-22 10:26:22.678059 dbt-graph-builder-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 10:26:22.678059 dbt-graph-builder-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:26:22.674059 dbt-graph-builder-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:26:22.678059 dbt-graph-builder-0.0.1/src/dbt_graph_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:26:22.678059 dbt-graph-builder-0.0.1/src/dbt_graph_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-22 10:26:22.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-22 10:26:22.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:26:22.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 10:26:22.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 10:26:22.000000 dbt-graph-builder-0.0.1/src/dbt_graph_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:26:22.678059 dbt-graph-builder-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-22 10:25:58.000000 dbt-graph-builder-0.0.1/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.864764 dbt-graph-builder-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/src/dbt_graph_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_graph_dag_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_graph_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_graph_ephemeral_operator.py
```

### Comparing `dbt-graph-builder-0.0.1/LICENSE` & `dbt-graph-builder-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.0.1/PKG-INFO` & `dbt-graph-builder-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.0.1
+Version: 0.1.0
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dbt-graph-builder-0.0.1/README.md` & `dbt-graph-builder-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.0.1/pyproject.toml` & `dbt-graph-builder-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dbt-graph-builder"
-version = "0.0.1"
+version = "0.1.0"
 description = "DBT Graph Builder"
 authors = [
     {name = "Piotr Tutak", email = "piotr.tutak@getindata.com"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -78,9 +78,10 @@
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pre-commit",
     "pytest",
     "pytest-cov",
+    "pytest-xdist",
     "pytest-github-actions-annotate-failures",
 ]
```

### Comparing `dbt-graph-builder-0.0.1/src/dbt_graph_builder/gateway.py` & `dbt-graph-builder-0.1.0/src/dbt_graph_builder/gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,44 +116,44 @@
     if is_model_run_task(dep) and manifest["nodes"][dep]["schema"] == separation_layer_left:
         upstream_dependencies_connected_to_downstream.append(dep)
 
 
 def add_gateway_to_dependencies(
     gateway_name: str, filtered_dependencies: list[str], filtered_records: list[str]
 ) -> None:
-    """_summary_.
+    """Add gateway to dependencies.
 
     Args:
-        gateway_name (str): _description_
-        filtered_dependencies (list[str]): _description_
-        filtered_records (list[str]): _description_
+        gateway_name (str): Gateway name.
+        filtered_dependencies (list[str]): Filtered dependencies.
+        filtered_records (list[str]): Filtered records.
     """
     if len(filtered_dependencies) < len(filtered_records):
         filtered_dependencies.append(gateway_name)
 
 
 def create_gateway_name(separation_layer: SeparationLayer, gateway_task_name: str) -> str:
-    """_summary_.
+    """Create gateway name.
 
     Args:
-        separation_layer (SeparationLayer): _description_
-        gateway_task_name (str): _description_
+        separation_layer (SeparationLayer): Separation layer.
+        gateway_task_name (str): Gateway task name.
 
     Returns:
-        str: _description_
+        str: Created gateway name.
     """
     return f"{separation_layer.left}_{separation_layer.right}_{gateway_task_name}"
 
 
 def should_gateway_be_added(node_schema: str, separation_schemas: list[str]) -> bool:
     """Check if the gateway should be added.
 
     Args:
         node_schema (str): Node schema.
-        separation_schemas (list[str]): _description_
+        separation_schemas (list[str]): Separation schemas.
 
     Returns:
-        bool: _description_
+        bool: True if the gateway should be added, False otherwise.
     """
     valid_schemas_input_length = len(separation_schemas) >= 2
     schema_is_in_given_schemas = node_schema in separation_schemas
     return valid_schemas_input_length and schema_is_in_given_schemas
```

### Comparing `dbt-graph-builder-0.0.1/src/dbt_graph_builder/graph.py` & `dbt-graph-builder-0.1.0/src/dbt_graph_builder/graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import itertools
 import logging
 from typing import Any
 
 import networkx as nx
+from networkx.classes.reportviews import NodeDataView, OutEdgeDataView
 
 from dbt_graph_builder.gateway import (
     NodeProperties,
     SeparationLayer,
     TaskGraphConfiguration,
     add_gateway_to_dependencies,
     create_gateway_name,
@@ -19,27 +20,25 @@
     is_ephemeral_task,
     is_model_run_task,
     is_source_sensor_task,
     is_test_task,
 )
 
 
-class DbtAirflowGraph:
-    """_summary_."""
-
-    graph: nx.DiGraph
+class DbtManifestGraph:
+    """DbtManifestGraph class is used to create a DAG from DBT manifest.json file."""
 
     def __init__(self, configuration: TaskGraphConfiguration) -> None:
-        """Create DbtAirflowGraph.
+        """Create DbtManifestGraph.
 
         Args:
             configuration (TaskGraphConfiguration): _description_
         """
-        self.graph = nx.DiGraph()
-        self.configuration = configuration
+        self._graph = nx.DiGraph()
+        self._configuration = configuration
 
     def add_execution_tasks(self, manifest: dict[str, Any]) -> None:
         """Add execution tasks.
 
         Args:
             manifest (dict): DBT manifest.
         """
@@ -53,16 +52,16 @@
                 is_test_task(node_name)
                 and len(self._get_model_dependencies_from_manifest_node(manifest_node, manifest)) > 1
             ):
                 logging.info("Creating tasks for: " + node_name)
                 self._add_graph_node_for_multiple_deps_test(node_name, manifest_node, manifest)
 
     def _add_gateway_execution_tasks(self, manifest: dict[str, Any]) -> None:
-        if self.configuration.gateway.separation_schemas.__len__() >= 2:
-            separation_layers = self.configuration.gateway.separation_schemas
+        if self._configuration.gateway.separation_schemas.__len__() >= 2:
+            separation_layers = self._configuration.gateway.separation_schemas
 
             for index, _ in enumerate(separation_layers[:-1]):
                 separation_layer_left = separation_layers[index]
                 separation_layer_right = separation_layers[index + 1]
                 self._add_gateway_node(
                     manifest=manifest,
                     separation_layer=SeparationLayer(left=separation_layer_left, right=separation_layer_right),
@@ -77,87 +76,103 @@
         manifest_child_map = manifest["child_map"]
         for source_name, manifest_source in manifest["sources"].items():
             if "dag" in manifest_source["source_meta"] and len(manifest_child_map[source_name]) > 0:
                 logging.info("Creating source sensor for: " + source_name)
                 self._add_sensor_source_node(source_name, manifest_source)
 
     def create_edges_from_dependencies(self, include_sensors: bool = False) -> None:
-        """_summary_.
+        """Create edges from dependencies.
 
         Args:
-            include_sensors (bool, optional): _description_. Defaults to False.
+            include_sensors (bool, optional): If True, include sensors in the graph. Defaults to False.
         """
-        for graph_node_name, graph_node in self.graph.nodes(data=True):
+        for graph_node_name, graph_node in self.get_graph_nodes():
             for dependency in graph_node.get("depends_on", []):
                 if is_source_sensor_task(dependency) and not include_sensors:
                     continue
-                if not self.graph.has_node(dependency):
+                if not self._graph.has_node(dependency):
                     continue
-                self.graph.add_edge(dependency, graph_node_name)
+                self._graph.add_edge(dependency, graph_node_name)
+
+    def get_graph_nodes(self) -> NodeDataView:
+        """Get graph nodes.
+
+        Returns:
+            NodeDataView: a view of graph nodes.
+        """
+        return self._graph.nodes(data=True)
+
+    def get_graph_edges(self) -> OutEdgeDataView:
+        """Get graph edges.
+
+        Returns:
+            OutEdgeDataView: A list of graph edges.
+        """
+        return self._graph.edges()
 
     def get_graph_sources(self) -> list[str]:
         """Return a list of graph source nodes.
 
         Returns:
             list[str]: A list of graph source nodes.
         """
-        return [node_name for node_name in self.graph.nodes() if len(list(self.graph.predecessors(node_name))) == 0]
+        return [node_name for node_name in self._graph.nodes() if len(list(self._graph.predecessors(node_name))) == 0]
 
     def get_graph_sinks(self) -> list[str]:
         """Return a list of graph sink nodes.
 
         Returns:
             list[str]: A list of graph sink nodes.
         """
-        return [node_name for node_name in self.graph.nodes() if len(list(self.graph.successors(node_name))) == 0]
+        return [node_name for node_name in self._graph.nodes() if len(list(self._graph.successors(node_name))) == 0]
 
     def remove_ephemeral_nodes_from_graph(self) -> None:
         """Remove ephemeral nodes from the graph."""
         ephemeral_nodes = [
-            node_name for node_name, node in self.graph.nodes(data=True) if node["node_type"] == NodeType.EPHEMERAL
+            node_name for node_name, node in self._graph.nodes(data=True) if node["node_type"] == NodeType.EPHEMERAL
         ]
         for node_name in ephemeral_nodes:
-            self.graph.add_edges_from(
+            self._graph.add_edges_from(
                 itertools.product(
-                    list(self.graph.predecessors(node_name)),
-                    list(self.graph.successors(node_name)),
+                    list(self._graph.predecessors(node_name)),
+                    list(self._graph.successors(node_name)),
                 )
             )
-            self.graph.remove_node(node_name)
+            self._graph.remove_node(node_name)
 
     def contract_test_nodes(self) -> None:
         """Contract test nodes."""
         tests_with_more_deps = self._get_test_with_multiple_deps_names_by_deps()
         for depends_on_tuple, test_node_names in tests_with_more_deps.items():
             self._contract_test_nodes_same_deps(depends_on_tuple, test_node_names)
 
     def _add_execution_graph_node(
         self, node_name: str, manifest_node: dict[str, Any], node_type: NodeType, manifest: dict[str, Any]
     ) -> None:
-        self.graph.add_node(
+        self._graph.add_node(
             node_name,
             select=manifest_node["name"],
             depends_on=self._get_model_dependencies_from_manifest_node(manifest_node, manifest),
             node_type=node_type,
         )
 
     def _add_sensor_source_node(self, node_name: str, manifest_node: dict[str, Any]) -> None:
-        self.graph.add_node(
+        self._graph.add_node(
             node_name,
             select=manifest_node["name"],
             dag=manifest_node["source_meta"]["dag"],
             node_type=NodeType.SOURCE_SENSOR,
         )
 
     def _add_gateway_node(self, manifest: dict[str, Any], separation_layer: SeparationLayer) -> None:
         node_name = create_gateway_name(
             separation_layer=separation_layer,
-            gateway_task_name=self.configuration.gateway.gateway_task_name,
+            gateway_task_name=self._configuration.gateway.gateway_task_name,
         )
-        self.graph.add_node(
+        self._graph.add_node(
             node_name,
             select=node_name,
             depends_on=get_gateway_dependencies(separation_layer=separation_layer, manifest=manifest),
             node_type=NodeType.MOCK_GATEWAY,
         )
 
     def _add_graph_node_for_model_run_task(
@@ -176,53 +191,53 @@
         self._add_execution_graph_node(node_name, manifest_node, NodeType.MULTIPLE_DEPS_TEST, manifest)
 
     def _get_test_with_multiple_deps_names_by_deps(
         self,
     ) -> dict[tuple[str, ...], list[str]]:
         tests_with_more_deps: dict[tuple[str, ...], list[str]] = {}
 
-        for node_name, node in self.graph.nodes(data=True):
+        for node_name, node in self._graph.nodes(data=True):
             if node["node_type"] == NodeType.MULTIPLE_DEPS_TEST:
                 model_dependencies = node["depends_on"]
                 model_dependencies.sort()
                 if tuple(model_dependencies) not in tests_with_more_deps:
                     tests_with_more_deps[tuple(model_dependencies)] = []
                 tests_with_more_deps[tuple(model_dependencies)].append(node_name)
 
         return tests_with_more_deps
 
     def _contract_test_nodes_same_deps(self, depends_on_tuple: tuple[str, ...], test_node_names: list[str]) -> None:
-        test_names = [self.graph.nodes[test_node]["select"] for test_node in test_node_names]
+        test_names = [self._graph.nodes[test_node]["select"] for test_node in test_node_names]
 
         first_test_node = test_node_names[0]
         for test_node in test_node_names[1:]:
             nx.contracted_nodes(
-                self.graph,
+                self._graph,
                 first_test_node,
                 test_node,
                 self_loops=False,
                 copy=False,  # in-memory
             )
 
-        self.graph.nodes[first_test_node]["select"] = " ".join(test_names)
+        self._graph.nodes[first_test_node]["select"] = " ".join(test_names)
         nx.relabel_nodes(
-            self.graph,
+            self._graph,
             {first_test_node: self._build_multiple_deps_test_name(depends_on_tuple)},
             copy=False,
         )
 
     def _get_model_dependencies_from_manifest_node(self, node: dict[str, Any], manifest: dict[str, Any]) -> list[str]:
-        filtered_records = list(filter(DbtAirflowGraph._is_valid_dependency, node["depends_on"]["nodes"]))
+        filtered_records = list(filter(DbtManifestGraph._is_valid_dependency, node["depends_on"]["nodes"]))
         node_schema = node.get("schema", None)
 
         if should_gateway_be_added(
             node_schema=node_schema,
-            separation_schemas=self.configuration.gateway.separation_schemas,
+            separation_schemas=self._configuration.gateway.separation_schemas,
         ):
-            node_schema_index = self.configuration.gateway.separation_schemas.index(node_schema)
+            node_schema_index = self._configuration.gateway.separation_schemas.index(node_schema)
             if node_schema_index >= 1:
                 filtered_records = self._filter_to_gateway_conditions(
                     node_schema_index=node_schema_index,
                     manifest=manifest,
                     node=node,
                     filtered_records=filtered_records,
                 )
@@ -232,15 +247,15 @@
     def _filter_to_gateway_conditions(
         self,
         node_schema_index: int,
         manifest: dict[str, Any],
         node: dict[str, Any],
         filtered_records: list[str],
     ) -> list[str]:
-        separation_layers = self.configuration.gateway.separation_schemas
+        separation_layers = self._configuration.gateway.separation_schemas
         separation_layer_left = separation_layers[node_schema_index - 1]
         separation_layer_right = separation_layers[node_schema_index]
 
         filtered_dependencies = list(
             filter(
                 lambda dep_node: is_gateway_valid_dependency(
                     separation_layer=SeparationLayer(left=separation_layer_left, right=separation_layer_right),
@@ -252,15 +267,15 @@
         )
 
         add_gateway_to_dependencies(
             filtered_dependencies=filtered_dependencies,
             filtered_records=filtered_records,
             gateway_name=create_gateway_name(
                 separation_layer=SeparationLayer(left=separation_layer_left, right=separation_layer_right),
-                gateway_task_name=self.configuration.gateway.gateway_task_name,
+                gateway_task_name=self._configuration.gateway.gateway_task_name,
             ),
         )
         return filtered_dependencies
 
     @staticmethod
     def _is_valid_dependency(node_name: str) -> bool:
         return is_model_run_task(node_name) or is_source_sensor_task(node_name)  # type: ignore
```

### Comparing `dbt-graph-builder-0.0.1/src/dbt_graph_builder/utils.py` & `dbt-graph-builder-0.1.0/src/dbt_graph_builder/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.0.1/src/dbt_graph_builder.egg-info/PKG-INFO` & `dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.0.1
+Version: 0.1.0
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

