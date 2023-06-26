# Comparing `tmp/knowledge-graph-0.0.8.tar.gz` & `tmp/knowledge-graph-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledge-graph-0.0.8.tar", last modified: Tue Jul  5 09:51:03 2022, max compression
+gzip compressed data, was "knowledge-graph-0.0.9.tar", last modified: Wed Jul 20 08:57:14 2022, max compression
```

## Comparing `knowledge-graph-0.0.8.tar` & `knowledge-graph-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 09:51:03.110389 knowledge-graph-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-07-05 09:51:03.110389 knowledge-graph-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 09:51:03.110389 knowledge-graph-0.0.8/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/common_relations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/minigraph_builders.py
--rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/primitives.py
--rw-r--r--   0 runner    (1001) docker     (121)    15773 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/querying.py
--rw-r--r--   0 runner    (1001) docker     (121)     8571 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/querying_raw.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/querying_raw_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3254 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     3197 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/transform_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/triplet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3438 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/knowledge_graph/triplets_index.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 09:51:03.110389 knowledge-graph-0.0.8/knowledge_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-07-05 09:51:03.000000 knowledge-graph-0.0.8/knowledge_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-07-05 09:51:03.000000 knowledge-graph-0.0.8/knowledge_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-05 09:51:03.000000 knowledge-graph-0.0.8/knowledge_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-05 09:51:03.000000 knowledge-graph-0.0.8/knowledge_graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-05 09:51:03.000000 knowledge-graph-0.0.8/knowledge_graph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-05 09:51:03.110389 knowledge-graph-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-07-05 09:50:36.000000 knowledge-graph-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 08:57:14.562003 knowledge-graph-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-07-20 08:57:14.558002 knowledge-graph-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 08:57:14.558002 knowledge-graph-0.0.9/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/common_relations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5069 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/minigraph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15773 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/querying.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8571 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/querying_raw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/querying_raw_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3254 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3197 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/transform_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/triplet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3438 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/knowledge_graph/triplets_index.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 08:57:14.558002 knowledge-graph-0.0.9/knowledge_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-07-20 08:57:14.000000 knowledge-graph-0.0.9/knowledge_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-07-20 08:57:14.000000 knowledge-graph-0.0.9/knowledge_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 08:57:14.000000 knowledge-graph-0.0.9/knowledge_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-20 08:57:14.000000 knowledge-graph-0.0.9/knowledge_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-20 08:57:14.000000 knowledge-graph-0.0.9/knowledge_graph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-20 08:57:14.562003 knowledge-graph-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-07-20 08:56:44.000000 knowledge-graph-0.0.9/setup.py
```

### Comparing `knowledge-graph-0.0.8/LICENSE` & `knowledge-graph-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/PKG-INFO` & `knowledge-graph-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledge-graph
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library to store data in a knowledge graph
 Home-page: https://github.com/hyroai/knowledge-graph/
 Author: Hyro AI
 Author-email: contact@hyro.ai
 License: UNKNOWN
 Keywords: tag1,tag2
 Platform: UNKNOWN
```

### Comparing `knowledge-graph-0.0.8/README.md` & `knowledge-graph-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/__init__.py` & `knowledge-graph-0.0.9/knowledge_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/common_relations.py` & `knowledge-graph-0.0.9/knowledge_graph/common_relations.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/minigraph_builders.py` & `knowledge-graph-0.0.9/knowledge_graph/minigraph_builders.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/primitives.py` & `knowledge-graph-0.0.9/knowledge_graph/primitives.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/querying.py` & `knowledge-graph-0.0.9/knowledge_graph/querying.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/querying_raw.py` & `knowledge-graph-0.0.9/knowledge_graph/querying_raw.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/querying_raw_test.py` & `knowledge-graph-0.0.9/knowledge_graph/querying_raw_test.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/storage.py` & `knowledge-graph-0.0.9/knowledge_graph/storage.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/transform.py` & `knowledge-graph-0.0.9/knowledge_graph/transform.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/transform_test.py` & `knowledge-graph-0.0.9/knowledge_graph/transform_test.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/triplet.py` & `knowledge-graph-0.0.9/knowledge_graph/triplet.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph/triplets_index.py` & `knowledge-graph-0.0.9/knowledge_graph/triplets_index.py`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/knowledge_graph.egg-info/PKG-INFO` & `knowledge-graph-0.0.9/knowledge_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledge-graph
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library to store data in a knowledge graph
 Home-page: https://github.com/hyroai/knowledge-graph/
 Author: Hyro AI
 Author-email: contact@hyro.ai
 License: UNKNOWN
 Keywords: tag1,tag2
 Platform: UNKNOWN
```

### Comparing `knowledge-graph-0.0.8/knowledge_graph.egg-info/SOURCES.txt` & `knowledge-graph-0.0.9/knowledge_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `knowledge-graph-0.0.8/setup.py` & `knowledge-graph-0.0.9/setup.py`

 * *Files identical despite different names*

