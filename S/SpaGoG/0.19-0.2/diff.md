# Comparing `tmp/SpaGoG-0.19.tar.gz` & `tmp/SpaGoG-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpaGoG-0.19.tar", last modified: Mon Jun 26 07:16:08 2023, max compression
+gzip compressed data, was "dist/SpaGoG-0.2.tar", last modified: Mon Jun 26 08:35:45 2023, max compression
```

## Comparing `SpaGoG-0.19.tar` & `SpaGoG-0.2.tar`

### file list

```diff
@@ -1,9 +1,49 @@
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 07:16:08.000000 SpaGoG-0.19/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1324 2023-06-26 07:15:47.000000 SpaGoG-0.19/setup.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       39 2023-05-12 23:49:44.000000 SpaGoG-0.19/setup.cfg
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.19/README
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      385 2023-06-26 07:16:08.000000 SpaGoG-0.19/PKG-INFO
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 07:16:08.000000 SpaGoG-0.19/spagog/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     5201 2023-06-23 22:45:43.000000 SpaGoG-0.19/spagog/main.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.19/spagog/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11778 2023-06-23 22:45:43.000000 SpaGoG-0.19/spagog/experiments.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1354 2023-06-26 07:59:25.000000 SpaGoG-0.2/setup.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/SpaGoG.egg-info/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1055 2023-06-26 08:35:45.000000 SpaGoG-0.2/SpaGoG.egg-info/SOURCES.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-06-26 08:35:45.000000 SpaGoG-0.2/SpaGoG.egg-info/dependency_links.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        7 2023-06-26 08:35:45.000000 SpaGoG-0.2/SpaGoG.egg-info/top_level.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       40 2023-06-26 08:35:45.000000 SpaGoG-0.2/SpaGoG.egg-info/requires.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      372 2023-06-26 08:35:45.000000 SpaGoG-0.2/SpaGoG.egg-info/PKG-INFO
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       79 2023-06-26 08:35:45.000000 SpaGoG-0.2/setup.cfg
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.2/README
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      372 2023-06-26 08:35:45.000000 SpaGoG-0.2/PKG-INFO
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/spagog/
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/spagog/models/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    17286 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/models/graphNodeClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/models/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6708 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/models/graphClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    14164 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/models/abstractNN.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     3979 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/models/nodeClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      423 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/models/abstractModel.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/spagog/datasets/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7421 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/datasets/tabDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1986 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/datasets/graphDataset.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/datasets/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    11819 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/datasets/tabDataset.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7321 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/datasets/graphDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7661 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/datasets/graphsDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    13210 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/datasets/graphsDataset.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/spagog/utils/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6338 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/utils/knn.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     2887 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/utils/gfp.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/utils/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/spagog/utils/metrics/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/utils/metrics/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1799 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/utils/metrics/metrics.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/spagog/utils/data/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6347 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/utils/data/tab2graph.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/utils/data/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/spagog/default_params/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      236 2023-05-12 23:49:43.000000 SpaGoG-0.2/spagog/default_params/gc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      594 2023-05-12 23:49:43.000000 SpaGoG-0.2/spagog/default_params/gnc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:43.000000 SpaGoG-0.2/spagog/default_params/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      706 2023-05-12 23:49:43.000000 SpaGoG-0.2/spagog/default_params/load_params.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      595 2023-05-12 23:49:43.000000 SpaGoG-0.2/spagog/default_params/gc+nc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     5201 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/main.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.2/spagog/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    11963 2023-06-26 08:07:41.000000 SpaGoG-0.2/spagog/experiments.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 08:35:45.000000 SpaGoG-0.2/spagog/data/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     3426 2023-06-22 20:14:46.000000 SpaGoG-0.2/spagog/data/load_data.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:40.000000 SpaGoG-0.2/spagog/data/__init__.py
```

### Comparing `SpaGoG-0.19/setup.py` & `SpaGoG-0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+import setuptools
 from distutils.core import setup
 
 setup(
     name='SpaGoG',  # How you named your package folder (MyLib)
-    packages=['spagog'],  # Chose the same as "name"
-    version='0.19',  # Start with a small number and increase it with every change you make
+    packages=setuptools.find_packages(),  # Chose the same as "name"
+    version='0.2',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Sparse data classification using Graph of Graphs',  # Give a short description about your library
     author='Shachar Hananya',  # Type in your name
     author_email='shacharhananya@gmail.com',  # Type in your E-Mail
     url='https://github.com/HananyaS/SpaGoG',  # Provide either the link to your github or to your website
-    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.19.tar.gz',  # I explain this later on
+    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.2.tar.gz',  # I explain this later on
     keywords=['GoG', 'Missing values', 'Graphs'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
         'pandas',
         'torch',
         'torch-geometric',
         'matplotlib',
     ],
     # classifiers=[
     #     'License :: OSI Approved :: MIT License',  # Again, pick a license
     #     'Programming Language :: Python :: 3.8',
     # ],
     # add the json files that appear in default_params folder
-    # package_data={'spagog': ['default_params/*.json']},
+    package_data={'spagog': ['default_params/*.json']},
 )
```

### Comparing `SpaGoG-0.19/spagog/main.py` & `SpaGoG-0.2/spagog/main.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.19/spagog/experiments.py` & `SpaGoG-0.2/spagog/experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-import pandas as pd
+import os
 import torch
+import pandas as pd
 
 from .datasets.tabDataset import TabDataset
 from .datasets.graphsDataset import GraphsDataset
 
 from .models.graphClassification import ValuesAndGraphStructure as GC
 from .models.graphNodeClassification import GraphNodeClassification as GNC
 from .models.nodeClassification import NodeClassification
 
+from pkg_resources import resource_filename
+
 PROJECT_DIR = "."
 
 
 def run_gc(
         tab_dataset: TabDataset,
         params: dict,
         early_stopping: int = 30,
@@ -177,22 +180,24 @@
         alpha=params["alpha"],
         batch_size=params.get("batch_size", 10),
         early_stopping_patience=early_stopping,
         verbose=verbose,
         clf_from=params["clf_from"]  # clf_from
     )
 
-    y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"], probs=False,
+    y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"],
+                           probs=False,
                            to_numpy=to_numpy)
 
     if evaluate_metrics and verbose == 1:
         print(f"Test accuracy: {(test_loader.dataset.gdp.Y.flatten() == y_test).float().mean():.4f}")
 
     if probs:
-        y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"], probs=True,
+        y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"],
+                               probs=True,
                                to_numpy=to_numpy)
 
     return y_test, cache
 
 
 def run_gc_nc(
         tab_dataset: TabDataset,
@@ -343,15 +348,16 @@
     if probs:
         y_test = nc_model.predict(test_graph, probs=True, to_numpy=to_numpy)
 
     return y_test, cache
 
 
 def get_default_params_file(model):
-    return f"default_params/{model}.json"
+    abs_path = resource_filename(__name__, ".")
+    return os.path.join(abs_path, f"default_params/{model}.json")
 
 
 def get_tab_data(
         train_X: pd.DataFrame,
         train_Y: pd.DataFrame,
         test_X: pd.DataFrame,
         test_Y: pd.DataFrame = None,
```

