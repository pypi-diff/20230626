# Comparing `tmp/dbt-graph-builder-0.1.0.tar.gz` & `tmp/dbt-graph-builder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-graph-builder-0.1.0.tar", last modified: Mon Jun 26 12:58:27 2023, max compression
+gzip compressed data, was "dbt-graph-builder-0.1.1.tar", last modified: Mon Jun 26 13:56:12 2023, max compression
```

## Comparing `dbt-graph-builder-0.1.0.tar` & `dbt-graph-builder-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.864764 dbt-graph-builder-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/src/dbt_graph_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 12:58:27.000000 dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:58:27.868764 dbt-graph-builder-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_graph_dag_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_graph_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-26 12:58:05.000000 dbt-graph-builder-0.1.0/tests/test_graph_ephemeral_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:56:12.415528 dbt-graph-builder-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-26 13:56:12.415528 dbt-graph-builder-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:56:12.415528 dbt-graph-builder-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:56:12.411528 dbt-graph-builder-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:56:12.411528 dbt-graph-builder-0.1.1/src/dbt_graph_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:56:12.415528 dbt-graph-builder-0.1.1/src/dbt_graph_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-26 13:56:12.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-26 13:56:12.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:56:12.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 13:56:12.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 13:56:12.000000 dbt-graph-builder-0.1.1/src/dbt_graph_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:56:12.415528 dbt-graph-builder-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/tests/test_graph_dag_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/tests/test_graph_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-26 13:55:52.000000 dbt-graph-builder-0.1.1/tests/test_graph_ephemeral_operator.py
```

### Comparing `dbt-graph-builder-0.1.0/LICENSE` & `dbt-graph-builder-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/PKG-INFO` & `dbt-graph-builder-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.1.0
+Version: 0.1.1
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dbt-graph-builder-0.1.0/README.md` & `dbt-graph-builder-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/pyproject.toml` & `dbt-graph-builder-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dbt-graph-builder"
-version = "0.1.0"
+version = "0.1.1"
 description = "DBT Graph Builder"
 authors = [
     {name = "Piotr Tutak", email = "piotr.tutak@getindata.com"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "pyspark>=3.4.0",
-    "apache-airflow>=2.6.2",
     "networkx>=2.6.3",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = {file = "LICENSE"}
 
 [tool.bandit]
```

### Comparing `dbt-graph-builder-0.1.0/src/dbt_graph_builder/builder.py` & `dbt-graph-builder-0.1.1/src/dbt_graph_builder/builder.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/src/dbt_graph_builder/gateway.py` & `dbt-graph-builder-0.1.1/src/dbt_graph_builder/gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/src/dbt_graph_builder/graph.py` & `dbt-graph-builder-0.1.1/src/dbt_graph_builder/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/src/dbt_graph_builder/utils.py` & `dbt-graph-builder-0.1.1/src/dbt_graph_builder/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/PKG-INFO` & `dbt-graph-builder-0.1.1/src/dbt_graph_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.1.0
+Version: 0.1.1
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dbt-graph-builder-0.1.0/src/dbt_graph_builder.egg-info/SOURCES.txt` & `dbt-graph-builder-0.1.1/src/dbt_graph_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/tests/test_gateway.py` & `dbt-graph-builder-0.1.1/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/tests/test_graph.py` & `dbt-graph-builder-0.1.1/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/tests/test_graph_dag_dependencies.py` & `dbt-graph-builder-0.1.1/tests/test_graph_dag_dependencies.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/tests/test_graph_dependencies.py` & `dbt-graph-builder-0.1.1/tests/test_graph_dependencies.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.1.0/tests/test_graph_ephemeral_operator.py` & `dbt-graph-builder-0.1.1/tests/test_graph_ephemeral_operator.py`

 * *Files identical despite different names*

